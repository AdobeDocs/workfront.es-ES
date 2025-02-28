---
product-area: projects;templates
navigation-topic: manage-projects
title: Guardar un proyecto como plantilla
description: Guardar un proyecto como plantilla “Guardar como plantilla” en el nivel de proyecto, para que los usuarios lo vean en la interfaz de usuario; este artículo está vinculado con otro artículo que trata esto en más profundidad (paso a paso). Esta funcionalidad debe permanecer en las áreas de proyectos Y plantillas.
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 97%

---

# Guardar un proyecto como plantilla

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

Si decide que un proyecto se va a repetir en algún momento futuro, puede crear una plantilla a partir de ese proyecto existente. En adelante, puede volver a utilizar la plantilla para crear proyectos futuros que puedan contener información similar o que puedan compartir la misma cronología o asignaciones con el proyecto existente.

## Requisitos de acceso

<!--drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or 
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you save the project as a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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
   <td> <p>Acceso de edición a las plantillas</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos Ver o superiores para un proyecto </p> <p>Los permisos de administración se obtienen en la plantilla después de guardar el proyecto como plantilla</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Guardar un proyecto como plantilla

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
1. En la sección **Opciones**, seleccione la casilla de verificación situada junto a la información que desee borrar de la plantilla.

   ![](assets/save-as-template-options-step-350x109.png)

1. Haga clic en **Siguiente paso**.
1. En la sección **Excluir**, seleccione las tareas que desee excluir del proyecto.

   ![](assets/save-as-template-exclude-350x205.png)

1. Haga clic en **Finalizar y guardar plantilla**.

   La plantilla ahora aparece en la lista de plantillas disponibles y se puede adjuntar a un proyecto existente o utilizarse para crear uno nuevo.
