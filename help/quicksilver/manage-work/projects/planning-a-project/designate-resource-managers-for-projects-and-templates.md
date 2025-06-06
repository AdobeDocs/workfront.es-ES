---
product-area: projects;templates
navigation-topic: plan-a-project
title: Designar administradores de recursos para un proyecto o una plantilla
description: Puede designar administradores de recursos para un proyecto con el fin de indicar quién es el responsable de administrar los recursos del proyecto.
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 98%

---

# Designar administradores de recursos para un proyecto o una plantilla

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

Puede designar administradores de recursos para un proyecto con el fin de indicar quién es el responsable de administrar los recursos del proyecto. Este es un campo informativo y no está conectado a ninguna herramienta de administración de recursos.

<!-- drafted for res scheduling deprecation blurb for preview release
Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in Adobe Workfront, in the Production environment.
  
>[!CAUTION]  
>  
>  
> <span class="preview">Some of the information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span>  
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span>  
>  
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../../resource-mgmt/workload-balancer/workload-balancer.md).</span>  
>  
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

## Requisitos de acceso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Templates</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> 
   
   <p><b>NOTE</b>
   
   Users who are added as Resource Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a proyectos y plantillas</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración sobre el proyecto o la plantilla</p>

<p><b>NOTA</b>

Los usuarios que se añaden como administradores de recursos a un proyecto o una plantilla obtienen inmediatamente permisos de administración sobre el proyecto o la plantilla</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Consideraciones sobre los administradores de recursos

>[!NOTE]
>
>El Administrador de recursos no es una función; es un campo disponible en un proyecto o una plantilla que se puede actualizar manualmente.

* Puede designar hasta 30 usuarios como administradores de recursos para un proyecto o plantilla individual.

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Workload Balancer overview](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* No se pueden designar equipos o grupos como administradores de recursos. Solo puede designar usuarios como administradores de recursos.

* Los usuarios que designe como administradores de recursos de un proyecto o plantilla no se convierten automáticamente en parte del equipo del proyecto.

  Para obtener información sobre los equipos del proyecto, consulte [Administrar el equipo del proyecto](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* Puede designar administradores de recursos para proyectos o para plantillas de proyectos. Cuando se designan administradores de recursos de una plantilla de proyecto, los usuarios que se designen como administradores de recursos de la plantilla se convertirán automáticamente en administradores de recursos de cualquier proyecto que se cree con esa plantilla.
* Puede ver el campo Administrador de recursos en las áreas siguientes:

   * Al editar un proyecto, tal como se describe en este artículo.
   * Al editar una plantilla, tal como se describe en este artículo.
   * Al crear informes de proyecto o plantilla. Para obtener información sobre cómo administrar informes, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * Al crear o personalizar una vista de proyecto o de plantilla para una lista. Para obtener más información, consulte [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* Puede añadir o quitar rápidamente Administradores de recursos de varios proyectos o plantillas añadiendo el campo Administrador de recursos a una vista de una lista o proyecto y editando este campo mediante la edición en línea.

## Designar administradores de recursos para un proyecto

1. Realice una de las siguientes acciones:

   * Para añadir administradores de recursos a un solo proyecto, vaya al proyecto donde desee designar uno o varios administradores de recursos y, a continuación, haga clic en el **menú Más** junto al nombre del proyecto y, a continuación, en **Editar.**

   * Para añadir administradores de recursos a varios proyectos simultáneamente, vaya a una lista de proyectos, seleccione los proyectos donde desee designar uno o más administradores de recursos y, a continuación, haga clic en **Editar**.

     Los administradores de recursos existentes no se eliminan de los proyectos que está editando; los usuarios que añada de esta manera se añadirán como administradores de recursos del proyecto, además de los administradores de recursos existentes.

   * Para añadir administradores de recursos a un nuevo proyecto, empiece a crear uno nuevo.

     Para obtener información sobre cómo crear un proyecto, consulte [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

1. En la sección **Información general** del cuadro de diálogo Editar proyecto, haga clic en el campo **Administrador de recursos**.
1. Empiece escribiendo el nombre del usuario que desea añadir como administrador de recursos para el proyecto y, a continuación, haga clic en el nombre cuando aparezca en la lista.

   Repita este paso para añadir varios administradores de recursos para el proyecto.

1. Haga clic en **Guardar cambios**.

## Designar administradores de recursos para una plantilla

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Plantillas**.

1. Realice una de las siguientes acciones:

   * Para añadir administradores de recursos a una sola plantilla, vaya a la plantilla donde desee designar uno o varios administradores de recursos y, a continuación, haga clic en el **menú Más** junto al nombre de la plantilla y, a continuación, en **Editar .**

   * Para añadir administradores de recursos a varias plantillas simultáneamente, vaya a una lista de plantillas, seleccione las plantillas en las que desee designar uno o varios administradores de recursos y, a continuación, haga clic en **Editar**.

     Los administradores de recursos existentes no se eliminan de las plantillas que está editando; los usuarios que añada de esta forma se añadirán como administradores de recursos a la plantilla, además de los administradores de recursos existentes.

   * Para añadir administradores de recursos a una plantilla nueva, haga clic en **Nueva plantilla**, luego haga clic en el **menú Más** junto al nombre de la plantilla y, a continuación, en **Editar .**

1. En la sección **Información general**, haga clic en el campo **Administrador de recursos**.
1. Comience a escribir el nombre del usuario que desea añadir como administrador de recursos para la plantilla y, a continuación, haga clic en el nombre cuando aparezca en la lista.

   Repita este paso para añadir varios administradores de recursos a la plantilla.

1. Haga clic en **Guardar cambios**.
