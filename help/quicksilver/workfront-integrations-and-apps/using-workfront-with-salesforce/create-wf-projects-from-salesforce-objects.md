---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: 'Crear proyectos de  [!DNL Adobe Workfront]  a partir de objetos de  [!DNL Salesforce] '
description: Después de instalar [!DNL Adobe Workfront] for Salesforce, puede definir déclencheur que crean [!DNL Workfront] proyectos cuando se cumplan determinados criterios en [!DNL Salesforce] Oportunidades y cuentas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '1581'
ht-degree: 10%

---

# Crear [!DNL Adobe Workfront] proyectos a partir de [!DNL Salesforce] objetos

>[!IMPORTANT]
>
>Para ofrecer integraciones más estables y escalables, estamos adoptando un enfoque de integración moderno y flexible mediante la automatización e integración (Fusion) de Workfront. Como parte de este proceso de transición, la integración de Workfront para Salesforce no estará disponible después del **28 de febrero de 2026**.
>
>Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Salesforce.
>
>Para obtener una descripción general de la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obtener información sobre las capacidades específicas de los módulos de integración y automatización de Workfront para Salesforce, consulte [módulos de Salesforce](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Después de instalar [!DNL Adobe Workfront] para Salesforce, puede definir déclencheur que creen [!DNL Workfront] proyectos cuando se cumplan ciertos criterios en [!DNL Salesforce] [!UICONTROL Oportunidades] y [!UICONTROL Cuentas].

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad que se describe en este artículo:

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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con la persona con la función de administrador de [!DNL Workfront].

## Requisitos previos

Para enviar una solicitud [!DNL Workfront] desde una [!DNL Salesforce] [!UICONTROL oportunidad] o cuenta
asegúrese de que dispone de lo siguiente en su entorno:

* El administrador de [!DNL Workfront] ha instalado [!DNL Workfront for Salesforce].\
   Para obtener más información sobre la instalación de [!DNL Workfront for Salesforce], consulte [Instalar  [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* El administrador de [!DNL Workfront] ha agregado la sección [!DNL Workfront] a su [!UICONTROL oportunidad] y cuenta
diseños de página.\
   Para obtener más información sobre cómo añadir la sección [!DNL Workfront] a un diseño de página, consulte [Configurar la sección  [!DNL Adobe Workfront]  para los usuarios de  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Tiene una cuenta de [!DNL Workfront] y puede iniciar sesión en ella desde la sección [!DNL Workfront] dentro de su [!UICONTROL oportunidad] o cuenta
.

## Configurando la creación de [!DNL Workfront] proyectos desde [!DNL Salesforce]

* [Explicación de la creación automática de proyectos](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Configuración de Déclencheur](#configuring-triggers-configuring-triggers)
* [Explicación de nombres de proyecto](#understanding-project-names-understanding-project-names)

### Explicación de la creación automática de proyectos {#understanding-the-automatic-creation-of-projects}

Como administrador del sistema de [!DNL Salesforce], puede definir déclencheur que puedan crear automáticamente proyectos en [!DNL Workfront] cuando sucedan las siguientes cosas en [!DNL Salesforce]:

* Se ha actualizado [!UICONTROL Stage] de [!UICONTROL Opportunity].
* El [!UICONTROL tipo] de una cuenta
se ha actualizado.

Los déclencheur solo se pueden configurar después de instalar [!DNL Workfront for Salesforce].  \
Para obtener información acerca de la instalación de [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Tenga en cuenta lo siguiente al configurar déclencheur para crear automáticamente [!DNL Workfront] proyectos cuando se creen o actualicen [!DNL Salesforce] elementos:

* Debe ser administrador de sistema de [!DNL Salesforce] y de [!DNL Workfront] para configurar las déclencheur.
* Después de configurar las déclencheur, cualquier persona que actualice la [!UICONTROL fase] de una [!UICONTROL oportunidad] o el [!UICONTROL tipo] de una cuenta
puede almacenar en déclencheur la creación de un proyecto [!DNL Workfront]. Esto incluye a [!DNL Salesforce] usuarios que no tienen una cuenta de [!DNL Workfront].
* No hay límite en cuanto a la cantidad de activadores que puede tener.
* No se pueden crear varios déclencheur basados en las mismas condiciones. Los déclencheur son únicos de forma predeterminada.
* Una vez creado el proyecto, se vincula automáticamente a la oportunidad o a la cuenta en la que se generó. Una vez establecido, este vínculo no se puede romper.
* Se puede vincular una oportunidad o cuenta a varios proyectos en [!DNL Workfront] si se ha cumplido varias veces una condición desencadenada en la duración de la oportunidad o de la cuenta.

  Por ejemplo, si define más de un [!UICONTROL escenario] para una [!UICONTROL oportunidad] de déclencheur de un proyecto, se creará un proyecto para cada etapa definida en la que llegue la oportunidad, durante la vida de dicha oportunidad. Además, si actualiza la [!UICONTROL fase] de una [!UICONTROL oportunidad] de una fase definida a otra y, a continuación, la actualiza de nuevo a la fase definida, se creará un segundo proyecto por segunda vez que actualice el campo [!UICONTROL fase] a la misma fase definida.

* Un proyecto de [!DNL Workfront] solo se puede vincular a una oportunidad o cuenta en [!DNL Salesforce] en un momento dado, pero no a ambas al mismo tiempo.

### Configuración de Déclencheur {#configuring-triggers}

Una vez configuradas las déclencheur, el proceso de creación de [!DNL Workfront] proyectos está habilitado para los marcos [!UICONTROL Salesforce Classic] o [!DNL Lightning Experience].

Para configurar déclencheur en [!UICONTROL Salesforce]:

1. Inicie sesión en [!DNL Salesforce] como administrador del sistema.
1. (Condicional) En [!DNL Salesforce Classic], haga clic en **[!UICONTROL Configuración]** y, en la sección **[!UICONTROL Generar]**, expanda **[!UICONTROL Rayo]**.

   O

   En [!DNL Salesforce] Lightning Experience, haz clic en el icono **[!UICONTROL Configuración]**, luego en **[!UICONTROL Configuración]** y en **[!UICONTROL HERRAMIENTAS DE PLATAFORMA]** para expandir **[!UICONTROL Aplicaciones]**.

1. Haga clic en **[!UICONTROL Paquetes instalados]**.

   Observe que el paquete **[!DNL Workfront]** se ha instalado.

1. Haga clic en **[!UICONTROL Configurar]** junto a **[!DNL Workfront]**.

1. Inicie sesión en [!DNL Workfront] como administrador del sistema.

   Se muestra la página **[!UICONTROL Déclencheur]**.

   ![salesforce_déclencheur_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Haga clic en **[!UICONTROL Nuevo Déclencheur]**.
1. En el menú desplegable **[!UICONTROL [!DNL Salesforce]Objeto]**, seleccione **[!UICONTROL Oportunidad]**.

   Este campo es obligatorio.

1. (Condicional) Especifique lo siguiente:

   1. En el menú desplegable **[!UICONTROL Fase]**, seleccione una **[!UICONTROL Fase]**.\

      Cuando una oportunidad llega a la [!UICONTROL fase] especificada aquí, se crea un proyecto en [!DNL Workfront]. Este campo es obligatorio.

   1. En el campo **[!UICONTROL Portfolio o Programa]**, empiece a escribir el nombre de un Portfolio o Programa en el que desee colocar el proyecto en [!DNL Workfront] y, a continuación, selecciónelo cuando aparezca en la lista.\

      Si no especifica un Portfolio o un programa, se creará el nuevo proyecto y se agregará a la lista [!UICONTROL Proyectos de mi propiedad] del usuario que inició sesión en [!DNL Workfront] al configurar las déclencheur. Ese usuario también es el propietario del proyecto nuevo.

   1. Empiece a escribir el nombre de la plantilla que desea asociar al nuevo proyecto [!DNL Workfront] y selecciónela cuando aparezca en la lista.\

      Este campo es obligatorio.


      >[!NOTE]
      >
      >Si ha especificado un Propietario de plantilla en la plantilla que planea utilizar para esta integración, se convertirá en el Propietario del proyecto del nuevo proyecto. Los nuevos proyectos aparecerán en la lista [!UICONTROL Proyectos de mi propiedad] del usuario que es el propietario del nuevo proyecto, según la plantilla.

   1. (Opcional) Seleccione el campo **[!UICONTROL Crear un nuevo proyecto para cada tipo de producto vendido]**, si desea crear un nuevo proyecto para cada tipo de producto vendido bajo cualquier oportunidad.
   1. (Condicional) Seleccione un **[!UICONTROL Producto]** en el menú desplegable **[!UICONTROL Producto]**.

      Este campo es obligatorio.

   1. (Condicional) Empiece a escribir el nombre de una **[!UICONTROL plantilla]** que desee asociar con el nuevo proyecto [!DNL Workfront] si el producto especificado se encuentra en la [!UICONTROL oportunidad]. Selecciónelo cuando aparezca en la lista.

      Este campo es obligatorio.

      El proyecto creado cuando se agrega un nuevo producto a la oportunidad [!DNL Salesforce] se coloca en el mismo Portfolio o programa seleccionado para la oportunidad.

      >[!IMPORTANT]
      >
      >El proyecto se crea solamente cuando el escenario se actualiza en [!UICONTROL Oportunidad]. Se crea un proyecto único para cada producto especificado cuando se actualiza el campo Fase y no cuando los productos se agregan a [!UICONTROL Oportunidades].

1. (Opcional) Haga clic en **[!UICONTROL Nuevo Déclencheur]**.
1. (Opcional) En el menú desplegable **[!UICONTROL [!DNL Salesforce]Objeto]**, seleccione **Cuenta
**.

   Este campo es obligatorio.
1. (Condicional) Especifique lo siguiente:

   1. Seleccione un **[!UICONTROL Tipo]** del menú desplegable **[!UICONTROL Tipo]**.

      Cuando cualquier **Cuenta
** se designa como **[!UICONTROL Tipo]** especificado aquí en [!DNL Salesforce], se crea un **[!UICONTROL Proyecto]** en [!DNL Workfront].

      Este campo es obligatorio.

   1. (Opcional) Empiece a escribir el nombre de un **[!UICONTROL Portfolio]** o **[!UICONTROL Programa]** en el que desee colocar el proyecto en [!DNL Workfront] en el campo **[!UICONTROL Portfolio o Programa]** y, a continuación, selecciónelo cuando aparezca en la lista.

      Si no especifica un Portfolio o un programa, el nuevo proyecto se creará y se agregará a la lista **[!UICONTROL Proyectos de mi propiedad]** del usuario que inició sesión en [!DNL Workfront] desde [!DNL Salesforce]. El usuario también es el propietario del proyecto para el nuevo proyecto.

   1. Empiece a escribir el nombre de una **[!UICONTROL plantilla]** que desee asociar con el nuevo proyecto [!DNL Workfront] y, a continuación, selecciónela cuando aparezca en la lista.

      Este campo es obligatorio.

      >[!NOTE]
      >
      >Si ha especificado un Propietario de plantilla en la plantilla que planea utilizar para esta integración, se convertirá en el Propietario del proyecto del nuevo proyecto. Los nuevos proyectos aparecerán en la lista **[!UICONTROL Proyectos de mi propiedad]** del usuario que es el propietario del nuevo proyecto, según la plantilla.

   ![salesforce_déclencheur_page_with_cleanup_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Haga clic en **[!UICONTROL Guardar]**.

   Ahora se generan [!DNL Workfront] proyectos cada vez que se cumple cualquiera de los déclencheur.

### Explicación de nombres de proyecto {#understanding-project-names}

Dependiendo del déclencheur que haya generado los proyectos, los nombres de los proyectos en [!DNL Workfront] podrían seguir uno de estos patrones:

* Si el proyecto se crea a partir de un déclencheur de oportunidad o cuenta, el nombre del proyecto es: *`<Salesforce object name>`: `<Project template name>` (a través de [!DNL Salesforce])*.
* Si el proyecto se crea a partir de un déclencheur de oportunidades que también incluye la adición de un nuevo producto, el nombre del proyecto es: *`<Salesforce object name>`: `<Salesforce product name>` (a través de [!DNL Salesforce])*.

## Ver [!DNL Workfront] proyectos

Si el administrador de [!DNL Workfront] agregó la sección [!DNL Workfront] a su [!UICONTROL oportunidad] o cuenta
Diseño de página, puede ver los proyectos creados automáticamente en la pestaña [!UICONTROL Proyectos] de esta sección.\
Para obtener más información acerca de cómo agregar la sección [!DNL Workfront] al diseño de página de una [!UICONTROL oportunidad] o cuenta
, vea [Configurar la sección [!DNL Adobe Workfront] para [!DNL Salesforce] usuarios](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

Debe tener una cuenta de [!DNL Workfront] y haber iniciado sesión en [!DNL Workfront] para ver la ficha [!UICONTROL Proyectos].

Para ver los proyectos creados a partir de una [!UICONTROL oportunidad] o cuenta
:

1. Ir a [!UICONTROL oportunidad] o cuenta
.
1. Vaya a la sección **[!DNL Workfront]**.

   >[!NOTE]
   >
   >Dependiendo de cómo haya configurado el administrador de [!DNL Workfront] esta sección, podría tener un nombre diferente.

1. Seleccione la ficha **[!UICONTROL Proyectos]**.

   Todos los proyectos creados por déclencheur definidos se muestran en esta pestaña. Cualquier usuario de [!DNL Salesforce] que también tenga una cuenta de [!DNL Workfront] y que tenga permisos para ver estos proyectos en [!DNL Workfront] también puede verlos en [!DNL Salesforce] para la [!UICONTROL oportunidad] o la cuenta
que los generó.

   Puede ver la siguiente información sobre los proyectos creados por la integración:

   * Nombre del proyecto
   * Número de referencia
   * Fecha de entrada
   * Nombre del propietario
   * Estado
   * Condición
   * Fecha planificada de finalización
   * Porcentaje completado

     Cuando se actualice esta información en [!DNL Workfront], podrá ver los campos actualizados en esta lista.

1. (Opcional) Haga clic en el nombre de un proyecto para abrirlo en Workfront.
1. (Opcional) Haga clic en [!UICONTROL **[!UICONTROL Ir a Salesforce]**] en el área de [!UICONTROL Detalles del proyecto] o en el encabezado del proyecto para acceder a [!UICONTROL Oportunidad] o a la cuenta
donde se originó el proyecto. El administrador del sistema o del grupo debe agregar el campo [!UICONTROL Integraciones] a la plantilla de diseño para encontrarlo en el encabezado del proyecto.

   >[!NOTE]
   >
   >El vínculo [!UICONTROL Ir a Salesforce] es visible para todos los usuarios de [!DNL Workfront] que pueden ver el proyecto. Debe tener una cuenta de [!DNL Salesforce] para poder ir a la oportunidad o cuenta de [!DNL Salesforce] desde la que se generó el proyecto.
