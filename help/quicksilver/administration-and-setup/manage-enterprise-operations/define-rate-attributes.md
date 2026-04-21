---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Definir atributos de tasa
description: Los atributos de tasa amplían la funcionalidad de tarjeta de tasa y tasas de Adobe Workfront al permitirle añadir dimensiones adicionales a las tasas más allá de la función de trabajo. Workfront puede seleccionar automáticamente la tasa correcta para las asignaciones, lo que garantiza la precisión financiera y la coherencia entre los proyectos.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d570ef6a-935f-4dd0-9c54-a480163ec9d8
source-git-commit: 7686cd33a5c761dc57cb488ea49a4139665949d9
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 2%

---

# Definir atributos de tasa

Los atributos de tasa amplían la funcionalidad de tarjeta de tasa y tasas de Adobe Workfront al permitirle añadir dimensiones adicionales a las tasas más allá de la función de trabajo. Esto es crítico para las agencias y empresas donde las tasas varían no solo por rol sino también por factores como agencia, ubicación, marca, centro de costo u otros.
Al combinar estos atributos, Workfront puede seleccionar automáticamente la tasa correcta para las asignaciones, lo que garantiza la precisión financiera y la coherencia en todos los proyectos.

>[!IMPORTANT]
>
>Los atributos de tasa son una configuración fundamental de una sola vez.

Una vez que los atributos están habilitados y aplicados a las tarjetas de tasas y tasas, cambiarlos más adelante puede comprometer la integridad de los datos en toda la configuración financiera.

## Resumen de los atributos de tasa

Los atributos de tasa se consideran una configuración única porque:

* Los atributos pasan a formar parte del modelo de datos financieros una vez que se activan.
* Las tasas, las asignaciones, los valores planificados y los valores reales dependen de los valores de atributo elegidos.
* Cambiar atributos más adelante (cambiar el nombre, eliminar o reordenar) puede causar lo siguiente:

   * Pérdida de vinculación entre tasas y atributos
   * Tarifas no válidas o &quot;huérfanas&quot;
   * Desalineación en facturación e informes

Por estos motivos, los atributos deben diseñarse cuidadosamente durante la implementación inicial de Workfront y no cambiarse posteriormente.

### Objetos utilizados como atributos de tasa

Actualmente, Workfront admite tres objetos de sistema que pueden utilizarse como atributos de tasa:

* **Grupo**: con frecuencia se le cambia el nombre a _Agencia_ o _Unidad de negocio_.
* **Empresa**: puede representar a _Marca_, _Cliente_ o _Cliente_.
* **Ubicación**: Se suele usar como _Mercado_, _Región_ u _Oficina_.

  La ubicación se define jerárquicamente hasta 3 niveles. (Ejemplo: si define &quot;Ubicación&quot; como Los Ángeles, también se usarán California y EE. UU. en las coincidencias de tarifas).

Se puede cambiar el nombre de cada objeto para que coincida con la terminología de la organización al configurar los atributos.
Por ejemplo:

* Etiqueta &quot;Agency&quot; = Referencia de objeto de grupo
* Etiqueta &quot;Centro de coste&quot; = Referencia de objeto de subgrupo
* Etiqueta &quot;Ubicación&quot; = Referencia del objeto de ubicación

Esto permite que la configuración duplique la estructura de su empresa y, al mismo tiempo, mantenga la integridad del modelo de datos de Workfront.

### Notas sobre los atributos de tasa en Workfront

* Workfront admite hasta 5 niveles de atributos. El sistema siempre sigue la jerarquía de atributos y selecciona la coincidencia disponible más específica.

   * 0 = tipo base genérico
   * 1 - 5 = tasas progresivamente más específicas

* Puede cambiar el nombre de los atributos para que reflejen su negocio (Agencia, Marca, Mercado, Centro de costes, etc.).
* La configuración es de una sola vez: si se cambian los atributos más adelante se corre el riesgo de dañar la integridad de los datos financieros.
* Los atributos a los que no se hace referencia en ningún lugar del sistema se pueden eliminar de forma segura.

  Sin embargo, si un atributo ya está en uso (al que se hace referencia en las tarjetas de tasas, perfiles de usuario, recursos o asignaciones), la eliminación se bloquea para proteger la integridad de los datos. En estos casos, intentar eliminar el atributo, especialmente a través de una llamada de API, producirá un error.

* Probar antes del lanzamiento: cree una tarjeta de tarifa piloto y compruebe que las tarifas correctas se resuelven en las asignaciones.
* Documente su configuración: Comparta la configuración de atributos de tasa con sus equipos para que entiendan cómo funcionan las tasas.

### Dónde se pueden aplicar los atributos de tasa

Los atributos de tasa son compatibles con todas las áreas donde existen tasas en Workfront:

* Tarjetas de tasas: Defina tasas por rol más atributos.
* Anulaciones a nivel de proyecto: Aplique atributos al anular tasas a nivel de proyecto.
* Funciones del puesto (en Configuración): establezca las tasas de funciones del puesto por defecto con atributos.
* Usuarios (perfiles de usuario): asigne atributos nativos a usuarios individuales, de modo que sus asignaciones se resuelvan automáticamente en las tasas correctas.

<!--
BULLET POINT Staffing plan resources
BULLET POINT Non-labor resources: Attributes can also be defined on resources such as equipment or services.
-->

<!--Non-labor resource categories and -->Los roles no admiten atributos de tasa directamente en el nivel de objeto. Están conectados a atributos de tipo de cambio a través de los tipos definidos en ellos.

Cuando puede crear asignaciones de marcador de posición vinculadas a los valores de atributo correctos, las tasas se rellenarán en consecuencia.

* En el caso de los roles, cuando reemplace posteriormente el marcador de posición por un usuario real, el sistema restablece automáticamente los atributos de la asignación a los definidos en el perfil de ese usuario. En este punto, los atributos ya no se pueden editar en el nivel de asignación. Se heredan del usuario para preservar la coherencia y evitar la desalineación entre los atributos del usuario y las tasas aplicadas.

<!-- BULLET POINT For non-labor resource categories, placeholder assignments can be used similarly: You assign the category through a placeholder that carries the required attributes. Once the actual non-labor resource is substituted, the attributes are automatically pulled from the resource's profile. Just like with users, these attributes cannot be overridden manually at the assignment level, ensuring financial data integrity and preventing accidental mismatches between resources and their designated attributes.-->

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar atributos de tasa

Cada atributo tiene un conjunto de opciones configurables, incluidas las propiedades generales y los filtros.
Los filtros controlan cómo se sugieren y validan los valores de atributo al definir tasas. Son esenciales para mantener la coherencia en las selecciones de atributos, guiar a los usuarios hacia opciones válidas y evitar combinaciones no válidas.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Atributos de tarifa**.
1. Haga clic en un icono de signo más en el diagrama para agregar un atributo.

   >[!NOTE]
   >
   >Puede haber hasta cinco atributos en el diagrama. El orden de arriba a abajo define la jerarquía de cómo se aplican los atributos. Haga clic en el icono **Rotar** ![Rotar icono](assets/rotate-attribute-view-icon.png) para mostrar el diagrama de izquierda a derecha. También puede acercar o alejar el diagrama y ajustarlo a la pantalla.

1. Seleccione un atributo para abrir el panel de configuración en la parte derecha de la pantalla.

   ![Configurar atributos de tarifa](assets/configure-rate-attributes.png)

1. Cambie el nombre de los objetos (Grupo, Empresa, Ubicación) por los términos necesarios para su negocio (como Agencia, Ubicación, Centro de coste).
1. Haga clic en **Guardar** en cada atributo para guardar la convención de nombres.

   Los nombres de estos atributos se mostrarán en todas las tarjetas de tasas y tasas del sistema.

1. Establezca las propiedades de cada atributo en el panel de configuración:

   * **Obligatorio**: seleccione si el atributo es un campo obligatorio en tasas.
   * **Para usar en el cálculo de ingresos**: Incluye este atributo en los cálculos de tarifa de facturación.
   * **Se utilizará en el cálculo de costos**: Incluye este atributo en los cálculos de tasas de costos.

     >[!NOTE]
     >
     >Se debe seleccionar al menos una de las opciones de cálculo para que el atributo funcione en los cálculos financieros.

   * (Opcional) **Jerárquico**: permite que el atributo respete las relaciones principal-secundario, como Ciudad > Estado > País.

     Esta propiedad sólo está disponible para el objeto Location.

### Defina filtros para los atributos

Hay dos tipos de filtros disponibles para los atributos:

* Los filtros de sugerencias limitan la lista de opciones disponibles en función de la lógica del sistema o de selecciones de atributos anteriores. Hacen que los desplegables tengan en cuenta el contexto y sean fáciles de usar.

  Ejemplo: Agencia > Ubicación > Centro de coste

  En esta configuración, el atributo Centro de coste debe tener un filtro de sugerencias que haga referencia tanto a Agencia como a Ubicación.

  Al añadir una tasa, si primero selecciona Agencia = &quot;Estrella&quot;, la lista desplegable Ubicación solo sugerirá Ubicaciones que pertenezcan a &quot;Estrella&quot;.

  Si selecciona Ubicación = Chicago en la tarifa, la lista desplegable Centro de coste solo sugerirá Centros de coste vinculados a &quot;Estrella&quot; y Chicago.

* Los filtros de relación establecen la cadena de dependencia entre atributos. Garantizan que el sistema comprende cómo se relacionan los atributos entre sí y aplican dependencias válidas.

  Ejemplo: Agencia > Ubicación > Centro de coste

  En esta configuración, el atributo Agencia debe tener un filtro de relación que lo vincule a ubicaciones y centros de coste válidos.

Los filtros siempre deben configurarse en ambas direcciones. Si el atributo A tiene un filtro de relación con el atributo B, el atributo B debe tener un filtro de sugerencia de nuevo en el atributo A. Esto garantiza la integridad de los datos y una experiencia del usuario limpia.

1. Seleccione las opciones para definir los Filtros de sugerencias y los Filtros de relaciones para el atributo en el panel de configuración:

   * **Tipo de filtro**:

      * Un filtro **Standard** aplica una condición universal al objeto de atributo. Por ejemplo, Ubicación > Está activo = Verdadero (solo se mostrarán las ubicaciones activas).

        El filtro Estándar siempre se aplica, independientemente de si están seleccionados otros atributos.

      * Un filtro **Atributo** vincula un atributo con otro de la cadena. Por ejemplo, Ubicación > Referencia = Agencia (solo se mostrarán las ubicaciones vinculadas a la Agencia seleccionada).

        El filtro Attribute solo se aplica si el atributo al que se hace referencia tiene un valor. Por ejemplo, si se selecciona Agencia, solo se sugieren ubicaciones válidas. Si la Agencia está en blanco, se muestran todas las ubicaciones (pero pueden estar limitadas por los filtros estándar aplicados a la ubicación).

   * **Campo**: Campo directo del objeto de atributo, como Id. de ubicación o Indicador activo.
   * **Operador**: estas opciones dependen del tipo de campo seleccionado. Algunos ejemplos son Igual a, No es igual a, Está en blanco, Verdadero/Falso.
   * (Solo tipo de filtro estándar) **Value**: Por ejemplo, Is Active = True.
   * (Solo tipo de filtro de atributo) **Referencia**: Atributo del que depende este filtro, como Agencia.
   * (Solo tipo de filtro de atributo) **Campo de referencia**: Campo del atributo al que se hace referencia que debe coincidir, como Id. de agencia.

1. Haga clic en **Guardar** en cada atributo para guardar las propiedades y los filtros.
