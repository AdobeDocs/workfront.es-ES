---
content-type: overview
product-area: projects
navigation-topic: financials
title: Configurar un rol de trabajo para facturación
description: Workfront le permite facturar a un usuario con una función de trabajo diferente a su función de trabajo principal. Esto resulta útil cuando una persona realiza temporalmente un trabajo que debería facturarse a una tasa diferente.
author: Lisa
feature: Work Management
exl-id: d6e2947d-2f40-4591-b048-9a769caadf43
source-git-commit: a7f7099f3de147ed166ab19ac44608ba01eb6d31
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 6%

---

# Configurar un rol de trabajo para facturación

Workfront le permite facturar a un usuario con una función de trabajo diferente a su función de trabajo principal. Esto resulta útil cuando una persona realiza temporalmente un trabajo que debería facturarse a una tasa diferente.

Puede asignar un rol para facturación de dos formas:

* En el nivel de proyecto: Utilícelo cuando la persona deba facturarse en el mismo rol para todo el proyecto.
* En el nivel de asignación: Utilícelo cuando desee facturar de forma diferente en tareas específicas.

>[!NOTE]
>
>* Un rol de facturación se aplica solamente a las personas (usuarios). No se aplica a los roles genéricos ni a los marcadores de posición.
>* Agregar un Rol para Facturación afecta solamente la tarifa de facturación, no el costo.
>* La facturación de nivel de asignación siempre tiene prioridad sobre la facturación de nivel de proyecto.

Para obtener más información, consulte [Información general sobre la jerarquía de ingresos y costos](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) y [Crear asignaciones avanzadas](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

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
   <td> Editar acceso a las tarjetas de tarifa</td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Administrar permisos del proyecto </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Asignar un rol de facturación en el nivel de proyecto

Cuando crea un rol para la facturación en un proyecto:

* La función de facturación se aplica a todas las tareas y asignaciones dentro del proyecto para ese usuario.
* La facturación utiliza la tasa de facturación del rol seleccionado, pero el costo sigue el rol principal del usuario.

Para asignar un rol de facturación en el nivel de proyecto:

1. Abra un proyecto.
1. Haga clic en **Recurso de facturación** en el panel izquierdo.
1. Seleccione la ficha **Función del puesto para la facturación** si aún no se muestra.
1. Haga clic en **Agregar > Agregar rol para la facturación**.
1. En el cuadro **Agregar rol para facturación**, seleccione el **Usuario**.
1. Seleccione el **rol** que se usará como rol de trabajo para la facturación de este usuario en este proyecto.
1. (Opcional) Haga clic en **Agregar rol** para definir las fechas en vigencia del rol de facturación. Escriba las fechas de **inicio** y **fin** para el rol.

   ![Agregar rol para facturación a nivel de proyecto](assets/jrfb-project-level.png)

1. Vuelva a hacer clic en **Agregar rol** para especificar roles de facturación adicionales para diferentes periodos de tiempo.
1. Haga clic en **Guardar**.

### Ejemplo a nivel de proyecto

>[!BEGINSHADEBOX]

La función principal de John es Designer 1. El proyecto requiere un Designer sénior y John está rellenando.

Establecería el Rol de trabajo para facturación en **Designer sénior** en el nivel de proyecto.

Resultado:

* Ingresos de facturación es la tarifa de Designer sénior
* Coste es la tasa de coste de Designer 1 (tasa de coste real de John)

>[!ENDSHADEBOX]

## Asignar un Rol para Facturación en el nivel de asignación

Cuando agrega un rol para la facturación en una asignación, la configuración anula un rol de facturación de nivel de proyecto solamente para esa asignación específica.

Para asignar un rol para facturación en el nivel de asignación:

1. Abra un proyecto y busque la tarea.
1. Vaya a **Asignaciones avanzadas** de la tarea.

   Para obtener más información, consulte [Crear asignaciones avanzadas](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. En la cuadrícula de asignación de tareas, busque la columna **Rol de trabajo para la facturación**.
1. Seleccione un rol para cada asignación en la que desee una facturación diferente.

   >[!NOTE]
   >
   >Si un rol de facturación se ha asignado en el nivel de proyecto, aparecerá en la asignación. Puede hacer clic en el campo **Rol de la facturación** y seleccionar otro rol para usar en la asignación.
   >El icono de información le informa de si se ha definido un rol de facturación en el nivel de proyecto o de asignación.

   ![Rol de facturación en una asignación](assets/jrfb-assignment-level.png)

### Ejemplo en el nivel de asignación

>[!BEGINSHADEBOX]

La función principal de John es Designer 1. Se le factura como Designer Senior a nivel de proyecto, pero hay una tarea especial que requiere una tarifa de facturación de Designer Principal.

Establecería el Rol para la facturación en Designer principal solo en esa asignación.

Resultado:

* Todas las demás tareas de John se facturan como Designer Senior
* Esta tarea se factura como Designer principal
* El coste sigue siendo Designer 1

>[!ENDSHADEBOX]
