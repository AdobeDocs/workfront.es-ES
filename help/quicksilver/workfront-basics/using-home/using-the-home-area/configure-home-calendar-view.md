---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Configurar la configuración de la vista Calendario de Inicio
description: Puede configurar la configuración del Calendario principal para que se integre con una versión de Outlook basada en Web y le ayude a realizar un seguimiento de la carga de trabajo en relación con las horas de trabajo disponibles.
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# Configurar la configuración de vista de [!UICONTROL Calendario principal]

<!--Audited: 01/2024-->

Puede configurar la configuración de [!UICONTROL Calendario principal] para hacer lo siguiente:

* Integrarlo con una versión web de [!DNL Outlook], [!DNL Office 365] en la nube o [!DNL Outlook Live]. Puede mostrar todos los eventos del calendario de Outlook y de los calendarios asociados que seleccione en su [!UICONTROL Calendario principal] en Adobe Workfront.
* Ayudarle a realizar un seguimiento de la carga de trabajo en relación con las horas de trabajo disponibles en la barra [!UICONTROL Asignación].

Para obtener más información sobre el Calendario principal, consulte [[!UICONTROL Calendario principal] ver](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

En este artículo se describe cómo configurar el Calendario principal e integrar el Calendario principal con el calendario externo de Outlook.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>Actual: [!UICONTROL Work] o superior</p> 
   O
   <p>Nuevo: [!UICONTROL Standard]</p> 
   </td> 
  </tr> 
   </tbody> 
</table>

*Para averiguar qué plan o tipo de licencia tiene, póngase en contacto con el administrador de [!DNL Workfront]. Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Acerca de la integración de [!DNL Microsoft Outlook] calendarios

Tenga en cuenta lo siguiente al configurar el Calendario de Inicio con el calendario [!DNL Microsoft Outlook]:

* Solo puede integrar una versión basada en web de [!DNL Outlook] en [!DNL Office 365] o [!DNL Outlook Live] alojados en la nube.

  No se admiten [!DNL Outlook] locales ni [!DNL Outlook] en un servidor [!DNL Exchange] empresarial basado en la nube.

  Si su organización utiliza el inicio de sesión único, necesita [!DNL Microsoft 365 E3] o [!DNL E5].

* Los archivos adjuntos asociados con los eventos de [!DNL Outlook] no se adjuntan a los eventos de [!DNL Outlook] del Calendario principal.
* La integración con un calendario [!DNL Outlook] se debe completar para cada usuario de forma individual.
* Los eventos que aparecen en la barra [!UICONTROL Due] no aparecen en el calendario [!DNL Microsoft] a menos que los haya arrastrado desde la [!UICONTROL Lista de trabajos] hasta el calendario [!DNL Adobe Workfront]. Para obtener más información, consulte [[!UICONTROL Vencimiento] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) y [Lista de trabajos en el [!UICONTROL Calendario principal]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) en la vista [[!UICONTROL Calendario principal]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Al habilitar la integración con [!DNL Outlook], solo se sincronizarán los elementos de trabajo que se arrastran al [!UICONTROL Calendario principal] a partir de ese momento. Los elementos que estaban en el Calendario principal antes de habilitar la integración no aparecerán y deberá arrastrarlos de nuevo al Calendario principal si desea que aparezcan en [!DNL Outlook].
* Cuando comparte (o deja de compartir) un calendario [!DNL Outlook] con otras personas, o cuando cambia el nivel de permisos de un calendario que comparte con otras personas, este cambio no afecta a sus calendarios durante unos 30 minutos. Para obtener más información, consulte la documentación de [!DNL Microsoft Outlook].\
   En consecuencia, cuando integre el calendario [!DNL Workfront] con un calendario [!DNL Outlook] que comparta con otros usuarios, no verán los elementos de su calendario [!DNL Workfront] durante unos 30 minutos.

>[!NOTE]
>
>La configuración del calendario [!DNL Outlook] es completamente independiente del complemento [!DNL Outlook] ([!UICONTROL [!DNL Outlook] integración] o [!DNL Workfront Outlook]). No se requiere instalación para configurar el calendario, pero se necesita una instalación para el complemento [!DNL Outlook]. Para obtener más información sobre el complemento [!DNL Outlook], consulte [Configurar [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Configure la configuración de vista de [!UICONTROL Calendario principal] e integre la configuración con los calendarios de Outlook

1. En la vista [!UICONTROL Calendario principal], haga clic en el icono de engranaje de **[!UICONTROL Configuración]** ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png) en la esquina superior derecha para abrir el panel de **[!UICONTROL Configuración del calendario]** a la derecha.

   Si necesita información sobre cómo obtener acceso a la vista de [!UICONTROL Calendario principal], consulte [Ver el [!UICONTROL Calendario principal]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Opcional) Para integrar su calendario [!DNL Microsoft Outlook], haga clic en **[!UICONTROL Agregar cuenta]** en la esquina superior derecha del panel **[!UICONTROL Configuración del calendario]**. A continuación, si se le solicita, escriba su información de inicio de sesión de [!DNL Microsoft Outlook]. Puede repetir este paso para agregar varias cuentas de [!DNL Outlook].

   >[!NOTE]
   >
   >Debe dar permiso a [!DNL Workfront] para acceder a su calendario [!DNL Outlook]. Conceder permiso permite que [!DNL Workfront] mantenga el acceso a los datos del calendario, lea su perfil de [!DNL outlook] y lea y actualice su calendario de [!DNL Microsoft].

1. Actualice la ventana del explorador para ver información de su cuenta de [!DNL Outlook] en el calendario y en el panel [!UICONTROL Configuración del calendario].
1. Vuelva a hacer clic en el icono de engranaje **[!UICONTROL Configuración]** en la esquina superior derecha para abrir el panel **[!UICONTROL Configuración del calendario]**. ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. (Opcional) En cada cuenta de [!DNL Microsoft] que haya agregado en el paso anterior, seleccione **[!UICONTROL Ver]** o **[!UICONTROL Sincronizar]**:

   * **[!UICONTROL Ver]**: Esta es una opción de solo lectura que muestra [!DNL Microsoft] eventos de calendario en su [!UICONTROL Calendario principal].
   * **[!UICONTROL Sincronizar]**: esta opción permite una sincronización bidireccional entre los calendarios [!DNL Microsoft] y [!UICONTROL Inicio]. En otras palabras, [!DNL Workfront] [!UICONTROL Calendario principal] elementos se exportan a su calendario [!DNL Microsoft] y [!DNL Microsoft] elementos de calendario se importan a su Workfront [!UICONTROL Calendario principal] en tiempo real.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Opcional) En su cuenta de [!DNL Workfront] o en una cuenta integrada, seleccione los calendarios asociados que desee ver en su [!UICONTROL Calendario principal] (como el calendario de PTO, cumpleaños o festivos) y, a continuación, haga clic en el botón [!UICONTROL Actualizar] o [!UICONTROL Recargar] del explorador para ver los cambios.

1. (Opcional) En la sección **[!UICONTROL General]** de **[!UICONTROL Comenzar la semana el]**, seleccione el día que desee mostrar como primer día de la semana laboral en el Calendario principal.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. Configure las siguientes opciones:

   * **[!UICONTROL Mis días laborables]:** Seleccione los días que trabaje.
   * **[!UICONTROL Mi hora habitual de inicio]:** Seleccione la hora a la que comienza el día laborable.
   * **[!UICONTROL Mi hora final habitual]:** Seleccione la hora a la que finalizará el día laborable.

   [!DNL Workfront] usa estas tres opciones para calcular la cantidad de horas que trabaja en una semana. Este número afecta a la barra [!UICONTROL Asignación], lo que le ayuda a realizar un seguimiento de la carga de trabajo en relación con las horas de trabajo disponibles. Para obtener más información, consulte [[!UICONTROL Asignación] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) en el artículo [[!UICONTROL Calendario principal] vista](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Haga clic fuera del área **[!UICONTROL Configuración del calendario]** para cerrarla.

   [!DNL Workfront] guarda los cambios automáticamente.

Para obtener información sobre cómo usar la vista [!UICONTROL Calendario] para administrar las asignaciones de trabajo y los eventos de calendario integrados, consulte [Usar la vista [!UICONTROL Calendario principal]](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
