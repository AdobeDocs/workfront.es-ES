---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Configurar la configuración de la vista Calendario de Inicio
description: Puede configurar la configuración del Calendario principal para que se integre con una versión de Outlook basada en Web y le ayude a realizar un seguimiento de la carga de trabajo en relación con las horas de trabajo disponibles.
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 3b3ba7cc6a975af71205f7f524e1a9a91a9d3810
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 1%

---

# Configure su [!UICONTROL Calendario principal] configuración de vista

<!--Audited: 01/2024-->

Puede configurar las variables [!UICONTROL Calendario principal] Configuración para hacer lo siguiente:

* Integrarlo con una versión web de [!DNL Outlook], [!DNL Office 365] en la nube o [!DNL Outlook Live]. Puede mostrar todos los eventos del calendario de Outlook y de los calendarios asociados que seleccione en su [!UICONTROL Calendario principal] en Adobe Workfront.
* Le ayuda a realizar un seguimiento de la carga de trabajo en comparación con las horas de trabajo disponibles en [!UICONTROL Asignación] barra.

Para obtener más información sobre el Calendario de Inicio, consulte [[!UICONTROL Calendario principal] vista](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

En este artículo se describe cómo configurar el Calendario principal e integrar el Calendario principal con el calendario externo de Outlook.

## Requisitos de acceso

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

*Para saber qué plan o tipo de licencia tiene, póngase en contacto con su [!DNL Workfront] administrador. Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Acerca de la integración [!DNL Microsoft Outlook] calendarios

Tenga en cuenta lo siguiente al configurar el Calendario de Inicio con su [!DNL Microsoft Outlook] calendario:

* Solo se puede integrar una versión basada en web de [!DNL Outlook] en alojados en la nube [!DNL Office 365] o [!DNL Outlook Live].

  On-Premise [!DNL Outlook] y [!DNL Outlook] en una empresa basada en la nube [!DNL Exchange] servidor no son compatibles.

  Si su organización utiliza el inicio de sesión único, necesita lo siguiente [!DNL Microsoft 365 E3] o [!DNL E5].

* Archivos adjuntos asociados con su [!DNL Outlook] Los eventos de no se adjuntan al [!DNL Outlook] eventos en el Calendario de Inicio.
* Integración con un [!DNL Outlook] el calendario debe completarse individualmente para cada usuario.
* Eventos que aparecen en la [!UICONTROL Vencimiento] no aparecen en su [!DNL Microsoft] calendario a menos que los haya arrastrado desde el [!UICONTROL Lista de trabajos] a su [!DNL Adobe Workfront] Calendario. Para obtener más información, consulte [[!UICONTROL Vencimiento] barra](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) y [Lista de trabajos en [!UICONTROL Calendario principal]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) in [[!UICONTROL Calendario principal] vista](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Al habilitar la integración con [!DNL Outlook], solo los elementos de trabajo que se arrastran a [!UICONTROL Calendario principal] a partir de ese momento se sincronizará. Los elementos que estaban en el Calendario principal antes de habilitar la integración no aparecerán y debe arrastrarlos de nuevo al Calendario principal si desea que aparezcan en [!DNL Outlook].
* Al compartir (o dejar de compartir) un [!DNL Outlook] calendario con otras personas o cuando cambia el nivel de permisos de un calendario que comparte con otras personas, este cambio no afecta a sus calendarios durante unos 30 minutos. Para obtener más información, consulte la [!DNL Microsoft Outlook] documentación.\
   Por lo tanto, al integrar [!DNL Workfront] Calendario con un [!DNL Outlook] calendario que comparta con otros usuarios, no verán su [!DNL Workfront] Elementos de calendario durante unos 30 minutos.

>[!NOTE]
>
>El [!DNL Outlook] la configuración del calendario es completamente independiente del [!DNL Outlook] Complemento ([!UICONTROL [!DNL Outlook] Integración] o [!DNL Workfront Outlook]). No se requiere instalación para configurar el calendario, pero se necesita una instalación para el [!DNL Outlook] Complemento de. Para obtener más información sobre [!DNL Outlook] Complemento, consulte [Configuración de [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Configure su [!UICONTROL Calendario principal] ver la configuración e integrarla con los calendarios de Outlook

1. En el [!UICONTROL Calendario principal] , haga clic en el **[!UICONTROL Configuración]** icono de engranaje ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png) en la esquina superior derecha para abrir **[!UICONTROL Configuración del calendario]** panel a la derecha.

   Si necesita información sobre el acceso a [!UICONTROL Calendario principal] ver, consulte [Ver el [!UICONTROL Calendario principal]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Opcional) Para integrar su [!DNL Microsoft Outlook] calendario, haga clic en **[!UICONTROL Añadir cuenta]** en la esquina superior derecha de la **[!UICONTROL Configuración del calendario]** panel. A continuación, si se le solicita, introduzca su [!DNL Microsoft Outlook] información de inicio de sesión. Puede repetir este paso para agregar varias [!DNL Outlook] cuentas.

   >[!NOTE]
   >
   >Debe dar [!DNL Workfront] permiso para acceder a su [!DNL Outlook] calendario. Conceder permiso permite [!DNL Workfront] para mantener el acceso a los datos del calendario, lea su [!DNL outlook] perfil, y leer y actualizar su [!DNL Microsoft] calendario.

1. Actualice la ventana del explorador para ver información de su [!DNL Outlook] cuenta en el calendario y en la [!UICONTROL Configuración del calendario] panel.
1. Haga clic en **[!UICONTROL Configuración]** icono de engranaje de nuevo en la esquina superior derecha para abrir **[!UICONTROL Configuración del calendario]** panel. ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. (Opcional) En cada [!DNL Microsoft] cuenta que ha añadido en el paso anterior, seleccione **[!UICONTROL Ver]** o **[!UICONTROL Sincronización]**:

   * **[!UICONTROL Ver]**: Se trata de una opción de solo lectura que muestra [!DNL Microsoft] eventos de calendario en su [!UICONTROL Calendario principal].
   * **[!UICONTROL Sincronización]**: Esta opción permite una sincronización bidireccional entre los [!DNL Microsoft] y [!UICONTROL Inicio] calendarios. En otras palabras, [!DNL Workfront] [!UICONTROL Calendario principal] artículos exportados a su [!DNL Microsoft] calendario y [!DNL Microsoft] importación de elementos de calendario en Workfront [!UICONTROL Calendario principal] en tiempo real.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Opcional) En su [!DNL Workfront] cuenta o una cuenta integrada, seleccione los calendarios asociados que desee ver en su [!UICONTROL Calendario principal] (como su calendario de PTO, Cumpleaños o Festivos) y luego haga clic en el [!UICONTROL Actualizar] o [!UICONTROL Recargar] para ver los cambios.

1. (Opcional) En el **[!UICONTROL General]** sección debajo de **[!UICONTROL Comenzar semana el]**, seleccione el día que desea mostrar como primer día de la semana laboral en el Calendario principal.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. Configure las siguientes opciones:

   * **[!UICONTROL Mis días laborables]:** Seleccione los días que trabaje.
   * **[!UICONTROL Mi hora inicial habitual]:** Seleccione la hora a la que comienza el día laborable.
   * **[!UICONTROL Mi hora final habitual]:** Seleccione la hora a la que desea finalizar el día laborable.

   [!DNL Workfront] utiliza estas tres opciones para calcular la cantidad de horas que trabaja en una semana. Este número afecta al [!UICONTROL Asignación] , que le ayuda a realizar un seguimiento de la carga de trabajo en relación con las horas de trabajo disponibles. Para obtener más información, consulte [[!UICONTROL Asignación] barra](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) en el artículo [[!UICONTROL Calendario principal] vista](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Haga clic fuera de **[!UICONTROL Configuración del calendario]** para cerrarla.

   [!DNL Workfront] guarda los cambios automáticamente.

Para obtener información sobre el uso de [!UICONTROL Calendario] para administrar las asignaciones de trabajo y los eventos de calendario integrados, consulte [Utilice el [!UICONTROL Calendario principal] vista](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
