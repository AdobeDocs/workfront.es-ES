---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Administrar formularios personalizados adjuntos a objetos
description: Puede actualizar el orden en que se muestran los formularios personalizados adjuntos a un objeto, quitarlos o editar de forma masiva cómo se muestran los formularios personalizados en varios objetos.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 322257a21f5d415b0ac04e6944c4aaa53fc3ab3b
workflow-type: tm+mt
source-wordcount: '1088'
ht-degree: 89%

---

# Administrar formularios personalizados adjuntos a objetos

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Está disponible para todos los clientes en el entorno de vista previa y para un grupo selecto de clientes en el entorno de producción.</span>

Puede actualizar el orden en que se muestran los formularios personalizados adjuntos a un objeto, quitarlos o editar de forma masiva cómo se muestran los formularios personalizados en varios objetos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar las acciones descritas en este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a los objetos para los que administra los formularios personalizados</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos Contribuir o superiores para los objetos para los que administra formularios personalizados</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

* El administrador de Workfront o un usuario de Plan con acceso administrativo a los formularios personalizados deben crear formularios personalizados en su entorno. Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Debe tener formularios personalizados adjuntos a un objeto.

  Para obtener información sobre cómo aplicar formularios personalizados a un objeto, consulte [Añadir un formulario personalizado a un objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Reordenar varios formularios personalizados adjuntos a un objeto {#reorder-multiple-custom-forms-attached-to-an-object}

1. Vaya al objeto en el que desea cambiar el orden de los formularios personalizados añadidos y, a continuación, comience a editar el objeto.

   **Ejemplo:** por ejemplo, para administrar los formularios personalizados de un proyecto, vaya al proyecto, haga clic en el menú **Más** ![](assets/more-icon.png) y, a continuación, haga clic en **Editar**.

1. En la sección **Formularios personalizados** para proyectos, tareas y problemas, haga clic en el icono ![](assets/move-icon---dots.png) situado junto al nombre de un formulario personalizado. Para los demás objetos, haga clic en **Administrar formularios**. Esta opción solo se mostrará si hay al menos un formulario personalizado adjunto al objeto.
1. Arrastre un formulario ![](assets/move-icon---dots.png) a una nueva ubicación de la lista.
1. Para los formularios personalizados de proyectos, tareas y problemas, haga clic en **Guardar**.

   Para los demás objetos, haga clic en **He terminado de administrar** > **Guardar cambios**.

## Quitar un formulario personalizado de un objeto {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>Cuando se quita un formulario personalizado de un objeto, toda la información capturada en los campos personalizados del formulario se pierde y no se puede recuperar.

1. Vaya al objeto donde desea quitar el formulario personalizado y, a continuación, haga clic en la sección **Detalles** del panel izquierdo del objeto.

   Por ejemplo, vaya a un proyecto y haga clic en la sección **Detalles del proyecto**.

1. Haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png) en la esquina superior derecha de la página del objeto y, a continuación, haga clic en **Editar todo**.
1. Haga clic en el icono **Eliminar** ![](assets/delete-icon.png) a la derecha del nombre de un formulario personalizado y, a continuación, haga clic en **Eliminar** para confirmar y quitar el formulario del objeto o en **Cancelar** para evitar la eliminación.
1. Haga clic en **Guardar cambios** .

## Administrar varios formularios personalizados que contengan los mismos campos personalizados

Es posible que el mismo campo aparezca en varios formularios personalizados adjuntos al mismo objeto. En este caso, tenga en cuenta lo siguiente:

* El valor del campo es idéntico en todos los formularios.

  No es posible tener distintos valores para los mismos campos en formularios diferentes adjuntos al mismo objeto.

* Si tiene los mismos campos calculados en dos objetos diferentes, sus cálculos deben ser idénticos para evitar errores. Para obtener información sobre cómo añadir campos calculados a formularios personalizados que incluyen varios formularios, consulte [Añadir campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Administrar varios formularios personalizados al editar objetos de forma masiva

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>La administración de formularios personalizados adjuntos a objetos es idéntica para todos los objetos, excepto para los proyectos.
>
>Para obtener información sobre cómo añadir formularios personalizados a proyectos de forma masiva, consulte el artículo [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).

Cuando edita por lotes objetos que tienen aplicados varios formularios personalizados, puede editar la forma en que estos se muestran en ellos, así como editar campos comunes entre los formularios personalizados.

Solo los formularios personalizados adjuntos a todos los objetos seleccionados se pueden editar de manera masiva.

Para editar varios formularios personalizados al editar objetos por lotes, haga lo siguiente:

1. En una lista de objetos, seleccione los objetos donde están adjuntos los formularios personalizados y, a continuación, haga clic en el icono **Editar** ![](assets/edit-icon.png).
1. Haga clic en **Formularios personalizados**.

   Solo se pueden editar los formularios personalizados adjuntos a todos los objetos seleccionados.

   Los formularios personalizados adjuntos solo a algunos objetos no se muestran.

1. Comience a editar los campos en los formularios personalizados.

   Cuando se editan los campos, aparece un indicador visual en el campo que señala que se ha editado.

   Si un campo se incluye en más de un formulario personalizado, todos los valores de esos campos se actualizan en cada formulario al hacerlo en uno.

1. Haga clic en el menú desplegable **Seleccionar** y elija los formularios adicionales que desee añadir a todos los objetos escogidos.

   Tenga en cuenta lo siguiente al aplicar formularios adicionales:

   * Los objetos pueden tener hasta 10 formularios personalizados.
   * Los formularios solo se pueden aplicar cuando no se hayan aplicado ya a ninguno de los objetos que edita. Un formulario que ya está adjunto a uno de los objetos no aparece en el menú desplegable.
   * Después de aplicar un formulario adicional, los campos que el formulario tenga en común con otros formularios se mostrarán en la sección **Campos comunes** y se podrán editar.

1. (Opcional) Si ha añadido formularios personalizados a todos los objetos, pero aún no los ha guardado, puede cambiar el orden en que aparecen en ellos.

   Para obtener más información sobre cómo cambiar el orden de los formularios, vea [Reordenación de varios formularios personalizados adjuntos a un objeto](#reorder-multiple-custom-forms-attached-to-an-object) en este artículo.

1. Haga clic en **Quitar formulario** para quitar un formulario personalizado de los objetos.

   Para obtener más información sobre cómo quitar formularios personalizados de los objetos, vea [Eliminación de un formulario personalizado de un objeto](#remove-a-custom-form-from-an-object).

   Tenga en cuenta lo siguiente al eliminar formularios por lotes de varios objetos:

   * Si ha hecho cambios en el formulario, eliminarlo provoca que se pierdan y no se puedan recuperar.
   * Después de quitar un formulario, todos los campos que estuvieran en la sección **Campos comunes** se quitarán de esta sección y ya no se podrán editar aquí.

1. Haga clic en **Restaurar formulario** para restaurar el formulario al estado en el que se encontraba antes de editar los objetos.
1. (Opcional) Haga clic en la flecha de contraer situada junto al nombre de un formulario para contraerlos de uno en uno.

   O

   Haga clic en **Contraer formularios** para contraer todos los formularios al mismo tiempo.

1. (Opcional) Haga clic en la flecha de expansión situada junto al nombre de un formulario para expandirlos de uno en uno.

   O

   Haga clic en **Expandir formularios** para expandir todos los formularios al mismo tiempo. 

1. Haga clic en **Guardar cambios**.
