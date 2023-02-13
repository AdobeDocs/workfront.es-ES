---
title: Transferir datos de formulario personalizados al convertir un objeto
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Cuando el trabajo definido en un elemento de trabajo se vuelve demasiado grande, puede convertirlo en un elemento de trabajo más grande.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Transferir datos de formulario personalizados al convertir un objeto

Según las necesidades comerciales de su organización, el trabajo definido en una tarea o un problema podría llegar a ser demasiado grande para administrarlo dentro de la tarea o del problema. En este caso, puede convertirlos en un elemento de trabajo más grande:

* Puede convertir problemas en tareas o en proyectos
* Puede convertir tareas en proyectos

Para transferir datos de formulario personalizados de un problema a una tarea o un proyecto, debe completar las dos tareas de este artículo, en el orden siguiente.

Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) o [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront*</p> </td> 
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

&#42;Para saber qué plan, tipo de licencia o configuraciones de nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

## Primero: Copiar el formulario personalizado {#first-copy-the-custom-form}

En primer lugar, debe asegurarse de conservar los datos de formulario personalizados en una tarea o problema que desee convertir. Como los datos del formulario personalizado deben coincidir exactamente con el elemento convertido, se recomienda duplicar el formulario para poder adjuntarlo al nuevo objeto.

>[!TIP]
>
>Otra forma de conservar los datos de formulario personalizados en esta situación es agregar el tipo de objeto más grande al formulario personalizado. Para obtener instrucciones, consulte la sección [Iniciar la edición de un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) en el artículo [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Forms personalizado**.
1. Seleccione el formulario personalizado de tipo tarea o problema y haga clic en **Copiar**.
1. En el **Formulario personalizado** , especifique un nombre para el nuevo formulario.

1. En el **Tipo de formulario** menú desplegable, seleccione el tipo de objeto para el que desea crear el nuevo formulario personalizado

   **Ejemplo:** Si desea transferir los datos de formulario personalizados a un proyecto, seleccione Proyecto.

1. Haga clic en **Copiar formulario**.

   Este formulario personalizado copiado ahora se puede adjuntar a una tarea o proyecto.

1. Continúe con [Segundo: Convertir el problema o la tarea y transferir los datos de formulario personalizados](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Segundo: Convertir el problema o la tarea y transferir los datos de formulario personalizados {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Copie el formulario personalizado en el problema o la tarea que está convirtiendo, tal como se explica en la sección [Primero: Copiar el formulario personalizado](#first-copy-the-custom-form) en este artículo.
1. Convertir el problema o la tarea mediante la variable **Forms personalizado** en el cuadro que aparece para seleccionar el formulario personalizado que ha copiado. Para obtener instrucciones, consulte los siguientes artículos:

   * [Convertir un problema en un proyecto en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Conversión de un problema en una tarea en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Conversión de una tarea en un proyecto](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. En el **Convertir a (tipo de objeto)** que se muestra, haga clic en el botón **Añadir Forms** menú desplegable y seleccione el formulario que ha copiado en la sección anterior.

   La información capturada en los campos personalizados del problema se transfiere ahora al formulario personalizado de la tarea.

