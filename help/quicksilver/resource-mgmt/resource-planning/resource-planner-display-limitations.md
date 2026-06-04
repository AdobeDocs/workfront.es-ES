---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Limitaciones de visualización del Planificador de recursos
description: Para mejorar el rendimiento, Adobe Workfront limita la cantidad de información que se puede mostrar y la cantidad de información que se puede exportar desde el Planificador de recursos.
author: Lisa
feature: Resource Management
exl-id: 12f56f11-59fb-4318-b43a-5ac695ca1e7e
TQID: https://experienceleague.adobe.com/5ztX-x5EsELkZ-BvYjQIhWEGIGt3QVMj4bSiuJTqSeE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 948
ht-degree: 99%

---

# Limitaciones de visualización del Planificador de recursos

Para mejorar el rendimiento, Adobe Workfront limita la cantidad de información que se puede mostrar y la cantidad de información que se puede exportar desde el Planificador de recursos.

Cuando se acerca a este límite, Workfront muestra un mensaje de advertencia para informarle de que ha alcanzado el límite.

Si la información que espera ver en el Planificador de recursos no se muestra, es posible que esté tratando de mostrar demasiada información y que algunos datos no se hayan mostrado debido a esta limitación.

Recomendamos lo siguiente para obtener un rendimiento óptimo a la hora de mostrar y exportar el Planificador de recursos:

* Utilice los filtros para reducir la cantidad de información que se muestra en el Planificador de recursos y vea solamente la información que le interesa.
* Utilice todas las opciones de exportación para reducir la cantidad de información que exporta al mismo tiempo y para asegurarse de exportar únicamente la información pertinente.\
  Para obtener más información sobre el uso de filtros y las opciones de exportación en el Planificador de recursos, consulte [Información sobre filtros en el Planificador de recursos](../../resource-mgmt/resource-planning/filter-resource-planner.md).

  Para obtener información acerca de cómo exportar información desde el Planificador de recursos, consulte [Exportar información desde el Planificador de recursos](../../resource-mgmt/resource-planning/export-resource-planner.md).

La cantidad de información que puede mostrar o exportar depende de la vista que aplique y del entorno que utilice para acceder al Planificador de recursos.

## Limitaciones en la vista del proyecto

Tenga en cuenta lo siguiente al aplicar la vista del proyecto al Planificador de recursos:

* Solo puede ver los proyectos a los que tiene acceso de administración.
* Puede expandir cada proyecto para ver las funciones y los usuarios asociados a este.

  Si se desplaza hasta la parte inferior de la lista, puede ver hasta 300 proyectos, a menos que haya más de 30 000 filas de proyectos, funciones y usuarios. A continuación, recibe un mensaje de advertencia avisándole de que ha alcanzado el límite de 30 000 filas.

* Puede ver tres o cuatro períodos de tiempo a la vez, según el tamaño de la pantalla.

Tenga en cuenta lo siguiente al exportar información desde la vista Proyecto del Planificador de recursos, después de haber aplicado todos los filtros y opciones de exportación adecuados:

* Si selecciona exportar todo (proyectos, funciones y usuarios) en el Planificador de recursos, todos los objetos que coincidan con sus criterios aparecerán en el archivo exportado tanto si se ha desplazado al final de la lista para mostrarlos como si no.
* Las filas sin información de asignación se incluyen en el archivo exportado.

* Puede exportar hasta 30 000 filas.

## Limitaciones en la vista de función

Tenga en cuenta lo siguiente al aplicar la vista Función al Planificador de recursos, después de haber aplicado todos los filtros adecuados:

* Solo puede ver las funciones que están asociadas con proyectos que puede administrar.

* Si se desplaza hasta la parte inferior de la lista, puede ver hasta 300 funciones, a menos que haya más de 30 000 filas de funciones, proyectos y usuarios. A continuación, recibe un mensaje de advertencia avisándole de que ha alcanzado el límite de 30 000 filas para lo que puede ver en la pantalla.
* Puede expandir cada función para mostrar la lista de proyectos y la lista de usuarios que pueden desempeñar esas funciones en esos proyectos.

  Se muestran 20 proyectos de forma predeterminada y puede utilizar la opción Cargar más para mostrar proyectos adicionales o desplazarse debajo de cada proyecto para cargar más usuarios.

* Puede ver tres o cuatro períodos de tiempo, según el tamaño de la pantalla.

Tenga en cuenta lo siguiente cuando exporte información desde la vista Función del Planificador de recursos, después de haber aplicado todos los filtros y opciones de exportación adecuados:

* Si selecciona exportar todo (funciones, proyectos y usuarios) en el Planificador de recursos, todos los objetos que coincidan con sus criterios aparecerán en el archivo exportado tanto si se ha desplazado al final de la lista para mostrarlos como si no.
* Las filas sin información de asignación se incluyen en el archivo exportado.
* Puede exportar hasta 30 000 filas.

## Limitaciones en la vista de usuario

Tenga en cuenta lo siguiente al aplicar la vista de usuario al Planificador de recursos:

* Puede mostrar todos los usuarios que cumplan con los siguientes criterios:

   * Tienen acceso de visualización
   * Están activos
   * Ha iniciado sesión al menos una vez.

* Puede expandir cada usuario para mostrar los proyectos asociados a él y cada proyecto para mostrar las funciones asociadas a él.\
  Los 50 primeros proyectos y funciones se muestran de forma predeterminada y puede utilizar la opción Cargar más para mostrar proyectos o funciones adicionales.

  >[!NOTE]
  >
  >Si ha filtrado la lista de usuarios por proyectos, solo se pueden expandir los usuarios asociados con los proyectos filtrados, también se muestra la información de las horas

* Puede ver hasta 2000 usuarios en la interfaz web. Workfront muestra un mensaje de advertencia cuando se alcanza este límite.
* Puede ver tres o cuatro períodos de tiempo, según el tamaño de la pantalla.

Tenga en cuenta lo siguiente al exportar información desde la vista de Usuario del Planificador de recursos, después de haber aplicado todos los filtros y opciones de exportación adecuados:

* Cuando selecciona exportar todo (usuarios, funciones y proyectos) en el Planificador de recursos, todas las funciones, proyectos y usuarios se incluyen en el archivo exportado, independientemente de si están expandidos o no en la interfaz web.

* Puede exportar hasta 30 000 filas que contienen usuarios, así como los proyectos y funciones enumerados debajo, tanto si se ha desplazado al final de la lista para mostrarlos como si no. Todos los usuarios, proyectos y funciones se incluyen en el archivo exportado, independientemente de si están expandidos o no en la interfaz web.
* Las filas sin información de asignación se incluyen en el archivo exportado.
