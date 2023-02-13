---
title: 20.4 Mejoras en la gestión de recursos
description: 20.4 Mejoras en la gestión de recursos
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 9f660a38-4a59-4135-8178-0841088cc7d6
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 0%

---

# 20.4 Mejoras en la gestión de recursos

En esta página se describen todas las mejoras realizadas en la administración de recursos con la versión 20.4 para el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 9 de noviembre de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.4, consulte [Información general sobre la versión 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Planificar el trabajo utilizando el esfuerzo de trabajo en lugar de horas planificadas

Para darle flexibilidad a la hora de planificar el trabajo en sus proyectos, hemos introducido el nuevo concepto de esfuerzo de trabajo para las tareas. Puede estimar si el esfuerzo de trabajo de una tarea es pequeño, medio o grande sin calcular manualmente las horas planificadas de la tarea. Cada nivel de esfuerzo se calcula en función de un porcentaje de tiempo respecto a las horas típicas por día, según la configuración de la instancia.

Con esta nueva función ya están disponibles las siguientes mejoras:

* Habilite esta configuración para proyectos y plantillas para que esté disponible para tareas y tareas de plantilla
* Actualice esta configuración para cada tarea con un Tipo de duración simple que actualice automáticamente las horas planificadas de la tarea
* Deshabilite esta configuración con una plantilla de diseño para usuarios que prefieran seguir usando horas planificadas.
* Muestre el valor de este nuevo campo en una lista de tareas o en un informe.

Para obtener información sobre el esfuerzo de trabajo, consulte [Información general sobre el esfuerzo de trabajo](../../../manage-work/tasks/task-information/work-effort.md).

Esta función ahora se incluye en la función [Aspectos básicos del planificador, parte 2, ruta de aprendizaje](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-2-plan-a-project-20Y0z000000bm79EAA) en Workfront One.

## Colores basados en el estado del proyecto para elementos de trabajo en el equilibrador de carga de trabajo

Para obtener una mejor visibilidad y una mayor personalización de su experiencia en el equilibrador de carga de trabajo, ahora puede cambiar los colores de los proyectos y sus elementos de trabajo para que coincidan con el estado del estado de los proyectos. Los colores corresponden a los estados de proyecto de nivel de grupo o de nivel de sistema. Los colores mostrados pueden corresponder a los estados del sistema y del proyecto personalizado.

Para obtener información sobre la personalización de la vista en el equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ajustar la asignación de usuarios mediante valores de porcentaje en el equilibrador de carga de trabajo

Ahora puede administrar las asignaciones de los usuarios en el equilibrador de carga de trabajo mediante porcentajes en lugar de horas.

Para obtener información sobre la administración de asignaciones en el equilibrador de carga de trabajo, consulte [Administrar asignaciones de usuario en el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Mostrar u ocultar el trabajo completado en el equilibrador de carga de trabajo

Ahora, una nueva configuración permite mostrar u ocultar elementos de trabajo completados en el equilibrador de carga de trabajo. El ajuste está habilitado de forma predeterminada y los elementos de trabajo completados que coinciden con los criterios de filtrado y el lapso de tiempo seleccionado se muestran en el equilibrador de carga de trabajo.

Antes de esta mejora, los elementos de trabajo completados siempre se mostraban en el equilibrador de carga de trabajo.

Para obtener más información sobre el ajuste de la configuración en el equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Mejoras de uso en el equilibrador de carga de trabajo

Para garantizar una experiencia optimizada y fácil de usar al administrar sus recursos en el equilibrador de carga de trabajo, ya están disponibles las siguientes mejoras de uso:

* Ahora puede abrir el Resumen de problemas y tareas desde el icono Resumen en lugar del menú Más . Esta experiencia es ahora coherente con la de las listas.

   >[!NOTE]
   >
   >Esta opción solo está disponible en la nueva experiencia de Adobe Workfront.

* Puede acceder al menú Más a la izquierda de una barra de objetos en lugar de al final de una barra de objetos. Esto facilita la búsqueda cuando los objetos abarcan un largo período de tiempo.
* Puede acceder a las funciones de asignación con un método abreviado de teclado. Anteriormente, solo estaba disponible en el menú Más .
* Puede cargar todos los elementos restantes bajo el nombre de un usuario en lugar de solo los 20 elementos siguientes haciendo clic en Cargar más.

Para obtener más información sobre cómo navegar por el equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Gráfico de asignación de usuarios en el equilibrador de carga de trabajo

Para permitirle tener una representación visual de alto nivel de la asignación de los usuarios dentro de un lapso de tiempo determinado, una nueva configuración ahora habilita una vista de gráfico para ver cómo se muestran las asignaciones en el equilibrador de carga de trabajo. Al habilitar esta configuración, se muestra la asignación de los usuarios en un gráfico de líneas que indica las sobreasignaciones en bloques rojos y las subasignaciones en azul.

Para obtener más información sobre la configuración de la configuración en el equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visualizar el trabajo completado en el equilibrador de carga de trabajo

Para permitirle identificar fácilmente el trabajo que ya se ha completado para que pueda administrar correctamente las asignaciones de usuario, hemos habilitado un indicador visual en el equilibrador de carga de trabajo que muestra cuándo se han completado los elementos de un lapso de tiempo seleccionado. Ahora puede ver una marca de verificación verde para las tareas, problemas cuando se completan. El proyecto también muestra la marca de verificación verde cuando hay elementos de trabajo completados durante el lapso de tiempo mostrado en la pantalla.

Para obtener información sobre la visualización de información en el equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Nuevo filtro predeterminado para el área de trabajo asignado en el equilibrador de carga de trabajo

El filtro Predeterminado para el área Trabajo asignado del equilibrador de carga de trabajo ahora muestra solo los usuarios que son miembros de todos los equipos a los que está asociado, como usuario que ha iniciado sesión. El nuevo filtro ahora muestra la información más relevante para usted de forma predeterminada.

Antes de esta mejora, todos los usuarios a los que tenía acceso para ver se mostraban en esta área.

Para obtener información sobre el uso de filtros en el equilibrador de carga de trabajo, consulte [Administrar filtros en el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nuevo icono para cambiar entre horas y valores de porcentaje, o tiempo asignado y restante en el equilibrador de carga de trabajo

Se ha añadido una nueva configuración que le permite cambiar entre horas y porcentajes asignados a medida que ve el equilibrador de carga de trabajo. Con este nuevo icono, también hemos eliminado la sección Carga de trabajo de usuario en el panel Configuración . El equilibrador de carga de trabajo muestra el tiempo asignado de forma predeterminada y hemos movido el valor de horas restantes al nuevo icono de porcentaje o horas.

Esta mejora elimina los clics y hace que navegar por el equilibrador de carga de trabajo sea más fácil y eficiente.

Para obtener información sobre la administración de la configuración del equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Un nuevo filtro integrado para el equilibrador de carga de trabajo: Usuarios en proyectos

Para que su experiencia de filtrado en el equilibrador de carga de trabajo sea más eficiente, hemos añadido un nuevo filtro integrado en el área Trabajo asignado . Ahora puede aplicar el filtro Usuarios en proyectos , que muestra los usuarios asignados a tareas y problemas en los proyectos que especifique.

Para obtener información sobre el uso de filtros en el equilibrador de carga de trabajo, consulte [Filtrar información en el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

