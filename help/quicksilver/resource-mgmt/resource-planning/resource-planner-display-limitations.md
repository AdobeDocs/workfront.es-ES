---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Limitaciones de visualización del Planificador de recursos
description: Para mejorar el rendimiento, Adobe Workfront limita la cantidad de información que puede mostrar, así como la cantidad de información que puede exportar desde el Planificador de recursos.
author: Alina
feature: Resource Management
exl-id: 12f56f11-59fb-4318-b43a-5ac695ca1e7e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Limitaciones de visualización del Planificador de recursos

Para mejorar el rendimiento, Adobe Workfront limita la cantidad de información que puede mostrar, así como la cantidad de información que puede exportar desde el Planificador de recursos.

Cuando se acerca este límite, Workfront muestra un mensaje de advertencia para informarle de que ha alcanzado ese límite.

Si la información que espera ver en el Planificador de recursos no se muestra, es posible que esté intentando mostrar demasiada información y que algunos datos no se hayan mostrado debido a esta limitación.

Se recomienda lo siguiente para un rendimiento óptimo en la visualización y exportación del Planificador de recursos:

* Utilice filtros para reducir la cantidad de información que muestra en el Planificador de recursos y vea solo la información que le interesa.
* Utilice todas las opciones de exportación para reducir la cantidad de información que exporta al mismo tiempo y para asegurarse de exportar solo la información pertinente.\
   Para obtener más información sobre el uso de filtros y las opciones de exportación en el planificador de recursos, consulte [Filtrar información en el planificador de recursos](../../resource-mgmt/resource-planning/filter-resource-planner.md).

   Para obtener información sobre la exportación de información desde el planificador de recursos, consulte [Exportar información del planificador de recursos](../../resource-mgmt/resource-planning/export-resource-planner.md).

La cantidad de información que puede mostrar o exportar depende de la vista que aplique y del entorno que utilice para acceder al planificador de recursos.

## Limitaciones en la vista de proyecto

Tenga en cuenta lo siguiente al aplicar la vista Proyecto al planificador de recursos:

* Solo puede ver los proyectos a los que tiene acceso para administrar.
* Puede expandir cada proyecto para ver las funciones asociadas y cada función para ver los usuarios asociados a él.

   Puede ver hasta 300 proyectos cuando se desplaza hasta la parte inferior de la lista, a menos que haya más de 30 000 filas de proyectos, funciones y usuarios. A continuación, recibirá un mensaje de advertencia indicando que ha alcanzado el límite de 30 000 filas.

* Puede ver tres o cuatro períodos de tiempo a la vez, según el tamaño de la pantalla.

Tenga en cuenta lo siguiente al exportar información desde la vista Proyecto del planificador de recursos, después de haber aplicado todos los filtros y opciones de exportación adecuados:

* Cuando selecciona exportar todo (proyectos, funciones y usuarios) en el Planificador de recursos, todos los objetos que coinciden con sus criterios aparecen en el archivo exportado, independientemente de si se ha desplazado hasta la parte inferior de la lista para mostrarlos o no.
* Las filas sin información de asignación se incluyen en el archivo exportado.

* Puede exportar hasta 30 000 filas.

## Limitaciones en la vista de funciones

Tenga en cuenta lo siguiente al aplicar la vista Rol al planificador de recursos, después de aplicar todos los filtros adecuados:

* Solo puede ver las funciones que están asociadas con proyectos que puede administrar.

* Puede ver hasta 300 funciones cuando se desplaza hasta la parte inferior de la lista, a menos que haya más de 30 000 filas de funciones, proyectos y usuarios. A continuación, recibirá un mensaje de advertencia indicando que ha alcanzado el límite de 30 000 filas para lo que puede ver en la pantalla.
* Puede expandir cada función para mostrar una lista de proyectos y cada proyecto para mostrar una lista de usuarios que pueden desempeñar esas funciones en los proyectos.

   De forma predeterminada, se muestran 20 proyectos y puede utilizar la opción Cargar más para mostrar proyectos adicionales o desplazarse por cada proyecto para cargar más usuarios.

* Puede ver tres o cuatro períodos de tiempo, en función del tamaño de la pantalla.

Tenga en cuenta lo siguiente al exportar información desde la vista de funciones del planificador de recursos, después de aplicar todos los filtros y opciones de exportación adecuados:

* Cuando selecciona exportar todo (funciones, proyectos y usuarios) en el Planificador de recursos, todos los objetos que coinciden con sus criterios aparecen en el archivo exportado, independientemente de si se ha desplazado hasta la parte inferior de la lista para mostrarlos o no.
* Las filas sin información de asignación se incluyen en el archivo exportado.
* Puede exportar hasta 30 000 filas.

## Limitaciones en la vista de usuario

Tenga en cuenta lo siguiente al aplicar la vista Usuario al Planificador de Recursos:

* Puede mostrar todos los usuarios que cumplan los siguientes criterios:

   * Tiene acceso a la vista
   * Están activos
   * Han iniciado sesión al menos una vez.

* Puede expandir cada usuario para mostrar los proyectos asociados con él y cada proyecto para mostrar las funciones asociadas con él.\
   Los primeros 50 proyectos y funciones se muestran de forma predeterminada y puede utilizar la opción Cargar más para mostrar proyectos o funciones adicionales.

   >[!NOTE]
   >
   >Si ha filtrado la lista de usuarios por proyectos, solo se pueden expandir los usuarios asociados con los proyectos filtrados y también mostrar la información de la hora

* Se pueden ver hasta 2000 usuarios en la interfaz web. Workfront muestra un mensaje de advertencia cuando se alcanza este límite.
* Puede ver tres o cuatro períodos de tiempo, en función del tamaño de la pantalla.

Tenga en cuenta lo siguiente al exportar información desde la vista Usuario del planificador de recursos, después de haber aplicado todos los filtros y opciones de exportación adecuados:

* Cuando selecciona exportar todo (usuarios, funciones y proyectos) en el Planificador de recursos, todas las funciones, proyectos y usuarios se incluyen en el archivo exportado, tanto si están expandidos como si no en la interfaz web.

* Puede exportar hasta 30 000 filas que contengan usuarios, así como los proyectos y funciones enumerados debajo, independientemente de si se ha desplazado hasta la parte inferior de la lista para mostrarlos o no. Todos los usuarios, proyectos y funciones se incluyen en el archivo exportado, tanto si se expanden como si no en la interfaz web.
* Las filas sin información de asignación se incluyen en el archivo exportado.
