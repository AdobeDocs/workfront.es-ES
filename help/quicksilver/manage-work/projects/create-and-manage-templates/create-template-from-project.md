---
product-area: templates
navigation-topic: templates-navigation-topic
title: Crear plantilla a partir de proyecto
description: Puede crear plantillas al guardar un proyecto existente como plantilla.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 75%

---

# Crear plantilla a partir de proyecto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

Puede crear plantillas al guardar un proyecto existente como plantilla.

Después de guardar un proyecto existente como plantilla, puede utilizar la nueva plantilla para crear nuevos proyectos. Esto simplifica y acelera el proceso de creación de proyectos.

>[!NOTE]
>
>Al guardar un proyecto como plantilla, las fechas reales de las tareas y del proyecto no se guardan para la plantilla.
>
>Una plantilla y sus tareas no tienen fechas reales, sino una indicación de qué día (a partir de cuándo podría comenzar el proyecto futuro) podría comenzar una tarea y en qué día debería haberse completado la tarea. Cuando se utilizan plantillas para crear proyectos futuros, los proyectos recibirán fechas reales. Para obtener más información, consulte [Crear un proyecto](../create-projects/create-project.md).

## Requisitos de acceso

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
   <td> <p>Acceso de edición a las plantillas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos Ver o superiores para un proyecto </p> <p>Los permisos de administración se obtienen en la plantilla después de crearla</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Crear plantilla a partir de proyecto

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

   ![Guardar como plantilla en el primer paso](assets/save-as-template-first-step-350x159.png)

1. Haga clic en **Siguiente paso**.
1. En la sección **Opciones**, seleccione la casilla de verificación situada junto a la información que desee borrar de la plantilla.

   ![Guardar como opciones de plantilla](assets/save-as-template-options-step-350x109.png)

1. Haga clic en **Siguiente paso**.
1. En la sección **Excluir**, seleccione las tareas que desee excluir del proyecto.

   ![Guardar como plantilla excluir](assets/save-as-template-exclude-350x205.png)

1. Haga clic en **Finalizar y guardar plantilla**.

   La plantilla ahora aparece en la lista de plantillas disponibles y se puede adjuntar a un proyecto existente o utilizarse para crear uno nuevo.

 
