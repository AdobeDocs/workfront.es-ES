---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Mejoras de Project 2020.2
description: Esta página describe todas las mejoras de Project realizadas con la versión 2020.2 en el entorno de producción. Estas mejoras estaban disponibles en el entorno de producción en la semana del 11 de mayo de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 99%

---

# Mejoras de Project 2020.2

Esta página describe todas las mejoras de Project realizadas con la versión 2020.2 en el entorno de producción. Estas mejoras estaban disponibles en el entorno de producción en la semana del 11 de mayo de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 2020.2, consulte [Información general sobre la versión 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Para administradores de Workfront: nuevo mecanismo de seguridad cuando el estado del proyecto de los nuevos proyectos se oculta o desbloquea

En Configuración, configure una preferencia para asegurarse de que cada nuevo proyecto tiene un estado determinado cuando se crea el proyecto. Esto es importante porque un proyecto siempre necesita un estado para funcionar correctamente en Workfront, incluso cuando el proyecto es completamente nuevo.

Para asegurarse de que los nuevos proyectos siempre tienen un estado, incluso si un administrador oculta o desbloquea el estado configurado para nuevos proyectos, el sistema ahora asigna el primer estado de la lista Estado a todos los nuevos proyectos hasta que se vuelva a configurar el nuevo estado para nuevos proyectos.

Para obtener información acerca de cómo establecer la preferencia para el estado de todos los proyectos nuevos, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (o si usa Adobe Workfront Classic, consulte [Establecer preferencias del proyecto](https://experienceleague.adobe.com/es/docs/workfront/using/home)).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## Para administradores de Workfront: diseño mejorado en Preferencias del proyecto

La experiencia de establecer preferencias del proyecto ahora es más intuitiva y fácil de usar:

* Los títulos son más grandes que las etiquetas de opción para que pueda encontrar lo que busca más rápidamente.
* Las líneas divisorias y el espacio en blanco adicional separan cada sección para que se pueda centrar más fácilmente en lo que está haciendo.
* Si escribe un número no válido para una opción como “Horas habituales por día laborable”, aparece un mensaje de advertencia inmediatamente en lugar de aparecer después de hacer clic en Guardar.
* Las etiquetas de opción coinciden con el texto de interfaz correspondiente en cualquier otra parte de Workfront, como el área de Detalles e informes.

Para obtener información sobre el área de Preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (o si usa Adobe Workfront Classic, consulte [Configurar las preferencias del proyecto](https://experienceleague.adobe.com/es/docs/workfront/using/home)).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## El filtro, la vista y la agrupación seleccionados se mantienen en las listas de informes

Ahora, se selecciona el último filtro, vista o agrupación aplicados a un informe específico, incluso si el usuario cierra la sesión y vuelve a iniciarla en Workfront.

Anteriormente, después de que un usuario aplicaba un filtro, una vista o una agrupación a una lista de informes y salía de esa página, el filtro, la vista o la agrupación predeterminados aparecían la siguiente vez que el usuario accedía al mismo informe.

**Disponible en estos entornos:**

* La nueva experiencia de Adobe Workfront
* Adobe Workfront Classic

## Mover y copiar tareas a otro proyecto, mantiene la restricción de tareas cuando estas pueden ajustarse a la línea de tiempo del proyecto

Hemos mejorado la forma en que Workfront gestiona la restricción de fecha específica de una tarea al copiarla o moverla a otro proyecto. Algunos ejemplos de restricciones de tareas específicas de fecha son Debe iniciarse el, Debe finalizarse el, Fechas fijas, No iniciar después del, etc.

Por ejemplo, cuando mueve o copia una tarea con una delimitación Debe iniciarse el a otro proyecto cuya fecha planificada de inicio es anterior a la fecha de inicio de la tarea, la tarea mantiene la delimitación después de copiarla o moverla. Cuando se mueve o copia una tarea con una delimitación Debe iniciarse el a un proyecto cuya fecha planificada de inicio es posterior a la fecha de inicio de la tarea, la delimitación de la tarea cambia a Lo antes posible.

Antes de este cambio, la restricción de tarea siempre cambia a Lo antes posible.

Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md) (o si está usando Adobe Workfront Classic, consulte [Mover tareas](https://experienceleague.adobe.com/es/docs/workfront/using/home)).

Para obtener información acerca de cómo copiar tareas, consulte [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (o si usa Adobe Workfront Classic, consulte [Copiar y duplicar tareas](https://experienceleague.adobe.com/es/docs/workfront/using/home)).

Para obtener una descripción general de todas las restricciones de tarea, consulte [Información general sobre la restricción de tarea](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (o si está usando Adobe Workfront Classic, consulte [Información general sobre la restricción de tarea](https://experienceleague.adobe.com/es/docs/workfront/using/home)).

**Disponible en estos entornos:**

* Adobe Workfront Classic
* La nueva experiencia de Adobe Workfront

## Prevención de la pérdida de datos al realizar cambios en la pestaña Detalles o en una lista de tareas

Para evitar la pérdida de datos al actualizar la información en la página Detalles de un objeto o las tareas de una lista de tareas en el nivel de proyecto cuando se guardan los cambios manualmente, ahora se muestra un mensaje de advertencia para avisarle de que tiene cambios sin guardar antes de intentar editar la información del encabezado. Las únicas acciones permitidas antes de guardar los cambios son la suscripción o la adición del objeto a los favoritos.

Para obtener información sobre la edición de tareas en una lista, consulte [Editar tareas en una lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Disponible en estos entornos:**

* La nueva experiencia de Adobe Workfront

