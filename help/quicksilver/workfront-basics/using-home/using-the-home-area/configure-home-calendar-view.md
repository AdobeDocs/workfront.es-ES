---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Configurar las opciones de vista del Calendario de inicio
description: Puede configurar la configuración del Calendario de inicio para integrarla con una versión de Outlook basada en Web y ayudarle a realizar un seguimiento de la carga de trabajo en relación con las horas de trabajo disponibles.
author: Lisa
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# Configure las [!UICONTROL Calendario principal] configuración de vista

Puede configurar la variable [!UICONTROL Calendario principal] para hacer lo siguiente:

* Integración con una versión web de [!DNL Outlook] en nube [!DNL Office 365] o [!DNL Outlook Live]. Puede mostrar todos los eventos del calendario de Outlook y cualquier calendario asociado que seleccione, como los calendarios de cumpleaños y días festivos, en su [!UICONTROL Calendario principal].
* Ayudarle a realizar un seguimiento de la carga de trabajo en relación con las horas de trabajo disponibles en [!UICONTROL Asignación] barra.

Para obtener más información sobre el Calendario de inicio, consulte [[!UICONTROL Calendario principal] ver](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Work] o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan o tipo de licencia tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Acerca de la integración [!DNL Microsoft Outlook] calendarios

Tenga en cuenta lo siguiente a la hora de configurar el Calendario de inicio con su [!DNL Microsoft Outlook] calendario:

* Solo puede integrar una versión basada en web de [!DNL Outlook] en nube [!DNL Office 365] o [!DNL Outlook Live].

   Local [!DNL Outlook] y [!DNL Outlook] en una empresa basada en la nube [!DNL Exchange] no son compatibles.

   Si su organización utiliza el inicio de sesión único, necesita [!DNL Microsoft 365 E3] o [!DNL E5].

* Archivos adjuntos asociados con su [!DNL Outlook] no se adjuntan al [!DNL Outlook] en su Calendario de inicio.
* Integración con un [!DNL Outlook] el calendario debe completarse para cada usuario individualmente.
* Eventos que aparecen en la variable [!UICONTROL Vencido] no aparecen en su [!DNL Microsoft] a menos que los haya arrastrado desde el [!UICONTROL Lista de trabajo] a su [!DNL Adobe Workfront] Calendario. Para obtener más información, consulte [[!UICONTROL Vencido] barra](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) y [Lista de trabajo de [!UICONTROL Calendario principal]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) en [[!UICONTROL Calendario principal] ver](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Al habilitar la integración con [!DNL Outlook], solo los elementos de trabajo que se arrastran al [!UICONTROL Calendario principal] a partir de ese momento, se sincronizará. Los elementos que estaban en el Calendario de inicio antes de habilitar la integración no aparecerán y debe arrastrarlos de nuevo al Calendario de inicio si desea que aparezcan en [!DNL Outlook].
* Cuando comparte (o deja de compartir) un [!DNL Outlook] calendario con otras personas, o cuando cambia el nivel de permiso de un calendario que comparte con otras personas, este cambio no afecta a sus calendarios durante unos 30 minutos (para obtener más información, consulte la [!DNL Microsoft Outlook] documentación).\
   Por lo tanto, al integrar [!DNL Workfront] Calendario con un [!DNL Outlook] que comparta con otros usuarios, no verán su [!DNL Workfront] Elementos del calendario durante unos 30 minutos.

>[!NOTE]
>
>La variable [!DNL Outlook] la configuración del calendario es completamente independiente de [!DNL Outlook] Complemento ([!UICONTROL [!DNL Outlook] Integración] o [!DNL Workfront Outlook]). No se requiere instalación para configurar el calendario, pero se necesita una instalación para el [!DNL Outlook] Complemento. Para obtener más información sobre [!DNL Outlook] Consulte el complemento [Configuración [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Configure las [!UICONTROL Calendario principal] configuración de vista

1. En el [!UICONTROL Calendario principal] haga clic en la **[!UICONTROL Configuración]** icono de engranaje ![Calendar_Settings_engranaje_icon.png](assets/calendar-settings-gear-icon.png) en la esquina superior derecha para abrir **[!UICONTROL Configuración del calendario]** en el lado derecho de la ventana.

   Si necesita información sobre cómo acceder a la variable [!UICONTROL Calendario principal] ver, consulte [Consulte la [!UICONTROL Calendario principal]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Opcional) Para integrar su [!DNL Microsoft Outlook] calendario, haga clic en **[!UICONTROL Agregar cuenta]** en la esquina superior derecha del **[!UICONTROL Configuración del calendario]** panel. A continuación, si se le solicita que lo haga, introduzca su [!DNL Microsoft Outlook] información de inicio de sesión. Puede repetir este paso para agregar varias [!DNL Outlook] cuentas.

   >[!NOTE]
   >
   >Debe dar [!DNL Workfront] permiso para acceder a su [!DNL Outlook] calendario. La concesión de permisos permite [!DNL Workfront] para mantener el acceso a los datos del calendario, lea su [!DNL outlook] y lea y actualice su [!DNL Microsoft] calendario.

1. Actualice la ventana del explorador para ver la información de su [!DNL Outlook] en el calendario y en la [!UICONTROL Configuración del calendario] panel.
1. Haga clic en el **[!UICONTROL Configuración]** icono de engranaje de nuevo en la esquina superior derecha para abrir el **[!UICONTROL Configuración del calendario]** panel. ![Calendar_Settings_engranaje_icon.png](assets/calendar-settings-gear-icon.png)

1. (Opcional) Debajo de cada [!DNL Microsoft] cuenta agregada en el paso anterior, seleccione **[!UICONTROL Ver]** o **[!UICONTROL Sincronización]**:

   * **[!UICONTROL Ver]**: Esta es una opción de solo lectura que se muestra [!DNL Microsoft] eventos de calendario [!UICONTROL Calendario principal].
   * **[!UICONTROL Sincronización]**: Esta opción permite una sincronización bidireccional entre las [!DNL Microsoft] y [!UICONTROL Página principal] calendarios. En otras palabras, [!DNL Workfront] [!UICONTROL Calendario principal] los artículos exportan a su [!DNL Microsoft] calendario y [!DNL Microsoft] importación de elementos de calendario a Workfront [!UICONTROL Calendario principal] en tiempo real.

      ![](assets/view-sync-checkboxes-qs.png)

1. (Opcional) En [!DNL Workfront] o una cuenta integrada, seleccione los calendarios asociados que desee ver en su [!UICONTROL Calendario principal] (como su PTO, cumpleaños o calendario festivo) y luego haga clic en el [!UICONTROL Actualizar] o [!UICONTROL Volver a cargar] para ver los cambios.

1. (Opcional) En la **[!UICONTROL General]** sección bajo **[!UICONTROL Iniciar semana en]**, seleccione el día que desee mostrar como el primer día de la semana laboral en el Calendario de inicio.

1. Configure las siguientes opciones:

   * **[!UICONTROL Mis días de trabajo]:** Seleccione los días de trabajo.
   * **[!UICONTROL Mi hora de inicio habitual]:** Seleccione la hora a la que inicia el día laboral.
   * **[!UICONTROL Mi hora de finalización habitual]:** Seleccione la hora a la que termina el día laboral.

   [!DNL Workfront] utiliza estos tres ajustes para calcular el número de horas que trabaja en una semana. Este número afecta a la variable [!UICONTROL Asignación] , lo que le ayuda a realizar un seguimiento de la carga de trabajo en relación con las horas de trabajo disponibles. Para obtener más información, consulte [[!UICONTROL Asignación] barra](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) en el artículo [[!UICONTROL Calendario principal] ver](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Haga clic fuera del **[!UICONTROL Configuración del calendario]** para descartarla.

   [!DNL Workfront] guarda los cambios automáticamente.

Para obtener información sobre cómo usar la variable [!UICONTROL Calendario] para administrar las asignaciones de trabajo y los eventos de calendario integrados, consulte [Utilice la variable [!UICONTROL Calendario principal] ver](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
