---
product-area: templates
navigation-topic: templates-navigation-topic
title: Adjuntar una plantilla a un proyecto
description: Puede adjuntar una plantilla a un proyecto durante la fase de creación inicial del proyecto o después de haberla creado.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 0%

---

# Adjuntar una plantilla a un proyecto

Puede adjuntar una plantilla a un proyecto durante la fase de creación inicial del proyecto o después de haberla creado.

Para obtener más información sobre la creación de un proyecto mediante una plantilla, consulte [Creación de un proyecto mediante una plantilla](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos descritos en este artículo:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos </p> <p>Para obtener información sobre el acceso al proyecto, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Concesión de acceso a proyectos</a>.</p> <p>Ver acceso a Plantillas</p> <p>Para obtener información sobre los permisos de plantilla, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Compartir una plantilla</a>. </p> <p>Para obtener información sobre el acceso a plantillas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Concesión de acceso a plantillas</a>.</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el proyecto</p> <p>Para obtener información sobre los permisos del proyecto, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Uso compartido de un proyecto en Adobe Workfront</a>. </p> <p>Ver permisos o superiores a la plantilla</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
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

Puede adjuntar una plantilla a un proyecto en Workfront desde la página del proyecto o desde una lista o informe de proyecto.

1. Vaya al proyecto al que desea adjuntar una plantilla y haga clic en el botón **Más** icono ![](assets/qs-more-icon-on-an-object.png) a la derecha del nombre del proyecto

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   O

   Vaya a una lista de proyectos o a un informe y seleccione un proyecto. A continuación, haga clic en el **Más** icono ![](assets/qs-more-icon-on-an-object.png) en la parte superior de la lista.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)


1. Haga clic en **Adjuntar plantilla**.

   Aparece el cuadro Adjuntar plantilla .

1. Empiece a escribir el nombre de la plantilla que desea adjuntar en la **Buscar plantillas** y haga clic en él cuando aparezca.en la lista

   O

   Haga clic en el nombre de una plantilla en la **Otras plantillas** .

   Se muestra una vista previa de la plantilla a la derecha que contiene la siguiente información sobre la plantilla:

   * Duración
   * Propietario
   * El número de tareas de nivel superior (incluye una lista de las tres primeras tareas de nivel superior)
   * Número total de tareas
   * Nombres de los formularios personalizados adjuntos

   ![](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (Opcional) Haga clic en el **Favoritos** icono ![](assets/favorites-icon-small.png) a la izquierda del nombre de la plantilla para marcarla como favorita. Esto mueve la plantilla a la lista Favoritos.

   ![](assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png)

1. (Opcional) Haga clic en el **Favoritos** icono ![](assets/favorites-icon-selected.png) para quitarlo de la lista Favoritos.
1. Haga clic en **Personalizar y adjuntar**.

   ![](assets/attach-template-large-box-nwe-350x262.png)

1. Actualice la información en las secciones siguientes antes de adjuntar la plantilla (o haga clic en **Adjuntar plantilla** en cualquier momento):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Sección Tareas</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Las tareas de plantilla seleccionadas a continuación se importan al proyecto. Anule la selección de los que desea excluir. </td> 
      <td>Anule la selección de las tareas que desee excluir de la plantilla antes de adjuntarlas al proyecto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seleccione la tarea de proyecto que desee como predecesora para las tareas de esta plantilla.</td> 
      <td> <p>Haga clic en el campo para mostrar una lista de tareas de proyecto. Seleccione qué tarea de proyecto desea finalizar antes de que puedan iniciarse las tareas de plantilla. Como alternativa, puede omitir este paso y configurar relaciones dentro del proyecto después de adjuntar la plantilla. </p> <p> Seleccione el <strong>Tipo de dependencia</strong>, <strong>Lag</strong> información y si desea que el predecesor sea <strong>Enforzado</strong> o no. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seleccione la tarea de proyecto que desea como principal de las tareas de esta plantilla.</td> 
      <td> Seleccione qué tarea de proyecto desea designar como tarea principal para todas las tareas de plantilla. Si no realiza una selección, todas las tareas de plantilla aparecen al final de las tareas de proyecto actuales. Puede omitir este paso y mover tareas en el proyecto después de adjuntar la plantilla.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Sección Opciones</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Los elementos seleccionados a continuación se transfieren al proyecto. Anule la selección de los que desea excluir.</td> 
      <td> <p>Anule la selección de las casillas de verificación situadas junto a la información que desee borrar de la plantilla antes de adjuntarla al proyecto. Esta información no se transfiere de la plantilla al proyecto. Para obtener más información sobre cada campo, consulte <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Descripción general de cómo adjuntar una plantilla a un proyecto</a>. </p> <p>Importante: Si marca la <strong>Configuración de problemas y propiedades de cola</strong> , los Detalles de cola de la plantilla sobrescriben los del proyecto. En este caso, las reglas de enrutamiento, los temas de cola y los grupos de temas de la plantilla se añaden a los del proyecto. <br>Si el proyecto está configurado como cola de solicitudes y la plantilla adjunta al proyecto no está configurada como cola de solicitudes, la información de la cola del proyecto se elimina si deja el <strong>Configuración de problemas y propiedades de cola</strong> casilla marcada. <br>Si anula la selección de <strong>Propiedades de cola y configuración de problemas</strong> , se conservan todas las opciones de configuración de cola del proyecto y no se adjunta ninguna configuración de configuración de cola de la plantilla. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Sección Forms personalizada</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Forms personalizado</td> 
      <td> <p>Cuando los formularios personalizados se adjuntan a la plantilla, sus nombres se muestran en el panel izquierdo. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Actualice la información en los formularios personalizados. Esta información se transfiere al proyecto.

   >[!TIP]
   >
   >* Este paso es obligatorio cuando los formularios personalizados de la plantilla contienen campos obligatorios que están vacíos.
   >* Si los campos de la plantilla los formularios personalizados ya existen en el proyecto y contienen información, conservan la información que ya está en el proyecto. No se pueden editar durante la adición de la plantilla.


1. Haga clic en **Adjuntar plantilla.**
1. Haga clic en **Cancelar datos adjuntos** para dejar de adjuntar la plantilla.

   O

   Permita que el archivo adjunto termine de añadir la plantilla al proyecto.

   Después de adjuntar la plantilla, puede editar el proyecto y ajustar cualquier tarea, información o configuración según sea necesario.

1. (Opcional) Haga clic en **Detalles del proyecto**, luego **Información general** para ver el nombre de la plantilla adjunta en la **Relaciones de proyecto** .

   >[!TIP]
   >
   >Si se adjunta más de una plantilla al proyecto, solo la plantilla que se adjuntó primero se muestra en este campo. Para obtener más información, consulte la [Adjuntar varias plantillas a un proyecto existente y ver la información de la plantilla](#attach-multiple-templates-to-an-existing-project-and-view-template-information) en este artículo.

1. (Opcional) Elimine la información de la plantilla del proyecto en el que la adjuntó. Para obtener más información, consulte [Eliminar información de plantilla de un proyecto](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md).

## Adjuntar varias plantillas a un proyecto existente y ver la información de la plantilla {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

Puede adjuntar varias plantillas (de una en una) al mismo proyecto, siguiendo los pasos descritos en la sección [Adjuntar una plantilla a un proyecto existente](#attach-a-template-to-an-existing-project) en este artículo. Esto agrega las tareas y otra información de cada plantilla al proyecto.

>[!TIP]
>
>Cuando se adjuntan varias plantillas a un proyecto, solo el que se adjuntó primero se muestra en el área Detalles del proyecto .

Para comprender qué plantilla se aplica a un proyecto:

1. Vaya a un proyecto que tenga una plantilla adjunta.
1. Haga clic en **Detalles del proyecto** en el panel izquierdo.
1. Busque el nombre de la plantilla adjunta al proyecto en la **Plantilla** en la parte inferior del **Información general** sección bajo **Relaciones de proyecto** .

   ![](assets/nwe-template-info-on-project-350x356.png)

 

 
