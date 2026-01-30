---
product-area: projects
navigation-topic: update-work-in-a-project
title: Actualizar la condición de un proyecto
description: La condición de un proyecto es un indicador que se coloca para indicar si el trabajo asociado con él se está realizando sin problemas o si se ha encontrado con algún obstáculo. Esto es diferente al estado del proyecto, que indica si está trabajando activamente en él o no.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 82%

---

# Actualizar la condición de un proyecto

La condición de un proyecto es un indicador que se coloca para indicar si el trabajo asociado con él se está realizando sin problemas o si se ha encontrado con algún obstáculo. Esto es diferente al estado del proyecto, que indica si está trabajando activamente en él o no.

Puede establecer la condición de un proyecto de forma automática o manual. Para cambiar la condición de un proyecto manualmente, debe ser el propietario del proyecto o tener derechos de administración sobre él.

El administrador de Adobe Workfront puede crear condiciones personalizadas para su entorno, tal como se describe en [Crear o editar una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
  <p>Estándar</p>
   <p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a los proyectos</p> <p>Editar el acceso a tareas y problemas </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización o superiores en tareas y problemas para ver su condición</p>
   <p>Administrar permisos en tareas y problemas para actualizar la condición</p>
     </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the new licenses:
  <p>Standard</p>
   
   For current licenses:
   <ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
     </td> 
  </tr> 
 </tbody> 
</table>-->

## Establecer automáticamente la condición

La configuración automática de la condición de un proyecto viene determinada por el tipo de condición del proyecto. El tipo de condición debe establecerse en Estado de progreso para que Workfront establezca automáticamente la condición del proyecto.

El administrador de Workfront o de grupo determina el valor predeterminado del campo Tipo de condición para los nuevos proyectos del sistema al establecer las preferencias de proyecto en el área de Configuración. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Al crear un proyecto, la condición del proyecto se establece automáticamente para que coincida con el estado de progreso del proyecto en ese momento. El estado del progreso del proyecto se basa en el progreso de las tareas del proyecto.

Para obtener información sobre las condiciones del proyecto y cómo se calculan en función del estado de progreso, consulte [Información general sobre el estado de progreso del proyecto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## Actualizar manualmente la condición de un proyecto

Si establece el tipo de condición del proyecto en Manual en lugar de en Estado de progreso, puede actualizar manualmente la condición de un proyecto.

1. Vaya al proyecto para el que desea actualizar la condición.
1. Haga clic en **Detalles del proyecto** en el panel izquierdo.

1. Asegúrese de que el campo **Tipo de condición** esté establecido en **Manual**.

   ![Detalles del proyecto: información general, seleccionar condición](assets/project-details-overview-select-condition.png)

1. En el campo **Condición**, seleccione de entre las siguientes opciones la que se ajuste a su forma de entender si el trabajo asociado al mismo se está desarrollando sin problemas o si existen retrasos:

   * **Bien encaminado**
   * **En riesgo**
   * **Con problemas**

   Para obtener más información sobre las condiciones del proyecto, consulte [Información general sobre la condición del proyecto y el tipo de condición](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >Las condiciones se pueden personalizar para su entorno, por lo que puede encontrar más de tres opciones para Condición en su entorno. Los nombres de las condiciones pueden ser diferentes a los enumerados anteriormente. Para obtener información sobre cómo personalizar las condiciones en Workfront, consulte [Crear o editar una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Haga clic en **Guardar cambios**.
