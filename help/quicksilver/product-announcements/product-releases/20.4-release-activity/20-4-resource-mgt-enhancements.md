---
title: 20.4 Mejoras en la administración de recursos
description: 20.4 Mejoras en la administración de recursos
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9f660a38-4a59-4135-8178-0841088cc7d6
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 99%

---

# 20.4 Mejoras en la administración de recursos

Esta página describe todas las mejoras de Administración de recursos realizadas con la versión 20.4 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 9 de noviembre de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.4, consulte [Información general de la versión 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Planificar el trabajo mediante esfuerzo laboral en lugar de horas planificadas

Para ofrecerle flexibilidad a la hora de planificar el trabajo en sus proyectos, hemos introducido el nuevo concepto de esfuerzo laboral para las tareas. Puede estimar si el esfuerzo laboral de una tarea es pequeño, mediano o grande sin estimar manualmente las horas planificadas para la tarea. Cada nivel de esfuerzo se calcula en función de un porcentaje de tiempo desde las horas típicas al día configuradas en la instancia.

Las siguientes mejoras ya están disponibles con esta nueva función:

* Habilite esta opción para proyectos y plantillas a fin de que esté disponible para tareas y tareas de plantilla
* Actualice esta configuración para cada tarea con un Tipo de duración simple que actualice automáticamente las Horas planificadas de la tarea
* Deshabilite esta configuración con una plantilla de diseño para los usuarios que prefieran seguir usando las horas planificadas.
* Muester el valor de este nuevo campo en una lista de tareas o un informe.

Para obtener información sobre el esfuerzo laboral, consulte [Información general del esfuerzo laboral](../../../manage-work/tasks/task-information/work-effort.md).

Esta característica ahora se incluye en la ruta de aprendizaje [Aspectos básicos del planificador, parte 2](https://experienceleague.adobe.com/en/docs/workfront/using/home) en Workfront One.

## Colores basados en el estado del proyecto para elementos de trabajo en el Distribuidor de cargas de trabajo

Para obtener una mejor visibilidad y una mayor personalización de la experiencia en el Distribuidor de cargas de trabajo, ahora puede cambiar los colores de los proyectos y sus elementos de trabajo para que coincidan con el estado de los proyectos. Los colores corresponden a estados de proyecto de nivel de grupo o de nivel de sistema. Los colores mostrados pueden corresponder tanto a los estados del sistema como a los del proyecto personalizado.

Para obtener información sobre cómo personalizar la vista en el Distribuidor de cargas de trabajo, consulte [Navegar por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ajustar la asignación de usuarios mediante valores de porcentaje en el Distribuidor de cargas de trabajo

Ahora puede administrar las asignaciones de los usuarios en el Distribuidor de cargas de trabajo mediante porcentajes en lugar de horas.

Para obtener información sobre cómo administrar asignaciones en el Distribuidor de cargas de trabajo, consulte [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Mostrar u ocultar trabajo completado en el Distribuidor de cargas de trabajo

Ahora, una nueva configuración le permite mostrar u ocultar los elementos de trabajo completados en el Distribuidor de cargas de trabajo. La configuración está habilitada de forma predeterminada y los elementos de trabajo completados que coinciden con los criterios de filtrado y el lapso de tiempo seleccionados se muestran en el Distribuidor de cargas de trabajo.

Antes de esta mejora, los elementos de trabajo completados siempre se mostraban en el Distribuidor de cargas de trabajo.

Para obtener más información acerca de cómo ajustar la configuración en el Distribuidor de cargas de trabajo, consulte [Desplazarse por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Mejoras de uso en el Distribuidor de cargas de trabajo

Para garantizar una experiencia optimizada y fácil de usar al administrar los recursos en el Distribuidor de cargas de trabajo, ya están disponibles las siguientes mejoras de uso:

* Ahora puede abrir el Resumen de problemas y tareas desde el icono Resumen en lugar del menú Más. Esta experiencia es ahora coherente con la de las listas.

  >[!NOTE]
  >
  >Esta opción solo está disponible en la nueva experiencia de Adobe Workfront.

* Puede acceder al menú Más a la izquierda de una barra de objetos en lugar de al final de una barra de objetos. Esto facilita la búsqueda cuando los objetos abarcan un largo período de tiempo.
* Puede acceder a las funciones de asignación con un método abreviado de teclado. Anteriormente, solo estaba disponible en el menú Más.
* Puede cargar todos los elementos restantes bajo el nombre de un usuario en lugar de solo los 20 elementos siguientes haciendo clic en Cargar más.

Para obtener más información sobre cómo navegar por el Distribuidor de cargas de trabajo, consulte [Navegar por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Gráfico de asignación de usuarios en el Distribuidor de cargas de trabajo

Para permitirle tener una representación visual de alto nivel de la asignación de los usuarios en un lapso de tiempo determinado, una nueva configuración ahora habilita una vista de gráfico de cómo se muestran las asignaciones en el Distribuidor de cargas de trabajo. Al habilitar esta configuración, se muestra la asignación de los usuarios en un gráfico de líneas que indica las sobreasignaciones en bloques rojos y las infraasignaciones en azul.

Para obtener más información acerca de la configuración en el Distribuidor de cargas de trabajo, consulte [Desplazarse por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visualización del trabajo completado en el Distribuidor de cargas de trabajo

Para permitirle identificar fácilmente el trabajo que ya se ha completado y poder administrar las asignaciones de usuario correctamente, hemos habilitado un indicador visual en el Distribuidor de cargas de trabajo que muestra cuándo se han completado los elementos de un lapso de tiempo seleccionado. Ahora puede ver una marca de verificación verde para las tareas y los problemas cuando se completan. El proyecto también muestra la marca de verificación verde cuando hay elementos de trabajo completados durante el lapso de tiempo mostrado en la pantalla.

Para obtener información acerca de cómo ver información en el Distribuidor de cargas de trabajo, consulte [Desplazarse por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Nuevo filtro predeterminado para el área de Trabajo asignado en el Distribuidor de cargas de trabajo

El filtro predeterminado para el área de Trabajo asignado en el Distribuidor de cargas de trabajo ahora muestra solo los usuarios que son miembros de todos los equipos a los que usted, como usuario que ha iniciado sesión, está asociado. El nuevo filtro ahora muestra la información más relevante para usted, de forma predeterminada.

Antes de esta mejora, todos los usuarios a los que tenía acceso se mostraban en esta área.

Para obtener información sobre el uso de filtros en el Distribuidor de cargas de trabajo, consulte [Administrar filtros en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nuevo icono para cambiar entre horas y valores de porcentaje, o entre el tiempo asignado y el tiempo restante en el Distribuidor de cargas de trabajo

Se ha añadido una nueva configuración que le permite cambiar entre las horas asignadas y los porcentajes a medida que se ve el Distribuidor de cargas de trabajo. Con este nuevo icono, también hemos eliminado la sección Carga de trabajo del usuario en el panel Configuración. El Distribuidor de cargas de trabajo muestra el tiempo asignado de forma predeterminada y se ha movido la configuración de horas restantes al nuevo icono de porcentaje u horas.

Esta mejora elimina los clics y hace que la navegación por el Distribuidor de cargas de trabajo sea más fácil y eficiente.

Para obtener información acerca de cómo administrar la configuración del Distribuidor de cargas de trabajo, consulte [Navegar por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Un nuevo filtro integrado para el Distribuidor de cargas de trabajo: usuarios en proyectos

Para que su experiencia de filtrado en el Distribuidor de cargas de trabajo sea más eficiente, hemos añadido un nuevo filtro integrado en el área de Trabajo asignado. Ahora puede aplicar el filtro Usuarios en proyectos, que muestra los usuarios asignados a tareas y problemas en los proyectos que especifique.

Para obtener información sobre el uso de filtros en el Distribuidor de cargas de trabajo, consulte [Información sobre filtros en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

