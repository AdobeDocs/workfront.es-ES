---
product-area: projects;user-management
keywords: editar,formularios,enriquecido,texto,especial,formato,campos,personalizado,información,personalizar,objetos
navigation-topic: work-with-custom-forms
title: Editar información en campos de formulario personalizados
description: Puede editar la información de un formulario personalizado después de adjuntar el formulario a un objeto. Para obtener información sobre cómo agregar formularios personalizados a objetos, consulte Agregar un formulario personalizado a un objeto.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 0%

---

# Editar información en campos de formulario personalizados

Puede editar la información de un formulario personalizado después de adjuntar el formulario a un objeto. Para obtener información acerca de cómo agregar formularios personalizados a objetos, vea [Agregar un formulario personalizado a un objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>plan Adobe Workfront*</p> </td> 
   <td>Equipo o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licencias de Adobe Workfront*</p> </td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Editar el acceso al objeto para el que desea editar el formulario personalizado</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Permisos de objeto</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribute o permisos superiores en el objeto para el que desea editar el formulario personalizado</p> </li> 
     <li>Vea los permisos de los campos que desea editar. Para obtener información acerca de los permisos de uso compartido para campos personalizados, vea <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md" class="MCXref xref">Configurar el uso compartido para campos y widgets personalizados</a>.</li> 
     <li> <p>Editar permisos para las secciones del formulario en las que se encuentran los campos que desea editar</p> </li> 
    </ul> <p>Para obtener información sobre cómo solicitar acceso adicional para objetos, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

* El administrador de Workfront o un usuario de Plan con acceso administrativo a los formularios personalizados deben crear formularios personalizados en su entorno. Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Debe tener formularios personalizados adjuntos a un objeto.

  Para obtener información acerca de cómo aplicar formularios personalizados a un objeto, vea [Agregar un formulario personalizado a un objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Edición de información en un formulario personalizado

La edición de información en un formulario personalizado adjunto a un objeto es idéntica para todos los objetos. Para obtener información sobre qué objetos pueden tener un formulario personalizado, vea [Información general sobre formularios personalizados](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. Vaya a un objeto cuya información desee editar en el formulario personalizado.
1. Haga clic en **`<Object type>`detalles** en el panel izquierdo.

   Por ejemplo, cuando edite información en un formulario personalizado de proyecto, haga clic en **Detalles del proyecto**.

1. Desplácese hasta el formulario personalizado. Cuando hay un formulario personalizado adjunto al objeto, el nombre del formulario se muestra como un área en la sección Detalles.
1. Si es necesario, haga clic en la flecha ![](assets/expand-arrow-right.png) a la izquierda del nombre del formulario personalizado para expandirlo.
1. Cerca de la esquina superior derecha de la página, haga clic en el icono Editar ![](assets/edit-icon.png).
1. Comience a introducir información en cualquier campo al que tenga acceso.

   ![](assets/click-in-field-to-edit-info-350x132.png)

   O

   Si todavía no se ha especificado información en el formulario, haga clic en **Agregar+** para cualquier campo al que tenga acceso y empiece a escribir información.

   ![](assets/plus-add-to-edit-info-350x180.png)

   Si hay varios formularios personalizados adjuntos al objeto, puede hacerlo para cada formulario.

   Según el tipo de campo en el que trabaje, tenga en cuenta lo siguiente:

   * Solo se puede seleccionar una opción para los campos de botón de opción.
   * Puede seleccionar una o varias opciones en un campo de casilla de verificación, según la configuración que haya realizado el creador del formulario en el campo.
   * Puede seleccionar una o varias opciones en un campo desplegable de selección múltiple, según la configuración del campo que haya realizado el creador del formulario.
   * Solo se puede aplicar formato a los campos de texto (negrita, cursiva o subrayado) si el usuario que ha creado el formulario los ha configurado como campos de texto con formato. No se puede dar formato a los campos de texto de una sola línea y a los campos de texto de párrafo.
   * Solo se puede actualizar la hora del día en un tipo de campo de fecha si el usuario que ha creado el formulario lo ha incluido al crear el campo.

   Para obtener información acerca de todos los tipos de campo, vea [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Haga clic en **Guardar cambios**.

   >[!IMPORTANT]
   >
   >Debe completar todos los campos obligatorios del formulario para poder guardarlo. El nombre de un campo obligatorio va seguido de un asterisco.
   >
   >![](assets/nwe-required-custom-field.png)

   Cuando alguien cambia datos en otro objeto al que se hace referencia mediante campos personalizados calculados en su objeto, los cambios no se reflejan automáticamente en su objeto. Para obtener información acerca de cómo actualizar manualmente todos los campos personalizados calculados en el objeto, vea [Volver a calcular todos los campos personalizados calculados para un objeto](#recalculate-all-calculated-custom-fields-for-an-object) en este artículo.

   Cuando se modifican los campos dependientes de la página, los campos calculados del formulario personalizado se vuelven a calcular dinámicamente en tiempo real. Puede ver el nuevo valor de campo calculado sin guardar el formulario, pero en realidad no se aplica al formulario y al objeto hasta que no guarda los cambios. Esto se aplica a los campos calculados en los formularios predeterminados y a los formularios personalizados.

   También puede actualizar manualmente todos los campos personalizados calculados para un objeto al editar el objeto de forma masiva junto con otros objetos de una lista. Para obtener instrucciones, vea [Volver a calcular todos los campos personalizados calculados para varios objetos de una lista al editar los objetos](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) en este artículo.

## Volver a calcular todos los campos personalizados calculados para un objeto  {#recalculate-all-calculated-custom-fields-for-an-object}

1. Vaya a la página principal del objeto cuyos campos personalizados desea volver a calcular.
1. Haga clic en el menú **Más** ![](assets/more-icon.png) que se encuentra a la derecha del nombre del objeto y, a continuación, haga clic en **Volver a calcular expresiones**.

   Esto vuelve a calcular todos los campos personalizados del formulario del objeto.

## Volver a calcular todos los campos personalizados calculados para varios objetos de una lista al editar los objetos {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

Puede recalcular manualmente los campos personalizados de varios objetos editándolos por lotes desde una lista o informe.

1. Vaya a una lista de objetos que contienen formularios personalizados con campos calculados.
1. Seleccione los objetos cuyos campos personalizados calculados desee actualizar.
1. Haga clic en el **icono Editar**.
1. Haga clic en **Forms personalizado** en el menú de la izquierda y, a continuación, seleccione **Volver a calcular expresiones personalizadas**.
1. Haga clic en **Guardar** **Cambios**.

   Workfront calcula todos los campos personalizados de todos los objetos seleccionados.

>[!TIP]
>
>Según la complejidad de los proyectos, se recomienda no seleccionar un gran número de proyectos al volver a calcular los campos personalizados calculados de forma masiva para garantizar un rendimiento óptimo. Algunas cosas que podrían hacer que un proyecto sea demasiado complejo podrían ser varias dependencias o asignaciones o un gran número de campos personalizados.
>
>Para volver a calcular las expresiones personalizadas de forma masiva desde una lista de proyectos:
>
>1. Vaya a un informe o lista de proyectos y seleccione uno o varios proyectos.
>1. Haga clic en el menú **Más** ![](assets/more-icon.png) y, a continuación, haga clic en **Volver a calcular expresiones personalizadas**.
>
>![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
>
>Workfront calcula todos los campos personalizados de todos los proyectos seleccionados.
