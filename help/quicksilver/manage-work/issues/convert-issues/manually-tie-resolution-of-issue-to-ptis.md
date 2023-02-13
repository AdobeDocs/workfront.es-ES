---
product-area: projects
navigation-topic: convert-issues
title: Vincular manualmente la resolución de un problema con otros problemas, tareas o proyectos
description: Puede vincular manualmente la resolución de un problema a la resolución de un proyecto, tarea o problema sin convertir el problema. El problema se convierte en uno de los objetos resueltos del proyecto, la tarea o el problema que seleccione. Al hacerlo, un cambio en el estado del proyecto, la tarea o el problema déclencheur un cambio en el estado del problema original.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# Vincular manualmente la resolución de un problema con otros problemas, tareas o proyectos

Puede vincular manualmente la resolución de un problema a la resolución de un proyecto, tarea o problema sin convertir el problema. El problema se convierte en uno de los objetos resueltos del proyecto, la tarea o el problema que seleccione. Al hacerlo, un cambio en el estado del proyecto, la tarea o el problema déclencheur un cambio en el estado del problema original.

>[!TIP]
>
>Cuando se vincula la resolución de un problema con la resolución de otro objeto, ya no se puede editar manualmente el estado del problema original.

Para obtener más información sobre la resolución y resolución de objetos, consulte [Información general sobre la resolución y resolución de objetos](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas, Tareas y Proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos para el problema que vincula a otro problema, tarea o proyecto</p> <p>Ver los permisos o los permisos superiores del problema, tarea o proyecto que agregue al problema existente</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de comenzar, debe:

* Tenga un problema cuya resolución desee vincular con la resolución de otro problema, tarea o proyecto

* Tener un problema, tarea o proyecto adicional

## Vincular la resolución de un problema con la resolución de otro problema, tarea o proyecto

1. Vaya a un problema cuya resolución desee vincular con la resolución de otro problema o una tarea o proyecto.
1. Haga clic en el **Detalles del problema** > **Información general** .

   ![](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. Vaya a la **Información general** en el **Detalles del problema** para obtener más información.
1. Haga clic en el **Resuelto por** y seleccione entre los siguientes tipos de objetos resueltos:  

   * **Proyecto**
   * **Tarea**
   * **Problema**

1. Se muestra el campo del objeto de resolución.
1. Después de seleccionar el objeto, empiece a escribir el nombre de un proyecto, tarea o problema específico en el campo disponible y selecciónelo cuando aparezca en la lista desplegable.
1. Haga clic en **Guardar** **Cambios**.\
   El problema original se convierte en el objeto resuelto para el proyecto, la tarea o el problema seleccionado en los pasos 4 y 5. Esto significa que el problema original se completa cuando se completa el objeto resuelto (el proyecto, la tarea o el problema al que lo vinculó).

   >[!NOTE]
   >
   >Un proyecto, tarea o problema puede tener varios problemas como Objetos resueltos.

 
