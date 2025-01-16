---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Crear nuevas plantillas en  [!DNL Adobe Workfront Fusion]
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 14%

---

# Crear nuevas plantillas en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Crear nuevas plantillas](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-and-manage-templates/create-new-fusion-templates.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Puede crear nuevas plantillas de escenario en [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Antes de crear una plantilla nueva, puede comprobar la ficha [!UICONTROL Plantillas públicas] para asegurarse de que la plantilla que desea crear no esté disponible.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia** de [!UICONTROL Adobe Workfront Fusion]</td> 
  <td>
   <p>Requisito de licencia actual: no se requiere la licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber de qué plan, tipo de licencia o acceso dispone, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Crear una plantilla nueva

Puede crear una plantilla en un proceso similar a la creación de un escenario. Los administradores de Fusion también pueden crear plantillas a partir de escenarios existentes.

* [Creación de una plantilla](#build-a-template)
* [Creación de una plantilla a partir de un escenario](#create-a-template-from-a-scenario)

### Creación de una plantilla

1. Haga clic en **[!UICONTROL Plantillas]** ![](assets/fusion-template-icon.png) en el panel de navegación izquierdo.
1. Haga clic en **[!UICONTROL Crear una nueva plantilla]** en la esquina superior derecha.
1. (Opcional) Cambie el nombre de la plantilla reemplazando el **[!UICONTROL Nuevo nombre de plantilla]** predeterminado en la esquina superior izquierda.
1. (Opcional) Para cambiar el idioma de la plantilla, haga clic en **[!UICONTROL Configurar una plantilla]** ![](assets/fusion-scenario-settings-icon.png) y seleccione el idioma en la lista desplegable Idioma.

   >[!IMPORTANT]
   >
   >La selección Idiomas corresponde a los idiomas disponibles en la configuración del sistema y afecta únicamente al nombre de la plantilla pública y su descripción. No puede cambiar un idioma de plantilla una vez guardada la plantilla.

1. (Opcional) Para escribir una descripción de la plantilla, haga clic en **[!UICONTROL Configurar una plantilla]** ![](assets/fusion-scenario-settings-icon.png) e introduzca la descripción.
1. Agregue aplicaciones, módulos y herramientas del mismo modo que lo haría al crear un escenario estándar.

   Para agregar ayuda contextual a los módulos, consulte [Configurar la funcionalidad del [!UICONTROL Asistente]](#set-up-wizard-functionality) en este artículo.

   Para obtener más información sobre cómo crear un escenario, vea [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Si la plantilla incluye módulos que requieren agregar la conexión, las credenciales u otra información confidencial, esta información no se comparte con los usuarios de la plantilla.

1. (Opcional) Haga clic en **[!UICONTROL Ejecutar una vez]** para probar la plantilla.
1. Haga clic en el icono **[!UICONTROL Guardar]** ![](assets/save-icon.png).

>[!NOTE]
>
>Al guardar la plantilla, se hace visible para todos los integrantes del equipo. Si desea que la plantilla sea accesible fuera del equipo, debe enviar una solicitud para que se apruebe y publique. La solicitud llega a Adobe Workfront para su aprobación y, una vez aprobada, otras personas externas al equipo pueden acceder a ella.
>
>Para obtener información sobre cómo publicar plantillas, consulte [Publish y compartir [!DNL Adobe Workfront Fusion] plantillas](/help/quicksilver/workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

### Creación de una plantilla a partir de un escenario

>[!NOTE]
>
>Debe ser administrador de Fusion para crear una plantilla a partir de un escenario.

1. Abra la página de detalles del escenario desde el que desea crear un escenario.
1. Haga clic en el menú desplegable **Administrador** situado cerca de la esquina superior derecha de la página.
1. Seleccione **Clonar como plantilla**.

   El escenario se copia en una página Nueva plantilla.
1. (Opcional) Cambie el nombre de la plantilla reemplazando el **[!UICONTROL Nuevo nombre de plantilla]** predeterminado en la esquina superior izquierda.
1. (Opcional) Para cambiar el idioma de la plantilla, haga clic en **[!UICONTROL Configurar una plantilla]** ![](assets/fusion-scenario-settings-icon.png) y seleccione el idioma en la lista desplegable Idioma.

   >[!IMPORTANT]
   >
   >La selección Idiomas corresponde a los idiomas disponibles en la configuración del sistema y afecta únicamente al nombre de la plantilla pública y su descripción. No puede cambiar un idioma de plantilla una vez guardada la plantilla.

1. (Opcional) Para escribir una descripción de la plantilla, haga clic en **[!UICONTROL Configurar una plantilla]** ![](assets/fusion-scenario-settings-icon.png) e introduzca la descripción.
1. Edite aplicaciones, módulos y herramientas del mismo modo que lo haría al editar un escenario estándar.

   Para agregar ayuda contextual a los módulos, consulte [Configurar la funcionalidad del [!UICONTROL Asistente]](#set-up-wizard-functionality) en este artículo.

   >[!NOTE]
   >
   >Si la plantilla incluye módulos que requieren agregar la conexión, las credenciales u otra información confidencial, esta información no se comparte con los usuarios de la plantilla.

1. (Opcional) Haga clic en **[!UICONTROL Ejecutar una vez]** para probar la plantilla.
1. Haga clic en el icono **[!UICONTROL Guardar]** ![](assets/save-icon.png).

## Configurar la funcionalidad de [!UICONTROL Wizard] {#set-up-wizard-functionality}

El [!DNL Workfront Fusion template] [!UICONTROL Asistente] le permite proporcionar a futuros usuarios de su plantilla instrucciones o información relacionada con los campos específicos utilizados en los módulos.

1. Haga clic en el módulo agregado a la plantilla para ver los campos del módulo.
1. Busque el campo donde desea agregar información de [!UICONTROL Wizard] y habilite **[!UICONTROL Usar en Wizard]** para ese campo.
1. Escriba la información que desea que sea visible para los usuarios en el campo [!UICONTROL Ayuda].
1. (Opcional) Para permitir que los usuarios vean este texto al usar la plantilla, habilite **[!UICONTROL Usar como valor predeterminado]**.
1. Repita los pasos 2-4 para cada campo para el que desee proporcionar información.
1. Haga clic en **[!UICONTROL Aceptar]** para guardar los cambios y cerrar el módulo.
