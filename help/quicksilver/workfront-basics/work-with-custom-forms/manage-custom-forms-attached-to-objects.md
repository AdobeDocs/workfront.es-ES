---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Administrar formularios personalizados adjuntos a objetos
description: Se puede actualizar el orden en que aparecen los formularios personalizados adjuntos a un objeto, eliminarlos o editarlos de forma masiva para mostrar los formularios personalizados en varios objetos.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 6580fec18982215dbc2535d5f2ab159fc32ac3f5
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# Administrar formularios personalizados adjuntos a objetos

Se puede actualizar el orden en que aparecen los formularios personalizados adjuntos a un objeto, eliminarlos o editarlos de forma masiva para mostrar los formularios personalizados en varios objetos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar las acciones descritas en este artículo:

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
   <td> <p>Editar acceso a los objetos para los que se administran formularios personalizados</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Contribute o superior a los objetos para los que administra formularios personalizados</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

* El administrador de Workfront o un usuario de Plan con acceso administrativo a formularios personalizados deben crear formularios personalizados en su entorno. Para obtener más información, consulte [Crear o editar un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* Debe tener formularios personalizados adjuntos a un objeto.

   Para obtener información sobre cómo aplicar formularios personalizados a un objeto, consulte [Adición de un formulario personalizado a un objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Reordenar varios formularios personalizados adjuntos a un objeto {#reorder-multiple-custom-forms-attached-to-an-object}

1. Vaya al objeto en el que desea cambiar el orden de los formularios personalizados añadidos y, a continuación, comience a editar el objeto.

   **Ejemplo:** Por ejemplo, para administrar los formularios personalizados de un proyecto, vaya al proyecto y haga clic en el botón **Más** menú ![](assets/more-icon.png)y haga clic en **Editar** .

1. En el **Forms personalizado** para proyectos, tareas y problemas, haga clic en la ![](assets/move-icon---dots.png) junto al nombre de un formulario personalizado. Para el resto de objetos, haga clic en **Administrar Forms**. Esta opción solo se muestra si al menos un formulario personalizado está adjunto al objeto.
1. Arrastrar un formulario ![](assets/move-icon---dots.png) a una nueva ubicación de la lista.
1. Para proyectos, tareas y problemas con los formularios personalizados, haga clic en **Guardar**.

   Para el resto de objetos, haga clic en **He terminado de administrar** > **Guardar cambios**.

## Eliminación de un formulario personalizado de un objeto {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>Cuando se quita un formulario personalizado de un objeto, toda la información capturada en los campos personalizados del formulario se pierde y no se puede recuperar.

1. Vaya al objeto en el que desea quitar el formulario personalizado y empiece a editar el objeto.

   Por ejemplo, vaya a un proyecto y haga clic en el **Más** menú ![](assets/more-icon.png)y haga clic en **Editar** .

1. Haga clic en **Forms personalizado**.
1. Para proyectos, tareas y problemas con los formularios personalizados, haga clic en el botón **X** a la derecha de un formulario para quitarlo del objeto.

   Para el resto de objetos, haga clic en **Administrar Forms** y, a continuación, haga clic en el botón **X** a la derecha de un formulario para quitarlo del objeto.

1. Haga clic en **Guardar** .

## Administrar varios formularios personalizados que contienen los mismos campos personalizados

Es posible que el mismo campo aparezca en varios formularios personalizados adjuntos al mismo objeto. En este caso, tenga en cuenta lo siguiente:

* El valor del campo es idéntico en todos los formularios.

   No puede haber valores diferentes para los mismos campos en formularios diferentes adjuntos al mismo objeto.

* Si tiene los mismos campos calculados en dos objetos diferentes, sus cálculos deben ser idénticos para evitar errores. Para obtener información sobre cómo agregar campos calculados a formularios personalizados, incluidos varios formularios, consulte [Agregar datos calculados a un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) .

## Editar varios formularios personalizados al editar objetos por lotes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section will need to be edited when the bulk Edit box is released to NWE; add some screen shots for NWE) </p>
-->

Cuando se editan objetos por lotes que tienen varios formularios personalizados aplicados, se puede editar la forma en que se muestran los formularios personalizados en esos objetos, así como editar campos comunes en los formularios personalizados.

En una edición masiva solo se pueden editar los formularios personalizados adjuntos a todos los objetos seleccionados.

Para editar varios formularios personalizados al editar objetos de forma masiva:

1. En los objetos de una lista, seleccione los objetos a los que están adjuntos los formularios personalizados y, a continuación, haga clic en el botón **Editar** icono ![](assets/edit-icon.png).
1. Haga clic en **Forms personalizado**.

   Solo se pueden editar los formularios personalizados adjuntos a todos los objetos seleccionados.

   Los formularios personalizados adjuntos únicamente a algunos de los objetos no se muestran.

1. Comience a editar campos en los formularios personalizados.

   Cuando se editan los campos, se muestra un indicador visual en el campo que muestra que se ha editado el campo.

   Si un campo se incluye en más de un formulario personalizado, todos los valores de esos campos se actualizan en cada formulario al actualizar el campo en uno de los formularios.

1. Haga clic en el **Realización de una selección** menú desplegable y seleccione formularios adicionales para agregar a todos los objetos seleccionados.

   Tenga en cuenta lo siguiente al aplicar formularios adicionales:

   * Los objetos pueden tener hasta 10 formularios personalizados.
   * Los formularios solo se pueden aplicar cuando el formulario no se haya aplicado a ninguno de los objetos que esté editando. Un formulario que ya está adjunto a uno de los objetos no aparece en el menú desplegable.
   * Después de aplicar un formulario adicional, todos los campos que tengan un formulario común con otros formularios se muestran en la variable **Campos comunes** y se pueden editar.

1. (Opcional) Si ha agregado formularios personalizados a todos los objetos pero aún no los ha guardado, puede cambiar el orden en que aparecen los formularios personalizados en los objetos.

   Para obtener más información sobre cómo cambiar el orden de los formularios, consulte [Reordenar varios formularios personalizados adjuntos a un objeto](#reorder-multiple-custom-forms-attached-to-an-object) en este artículo.

1. Haga clic en **Quitar formulario** para quitar un formulario personalizado de los objetos.

   Para obtener más información sobre cómo quitar formularios personalizados de objetos, consulte [Eliminación de un formulario personalizado de un objeto](#remove-a-custom-form-from-an-object).

   Tenga en cuenta lo siguiente al quitar formularios de forma masiva de varios objetos:

   * Si ha realizado cambios en el formulario, eliminarlo hace que los cambios se pierdan y no se puedan recuperar.
   * Después de quitar un formulario, los campos de ese formulario que se encuentren en la variable **Campos comunes** se eliminan de esta sección y ya no se pueden editar aquí.

1. Haga clic en **Restaurar formulario** para restaurar el formulario al estado en el que se encontraba antes de editar los objetos.
1. (Opcional) Haga clic en la flecha de contracción situada junto al nombre del formulario para contraer de uno en uno.

   O

   Haga clic en **Contraer Forms** para contraer todos los formularios al mismo tiempo.

1. (Opcional) Haga clic en la flecha de expansión situada junto al nombre del formulario para expandir un formulario a la vez.

   O

   Haga clic en **Expandir Forms** para expandir todos los formularios al mismo tiempo. 

1. Haga clic en **Guardar cambios**.
