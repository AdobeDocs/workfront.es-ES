---
product-area: templates
navigation-topic: templates-navigation-topic
title: Adjuntar una plantilla a un proyecto
description: Puede adjuntar una plantilla a un proyecto ya sea durante la fase de creación inicial del proyecto o después de haberlo creado.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 91%

---

# Adjuntar una plantilla a un proyecto

Puede adjuntar una plantilla a un proyecto ya sea durante la fase de creación inicial del proyecto o después de haberlo creado.

Para obtener más información sobre cómo crear un proyecto con una plantilla, consulte [Crear un proyecto mediante una plantilla](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos que se describen en este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a proyectos </p> <p>Para obtener información acerca del acceso al proyecto, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Conceder acceso a proyectos</a>.</p> <p>Acceso de visualización a las plantillas</p> <p>Para obtener información acerca de los permisos de las plantillas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Compartir una plantilla</a>. </p> <p>Para obtener información sobre el acceso a las plantillas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Conceder acceso a las plantillas</a>.</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos del proyecto</p> <p>Para obtener información acerca de los permisos del proyecto, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Compartir un proyecto en Adobe Workfront</a>. </p> <p>Permisos de visualización o superiores de la plantilla</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations when adding templates to projects</h2>
<p>(NOTE: moved this to an Overview article of its own) </p>
<p>Consider the following when adding templates to projects:</p>
<ul>
<li> <p>You can attach only active templates to projects. </p> </li>
<li> <p>You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator <span>or a group administrator</span> has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> </li>
<li> <p>Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. </p> </li>
<li> <p>Most template settings are added to the project. </p> </li>
<li> <p>Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<span class="autonumber"><span><b>Example: </b></span></span>
<p>For example, these settings are added to the project:</p>
<ul>
<li>Start&nbsp;From field</li>
<li>Custom forms and the information on them</li>
<li>Queue Details </li>
<li>Financial settings </li>
</ul>
</div> </li>
</ul>
</div>
-->

## Adjuntar una plantilla a un proyecto existente {#attach-a-template-to-an-existing-project}

Puede adjuntar una plantilla a un proyecto en Workfront desde la página del proyecto o desde una lista de proyectos o un informe.

1. Vaya al proyecto al que desee adjuntar una plantilla y haga clic en el icono **Más** ![Más icono](assets/qs-more-icon-on-an-object.png) a la derecha del nombre del proyecto

   ![Más lista desplegable](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   O

   Vaya a una lista de proyectos o a un informe, seleccione un proyecto y haga clic en el icono **Más** ![Icono de más](assets/qs-more-icon-on-an-object.png) que se encuentra en la parte superior de la lista.

   ![Menú más expandido](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)


1. Haga clic en **Adjuntar plantilla**.

   Aparece el cuadro Adjuntar plantilla.

1. Empiece a escribir el nombre de la plantilla que desea adjuntar en el campo **Buscar plantillas** y, a continuación, haga clic en ella cuando se muestre en la lista

   O

   Haga clic en el nombre de una plantilla en el área **Otras plantillas**.

   A la derecha se muestra una vista previa de la plantilla, que contiene la siguiente información sobre la plantilla:

   * Duración
   * Propietario
   * El número de tareas de nivel superior (incluye una lista de las tres primeras tareas de nivel superior)
   * Número total de tareas
   * Nombres de los formularios personalizados adjuntos

   ![Adjuntar cuadro de plantilla](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (Opcional) Haga clic en el icono **Favoritos** ![Icono de favoritos](assets/favorites-icon-small.png) que se encuentra a la izquierda del nombre de la plantilla para marcarla como favorita. Esto mueve la plantilla a la lista Favoritos.

   ![Icono de favoritos en la lista de plantillas](assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png)

1. (Opcional) Vuelva a hacer clic en el icono **Favoritos** ![Icono de favoritos](assets/favorites-icon-selected.png) para quitarlo de la lista Favoritos.
1. Haga clic en **Personalizar y adjuntar**.

   ![Adjuntar plantilla](assets/attach-template-large-box-nwe-350x262.png)

1. Actualice la información de las secciones siguientes antes de adjuntar la plantilla (o bien, haga clic en **Adjuntar plantilla** en cualquier momento):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Sección Tareas</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Las siguientes tareas de plantilla seleccionadas se importan al proyecto. Anule la selección de aquellas que quiera excluir. </td> 
      <td>Anule la selección de cualquier tarea que desee excluir de la plantilla antes de adjuntarla al proyecto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seleccione la tarea del proyecto que desee como predecesora para las tareas de esta plantilla.</td> 
      <td> <p>Haga clic en el campo para mostrar una lista de las tareas del proyecto. Seleccione qué tarea del proyecto desea finalizar antes de que se inicien las tareas de la plantilla. De forma alternativa, puede omitir este paso y configurar relaciones dentro del proyecto después de adjuntar la plantilla. </p> <p> Seleccione la información de <strong>Tipo de dependencia</strong>, <strong>Retardo</strong> y si desea que la predecesora sea <strong>Forzada</strong> o no. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seleccione la tarea del proyecto que desee como principal de las tareas de esta plantilla.</td> 
      <td> Seleccione qué tarea del proyecto desea designar como tarea principal para todas las tareas de la plantilla. Si no selecciona ninguna, todas las tareas de la plantilla aparecerán al final de las tareas del proyecto actual. Puede omitir este paso y mover las tareas en el proyecto después de adjuntar la plantilla.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Sección Opciones</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Los siguientes elementos seleccionados se transfieren al proyecto. Anule la selección de aquellos que quiera excluir.</td> 
      <td> <p>Anule la selección de las casillas de verificación situadas junto a la información que desee borrar de la plantilla antes de adjuntarla al proyecto. Esta información no se transfiere de la plantilla al proyecto. Para obtener más información sobre cada campo, consulte <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Información general sobre cómo adjuntar una plantilla a un proyecto</a>. </p> <p>Importante: Si marca la casilla <strong>Propiedades de cola y configuración de problema</strong>, los detalles de cola de la plantilla sobrescribirán los del proyecto. En este caso, las reglas de enrutamiento, los temas de cola y los grupos de temas de la plantilla se añaden a los del proyecto. <br>Si el proyecto está configurado como cola de solicitudes y la plantilla que adjunta al proyecto no está configurada como cola de solicitudes, la información de cola del proyecto se quitará si deja seleccionada la casilla <strong>Propiedades de cola y configuración de problema</strong>. <br>Si anula la selección de la casilla <strong>Propiedades de cola y configuración de problema</strong>, se conservarán todos los ajustes de la configuración de cola del proyecto y no se adjuntará ningún ajuste de configuración de cola de la plantilla. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Información general sobre formularios personalizados</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td> <p>Cuando se adjuntan formularios personalizados a la plantilla, sus nombres se muestran en el panel izquierdo. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Actualice la información de los formularios personalizados. Esta información se transfiere al proyecto.

   >[!TIP]
   >
   >* Este paso es obligatorio cuando los formularios personalizados de la plantilla contienen campos obligatorios que están vacíos.
   >* Si los campos de los formularios personalizados de la plantilla ya existen en el proyecto y contienen información, conservan la información que ya existe en el proyecto. No puede editarlos al adjuntar la plantilla.

1. Haga clic en **Adjuntar plantilla.**
1. Haga clic en **Cancelar archivo adjunto** para dejar de adjuntar la plantilla.

   O

   Permita que el archivo adjunto termine de añadir la plantilla al proyecto.

   Después de adjuntar la plantilla, puede editar el proyecto y ajustar cualquier tarea, información o configuración según sea necesario.

1. (Opcional) Haga clic en **Detalles del proyecto** y, a continuación, en **Información general** para ver el nombre de la plantilla que adjuntó en el área **Relaciones del proyecto**.

   >[!TIP]
   >
   >Si adjunta más de una plantilla al proyecto, solo se mostrará en este campo la plantilla que adjuntó primero. Para obtener más información, consulte la sección [Adjuntar varias plantillas a un proyecto existente y ver la información de las plantillas](#attach-multiple-templates-to-an-existing-project-and-view-template-information) en este artículo.

1. (Opcional) Quite la información de la plantilla del proyecto donde la adjuntó. Para obtener más información, consulte [Quitar la información de plantilla de un proyecto](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md).

## Adjuntar varias plantillas a un proyecto existente y ver la información de las plantillas {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

Puede adjuntar varias plantillas (de una en una) al mismo proyecto, siguiendo los pasos descritos en la sección [Adjuntar una plantilla a un proyecto existente](#attach-a-template-to-an-existing-project) en este artículo. Esto añade al proyecto las tareas y otra información de cada plantilla.

>[!TIP]
>
>Cuando se adjuntan varias plantillas a un proyecto, en el área Detalles del proyecto solo aparece la que se adjuntó en primer lugar.

Para comprender qué plantilla se aplica a un proyecto:

1. Vaya a un proyecto que tenga una plantilla adjunta.
1. Haga clic en **Detalles del proyecto** en el panel izquierdo.
1. Busque el nombre de la plantilla adjunta al proyecto en el campo **Plantilla** en la parte inferior de la sección **Información general** en **Relaciones del proyecto** .

   ![Información de plantilla en el proyecto](assets/nwe-template-info-on-project-350x356.png)


