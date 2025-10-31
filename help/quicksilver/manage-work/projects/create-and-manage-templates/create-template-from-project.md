---
product-area: templates
navigation-topic: templates-navigation-topic
title: Crear plantilla a partir de proyecto
description: Puede crear plantillas al guardar un proyecto existente como plantilla.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 39%

---

# Crear plantilla a partir de proyecto

<!--Audited: 10/2025-->

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

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a las plantillas</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos Ver o superiores para un proyecto </p> <p>Los permisos de administración se obtienen en la plantilla después de crearla</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you create it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Crear plantilla a partir de proyecto

1. Vaya al proyecto que desee guardar como plantilla.
1. Haga clic en el menú **Más** ![Icono de más](assets/more-icon.png) y luego en **Guardar como plantilla**.
1. Especifique la siguiente información para la plantilla:

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
    </tbody> 
   </table>

1. Haga clic en **Formularios personalizados** en el panel izquierdo. 
1. Haga clic en el campo **Agregar formulario personalizado** y empiece a escribir el nombre de un formulario personalizado de proyecto o seleccione uno de la lista.

   Si algún formulario personalizado ya está asociado al proyecto, en los formularios se muestra toda la información de los campos existentes de esos formularios personalizados.

   Puede incluir hasta 10 formularios personalizados en una sola plantilla.

1. Pase el ratón sobre el nombre de un formulario y, a continuación, haga clic para arrastrarlo y soltarlo en un lugar nuevo.

   ![Guardar proyecto como plantilla de principio del cuadro](assets/save-project-as-template-top-of-the-form.png)

1. Haga clic en **Opciones** en el panel izquierdo y, a continuación, seleccione los campos o elementos que desee transferir a la plantilla.

   Todos los elementos están seleccionados de forma predeterminada. Los elementos no seleccionados no se transfieren a la plantilla.

   ![Guardar como opciones de plantilla](assets/save-project-as-template-options-area.png)

1. Haga clic en **Excluir** en el panel izquierdo y, a continuación, seleccione las tareas que desee excluir del proyecto.

   ![Guardar como plantilla excluir](assets/save-project-as-template-exclude-area.png)

1. Haga clic en **Finalizar y guardar plantilla**.

   La plantilla ahora aparece en la lista de plantillas disponibles. Los usuarios pueden adjuntar la nueva plantilla a un proyecto existente o utilizarla para crear un proyecto.


