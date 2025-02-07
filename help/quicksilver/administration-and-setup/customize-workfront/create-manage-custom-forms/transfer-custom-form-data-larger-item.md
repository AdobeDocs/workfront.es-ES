---
title: Transferir datos de formulario personalizados al convertir un objeto
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Cuando el trabajo definido en un elemento de trabajo es demasiado grande, puede convertirlo en un elemento de trabajo más grande.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 98%

---

# Transferir datos de formulario personalizados al convertir un objeto

Según las necesidades comerciales de su organización, el trabajo definido en una tarea o un problema puede llegar a ser demasiado grande para administrarlo dentro de la tarea o el problema. En este caso, puede convertirlo en un elemento de trabajo más grande:

* Puede convertir problemas en tareas o en proyectos
* Puede convertir tareas en proyectos

Para transferir datos de formularios personalizados de un problema a una tarea o un proyecto, debe completar las dos tareas de este artículo en el orden siguiente.

Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) o [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Para realizar los pasos de este artículo, debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Plan de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Primero: añadir objetos adicionales al formulario personalizado

{{step-1-to-setup}}

1. Haga clic en **Formularios personalizados**.
1. Busque el formulario que necesita y luego haga clic en ![Editar icono](assets/edit-icon.png).
1. En la parte superior del formulario, añada el objeto al que piensa convertir la tarea o el problema.

   >[!INFO]
   >
   >**Ejemplo**: si desea transferir los datos del formulario personalizado a un proyecto, seleccione Proyecto.

1. Haga clic en **Aplicar** en la parte inferior del formulario.

1. Continúe hasta [Segundo: convertir el problema o la tarea y transferir los datos del formulario personalizado](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Segundo: convertir el problema o la tarea y transferir los datos del formulario personalizado {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Añada objetos adicionales al formulario personalizado en el problema o la tarea que está convirtiendo, tal como se explica en la sección [Primero: añadir objetos adicionales al formulario personalizado](#first-add-additonal-objects-to-the-custom-form) en este artículo.
1. Convierta el problema o la tarea mediante la opción **Formularios personalizados** en el cuadro que se muestra para seleccionar el formulario personalizado que necesita. Para obtener instrucciones, consulte los siguientes artículos:

   * [Convertir un problema en un proyecto en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Conversión de un problema en una tarea en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Convertir una tarea en un proyecto](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. En el cuadro de diálogo **Convertir en (tipo de objeto)** que se muestra, haga clic en el menú desplegable **Agregar formularios** y seleccione el formulario que copió en la sección anterior.

   La información capturada en los campos personalizados del problema ahora se transfiere al formulario personalizado de la tarea.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->