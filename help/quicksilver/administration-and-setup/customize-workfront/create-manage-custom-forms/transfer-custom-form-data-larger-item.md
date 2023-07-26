---
title: Transferir datos de formulario personalizados al convertir un objeto
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Cuando el trabajo definido en un elemento de trabajo se vuelve demasiado grande, puede convertirlo en un elemento de trabajo más grande.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Transferir datos de formulario personalizados al convertir un objeto

Según las necesidades comerciales de su organización, el trabajo definido en una tarea o un problema puede llegar a ser demasiado grande para administrarlo dentro de la tarea o el problema. En este caso, puede convertirlos en un elemento de trabajo más grande:

* Puede convertir problemas en tareas o en proyectos
* Puede convertir tareas en proyectos

Para transferir datos de formulario personalizados de un problema a una tarea o un proyecto, debe completar las dos tareas de este artículo en el orden siguiente.

Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) o [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo los administradores de Workfront conceden este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué configuraciones de plan, tipo de licencia o nivel de acceso tiene, póngase en contacto con su administrador de Workfront.

## Primero: agregar objetos adicionales al formulario personalizado

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Clic **Forms personalizado**.
1. Busque el formulario que necesita y haga clic en **Editar**.
1. En la parte superior del formulario, agregue el objeto al que planea convertir la tarea o el problema.
   >[!INFO]
   >
   >**Ejemplo**: Si desea transferir los datos de formulario personalizados a un proyecto, seleccione Proyecto.

1. Clic **Aplicar** en la parte inferior del formulario.

1. Continúe en a [Segundo: Convierta el problema o la tarea y transfiera los datos del formulario personalizado](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Segundo: Convierta el problema o la tarea y transfiera los datos del formulario personalizado {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Agregue objetos adicionales al formulario personalizado sobre el problema o la tarea que está convirtiendo, tal como se explica en la sección [Primero: agregar objetos adicionales al formulario personalizado](#first-add-additonal-objects-to-the-custom-form) en este artículo.
1. Convertir el problema o la tarea mediante **Forms personalizado** en el cuadro que aparece para seleccionar el formulario personalizado que necesita. Para obtener instrucciones, consulte los siguientes artículos:

   * [Conversión de un problema en un proyecto en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Conversión de un problema en una tarea en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Conversión de una tarea en un proyecto](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. En el **Convertir a (tipo de objeto)** que aparece, haga clic en el **Añadir Forms** y seleccione el formulario que ha copiado en la sección anterior.

   La información capturada en los campos personalizados del problema ahora se transfiere al formulario personalizado de la tarea.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see the section [Start editing a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) in the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->