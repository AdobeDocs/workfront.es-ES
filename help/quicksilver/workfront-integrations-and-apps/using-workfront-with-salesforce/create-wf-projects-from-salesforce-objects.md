---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: Crear [!DNL Adobe Workfront] proyectos de [!DNL Salesforce] objetos
description: Después de instalar [!DNL Adobe Workfront] para Salesforce, puede definir déclencheur que creen [!DNL Workfront] proyectos cuando se cumplen determinados criterios en [!DNL Salesforce] Oportunidades y Cuentas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '1506'
ht-degree: 3%

---

# Crear [!DNL Adobe Workfront] proyectos de [!DNL Salesforce] objetos

Después de instalar [!DNL Adobe Workfront] para Salesforce, puede definir déclencheur que creen [!DNL Workfront] proyectos cuando se cumplen determinados criterios en [!DNL Salesforce] [!UICONTROL Oportunidades] y [!UICONTROL Cuentas].

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad descrita en este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Para enviar un [!DNL Workfront] solicitud de un [!DNL Salesforce] [!UICONTROL Oportunidad] o Asegúrese de que dispone de lo siguiente en su entorno:

* Su [!DNL Workfront] administrador instalado [!DNL Workfront for Salesforce].\
   Para obtener más información sobre la instalación [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Su [!DNL Workfront] el administrador ha añadido la variable [!DNL Workfront] para [!UICONTROL Oportunidad] y los diseños de la página Cuenta.\
   Para obtener más información sobre cómo agregar la variable [!DNL Workfront] para un diseño de página, consulte [Configure las variables [!DNL Adobe Workfront] para [!DNL Salesforce] usuarios](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Tiene un [!DNL Workfront] puede iniciar sesión en ella desde la [!DNL Workfront] dentro de su [!UICONTROL Oportunidad] o Cuenta .

## Configuración de la creación de [!DNL Workfront] Proyectos de [!DNL Salesforce]

* [Explicación de la creación automática de proyectos](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Configuración de Déclencheur](#configuring-triggers-configuring-triggers)
* [Explicación de los nombres de los proyectos](#understanding-project-names-understanding-project-names)

### Explicación de la creación automática de proyectos {#understanding-the-automatic-creation-of-projects}

Como [!DNL Salesforce] administrador del sistema, puede definir déclencheur que puedan crear proyectos automáticamente en [!DNL Workfront] cuando sucedan las siguientes cosas en [!DNL Salesforce]:

* La variable [!UICONTROL Prueba] de un [!UICONTROL Oportunidad] se actualiza.
* La variable [!UICONTROL Tipo] de una cuenta se actualiza.

Los déclencheur solo se pueden configurar una vez que haya instalado [!DNL Workfront for Salesforce].  \
Para obtener información sobre la instalación [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Tenga en cuenta lo siguiente al configurar déclencheur para crear automáticamente [!DNL Workfront] proyectos cuando [!DNL Salesforce] los elementos se crean o actualizan:

* Debe ser [!DNL Salesforce] y [!DNL Workfront] administrador del sistema para configurar déclencheur.
* Después de configurar las déclencheur, cualquier persona que actualice la variable [!UICONTROL Prueba] de un [!UICONTROL Oportunidad] o [!UICONTROL Tipo] de una cuenta puede déclencheur en la creación de un [!DNL Workfront] proyecto. Esto incluye [!DNL Salesforce] usuarios que no tengan un [!DNL Workfront] cuenta.
* No hay límite para la cantidad de déclencheur que se pueden tener.
* No se pueden crear varios déclencheur basados en las mismas condiciones. Los déclencheur son únicos de forma predeterminada.
* Una vez creado el proyecto, se vincula automáticamente a la oportunidad o a la cuenta donde se generó. Una vez establecido, este vínculo no se puede romper.
* Una oportunidad o cuenta se puede vincular a varios proyectos en [!DNL Workfront] cuando una condición activada se ha cumplido varias veces durante la vida de la oportunidad o de la cuenta.

   Por ejemplo, si define más de uno [!UICONTROL Prueba] para un [!UICONTROL Oportunidad] para el déclencheur de un proyecto, se crea un proyecto para cada fase definida a la que llegue la oportunidad, durante la vida de esa oportunidad. Además, si actualiza la variable [!UICONTROL Prueba] de un [!UICONTROL Oportunidad] de una fase definida a otra y, a continuación, actualícela de nuevo a la fase definida, se crea un segundo proyecto por segunda vez que actualice la [!UICONTROL Prueba] a la misma fase definida.

* Un proyecto en [!DNL Workfront] solo se puede vincular a una oportunidad o a una cuenta de [!DNL Salesforce] en cualquier momento, pero no a ambos al mismo tiempo.

### Configuración de Déclencheur {#configuring-triggers}

Una vez configurados los déclencheur, el proceso de creación [!DNL Workfront] proyectos está habilitado para [!UICONTROL Salesforce Classic] o [!DNL Lightning Experience] marcos.

Para configurar déclencheur en [!UICONTROL Salesforce]:

1. Iniciar sesión en [!DNL Salesforce] como administrador del sistema.
1. (Condicional) En [!DNL Salesforce Classic], haga clic en **[!UICONTROL Configuración]** y en la **[!UICONTROL Generar]** sección, expandir **[!UICONTROL Perno de rayo]**.

   O

   En [!DNL Salesforce] Experiencia de relámpago, haga clic en el botón **[!UICONTROL Configuración] icono**, luego **[!UICONTROL Configuración]** y en **[!UICONTROL HERRAMIENTAS DE PLATAFORMA]** expandir **[!UICONTROL Aplicaciones]**.

1. Haga clic en **[!UICONTROL Paquetes instalados]**.

   Observe que la variable **[!DNL Workfront]** se ha instalado.

1. Haga clic en **[!UICONTROL Configurar]** junto a **[!DNL Workfront]**.

1. Iniciar sesión en [!DNL Workfront] como administrador del sistema.

   La variable **[!UICONTROL Déclencheur]** se muestra.

   ![salesforce_déclencheur_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Haga clic en **[!UICONTROL Nuevo Déclencheur]**.
1. En el **[!UICONTROL [!DNL Salesforce]Objeto]** menú desplegable, seleccione **[!UICONTROL Oportunidad]**.

   Este campo es obligatorio.

1. (Condicional) Especifique lo siguiente:

   1. En el **[!UICONTROL Prueba]** menú desplegable, seleccione un **[!UICONTROL Prueba]**.\

      Cuando una oportunidad alcanza la variable [!UICONTROL Prueba] especificado aquí, se crea un proyecto en [!DNL Workfront]. Este campo es obligatorio.

   1. En el **[!UICONTROL Portfolio o programa]** , empiece a escribir el nombre de un Portfolio o Programa en el que desea colocar el proyecto [!DNL Workfront]y, a continuación, selecciónela cuando aparezca en la lista.\

      Si no especifica un Portfolio o un programa, el nuevo proyecto se crea y se agrega al [!UICONTROL Proyectos de los que soy propietario] lista del usuario con sesión iniciada en [!DNL Workfront] al configurar los déclencheur. Ese usuario también es el propietario del proyecto para el nuevo proyecto.

   1. Comience a escribir el nombre de una plantilla que desee asociar con la nueva [!DNL Workfront] y, a continuación, selecciónelo cuando aparezca en la lista.\

      Este campo es obligatorio.


      >[!NOTE]
      >
      >Si ha especificado un Propietario de plantilla en la plantilla que planea usar para esta integración, ese será el Propietario del proyecto nuevo. Los nuevos proyectos aparecen en el [!UICONTROL Proyectos de los que soy propietario] lista del usuario que es el propietario del nuevo proyecto, según la plantilla.

   1. (Opcional) Seleccione el **[!UICONTROL Crear un nuevo proyecto para cada tipo de producto vendido] field**, si desea crear un nuevo proyecto para cada tipo de producto que se vende en cualquier oportunidad.
   1. (Condicional) Seleccione un **[!UICONTROL Product]** en el **[!UICONTROL Product]** menú desplegable.

      Este campo es obligatorio.

   1. (Condicional) Empiece a escribir el nombre de una **[!UICONTROL Plantilla]** que desea asociar con el nuevo [!DNL Workfront] proyecto si el producto especificado está en el [!UICONTROL Oportunidad]. Selecciónela cuando aparezca en la lista.

      Este campo es obligatorio.

      El proyecto se crea cuando se agrega un nuevo producto al [!DNL Salesforce] La oportunidad se coloca en el mismo Portfolio o Programa seleccionado para la oportunidad.

      >[!IMPORTANT]
      >
      >El proyecto solo se crea cuando el escenario se actualiza en el [!UICONTROL Oportunidad]. Se crea un proyecto único para cada producto especificado cuando se actualiza el campo Etapa y no a medida que se agregan los productos a [!UICONTROL Oportunidades].

1. (Opcional) Haga clic en **[!UICONTROL Nuevo Déclencheur]**.
1. (Opcional) Desde la **[!UICONTROL [!DNL Salesforce]Objeto]** menú desplegable, seleccione **Cuenta **.

   Este campo es obligatorio.
1. (Condicional) Especifique lo siguiente:

   1. Seleccione un **[!UICONTROL Tipo]** de la variable **[!UICONTROL Tipo]** menú desplegable.

      Cuando se designa cualquier **Cuenta ** como el **[!UICONTROL Tipo]** especificado aquí en [!DNL Salesforce], **[!UICONTROL Proyecto]** se crea en [!DNL Workfront].

      Este campo es obligatorio.

   1. (Opcional) Empiece a escribir el nombre de un **[!UICONTROL Portfolio]** o **[!UICONTROL Programa]** donde desea colocar el proyecto [!DNL Workfront] en el **[!UICONTROL Portfolio o programa]** y, a continuación, selecciónelo cuando aparezca en la lista.

      Si no especifica un Portfolio o un programa, el nuevo proyecto se crea y se agrega al **[!UICONTROL Proyectos de los que soy propietario]** lista del usuario con sesión iniciada en [!DNL Workfront] from [!DNL Salesforce]. El usuario también es el propietario del proyecto para el nuevo proyecto.

   1. Empiece a escribir el nombre de un **[!UICONTROL Plantilla]** que desea asociar con el nuevo [!DNL Workfront] proyecto y selecciónelo cuando aparezca en la lista.

      Este campo es obligatorio.

      >[!NOTE]
      >
      >Si ha especificado un Propietario de plantilla en la plantilla que planea usar para esta integración, ese será el Propietario del proyecto nuevo. Los nuevos proyectos aparecen en el **[!UICONTROL Proyectos de los que soy propietario]** lista del usuario que es el propietario del nuevo proyecto, según la plantilla.
   ![salesforce_déclencheur_page_with_clean_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   [!DNL Workfront] ahora se generan proyectos cada vez que se cumple cualquiera de los déclencheur.

### Explicación de los nombres de los proyectos {#understanding-project-names}

Según el déclencheur que generó los proyectos, los nombres de los proyectos en [!DNL Workfront] podría seguir cualquiera de estos patrones:

* Si el proyecto se crea en función de una oportunidad o déclencheur de cuenta, el nombre del proyecto es: *`<Salesforce object name>`: `<Project template name>` (mediante [!DNL Salesforce])*.
* Si el proyecto se crea en función de un déclencheur de oportunidad que también incluya la adición de un nuevo producto, el nombre del proyecto es: *`<Salesforce object name>`: `<Salesforce product name>` (mediante [!DNL Salesforce])*.

## Ver [!DNL Workfront] proyectos

Si su [!DNL Workfront] el administrador añadió la variable [!DNL Workfront] para [!UICONTROL Oportunidad] Para el diseño de la página Cuenta , puede ver los proyectos creados automáticamente en la [!UICONTROL Proyectos] de esta sección.\
Para obtener más información sobre cómo agregar la variable [!DNL Workfront] al diseño de página de una [!UICONTROL Oportunidad] o Cuenta , consulte [Configure las variables [!DNL Adobe Workfront] para [!DNL Salesforce] usuarios](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

Debe tener un [!DNL Workfront] e inicie sesión en [!DNL Workfront] para ver el [!UICONTROL Proyectos] pestaña .

Para ver los proyectos creados a partir de un [!UICONTROL Oportunidad] o Cuenta :

1. Vaya a un [!UICONTROL Oportunidad] o Cuenta .
1. Vaya a la **[!DNL Workfront]** para obtener más información.

   >[!NOTE]
   >
   >Dependiendo de cómo [!DNL Workfront] administrador ha configurado esta sección, puede tener un nombre diferente.

1. Seleccione el **[!UICONTROL Proyectos]** pestaña .

   Todos los proyectos creados por déclencheur definidos se muestran en esta pestaña. Cualquier usuario de [!DNL Salesforce] que también tiene un [!DNL Workfront] y que pueden tener permisos para ver estos proyectos en [!DNL Workfront] también puede verlos en [!DNL Salesforce] para el [!UICONTROL Oportunidad] o la cuenta que los generó.

   Puede ver la siguiente información sobre los proyectos creados por la integración:

   * Nombre del proyecto
   * Número de referencia
   * Fecha de entrada
   * Nombre del propietario
   * Estado
   * Condición
   * Fecha planificada de finalización
   * Porcentaje completado

      Cuando esta información se actualiza en [!DNL Workfront], puede ver los campos actualizados en esta lista.

1. (Opcional) Haga clic en el nombre de un proyecto para abrirlo en Workfront.
1. (Opcional) Haga clic en [!UICONTROL **[!UICONTROL Ir a Salesforce]**] en el [!UICONTROL Detalles del proyecto] o el encabezado del proyecto para acceder al [!UICONTROL Oportunidad] o la cuenta en la que se originó el proyecto. El administrador del sistema o del grupo debe agregar la variable [!UICONTROL Integraciones] a la plantilla de diseño para encontrarla en el encabezado del proyecto.

   >[!NOTE]
   >
   >La variable [!UICONTROL Ir a Salesforce] el vínculo es visible para todos [!DNL Workfront] usuarios que pueden ver el proyecto. Debe tener un [!DNL Salesforce] para poder ir a la [!DNL Salesforce] Oportunidad o Cuenta desde donde se generó el proyecto.
