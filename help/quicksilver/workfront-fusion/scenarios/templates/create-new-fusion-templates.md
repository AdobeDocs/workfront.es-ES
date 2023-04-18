---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Cree nuevas plantillas en [!DNL Adobe Workfront Fusion]
description: Puede crear nuevas plantillas de escenario en [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: 612de6a98965552da6d534d9d2536237a96f7715
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 0%

---

# Cree nuevas plantillas en [!DNL Adobe Workfront Fusion]

Puede crear nuevas plantillas de escenario en [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Antes de crear una plantilla nueva, puede comprobar la variable [!UICONTROL Plantillas públicas] para asegurarse de que la plantilla que desea crear no está disponible.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

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
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Crear una plantilla nueva

Puede crear una plantilla en un proceso similar a la creación de un escenario. Los administradores de Fusion también pueden crear plantillas a partir de escenarios existentes.

* [Creación de una plantilla](#build-a-template)
* [Creación de una plantilla a partir de un escenario](#create-a-template-from-a-scenario)

### Creación de una plantilla

1. Haga clic en **[!UICONTROL Plantillas]** ![](assets/fusion-template-icon.png) en el panel de navegación izquierdo.
1. Haga clic en **[!UICONTROL Crear una plantilla nueva]** en la esquina superior derecha.
1. (Opcional) Cambie el nombre de la plantilla reemplazando el valor predeterminado **[!UICONTROL Nuevo nombre de plantilla]** en la esquina superior izquierda.
1. (Opcional) Para cambiar el idioma de la plantilla, haga clic en **[!UICONTROL Configuración de una plantilla]** ![](assets/fusion-scenario-settings-icon.png) y seleccione el idioma en la lista desplegable Idioma .

   >[!IMPORTANT]
   >
   >La selección de Idiomas corresponde a los idiomas disponibles en la configuración del sistema y afecta únicamente al nombre de la plantilla pública y su descripción. Una vez guardada la plantilla, no se puede cambiar un idioma de plantilla.

1. (Opcional) Para introducir una descripción de la plantilla, haga clic en **[!UICONTROL Configuración de una plantilla]** ![](assets/fusion-scenario-settings-icon.png) e introduzca la descripción.
1. Agregue aplicaciones, módulos y herramientas del mismo modo que haría al crear un escenario estándar.

   Para añadir ayuda contextual a los módulos, consulte [Configuración [!UICONTROL Asistente] funcionalidad](#set-up-wizard-functionality) en este artículo.

   Para obtener más información sobre la creación de un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Si la plantilla incluye módulos que requieren la adición de la conexión, las credenciales u otra información confidencial, esta información no se comparte con los usuarios de la plantilla.

1. (Opcional) Haga clic en **[!UICONTROL Ejecutar una vez]** para probar la plantilla.
1. Haga clic en el **[!UICONTROL Guardar]** icono ![](assets/save-icon.png).

>[!NOTE]
>
>Al guardar la plantilla, la hace visible para todos los integrantes del equipo. Si desea que la plantilla sea accesible fuera del equipo, debe publicarla y, a continuación, utilizar un vínculo compartido, o solicitar al administrador que apruebe y publique la plantilla.

### Creación de una plantilla a partir de un escenario

>[!NOTE]
>
>Debe ser administrador de Fusion para crear una plantilla a partir de un escenario.

1. Abra la página de detalles del escenario desde la que desea crear el escenario.
1. Haga clic en el **Administrador** desplegable cerca de la esquina superior derecha de la página.
1. Select **Clonar como plantilla**.

   El escenario se copia en una página Nueva plantilla .
1. (Opcional) Cambie el nombre de la plantilla reemplazando el valor predeterminado **[!UICONTROL Nuevo nombre de plantilla]** en la esquina superior izquierda.
1. (Opcional) Para cambiar el idioma de la plantilla, haga clic en **[!UICONTROL Configuración de una plantilla]** ![](assets/fusion-scenario-settings-icon.png) y seleccione el idioma en la lista desplegable Idioma .

   >[!IMPORTANT]
   >
   >La selección de Idiomas corresponde a los idiomas disponibles en la configuración del sistema y afecta únicamente al nombre de la plantilla pública y su descripción. Una vez guardada la plantilla, no se puede cambiar un idioma de plantilla.

1. (Opcional) Para introducir una descripción de la plantilla, haga clic en **[!UICONTROL Configuración de una plantilla]** ![](assets/fusion-scenario-settings-icon.png) e introduzca la descripción.
1. Edite aplicaciones, módulos y herramientas del mismo modo que lo haría al editar un escenario estándar.

   Para añadir ayuda contextual a los módulos, consulte [Configuración [!UICONTROL Asistente] funcionalidad](#set-up-wizard-functionality) en este artículo.

   >[!NOTE]
   >
   >Si la plantilla incluye módulos que requieren la adición de la conexión, las credenciales u otra información confidencial, esta información no se comparte con los usuarios de la plantilla.

1. (Opcional) Haga clic en **[!UICONTROL Ejecutar una vez]** para probar la plantilla.
1. Haga clic en el **[!UICONTROL Guardar]** icono ![](assets/save-icon.png).

## Configuración [!UICONTROL Asistente] funcionalidad {#set-up-wizard-functionality}

La variable [!DNL Workfront Fusion template] [!UICONTROL Asistente] permite proporcionar a los usuarios futuros de la plantilla instrucciones o información relacionada con los campos específicos utilizados en los módulos.

1. Haga clic en el módulo agregado a la plantilla para ver los campos del módulo.
1. Busque el campo al que desea agregar [!UICONTROL Asistente] y habilitar **[!UICONTROL Uso en el asistente]** para ese campo.
1. Introduzca la información que desea que sea visible para los usuarios en el [!UICONTROL Ayuda] campo .
1. (Opcional) Para permitir que los usuarios vean este texto al usar la plantilla, active **[!UICONTROL Utilizar como valor predeterminado]**.
1. Repita los pasos del 2 al 4 para cada campo para el que desee proporcionar información.
1. Haga clic en **[!UICONTROL OK]** para guardar los cambios y cerrar el módulo.
