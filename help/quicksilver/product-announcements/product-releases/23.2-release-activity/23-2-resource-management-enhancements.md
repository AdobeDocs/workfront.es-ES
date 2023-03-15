---
title: 23.2 Mejoras en la gestión de los recursos
description: 23.2 Mejoras en la gestión de los recursos
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 93071f9c9d359ff98a269b07f81ebcf251b1f23c
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 23.2 Mejoras en la gestión de los recursos

En esta página se describen todas las mejoras de administración de recursos realizadas con la versión 23.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno Producción con la versión 23.2.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de versión 23.2, consulte [Resumen de la versión 23.2](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Presentación del campo Tiempo de Trabajo para calcular con precisión la capacidad del usuario

>[!NOTE]
>
>Versión de vista previa: 16 de febrero de 2023; Versión de producción planificada: 2 de marzo de 2023

Para permitir que los administradores de recursos calculen con precisión la disponibilidad de sus usuarios y tengan en cuenta el tiempo que los usuarios dedican al trabajo real relacionado con el proyecto, presentamos el concepto de tiempo de trabajo a Adobe Workfront.

Puede definir el valor del campo Tiempo de trabajo para cada usuario, al crear o editar su perfil. Para obtener más información, consulte [Edición del perfil de un usuario](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

El campo Tiempo de trabajo representa el porcentaje de tiempo equivalente a tiempo completo (FTE) que el usuario está disponible para el trabajo real, sin incluir la sobrecarga. El tiempo de trabajo debe ser un número decimal con un valor entre 0 y 1. Por ejemplo, un 20% de disponibilidad para el trabajo real sería 0,2.

El valor predeterminado del campo es 1, lo que indica que un usuario gasta todo su FTE en trabajo real relacionado con el proyecto.

Como resultado de esta actualización, Workfront calcula la disponibilidad del usuario mediante las fórmulas siguientes, según la selección que realice en el área de preferencias de Gestión de recursos:

* Horario predeterminado:
* Capacidad del usuario = [(Horario programado - Excepciones programadas) * FTE - Tiempo libre] * Tiempo de trabajo
* Programación del usuario:
* Capacidad del usuario = (Horario de programación - Excepciones de programación - Tiempo libre) * Tiempo de trabajo.

Para obtener más información, consulte [Configurar [!UICONTROL Gestión de recursos] preferencias](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

[Ver una demostración en vídeo de esta función](https://video.tv.adobe.com/v/3415608/){target=_blank}