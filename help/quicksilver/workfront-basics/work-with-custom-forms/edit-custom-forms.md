---
product-area: projects;user-management
keywords: editar,formularios,enriquecido,texto,especial,formato,campos,personalizado,información,personalizar,objetos
navigation-topic: work-with-custom-forms
title: Editar información en campos de formulario personalizados
description: Puede editar la información de un formulario personalizado después de adjuntar el formulario a un objeto. Para obtener información sobre cómo agregar formularios personalizados a objetos, consulte Agregar un formulario personalizado a un objeto.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 11%

---

# Editar información en campos de formulario personalizados

<!--Audited: 10/2025-->

Puede editar la información de un formulario personalizado después de adjuntar el formulario a un objeto. Para obtener información acerca de cómo agregar formularios personalizados a objetos, vea [Agregar un formulario personalizado a un objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Paquete de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licencia de Adobe Workfront</p> </td> 
   <td> <p>Colaborador o superior</p> 
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso al objeto para el que desea editar el formulario personalizado</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Permisos de objeto</p> </td> 
   <td> 
    <ul> 
     <li> <p>Permisos de contribución o superiores en el objeto para el que desea editar el formulario personalizado</p> </li> 
     <li><p>Vea los permisos de los campos que desea editar.</p></li> 
     <li><p>Editar permisos para las secciones del formulario en las que se encuentran los campos que desea editar</p></li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Team or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront licenses*</p> </td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to the object for which you want to edit the custom form</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribute or higher permissions on the object for which you want to edit the custom form</p> </li> 
     <li>View permissions on the fields you want to edit. For information about sharing permissions for custom fields, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md" class="MCXref xref">Configure sharing for custom fields and widgets</a>.</li> 
     <li> <p>Edit permissions for the sections on the form where the fields you want to edit are located</p> </li> 
    </ul> <p>For information on requesting additional access for objects, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Requisitos previos

* El administrador de Workfront o un usuario de Plan con acceso administrativo a los formularios personalizados deben crear formularios personalizados en su entorno. Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Debe tener formularios personalizados adjuntos a un objeto.

  Para obtener información sobre cómo aplicar formularios personalizados a un objeto, consulte [Añadir un formulario personalizado a un objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Edición de información en un formulario personalizado

La edición de información en un formulario personalizado adjunto a un objeto es similar para la mayoría de los objetos.

Para obtener información sobre qué objetos pueden tener un formulario personalizado, vea [Información general sobre formularios personalizados](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. Vaya a cualquier lista de objetos para los que desee editar información en el formulario personalizado, excepto a una lista de iteraciones.
1. Seleccione uno o varios objetos de la lista y, a continuación, haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png) que se encuentra en la parte superior de la lista.
1. Haga clic en **Forms personalizado** en el panel izquierdo, dentro del cuadro **Editar &lt; objeto >**.

   Cuando hay un formulario personalizado adjunto al objeto, el nombre del formulario se muestra como un área en la sección **Forms personalizado**.
1. Comience a introducir información en cualquier campo al que tenga acceso.

   ![Cuadro de edición con formularios personalizados en el registro de facturación](assets/edit-box-with-custom-forms-on-billing-record.png)

   Si hay varios formularios personalizados adjuntos al objeto, hágalo para cada formulario.

   Según el tipo de campo en el que trabaje, tenga en cuenta lo siguiente:

   * Solo se puede seleccionar una opción para los campos de botón de opción.
   * Puede seleccionar una o varias opciones en un campo de casilla de verificación, según la configuración que haya realizado el creador del formulario en el campo.
   * Puede seleccionar una o varias opciones en un campo desplegable de selección múltiple, según la configuración del campo que haya realizado el creador del formulario.
   * Solo se puede aplicar formato a los campos de texto (negrita, cursiva o subrayado) si el usuario que ha creado el formulario los ha configurado como campos de texto con formato. No se puede dar formato a los campos de texto de una sola línea y a los campos de texto de párrafo.
   * Solo se puede actualizar la hora del día en un tipo de campo de fecha si el usuario que ha creado el formulario lo ha incluido al crear el campo.

   >[!NOTE]
   >
   >Los campos que permiten selecciones múltiples pueden limitar la cantidad de opciones que se pueden elegir. Las casillas de verificación y los desplegables de selección múltiple están limitados a 5000 selecciones.

   Para obtener información acerca de todos los tipos de campo, vea [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Haga clic en **Guardar**.

   >[!IMPORTANT]
   >
   >Debe completar todos los campos obligatorios del formulario para poder guardarlo. El nombre de un campo obligatorio va seguido de un asterisco.
   >
   >![Campo personalizado requerido](assets/nwe-required-custom-field.png)

   Cuando alguien cambia datos en otro objeto al que se hace referencia mediante campos personalizados calculados en su objeto, los cambios no se reflejan automáticamente en su objeto. Para obtener información acerca de cómo actualizar manualmente todos los campos personalizados calculados en el objeto, vea [Volver a calcular todos los campos personalizados calculados para un objeto](#recalculate-all-calculated-custom-fields-for-an-object) en este artículo.

   Cuando se modifican los campos dependientes de la página, los campos calculados del formulario personalizado se vuelven a calcular dinámicamente en tiempo real. Puede ver el nuevo valor de campo calculado sin guardar el formulario, pero en realidad no se aplica al formulario y al objeto hasta que no guarda los cambios. Esto se aplica a los campos calculados en los formularios predeterminados y a los formularios personalizados.

   También puede actualizar manualmente todos los campos personalizados calculados para un objeto al editar el objeto de forma masiva junto con otros objetos de una lista. Para obtener instrucciones, vea [Volver a calcular todos los campos personalizados calculados para varios objetos de una lista al editar los objetos](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) en este artículo.

1. (Condicional) Para actualizar los campos personalizados de un formulario personalizado de iteración, siga estos pasos:

   1. Vaya a una iteración.
   1. Haga clic en **Formularios personalizados** en el panel izquierdo. 
   1. Para agregar formularios personalizados, empiece a escribir el nombre de un formulario en el campo **Agregar formulario personalizado** en la esquina superior derecha de la página

      O

      Haga clic en el icono **Editar** en la misma área para comenzar a editar los campos de los formularios adjuntos.

      ![Editar formulario personalizado de iteración](assets/edit-iteration-custom-form.png)

   1. Haga clic en **Guardar cambios**.

## Volver a calcular campos personalizados para objetos

Periódicamente, según los cambios que se puedan producir en los formularios personalizados o en los campos a los que se haga referencia en los campos personalizados, los valores de los campos personalizados calculados pueden quedar obsoletos. En este caso, es posible que tenga que volver a calcular los campos personalizados o las expresiones personalizadas de los objetos.

Las secciones siguientes describen cómo se pueden recalcular las expresiones personalizadas para objetos con formularios personalizados.

>[!NOTE]
>
>No se pueden recalcular las expresiones personalizadas para grupos.

### Volver a calcular todos los campos personalizados calculados desde la página de un objeto

>[!IMPORTANT]
>
>Debe tener un formulario personalizado con campos calculados adjuntos al objeto antes de poder seguir los pasos de esta sección.

1. Vaya a la página principal de uno de los siguientes objetos cuyos campos personalizados desee volver a calcular:

   * Proyecto
   * Tarea
   * Problema
   * Portafolio
   * Programa
   * Documento

1. Haga clic en el menú **Más** ![Menú más](assets/more-icon.png) que se encuentra a la derecha del nombre del objeto y, a continuación, haga clic en **Volver a calcular expresiones**.

   Esto vuelve a calcular todos los campos personalizados del formulario del objeto.

### Volver a calcular todos los campos personalizados calculados para varios objetos de una lista al editar los objetos {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

Según los objetos para los que desee volver a calcular las expresiones personalizadas, puede hacerlo en las áreas siguientes:

* En una lista de objetos, en el menú Más situado en la parte superior de la lista.
* En el cuadro Editar, al seleccionar y editar varios objetos de forma masiva.

Para volver a calcular manualmente los campos personalizados de varios objetos editándolos por lotes desde una lista o informe:

1. Vaya a una lista de los siguientes tipos de objetos cuyos objetos contengan formularios personalizados con campos calculados:

   * Usuarios
   * Compañías
   * Registros de facturación

1. Seleccione los objetos cuyos campos personalizados calculados desee actualizar.
1. Haga clic en el **icono Editar**.
1. Haga clic en **Forms personalizado** en el menú de la izquierda y, a continuación, seleccione **Volver a calcular expresiones personalizadas**.
1. Haga clic en **Guardar** o en **Guardar cambios**.

   Workfront calcula todos los campos personalizados de todos los objetos seleccionados.

Para volver a calcular las expresiones personalizadas de una lista de objetos:

1. Vaya a una lista de proyectos o a un informe y seleccione uno o varios de los siguientes tipos de objetos:

   * Proyectos
   * Tareas
   * Problemas
   * Portafolios
   * Programas
   * Gastos
1. Haga clic en el menú **Más** ![Menú más](assets/more-icon.png) y, a continuación, haga clic en **Volver a calcular expresiones personalizadas**.

![Recalcular expresiones del cronograma de finanzas desplegable en listas de proyectos](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

Workfront calcula inmediatamente todos los campos personalizados de todos los proyectos seleccionados.
No todas las listas de todos los objetos tienen esta capacidad.

>[!NOTE]
>
>Al recalcular las expresiones para varios proyectos, según su complejidad, recomendamos no seleccionar un número demasiado grande de proyectos para garantizar un rendimiento óptimo.
>
>Algunas cosas que podrían hacer que un proyecto sea demasiado complejo podrían ser varias dependencias o asignaciones o un gran número de campos personalizados.

