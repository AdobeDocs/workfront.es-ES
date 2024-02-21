---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Mejoras de proyecto en 2020.2
description: Esta página describe todas las mejoras de Project realizadas con la versión 2020.2 en el entorno de producción. Estas mejoras estaban disponibles en el entorno de producción en la semana del 11 de mayo de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# Mejoras de proyecto en 2020.2

Esta página describe todas las mejoras de Project realizadas con la versión 2020.2 en el entorno de producción. Estas mejoras estaban disponibles en el entorno de producción en la semana del 11 de mayo de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 2020.2, consulte [información general sobre la versión 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Para administradores de Workfront: nueva seguridad contra fallos cuando el estado del proyecto de los nuevos proyectos se oculta o desbloquea

En Configuración, configure una preferencia para asegurarse de que cada nuevo proyecto tiene un estado determinado cuando se crea el proyecto. Esto es importante porque un proyecto siempre necesita un estado para funcionar correctamente en Workfront, incluso cuando el proyecto es completamente nuevo.

Para asegurarse de que los nuevos proyectos siempre tienen un estado, incluso si un administrador oculta o desbloquea el estado configurado para nuevos proyectos, el sistema ahora asigna el primer estado de la lista Estado a todos los nuevos proyectos hasta que se vuelva a configurar el nuevo estado para nuevos proyectos.

Para obtener información sobre cómo establecer la preferencia para el estado de todos los proyectos nuevos, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (o si utiliza Adobe Workfront Classic, consulte [Estableciendo preferencias del proyecto](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298)).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## Para administradores de Workfront: diseño mejorado en Preferencias del proyecto

La experiencia de establecer preferencias de proyecto ahora es más intuitiva y fácil de usar:

* Los títulos son más grandes que las etiquetas de opción, por lo que puede encontrar lo que busca más rápido.
* Dividir líneas y espacio en blanco adicional separa cada sección para que pueda centrarse más fácilmente en lo que está haciendo.
* Si escribe un número no válido para una opción como &quot;Horas habituales por día laborable&quot;, aparece un mensaje de advertencia inmediatamente en lugar de aparecer después de hacer clic en Guardar.
* Las etiquetas de opción coinciden con el texto de interfaz correspondiente en cualquier otra parte de Workfront, como el área de Detalles e informes.

Para obtener información sobre el área Preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (o si utiliza Adobe Workfront Classic, consulte [Estableciendo preferencias del proyecto](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298)).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## El filtro, la vista y la agrupación seleccionados se mantienen en las listas de informes

Ahora, se selecciona el último filtro, vista o agrupación aplicado a un informe específico, incluso si el usuario cierra la sesión y vuelve a iniciarla en Workfront.

Anteriormente, después de que un usuario aplicara un filtro, una vista o una agrupación a una lista de informes y luego saliera de esa página, el filtro, la vista o la agrupación predeterminados aparecían la próxima vez que el usuario navegaba al mismo informe.

**Disponible en estos entornos:**

* La nueva experiencia de Adobe Workfront
* Adobe Workfront Classic

## Mover y copiar tareas a otro proyecto mantiene la restricción de tareas cuando estas pueden ajustarse a la escala de tiempo del proyecto

Hemos mejorado la forma en que Workfront gestiona la restricción de tarea específica de una tarea al copiar la tarea o moverla a otro proyecto. Algunos ejemplos de restricciones de tareas específicas de fecha son Debe comenzar el, Debe finalizar el, Fechas fijas, No comenzar después del, etc.

Por ejemplo, cuando mueve o copia una tarea con una delimitación Debe comenzar el a otro proyecto cuya fecha planificada de inicio es anterior a la fecha de inicio de la tarea, la tarea mantiene la delimitación después de copiarla o moverla. Cuando se mueve o copia una tarea con una delimitación Debe comenzar el a un proyecto cuya fecha planificada de inicio es posterior a la fecha de inicio de la tarea, la delimitación de la tarea cambia a Lo antes posible.

Antes de este cambio, la restricción de tarea siempre cambia a Lo antes posible.

Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md) (o si utiliza Adobe Workfront Classic, consulte [Mover tareas](https://one.workfront.com/s/article/Moving-Tasks-2081996259)).

Para obtener información sobre cómo copiar tareas, consulte [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (o si utiliza Adobe Workfront Classic, consulte [Copiar y duplicar tareas](https://one.workfront.com/s/article/Copy-and-Duplicate-Tasks-218695605)).

Para obtener una descripción general de todas las restricciones de tarea, consulte [Información general sobre restricciones de tarea](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (o si utiliza Adobe Workfront Classic, consulte [Información general sobre restricciones de tarea](https://one.workfront.com/s/article/Task-Constraint-Overview-453396848)).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## Prevención de la pérdida de datos al realizar cambios en la pestaña Detalles o en una lista de tareas

Para evitar la pérdida de datos al actualizar información en la página Detalles de un objeto o tareas de una lista de tareas en el nivel de proyecto al guardar los cambios manualmente, ahora se muestra un mensaje de advertencia para notificarle que tiene cambios sin guardar antes de intentar editar la información en el encabezado. Las únicas acciones permitidas antes de guardar los cambios son suscribirse o agregar el objeto a los favoritos.

Para obtener información sobre la edición de tareas en una lista, consulte [Edición de tareas en una lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Disponible en estos entornos:**

* La nueva experiencia de Adobe Workfront

