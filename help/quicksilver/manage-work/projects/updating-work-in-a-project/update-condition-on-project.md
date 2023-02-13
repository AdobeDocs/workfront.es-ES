---
product-area: projects
navigation-topic: update-work-in-a-project
title: Actualizar condición para un proyecto
description: La condición de un proyecto es un indicador que se le coloca para indicar si el trabajo asociado a él va sin problemas o si se ha encontrado algún obstáculo. Es distinto al estado del proyecto, que indica si está trabajando activamente en él o no.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 1%

---

# Actualizar condición para un proyecto

La condición de un proyecto es un indicador que se le coloca para indicar si el trabajo asociado a él va sin problemas o si se ha encontrado algún obstáculo. Es distinto al estado del proyecto, que indica si está trabajando activamente en él o no.

Puede establecer la condición de un proyecto de forma automática o manual. Para cambiar manualmente la condición de un proyecto, debe ser el propietario del proyecto o tener derechos de gestión para él.

El administrador de Adobe Workfront puede crear condiciones personalizadas para su entorno, tal como se describe en [Creación o edición de una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Requisitos de acceso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the current licenses:
  <p>Standard</p>
   
   For legacy licenses:
   <ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Establecer automáticamente la condición

La configuración automática de la condición de un proyecto viene determinada por el tipo de condición del proyecto. El tipo de condición debe estar establecido en Progreso de estado para que Workfront establezca automáticamente la condición del proyecto.

El administrador de Workfront o de grupo determina el valor predeterminado del campo Tipo de condición para los nuevos proyectos del sistema al establecer las preferencias del proyecto en el área Configuración. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Cuando crea un proyecto, la condición del proyecto se establece automáticamente para que coincida con el estado de progreso del proyecto en ese momento. El estado de progreso del proyecto se basa en el progreso de las tareas del proyecto.

Para obtener información sobre las condiciones del proyecto y cómo se calculan en función del estado de progreso, consulte [Resumen del estado del progreso del proyecto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## Actualizar manualmente la condición de un proyecto

Si establece el tipo de condición de su proyecto en Manual en lugar de en Estado de progreso, puede actualizar manualmente la condición de un proyecto.

1. Vaya al proyecto para el que desea actualizar la condición.
1. Haga clic en el **Detalles del proyecto** para obtener más información.

   ![](assets/project-details-overview-edit-enabled-with-condition-shot-nwe-350x251.png)

1. Asegúrese de que la variable **Tipo de condición** el campo está definido como **Manual**.

1. En el **Condición** , seleccione entre las siguientes opciones la que coincida con su comprensión de si el trabajo asociado a él va sin problemas o si hay algún retraso:

   * **Bien encaminado**
   * **En riesgo**
   * **Con problemas**

   Para obtener más información sobre las condiciones del proyecto, consulte [Descripción general de la condición y el tipo de condición del proyecto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >Las condiciones se pueden personalizar para su entorno, por lo que puede encontrar más de tres opciones para Condición en su entorno. Los nombres de las Condiciones pueden ser diferentes de los indicados arriba. Para obtener información sobre la personalización de condiciones en Workfront, consulte [Creación o edición de una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Haga clic en **Guardar**.Click **Guardar cambios**.
