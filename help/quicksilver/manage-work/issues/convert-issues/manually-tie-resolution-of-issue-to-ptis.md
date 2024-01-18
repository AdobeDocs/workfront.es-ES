---
product-area: projects
navigation-topic: convert-issues
title: Asociar manualmente la resolución de un problema a otros problemas, tareas o proyectos
description: Puede asociar manualmente la resolución de un problema a la resolución de un proyecto, tarea o problema sin convertir el problema. El problema se convierte en uno de los objetos solucionables del proyecto, tarea o problema que seleccione. Al hacerlo, cualquier cambio en el estado del proyecto, tarea o problema déclencheur un cambio en el estado del problema original.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# Asociar manualmente la resolución de un problema a otros problemas, tareas o proyectos

Puede asociar manualmente la resolución de un problema a la resolución de un proyecto, tarea o problema sin convertir el problema. El problema se convierte en uno de los objetos solucionables del proyecto, tarea o problema que seleccione. Al hacerlo, cualquier cambio en el estado del proyecto, tarea o problema déclencheur un cambio en el estado del problema original.

>[!TIP]
>
>Cuando vincula la resolución de un problema con la resolución de otro objeto, ya no puede editar manualmente el estado del problema original.

Para obtener más información sobre la resolución de objetos y los objetos que se pueden resolver, consulte [Información general sobre la resolución y los objetos solucionables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas, Tareas y Proyectos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el problema que vincula a otro problema, tarea o proyecto</p> <p>Vea o aumente los permisos para el problema, tarea o proyecto que agregue al problema existente</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Requisitos previos

Antes de empezar, debe:

* Tiene un problema cuya resolución desea vincular con la resolución de otro problema, tarea o proyecto

* Tener un problema, tarea o proyecto adicional

## Vincular la resolución de un problema a la resolución de otro problema, tarea o proyecto

1. Vaya a un problema cuya resolución desee vincular con la resolución de otro problema o con la resolución de una tarea o proyecto.
1. Haga clic en **Detalles del problema** en el panel izquierdo y, a continuación, expanda **Información general** área.

   ![](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. Haga clic en **Resuelto por** y seleccione entre los siguientes tipos de objetos de resolución:

   * **Proyecto**
   * **Tarea**
   * **Problema**

   Según el objeto seleccionado, se muestran los campos siguientes:

   * **Resolviendo proyecto**
   * **Resolviendo tarea**
   * **Resolviendo problema**

1. Empiece a escribir el nombre de un proyecto, tarea o problema específico en la **Resolviendo proyecto**, **Tarea**, o **Problema** y, a continuación, haga clic en él cuando aparezca en la lista.

   >[!NOTE]
   >
   >No puede enlazar la resolución de un problema con la tarea o el proyecto donde se encuentra el problema. La tarea o el proyecto del problema no se muestran en los campos Tarea de resolución o Tarea de resolución.


1. Haga clic en **Guardar cambios**.

   El problema original se convierte en el objeto solucionable del proyecto, tarea o problema seleccionado en los pasos 4 y 5. Esto significa que el problema original se resuelve al finalizar el objeto de resolución (el proyecto, la tarea o el problema al que lo vinculó).

   >[!NOTE]
   >
   >Un proyecto, tarea o problema puede tener varios problemas como objetos solucionables.
