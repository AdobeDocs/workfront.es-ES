---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Agregar una solicitud a un informe
description: Los filtros y los indicadores son similares en el sentido de que ambos restringen la cantidad de información que se muestra en un informe.
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: 9396cd2ac073a57b7d99618cdf09e54ddcf95130
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 0%

---

# Agregar una solicitud a un informe

<!-- Audited: 11/2024 -->

## Diferencia entre indicadores y filtros

Los filtros y los indicadores son similares en el sentido de que ambos restringen la cantidad de información que se muestra en un informe.

Se genera un filtro cuando se desea que la información que se muestra en el informe se filtre con los mismos criterios cada vez que se ejecuta el informe. Los filtros se crean una vez y se codifican en el informe. Para obtener más información acerca de cómo generar filtros, vea el artículo [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Los indicadores son filtros abiertos que se pueden personalizar y aplicar de forma diferente cada vez que se ejecuta un informe.

Cuando agregue peticiones de datos al informe, puede personalizar la información de filtrado editando los criterios de petición de datos cada vez que ejecute el informe. El informe se ejecuta con un filtro diferente cada vez, según los modificadores que elija, en lugar de programar los modificadores una vez en el filtro del informe.

Los indicadores actúan como un filtro personalizable en los informes que se pueden actualizar justo antes de ejecutar el informe. Puede crear informes genéricos y luego reducir los resultados en función de la información que desee ver para ese día o de la información que sea relevante para un conjunto de criterios por separado. Por ejemplo, si tiene un informe de horas y desea cambiar la información del informe en función de los siguientes criterios:

* Las fechas en las que se registraron las horas
* Los usuarios que ingresaron las horas
* La cantidad de horas ingresadas

Debe generar tres indicadores donde las condiciones sean los criterios requeridos y el informe tendrá un aspecto diferente cada vez que lo ejecute, según la información que elija para sus indicadores.

Un filtro puede indicar a Adobe Workfront que muestre solo las horas ingresadas entre junio y agosto de este año. Sin embargo, si se le solicita, puede utilizar un lapso de tiempo diferente cada vez que ejecute el informe (por ejemplo, entre enero y febrero, u octubre y diciembre).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
    <td> 
      <p>Nuevo:</p>
         <ul>
         <li><p>Estándar</p></li>
         </ul>
      <p>Actual:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto*</td> 
   <td> <p>Administración de permisos de un informe</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Debe crear un informe antes de agregar una solicitud.

Para obtener instrucciones sobre cómo crear un informe, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)

## Crear una solicitud

1. Vaya al informe en el que desee agregar un mensaje.
1. Expanda **Acciones de informe** y, a continuación, haga clic en **Editar**.

1. Haga clic en el botón **Configuración de informes**.
1. Haga clic en la ficha **Indicadores del informe** y, a continuación, haga clic en **Agregar un mensaje**.\
   ![](assets/create-report-prompt-tab.png)

1. (Condicional) Seleccione el campo en el que desea basar la solicitud. Empiece a escribir el nombre del campo y, a continuación, haga clic en para seleccionarlo cuando aparezca en la lista.\
   Las opciones disponibles para los usuarios que ejecuten el informe variarán según el campo que seleccione.\
   Por ejemplo, si selecciona un campo de fecha como Fecha real de finalización en un informe de tareas, &quot;Fecha real de finalización&quot; es el nombre de la solicitud. Al editar esta solicitud mientras ejecuta este informe, puede elegir entre un conjunto de modificadores para crear la sentencia de filtrado. Este proceso es idéntico al de creación de un filtro. Para obtener más información acerca de los modificadores, vea [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Condicional) Haga clic en **Mensaje personalizado** para crear un mensaje personalizado.

   Una solicitud personalizada es una solicitud predefinida en la que se codifican los criterios de filtrado antes de ejecutar el informe. En este sentido, un mensaje personalizado está más cerca de un filtro que un mensaje.

   Sin embargo, el símbolo del sistema sigue siendo tan flexible como un símbolo del sistema normal, ya que puede elegir entre varias instrucciones predefinidas, en lugar de tener solo un filtro codificado en el informe.

   Especifique la siguiente información para la solicitud personalizada: La condición de una solicitud personalizada solo se puede editar en modo de texto. Esto permite aplicar varias condiciones en un solo campo.

   * **Nombre de campo:** Este es el nombre de la solicitud, tal como lo ve antes de ejecutar el informe.
   * **Etiqueta de elemento desplegable:** Este es el nombre de una de las opciones dentro de la solicitud tal como la ve antes de ejecutar el informe.
   * **Condición:** Escriba una condición que defina el mensaje.
   * **Predeterminado:** Puede seleccionar un elemento para que sea la opción predeterminada para esta solicitud.

   Utilice la misma sintaxis que utilizaría al introducir un filtro de modo de texto y una sus instrucciones con &quot;&amp;&quot;. Para obtener más información sobre cómo editar un filtro en modo de texto, vea [Editar un filtro en modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

   Por ejemplo, el campo **Condición** del mensaje personalizado para los siguientes escenarios podría tener este aspecto:

   * todas las tareas de proyectos futuros cuyo estado sea Idea, Solicitada, Planificada y Actual:

     ```
     project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
     ```

   * todas las tareas de proyectos completados (anteriores) en los que el estado del proyecto es Completado o Inactivo:

     ```
     project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
     ```

   Para obtener más información acerca de los modificadores de modo de texto, vea [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >No se pueden cambiar las condiciones de una petición de datos personalizada cuando se ejecuta el informe, como lo haría con una petición de datos estándar. Puede tener tantas condiciones predefinidas para un mensaje personalizado como necesite.

1. (Opcional) Repita el paso 4 o el paso 5 para crear tantos mensajes como sea necesario.
1. Haga clic en **Listo** y, a continuación, haga clic en **Guardar+Cerrar** para guardar el informe.

## Aplicar una solicitud a un informe

Cuando se agrega una solicitud a un informe, la ficha predeterminada del informe siempre es la ficha Peticiones de datos.

Para ejecutar un informe con una solicitud:

1. Vaya al informe con el mensaje.

   ![](assets/run-report-prompts.png)

1. Elija una condición para uno o todos los indicadores mostrados en la ficha **Indicadores**.\
   (Opcional) Puede dejar los indicadores en blanco y no filtrar el informe según las condiciones del mensaje.

1. Haga clic en **Ejecutar informe**.\
   (Condicional) Si ha rellenado los indicadores, el informe se filtra según las condiciones seleccionadas para los mensajes.\
   (Condicional) Si deja las solicitudes en blanco, el informe no se filtra por las condiciones de la solicitud. El informe se muestra como si no se hubiera filtrado.

   >[!NOTE]
   >
   >Un informe que contiene un filtro además de una petición de datos filtra los resultados según los criterios definidos en el filtro y la petición combinada.

## Limitaciones al compartir informes solicitados

>[!CAUTION]
>
>Cuando comparte un informe solicitado, tanto los usuarios que han iniciado sesión como los que no lo han hecho que ven el informe mediante el vínculo compartido público no pueden ejecutar el informe mediante sus mensajes. En este caso, los resultados del informe se muestran sin aplicar ningún indicador y la información mostrada se basará en el nivel de acceso y los permisos del usuario o en el nivel de acceso y los permisos de Ejecutar como usuario del informe, si se ha definido uno.

Las siguientes son limitaciones en el uso compartido de informes solicitados desde Workfront:

* Cuando comparte un informe públicamente, los usuarios no pueden ejecutarlo con mensajes aplicados, a menos que: tengan credenciales de Workfront, inicien sesión primero y naveguen hasta el informe directamente en Workfront (no a través del vínculo para compartir público).

  Para obtener más información sobre cómo compartir informes, consulte el artículo [Compartir un informe en Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

* Cuando se programa un informe solicitado para su envío, el informe que aparece en el archivo adjunto de correo electrónico incluye los datos del informe sin solicitarlo. Cuando el usuario hace clic en el vínculo del correo electrónico para acceder al informe, debe iniciar sesión primero para ver el informe y ejecutar la solicitud por su cuenta.

  Para obtener información sobre cómo programar un informe entregado, consulte [Programar un envío automático de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).
