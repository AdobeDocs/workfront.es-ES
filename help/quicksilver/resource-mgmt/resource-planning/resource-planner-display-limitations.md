---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Limitaciones de visualización del Planificador de recursos
description: Para mejorar el rendimiento, Adobe Workfront limita la cantidad de información que se puede mostrar y la cantidad de información que se puede exportar desde el Planificador de recursos.
author: Alina
feature: Resource Management
exl-id: 12f56f11-59fb-4318-b43a-5ac695ca1e7e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---

# Limitaciones de visualización del Planificador de recursos

Para mejorar el rendimiento, Adobe Workfront limita la cantidad de información que se puede mostrar y la cantidad de información que se puede exportar desde el Planificador de recursos.

Cuando se acerca a este límite, Workfront muestra un mensaje de advertencia para informarle de que ha alcanzado el límite.

Si la información que espera ver en el Planificador de recursos no se muestra, es posible que esté tratando de mostrar demasiada información y algunos datos no se hayan mostrado debido a esta limitación.

Recomendamos lo siguiente para obtener un rendimiento óptimo al mostrar y exportar el Planificador de recursos:

* Utilice los filtros para reducir la cantidad de información que se muestra en el Planificador de recursos y vea solamente la información que le interesa.
* Utilice todas las opciones de exportación para reducir la cantidad de información que exporta al mismo tiempo y para asegurarse de exportar únicamente la información pertinente.\
  Para obtener más información sobre el uso de filtros y las opciones de exportación en el Planificador de recursos, consulte [Información sobre filtros en el Planificador de recursos](../../resource-mgmt/resource-planning/filter-resource-planner.md).

  Para obtener información acerca de cómo exportar información desde el Planificador de recursos, vea [Exportar información desde el Planificador de recursos](../../resource-mgmt/resource-planning/export-resource-planner.md).

La cantidad de información que puede mostrar o exportar depende de la vista que aplique y del entorno que utilice para acceder al Planificador de recursos.

## Limitaciones en la vista de proyecto

Tenga en cuenta lo siguiente al aplicar la vista Proyecto al Planificador de recursos:

* Solo puede ver los proyectos a los que tiene acceso para administrar.
* Puede expandir cada proyecto para ver las funciones asociadas a él y cada función para ver los usuarios asociados a él.

  Puede ver hasta 300 proyectos si se desplaza hasta la parte inferior de la lista, a menos que haya más de 30 000 filas de proyectos, funciones y usuarios. A continuación, recibirá un mensaje de advertencia avisándole de que ha alcanzado el límite de 30 000 filas.

* Puede ver tres o cuatro períodos de tiempo a la vez, según el tamaño de la pantalla.

Tenga en cuenta lo siguiente al exportar información desde la vista Proyecto del Planificador de recursos, después de haber aplicado todos los filtros y opciones de exportación adecuados:

* Si selecciona exportar todo (proyectos, funciones y usuarios) en el Planificador de recursos, todos los objetos que coincidan con sus criterios aparecerán en el archivo exportado tanto si se ha desplazado al final de la lista para mostrarlos como si no.
* Las filas sin información de asignación se incluyen en el archivo exportado.

* Puede exportar hasta 30 000 filas.

## Limitaciones en la vista de funciones

Tenga en cuenta lo siguiente al aplicar la vista Rol al Planificador de recursos, después de haber aplicado todos los filtros adecuados:

* Solo puede ver las funciones que están asociadas con proyectos que puede administrar.

* Puede ver hasta 300 funciones cuando se desplace hasta la parte inferior de la lista, a menos que haya más de 30 000 filas de funciones, proyectos y usuarios. A continuación, recibe un mensaje de advertencia avisándole de que ha alcanzado el límite de 30 000 filas para lo que puede ver en la pantalla.
* Puede expandir cada función para mostrar una lista de proyectos y cada proyecto para mostrar una lista de usuarios que pueden desempeñar esas funciones en los proyectos.

  20 proyectos se muestran de forma predeterminada y puede utilizar la opción Cargar más para mostrar proyectos adicionales o desplazarse debajo de cada proyecto para cargar más usuarios.

* Puede ver tres o cuatro períodos de tiempo, según el tamaño de la pantalla.

Tenga en cuenta lo siguiente cuando exporte información desde la vista Rol del Planificador de recursos, después de haber aplicado todos los filtros y opciones de exportación adecuados:

* Si selecciona exportar todo (funciones, proyectos y usuarios) en el Planificador de recursos, todos los objetos que coincidan con sus criterios aparecerán en el archivo exportado tanto si se ha desplazado al final de la lista para mostrarlos como si no.
* Las filas sin información de asignación se incluyen en el archivo exportado.
* Puede exportar hasta 30 000 filas.

## Limitaciones en la vista de usuario

Tenga en cuenta lo siguiente al aplicar la vista Usuario al Planificador de recursos:

* Puede mostrar todos los usuarios que cumplan los siguientes criterios:

   * Tiene acceso para ver
   * Están activos
   * Haber iniciado sesión al menos una vez.

* Puede expandir cada usuario para mostrar los proyectos asociados a él y cada proyecto para mostrar las funciones asociadas a él.\
  Los 50 primeros proyectos y funciones se muestran de forma predeterminada y puede utilizar la opción Cargar más para mostrar proyectos o funciones adicionales.

  >[!NOTE]
  >
  >Si ha filtrado la lista de usuarios por proyectos, solo se pueden expandir los usuarios asociados con los proyectos filtrados y también mostrar la información de las horas

* Puede ver hasta 2000 usuarios en la interfaz web. Workfront muestra un mensaje de advertencia cuando se alcanza este límite.
* Puede ver tres o cuatro períodos de tiempo, según el tamaño de la pantalla.

Tenga en cuenta lo siguiente al exportar información desde la vista Usuario del Planificador de recursos, después de haber aplicado todos los filtros y opciones de exportación adecuados:

* Cuando selecciona exportar todo (usuarios, funciones y proyectos) en el Planificador de recursos, todos los roles, proyectos y usuarios se incluyen en el archivo exportado, independientemente de si están expandidos o no en la interfaz web.

* Puede exportar hasta 30 000 filas que contienen usuarios, así como los proyectos y funciones enumerados debajo, tanto si se ha desplazado al final de la lista para mostrarlos como si no. Todos los usuarios, proyectos y funciones se incluyen en el archivo exportado, independientemente de si están expandidos o no en la interfaz web.
* Las filas sin información de asignación se incluyen en el archivo exportado.
