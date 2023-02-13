---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Actualizaciones rastreadas por el sistema
description: Adobe Workfront captura la actividad que se está realizando en ciertos objetos registrando la información de estado en el informe [!UICONTROL Actualizaciones] .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 5%

---

# Actualizaciones rastreadas por el sistema

[!DNL Adobe Workfront] captura la actividad que se está realizando en ciertos objetos registrando información de estado en el informe [!UICONTROL Actualizaciones] .

La variable [!UICONTROL Actualizaciones] incluye los siguientes tipos de actualizaciones:

* **Actualizaciones de usuario:** Introducido manualmente por los usuarios. También se denomina comentarios, respuestas y notas.

   ![](assets/updates-qs-350x125.png)

* **Actualizaciones del sistema:** Creado automáticamente por el sistema. Una actualización del sistema incluye una breve nota en la que se describe qué tipo de cambio se produjo en el elemento.

   <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

Los siguientes objetos pueden tener actualizaciones:

* Proyecto
* Tarea
* Problema
* Portafolio
* Programar
* Usuario
* Plantillas
* Tareas de plantilla
* Documentos
* Plantillas de horas

Su [!DNL Workfront] la licencia determina si las actualizaciones del sistema se muestran de forma predeterminada en la [!UICONTROL Actualizaciones] área de objetos. [!DNL Workfront] usuarios con un [!UICONTROL Plan] las licencias tienen actualizaciones del sistema mostradas en el [!UICONTROL Actualizaciones] de forma predeterminada. Sin embargo, los usuarios pueden filtrar las actualizaciones del sistema, tal como se describe en la sección [[!UICONTROL Habilitar] o desactivar actualizaciones del sistema](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) en [Actualizar trabajo](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). El resto [!DNL Workfront] licencias filtran las actualizaciones del sistema de forma predeterminada.

[!DNL Workfront] los administradores pueden definir qué tipo de cambios debe rastrear el sistema en la variable [!UICONTROL Actualizaciones] . No todos los objetos son configurables [!UICONTROL actualizar] fuentes de estado. Los siguientes objetos tienen un [!UICONTROL Actualizaciones] área que captura fuentes de actualización rastreadas por el sistema, pero que no tiene fuentes de estado de actualización configurables:

* Plantillas
* Tareas de plantilla
* Documentos
* Plantillas de horas

Para obtener más información sobre las fuentes de actualización del sistema y cómo habilitarlas, consulte [Configurar actualizaciones del sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md). Para obtener más información sobre la configuración de actualizaciones de usuarios, consulte [Configuración de preferencias para actualizaciones de usuarios](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
