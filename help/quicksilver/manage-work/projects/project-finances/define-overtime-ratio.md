---
content-type: overview
product-area: projects
navigation-topic: financials
title: Definir una proporción de horas extra
description: Puede definir una proporción de horas extra en una tarea para ajustar el cálculo de ingresos planificados para las asignaciones de tareas.
author: Lisa
feature: Work Management
exl-id: 832d3aab-3e09-4d83-91a6-be0145ce3554
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 15%

---

# Definir una proporción de horas extra

Cuando se agrega una proporción de horas extra a una tarea, se aplica a todas las asignaciones de la tarea. Multiplica todas las horas planificadas para esa tarea y afecta los cálculos de ingresos planificados.

La proporción de horas extra no puede variar para asignaciones dentro de la misma tarea. Si se requieren multiplicadores de horas extra diferentes, debe crear subtareas independientes bajo una tarea principal.

>[!NOTE]
>
>No hay ninguna validación que impida agregar la proporción de horas extra a una tarea que no sea de horas extra.

## Cálculo de horas extra en ingresos planificados

El sistema determina primero la tasa de facturación utilizando la jerarquía de tasas de facturación estándar. Para obtener más información, consulte [Información general sobre la jerarquía de ingresos y costos](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

Si existe la proporción de horas extra en la tarea, el cálculo es el siguiente:
Ingresos planificados = tarifa de facturación × proporción de horas extra × horas planificadas

Si la proporción de horas extra está en blanco, el cálculo es el siguiente:
Ingresos planificados = tarifa de facturación × horas planificadas

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>Estándar</td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Editar acceso a tareas, proyectos y datos financieros</td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td><p>Administrar permisos para una tarea que incluya Editar tarifas de facturación</p>
     <p>Permisos de aportación o superiores para el proyecto</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

El tipo de ingresos de la tarea debe ser Usuario y Rol por hora. Para obtener más información, consulte [Información general sobre la jerarquía de ingresos y costos](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

El campo **Proporción de horas extra** debe estar habilitado en la plantilla de diseño.

1. En la plantilla de diseño, haga clic en la flecha abajo debajo de **Personalizar lo que ven los usuarios** y, a continuación, haga clic en **Tarea**.
1. En la sección **Detalles**, seleccione el campo **Proporción de horas extra** en el área **Finanzas**.

   Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

## Definir la proporción de horas extra en una tarea

1. Vaya a la tarea que desee editar.

   Para obtener más información, consulte [Administrar finanzas de tareas en la sección Detalles de tareas](/help/quicksilver/manage-work/tasks/manage-tasks/task-finances-in-details.md).

1. Haga clic en **Detalles de tarea** en el panel de la izquierda.
1. En el área **Finanzas**, escriba el multiplicador de horas extra en el campo **Proporción de horas extra**.
1. Haga clic en **Guardar cambios**.
