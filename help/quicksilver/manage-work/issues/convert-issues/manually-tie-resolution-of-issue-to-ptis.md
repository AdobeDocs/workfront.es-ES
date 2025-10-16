---
product-area: projects
navigation-topic: convert-issues
title: Asociar manualmente la resolución de un problema a otros problemas, tareas o proyectos
description: Puede asociar manualmente la resolución de un problema con la resolución de un proyecto, tarea o problema sin convertir el problema. El problema se convierte en uno de los objetos solucionables del proyecto, tarea o problema que seleccione. Al hacerlo, cualquier cambio en el estado del proyecto, tarea o problema activa un cambio en el estado del problema original.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 94%

---

# Asociar manualmente la resolución de un problema a otros problemas, tareas o proyectos

<!--Audited: 08/2025-->

Puede asociar manualmente la resolución de un problema con la resolución de un proyecto, tarea o problema sin convertir el problema. El problema se convierte en uno de los objetos solucionables del proyecto, tarea o problema que seleccione. Al hacerlo, cualquier cambio en el estado del proyecto, tarea o problema activa un cambio en el estado del problema original.

>[!TIP]
>
>Cuando vincula la resolución de un problema con la resolución de otro objeto, ya no puede editar manualmente el estado del problema original.

Para obtener más información sobre los objetos que se resuelven y que se pueden resolver, consulte [Información general sobre los objetos que se resuelven y se pueden resolver](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Colaborador o superior</p> 
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas, Tareas y Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para el problema que vincula con otro problema, tarea o proyecto</p> <p>Permisos de visualización o superiores para el problema, tarea o proyecto que añade al problema existente</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues,&nbsp;Tasks, Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue you link to another issue, task, or project</p> <p>View or higher permissions to the issue, task, or project you add to the existing issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Requisitos previos

Antes de empezar, debe hacer lo siguiente:

* Tener un problema cuya resolución desea vincular con la resolución de otro problema, tarea o proyecto

* Tener un problema, tarea o proyecto adicional

## Vincular la resolución de un problema con la resolución de otro problema, tarea o proyecto

1. Vaya a un problema cuya resolución desee vincular con la resolución de otro problema o con la resolución de una tarea o proyecto.
1. Haga clic en **Detalles del problema** en el panel izquierdo y, a continuación, expanda el área de **Información general**.

   ![Icono de detalles del problema](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. Haga clic en el campo **Resuelto por** y seleccione uno de los siguientes tipos de objetos que se pueden resolver:

   * **Proyecto**
   * **Tarea**
   * **Problema**

   Según el objeto seleccionado, se muestran los campos siguientes:

   * **Resolviendo proyecto**
   * **Resolviendo tarea**
   * **Resolviendo problema**

1. Empiece a escribir el nombre de un proyecto, tarea o problema específico en el campo **Resolviendo proyecto**, **Tarea** o **Problema** y, a continuación, haga clic en él cuando aparezca en la lista.

   >[!NOTE]
   >
   >No puede enlazar la resolución de un problema con la tarea o el proyecto donde se encuentra el problema. La tarea o el proyecto del problema no se muestran en los campos Resolviendo tarea o Resolviendo proyecto.


1. Haga clic en **Guardar cambios**.

   El problema original se convierte en el objeto que se puede resolver del proyecto, tarea o problema seleccionado en los pasos 4 y 5. Esto significa que el problema original se resuelve cuando el objeto solucionable (el proyecto, la tarea o el problema al que lo vinculó) finalice.

   >[!NOTE]
   >
   >Un proyecto, tarea o problema puede tener varios problemas como objetos que se pueden resolver.
