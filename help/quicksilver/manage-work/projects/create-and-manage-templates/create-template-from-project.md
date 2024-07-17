---
product-area: templates
navigation-topic: templates-navigation-topic
title: Crear plantilla a partir de proyecto
description: Puede crear plantillas al guardar un proyecto existente como plantilla.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 1%

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
>Una plantilla y sus tareas no tienen fechas reales, sino una indicación de qué día (a partir de cuándo podría comenzar el proyecto futuro) podría comenzar una tarea y en qué día debería completarse la tarea. Al utilizar plantillas para crear proyectos futuros, los proyectos recibirán fechas reales. Para obtener más información, consulte [Crear un proyecto](../create-projects/create-project.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a plantillas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos superiores a un proyecto </p> <p>Los permisos de administración se obtienen en la plantilla después de crearla</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear plantilla a partir de proyecto

1. Vaya al proyecto que desea guardar como plantilla.
1. Haga clic en el menú **Más** ![](assets/qs-more-icon-on-an-object.png) y luego en **Guardar como plantilla**.
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
        <li><strong>No</strong>: otros usuarios no pueden encontrar la plantilla y no pueden adjuntarla a proyectos.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td>Utilice la lista desplegable para seleccionar cualquier formulario personalizado para adjuntarlo a la plantilla. Si ya se han asociado formularios personalizados al proyecto, se muestran todos los campos de datos de esos formularios personalizados.<br>Puede incluir hasta 10 formularios personalizados en una sola plantilla.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Administrar Forms** para quitar o reordenar los formularios. Para obtener información sobre cómo quitar y reordenar formularios personalizados en la plantilla, consulte [Formularios personalizados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. Haga clic en **Siguiente paso.**
1. En la sección **Opciones**, active la casilla de verificación situada junto a la información que desee borrar de la plantilla.

   ![](assets/save-as-template-options-step-350x109.png)

1. Haga clic en **Siguiente paso.**
1. En la sección **Excluir**, seleccione las tareas que desee excluir del proyecto.

   ![](assets/save-as-template-exclude-350x205.png)

1. Haga clic en **Finalizar y guardar plantilla.**

   La plantilla ahora aparece en la lista de plantillas disponibles y se puede adjuntar a un proyecto existente o utilizar para crear uno nuevo.

 
