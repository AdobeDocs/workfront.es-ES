---
product-area: projects;templates
navigation-topic: manage-projects
title: Guardar un proyecto como plantilla
description: Guardar un proyecto como plantilla “Guardar como plantilla” en el nivel de proyecto, para que los usuarios lo vean en la interfaz de usuario; este artículo está vinculado con otro artículo que trata esto en más profundidad (paso a paso). Esta funcionalidad debe permanecer en las áreas de proyectos Y plantillas.
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '787'
ht-degree: 64%

---

# Guardar un proyecto como plantilla

<!--Audited: 6/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

<div class="preview">

La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Las mismas funciones también estarán disponibles en el entorno de producción para todos los clientes una semana después de la versión de vista previa.

Para obtener más información, vea [Modernización de la interfaz](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Si decide que un proyecto se va a repetir en algún momento futuro, puede crear una plantilla a partir de ese proyecto existente. En adelante, puede volver a utilizar la plantilla para crear proyectos futuros que puedan contener información similar o que puedan compartir la misma cronología o asignaciones con el proyecto existente.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar </p>
   O 
   <p>Actual: plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a las plantillas</p> /td&gt; 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos Ver o superiores para un proyecto </p> <p>Los permisos de administración se obtienen en la plantilla después de guardar el proyecto como plantilla</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Guardar un proyecto como plantilla

Guardar un proyecto como plantilla difiere en los entornos de producción y vista previa.

### Guardar un proyecto como plantilla en el entorno de producción

1. Vaya al proyecto que desee guardar como plantilla.
1. Haga clic en el menú **Más** ![Icono de más](assets/qs-more-icon-on-an-object.png) y luego en **Guardar como plantilla**.
1. Especifique la siguiente información para la plantilla:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td>Especifique un nombre para la plantilla.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Proporcione una descripción para la plantilla.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activo</td> 
      <td> <p>Seleccione entre las siguientes opciones:</p> 
       <ul> 
        <li> <p><strong>Sí</strong>: otros usuarios pueden encontrar la plantilla y adjuntarla a proyectos.</p> </li> 
        <li><strong>No</strong>: otros usuarios no pueden encontrar la plantilla ni adjuntarla a proyectos.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td>Utilice la lista desplegable para seleccionar cualquier formulario personalizado que desee adjuntar a la plantilla. Si ya se han asociado formularios personalizados al proyecto, se muestran todos los campos de datos de esos formularios personalizados.<br>Puede incluir hasta 10 formularios personalizados en una misma plantilla.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Administrar formularios** para quitar o reordenar los formularios. Para obtener información sobre cómo quitar y reordenar formularios personalizados en la plantilla, consulte [Formularios personalizados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. Haga clic en **Siguiente paso**.
1. En la sección **Opciones**, active la casilla de verificación situada junto a la información que desee borrar de la plantilla.

   ![](assets/save-as-template-options-step-350x109.png)

1. Haga clic en **Siguiente paso**.
1. En la sección **Excluir**, seleccione las tareas que desee excluir del proyecto.

   ![](assets/save-as-template-exclude-350x205.png)

1. Haga clic en **Finalizar y guardar plantilla**.

   La plantilla ahora aparece en la lista de plantillas disponibles y se puede adjuntar a un proyecto existente o utilizarse para crear uno nuevo.


<div class="preview">

### Guardar un proyecto como plantilla en el entorno de vista previa

1. Vaya al proyecto que desee guardar como plantilla.
1. Haga clic en el menú **Más** ![Icono de más](assets/qs-more-icon-on-an-object.png) y luego en **Guardar como plantilla**.
1. En la sección **Guardar como plantilla**, especifique la siguiente información para la plantilla:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de plantilla</td> 
      <td>Especifique un nombre para la plantilla.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Proporcione una descripción para la plantilla.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activo</td> 
      <td> <p>Seleccione entre las siguientes opciones:</p> 
       <ul> 
        <li> <p><strong>Sí</strong>: otros usuarios pueden encontrar la plantilla y adjuntarla a proyectos.</p> </li> 
        <li><strong>No</strong>: otros usuarios no pueden encontrar la plantilla ni adjuntarla a proyectos.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td>Utilice la lista desplegable para seleccionar cualquier formulario personalizado que desee adjuntar a la plantilla. Si ya se han asociado formularios personalizados al proyecto, se muestran todos los campos de datos de esos formularios personalizados.<br>Puede incluir hasta 10 formularios personalizados en una misma plantilla.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Forms personalizado** en el panel izquierdo para quitar o reordenar los formularios.

   Para reordenar los formularios, arrástrelos y suéltelos en el orden correcto.
Para quitar un formulario, selecciónelo y haga clic en **Quitar**. Haga clic en **Cancelar** para quitar los formularios seleccionados.

   ![Área de formularios personalizados en el cuadro Guardar como plantilla](assets/custom-forms-ara-in-save-as-template-box.png)

1. Actualice la información en los formularios personalizados adjuntos si es necesario. La información se transferirá a la plantilla.

1. Haga clic en **Opciones** en la sección del panel izquierdo y, a continuación, active la casilla de verificación situada junto a la información que desee transferir a la plantilla. Los elementos no seleccionados no se transfieren a la plantilla. De forma predeterminada, todas las opciones no están seleccionadas.

   ![Área de opciones en el cuadro Guardar como plantilla](assets/options-area-in-save-as-template-box.png)

1. Haga clic en **Excluir** en el panel izquierdo y, a continuación, seleccione las tareas que desee excluir del proyecto. De forma predeterminada, todas las tareas no están seleccionadas.

   ![Excluir área en el cuadro Guardar como plantilla](assets/exclude-area-save-as-template-box.png)

1. Haga clic en **Finalizar y guardar plantilla**.

   La plantilla ahora aparece en la lista de plantillas disponibles y se puede adjuntar a un proyecto existente o utilizarse para crear uno nuevo.

</span>