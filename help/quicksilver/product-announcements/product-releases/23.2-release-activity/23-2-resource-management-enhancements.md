---
title: 23.2 Mejoras en la gestión de recursos
description: 23.2 Mejoras en la gestión de recursos
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b225ae19-eee7-4329-a42d-2a2bf9adad01
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# 23.2 Mejoras en la gestión de recursos

Esta página describe todas las mejoras realizadas en la administración de recursos con la versión 23.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción con la versión 23.2.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión 23.2, consulte [Descripción general de la versión 23.2](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Introducción al campo Tiempo de trabajo para calcular con precisión la capacidad del usuario

>[!NOTE]
>
>Versión preliminar: 16 de febrero de 2023; versión de producción planificada: 2 de marzo de 2023

Para permitir que los administradores de recursos calculen con precisión la disponibilidad de sus usuarios y tengan en cuenta el tiempo que los usuarios dedican al trabajo real relacionado con el proyecto, presentamos el concepto de Tiempo de trabajo a Adobe Workfront.

Puede definir el valor del campo Tiempo de trabajo de cada usuario al crear o editar su perfil. Para obtener más información, consulte [Editar el perfil de un usuario](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

El campo Tiempo de trabajo representa el porcentaje de tiempo equivalente a tiempo completo (FTE) que el usuario está disponible para el trabajo real, sin incluir los gastos generales. El tiempo de trabajo debe ser un número decimal con un valor entre 0 y 1. Por ejemplo, una disponibilidad del 20% para el trabajo real sería de 0,2.

El valor predeterminado del campo es 1, lo que indica que un usuario emplea todo su valor de FTE en trabajo real relacionado con el proyecto.

Como resultado de esta actualización, Workfront calcula la disponibilidad del usuario utilizando las siguientes fórmulas, según su selección en el área de preferencias de Administración de recursos:

* Horario predeterminado:
* Capacidad del usuario = [(Horas programadas - Excepciones de horario) * FTE - Tiempo libre ] * Tiempo de trabajo
* Horario del usuario:
* Capacidad del Usuario = (Horario - Excepciones de Horario - Tiempo Libre) * Tiempo de Trabajo.

Para obtener más información, consulte [Configurar las preferencias de [!UICONTROL Administración de recursos]](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

[Ver una demostración en vídeo de esta característica](https://video.tv.adobe.com/v/3415608/){target=_blank}
