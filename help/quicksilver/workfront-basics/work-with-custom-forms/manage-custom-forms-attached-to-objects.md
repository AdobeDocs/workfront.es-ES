---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Administrar formularios personalizados adjuntos a objetos
description: Puede actualizar el orden en que se muestran los formularios personalizados adjuntos a un objeto, quitarlos o editar de forma masiva la forma en que se muestran los formularios personalizados en varios objetos.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 0%

---

# Administrar formularios personalizados adjuntos a objetos

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Puede actualizar el orden en que se muestran los formularios personalizados adjuntos a un objeto, quitarlos o editar de forma masiva la forma en que se muestran los formularios personalizados en varios objetos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar las acciones descritas en este artículo:

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
   <td> <p>Editar el acceso a los objetos para los que administra formularios personalizados</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Contribute o superiores para los objetos para los que administra formularios personalizados</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

* El administrador de Workfront o un usuario de Plan con acceso administrativo a los formularios personalizados deben crear formularios personalizados en su entorno. Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Debe tener formularios personalizados adjuntos a un objeto.

  Para obtener información acerca de cómo aplicar formularios personalizados a un objeto, vea [Agregar un formulario personalizado a un objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Reordenar varios formularios personalizados adjuntos a un objeto {#reorder-multiple-custom-forms-attached-to-an-object}

1. Vaya al objeto en el que desea cambiar el orden de los formularios personalizados agregados y, a continuación, comience a editar el objeto.

   **Ejemplo:** Por ejemplo, para administrar los formularios personalizados de un proyecto, vaya al proyecto, haga clic en el menú **Más** ![](assets/more-icon.png) y, a continuación, haga clic en **Editar** .

1. En la sección **Forms personalizado** para proyectos, tareas y problemas, haga clic en el icono ![](assets/move-icon---dots.png) junto al nombre de un formulario personalizado. Para los demás objetos, haz clic en **Administrar Forms**. Esta opción solo se mostrará si hay al menos un formulario personalizado adjunto al objeto.
1. Arrastre un formulario ![](assets/move-icon---dots.png) a una nueva ubicación de la lista.
1. Para los formularios personalizados de proyectos, tareas y problemas, haga clic en **Guardar**.

   Para los demás objetos, haz clic en **He terminado de administrar** > **Guardar cambios**.

## Quitar un formulario personalizado de un objeto {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>Al quitar un formulario personalizado de un objeto, toda la información capturada en los campos personalizados del formulario se pierde y no se puede recuperar.

1. Vaya al objeto donde desea quitar el formulario personalizado y empiece a editar el objeto.

   Por ejemplo, ve a un proyecto, haz clic en el menú **Más** ![](assets/more-icon.png) y luego haz clic en **Editar** .

1. Haga clic en **Forms personalizado**.
1. Para los formularios personalizados de proyectos, tareas y problemas, haga clic en el icono **X** a la derecha de un formulario para quitarlo del objeto.

   Para todos los demás objetos, haz clic en **Administrar Forms** y luego haz clic en el icono **X** a la derecha de un formulario para quitarlo del objeto.

1. Haga clic en **Guardar** .

## Administrar varios formularios personalizados que contengan los mismos campos personalizados

Es posible que el mismo campo aparezca en varios formularios personalizados adjuntos al mismo objeto. En este caso, tenga en cuenta lo siguiente:

* El valor del campo es idéntico en todos los formularios.

  No puede tener valores diferentes para los mismos campos en formularios diferentes adjuntos al mismo objeto.

* Si tiene los mismos campos calculados en dos objetos diferentes, sus cálculos deben ser idénticos para evitar errores. Para obtener información sobre cómo agregar campos calculados a formularios personalizados que incluyen varios formularios, consulte [Agregar campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Administrar varios formularios personalizados al editar objetos por lotes

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>La administración de formularios personalizados a objetos es idéntica para todos los objetos, excepto para los proyectos.
>
>Para obtener información sobre cómo agregar formularios personalizados a proyectos en lotes, consulte el artículo [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).

Cuando edita por lotes objetos que tienen varios formularios personalizados aplicados, puede editar la forma en que se muestran los formularios personalizados en esos objetos, así como editar campos comunes entre los formularios personalizados.

Solo los formularios personalizados adjuntos a todos los objetos seleccionados se pueden editar en una edición masiva.

Para editar varios formularios personalizados al editar objetos de forma masiva:

1. En una lista de objetos, seleccione los objetos donde están adjuntos los formularios personalizados y, a continuación, haga clic en el icono **Editar** ![](assets/edit-icon.png).
1. Haga clic en **Forms personalizado**.

   Solo se pueden editar los formularios personalizados adjuntos a todos los objetos seleccionados.

   Los formularios personalizados adjuntos solo a algunos objetos no se muestran.

1. Comience a editar los campos en los formularios personalizados.

   Cuando se editan los campos, se muestra un indicador visual en el campo que indica que el campo se ha editado.

   Si un campo se incluye en más de un formulario personalizado, todos los valores de esos campos se actualizan en cada formulario al actualizar el campo en uno de los formularios.

1. Haga clic en el menú desplegable **Realizar una selección** y seleccione los formularios adicionales que desee agregar a todos los objetos seleccionados.

   Tenga en cuenta lo siguiente al aplicar formularios adicionales:

   * Los objetos pueden tener hasta 10 formularios personalizados.
   * Los formularios sólo se pueden aplicar cuando el formulario no se haya aplicado ya a ninguno de los objetos que está editando. Un formulario que ya está adjunto a uno de los objetos no aparece en el menú desplegable.
   * Después de aplicar un formulario adicional, los campos que el formulario tenga en común con otros formularios se mostrarán en la sección **Campos comunes** y se podrán editar.

1. (Opcional) Si ha agregado formularios personalizados a todos los objetos, pero aún no los ha guardado, puede cambiar el orden en que aparecen los formularios personalizados en los objetos.

   Para obtener más información sobre cómo cambiar el orden de los formularios, vea [Reordenar varios formularios personalizados adjuntos a un objeto](#reorder-multiple-custom-forms-attached-to-an-object) en este artículo.

1. Haga clic en **Quitar formulario** para quitar un formulario personalizado de los objetos.

   Para obtener más información sobre cómo quitar formularios personalizados de los objetos, vea [Quitar un formulario personalizado de un objeto](#remove-a-custom-form-from-an-object).

   Tenga en cuenta lo siguiente al eliminar formularios de forma masiva de varios objetos:

   * Si ha realizado cambios en el formulario, eliminarlo provoca que se pierdan los cambios y no se puedan recuperar.
   * Después de quitar un formulario, todos los campos de ese formulario que estaban en la sección **Campos comunes** se quitarán de esta sección y ya no se podrán editar aquí.

1. Haga clic en **Restaurar formulario** para restaurar el formulario al estado en el que se encontraba antes de editar los objetos.
1. (Opcional) Haga clic en la flecha de contracción situada junto al nombre del formulario para contraer un formulario cada vez.

   O

   Haga clic en **Contraer Forms** para contraer todos los formularios al mismo tiempo.

1. (Opcional) Haga clic en la flecha de expansión junto al nombre del formulario para expandir un formulario a la vez.

   O

   Haga clic en **Expandir Forms** para expandir todos los formularios al mismo tiempo. 

1. Haga clic en **Guardar cambios**.
