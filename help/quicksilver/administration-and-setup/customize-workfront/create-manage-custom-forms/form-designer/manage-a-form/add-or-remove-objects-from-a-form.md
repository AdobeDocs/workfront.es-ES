---
title: Agregar o eliminar tipos de objetos de un formulario personalizado existente con el diseñador de formularios
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede agregar o quitar tipos de objetos de formularios personalizados con el diseñador de formularios.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---


# Agregar o eliminar tipos de objetos de un formulario personalizado existente con el diseñador de formularios

Puede agregar o eliminar tipos de objetos de un formulario personalizado existente con el diseñador de formularios.

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
   <td>
   <p>Plan actual: Estándar</p>
   <p>o</p>
   <p>Plan heredado: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td><p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo los administradores de Workfront conceden este acceso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o configuraciones de nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

## Agregar tipos de objeto a un formulario personalizado existente

Puede agregar tipos de objeto adicionales al formulario para que se puedan adjuntar a varios objetos.

>[!NOTE]
>
>Los permisos de salto de sección pueden verse afectados por el tipo de objeto. Los saltos de sección de permisos de edición limitada para formularios personalizados solo están disponibles para los tipos de objeto Proyecto, Tarea, Problema y Usuario.
>
>Para obtener más información, consulte [Cómo pueden afectar varios tipos de objetos a los permisos de salto de sección](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Forms personalizado** en el panel izquierdo.

   En la vista que aparece, puede revisar todos los formularios personalizados creados para su organización. También puede ver quién creó cada formulario, con qué tipo de objeto funciona y si está activo.

1. Seleccione el formulario personalizado al que desee agregar tipos de objeto adicionales y haga clic en **Editar**.

1. En la parte superior del formulario, haga clic en el signo más + después de **Tipos de objetos** y, a continuación, seleccione el tipo que desee en el menú que se muestra. Puede repetir esto para agregar todos los tipos de objetos que desee.

   ![](assets/add-new-object.png)

1. Haga clic en **Guardar y cerrar**.

   >[!TIP]
   >
   >Puede hacer clic en **Aplicar** en cualquier momento mientras esté creando un formulario personalizado para guardar los cambios y mantener el formulario abierto.

## Eliminar tipos de objetos en un formulario personalizado

Puede eliminar tipos de objetos de un formulario personalizado existente. Un formulario personalizado debe tener al menos un tipo de objeto.

>[!CAUTION]
>
>Si hay personas que ya han adjuntado el formulario personalizado a objetos del tipo que desea eliminar y que le han agregado datos, esos datos se eliminarán de forma permanente cuando elimine ese tipo de objeto en el formulario. Puede incluir información histórica que los usuarios necesitarán más adelante.
>
>En general, se recomienda minimizar el número de veces que se edita un formulario personalizado que ya está en uso. No hay ningún sistema de notificación para avisar a las personas que usen el formulario personalizado sobre sus cambios.

Para eliminar un tipo de objeto:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Forms personalizado** en el panel izquierdo.
1. Seleccione el formulario personalizado que desee editar y haga clic en **Editar**.
1. Haga clic en la X de cualquiera de las **Tipos de objetos** que desea eliminar del formulario y, a continuación, haga clic en **Eliminar** en el mensaje de advertencia que aparece.

   ![](assets/delete-object-types.png)

1. (Opcional) Repita el paso anterior con cualquier otro tipo de objeto que desee quitar del formulario.
1. Haga clic en **Listo** y haga clic en **Cerrar y guardar**.
