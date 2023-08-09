---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Actualizaciones rastreadas por el sistema
description: Adobe Workfront registra la actividad que se está realizando en ciertos objetos mediante el registro de información de estado en el [!UICONTROL Actualizaciones] área.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: 413e5ff710b4c77b7ea2d870b34bb0627a4fcd86
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 6%

---

# Actualizaciones rastreadas por el sistema

[!DNL Adobe Workfront] registra la actividad que tiene lugar en ciertos objetos mediante el registro de información de estado en el [!UICONTROL Actualizaciones] área.

El [!UICONTROL Actualizaciones] incluye los siguientes tipos de actualizaciones:

* **Actualizaciones de usuarios:** Introducido manualmente por los usuarios. También se denominan comentarios, respuestas y notas.

  Para obtener más información sobre cómo configurar las actualizaciones de usuario, consulte [Configurar preferencias para actualizaciones de usuarios](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **Actualizaciones del sistema:** Realizado automáticamente por el sistema. Una actualización del sistema incluye una breve nota que describe el tipo de cambio que se ha producido en el elemento.

  Para obtener más información sobre las fuentes de actualización del sistema y cómo habilitarlas, consulte [Configurar actualizaciones del sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Consideraciones sobre las actualizaciones rastreadas por el sistema

* Las actualizaciones rastreadas por el sistema no están disponibles para todos los objetos que tienen el área de Actualizaciones. El [!UICONTROL Actualizaciones] está disponible para los siguientes objetos:

   * [!UICONTROL Proyecto]
   * [!UICONTROL Tarea]
   * [!UICONTROL Problema]
   * [!UICONTROL Portafolio]
   * [!UICONTROL Programar]
   * [!UICONTROL Usuario]
   * [!UICONTROL Plantilla]
   * [!UICONTROL Tarea de plantilla]
   * [!UICONTROL Equipo]
   * [!UICONTROL Documento]
   * [!UICONTROL Hoja de horas]
   * [!UICONTROL Historia]

     Entrada [!DNL Workfront], una historia es una tarea.
   * [!UICONTROL Iteración]
   * [!UICONTROL Meta]

     Debe tener una licencia adicional para tener acceso a [!UICONTROL Metas] área. Para obtener más información, consulte [Requisitos para utilizar Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Tarjeta] en un tablero

     Para obtener más información sobre actualizaciones de tarjetas, consulte [Añadir una tarjeta ad hoc a un tablero](../../../agile/get-started-with-boards/add-card-to-board.md).


* [!DNL Workfront] no realiza el seguimiento de ninguna actualización del sistema para los siguientes objetos:

   * [!UICONTROL Equipo]
   * [!UICONTROL Plantilla]
   * [!UICONTROL Tarea de plantilla]

<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* Los usuarios pueden ver las actualizaciones del sistema de forma predeterminada o pueden optar por no mostrarlas.

  Para obtener información acerca de cómo deshabilitar la visualización de actualizaciones del sistema, consulte la sección [Habilitar o deshabilitar actualizaciones del sistema](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) en el artículo [Actualizar trabajo](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

  >[!NOTE]
  >
  >Actualmente estamos rediseñando la experiencia de comentarios y la [!UICONTROL Actualizaciones] área en [!DNL Workfront].
  >
  > No puede ocultar las actualizaciones del sistema al utilizar la nueva experiencia de comentarios.
  > 
  >Para obtener más información sobre la nueva experiencia de comentarios, consulte [Nueva experiencia de comentarios](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

* Workfront registra las actualizaciones rastreadas por el sistema para los siguientes objetos, pero no hay opción para deshabilitar la visualización:

   * [!UICONTROL Portafolio]
   * [!UICONTROL Programar]
   * [!UICONTROL Iteración]

* [!DNL Workfront] Los administradores de pueden definir qué tipo de cambios debe seguir el sistema en la [!UICONTROL Actualizaciones] área. No todos los objetos que tienen un [!UICONTROL Actualizaciones] también tienen propiedades configurables [!UICONTROL actualizar] fuentes. Los objetos siguientes tienen un [!UICONTROL Actualizaciones] que captura fuentes de actualización rastreadas por el sistema, pero no tienen fuentes de actualización configurables:

   * [!UICONTROL Documento]
   * [!UICONTROL Hoja de horas]
   * [!UICONTROL Iteración]

