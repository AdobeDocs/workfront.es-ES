---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Información general sobre actualizaciones rastreadas del sistema
description: Adobe Workfront registra la actividad que se está llevando a cabo en ciertos objetos mediante el registro de información de estado en el área [!UICONTROL Updates] del objeto.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: 594f224e11b0e7708ed555410b7c331741113791
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 95%

---

# Información general sobre actualizaciones rastreadas del sistema

<!-- Audited: 06/2025-->

[!DNL Adobe Workfront] captura la actividad que tiene lugar en ciertos objetos al registrar la información de estado en la sección [!UICONTROL Updates] del objeto.

Para obtener información acerca de la sección Actualizaciones, consulte [Información general de la sección Actualizaciones](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

El área [!UICONTROL Actualizaciones] incluye los siguientes tipos de actualizaciones:

* **Actualizaciones de usuarios:** introducidas manualmente por los usuarios. También se denominan comentarios, respuestas y notas. Las actualizaciones de usuario se muestran en las pestañas Comentarios y Todas de la sección Actualizaciones de un objeto.

  Para obtener más información acerca de cómo configurar las actualizaciones de usuario, consulte [Configurar preferencias para actualizaciones de usuarios](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![Actualizaciones](assets/updates-qs-350x125.png)

* **Actualizaciones del sistema:** realizadas automáticamente por el sistema. Una actualización del sistema incluye una breve nota que describe el tipo de cambio que se ha producido en el elemento. Las actualizaciones del sistema se muestran en las pestañas Actividad del sistema y Todas de la sección Actualizaciones de un objeto.

  Para obtener más información sobre las fuentes de actualización del sistema y cómo habilitarlas, consulte [Configurar actualizaciones del sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![Ejemplo de actualizaciones del sistema](assets/system-updates-example-unified-stream.png)


  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Consideraciones sobre las actualizaciones rastreadas por el sistema

Las actualizaciones rastreadas por el sistema no están disponibles para todos los objetos que tienen el área de Actualizaciones.

* El área [!UICONTROL Updates] está disponible para los objetos siguientes:

   * [!UICONTROL Project]
   * [!UICONTROL Tarea]
   * [!UICONTROL Problema]
   * [!UICONTROL Portafolio]
   * [!UICONTROL Programa]
   * [!UICONTROL Usuario]
   * [!UICONTROL Plantilla]
   * [!UICONTROL Tarea de plantilla]
   * [!UICONTROL Equipo]
   * [!UICONTROL Documento]
   * [!UICONTROL Plantilla de horas]
   * [!UICONTROL Historia]

     En [!DNL Workfront], una historia es una tarea.
   * [!UICONTROL Iteración]
   * [!UICONTROL Meta]

     No todos los paquetes de Workfront incluyen Workfront Goals. Para obtener más información, consulte [Requisitos para usar Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Card] en un tablero

     Para obtener más información sobre las actualizaciones de las tarjetas, consulte [Usar tarjetas conectadas en tableros](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] no realiza un seguimiento de las actualizaciones del sistema para los objetos siguientes:

   * [!UICONTROL Team]
   * [!UICONTROL Plantilla]
   * [!UICONTROL Template Task]
   * [!UICONTROL Card] ad hoc
   * [!UICONTROL Iterations]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* Las actualizaciones de los usuarios se muestran en la pestaña Comentarios y las actualizaciones del sistema en las pestañas Actividad del sistema y Todos.

  Para obtener una lista de objetos que no tienen las fichas Actividad del sistema o Todos, consulte [Actualizar información general de sección](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)

* No puede añadir una respuesta a una actualización del sistema. Sin embargo, todas las respuestas realizadas a los registros de actividad del sistema en la experiencia de comentarios heredada antes del 11 de abril de 2024, se rellenan en la pestaña Actividad del sistema como de solo lectura.

<!--
* The following are differences between the new and the legacy commenting experience: 

   * When using the new commenting experience, user updates display in the Comments tab and system updates display in the System Activity <span class="preview">and the All</span> tabs.  

      For more information about the new commenting experience, see [New commenting experience](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

      <span class="preview">For a list of objects that do not have the System Activity or the All tabs, see [Update section overview](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)</span>

   * <span class="preview">When using the new commenting experience, you cannot add a comment to a system update. However, any replies made to system activity records in the legacy commenting experience are populated on the System Activity tab as read-only in the new commenting experience.</span>
   * When using the legacy commenting experience, the system and user updates display in one continuous feed. 

   * When using the legacy commenting experience, users can view system updates by default or they can choose to not display them. Disabling system updates is not possible when using the new commenting experience. 

      For information about disabling the display of system updates, see the section [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) in the article [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).  

   * <span class="preview">The legacy commenting experience has been disabled in the Preview environment. For more information, see [Second Quarter 2024 Update stream and notification enhancements](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md).</span>
-->

* Los administradores de [!DNL Workfront] pueden definir qué tipo de cambios debe rastrear el sistema en el área [!UICONTROL Actualizaciones]. No todos los objetos que tienen un área [!UICONTROL Updates] tienen también fuentes de [!UICONTROL update] configurables. Los objetos siguientes tienen un área de [!UICONTROL Updates] que captura las fuentes de actualizaciones rastreadas por el sistema, pero no tienen fuentes de actualizaciones configurables:

   * [!UICONTROL Document]
   * [!UICONTROL Plantilla de horas]
   * [!UICONTROL Iteración]
   * [!UICONTROL Meta]


