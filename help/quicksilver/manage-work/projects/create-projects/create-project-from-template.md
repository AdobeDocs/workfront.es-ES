---
product-area: projects;templates
navigation-topic: create-projects
title: Creación de un proyecto con una plantilla
description: Puede utilizar las plantillas como un marco de trabajo para crear proyectos en Adobe Workfront. Si tiene proyectos que se repiten con frecuencia, el uso de plantillas para la cronología general del nuevo proyecto evita tener que generar los mismos proyectos repetidamente.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: 9447310f0d4cf4504ee6d690116fb62f718fe23d
workflow-type: tm+mt
source-wordcount: '1089'
ht-degree: 0%

---

# Creación de un proyecto con una plantilla

<!-- Audited: 01/2024 -->

Puede utilizar las plantillas como un marco de trabajo para crear proyectos en Adobe Workfront. Si tiene proyectos que se repiten con frecuencia, el uso de plantillas para la cronología general del nuevo proyecto evita tener que generar los mismos proyectos repetidamente.

Las plantillas le proporcionan una forma de capturar procesos, información y configuraciones repetibles asociados a sus proyectos. La información asociada con una plantilla se transfiere al proyecto. Esto incluye tareas, asignaciones, duraciones, documentos, detalles financieros, riesgos y formularios personalizados.

>[!TIP]
>
>Workfront define el grupo y el estado del nuevo proyecto de la siguiente manera:
>
>* El estado predeterminado de un nuevo proyecto creado a partir de una plantilla corresponde al estado definido por el administrador de Workfront en el área principal Preferencias de proyecto, o por un administrador de grupo (o administrador de Workfront) en el área Preferencias de proyecto para un grupo. Para obtener información sobre cómo configurar las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Configurar las preferencias de proyecto de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* El grupo del nuevo proyecto es el grupo de la plantilla. Si la plantilla no está asociada a un grupo, el grupo del proyecto es el grupo de inicio del usuario que crea el proyecto.
>
>* Los estados disponibles para un nuevo proyecto coinciden con los estados del grupo del proyecto, que es el grupo de la plantilla o el grupo de inicio del usuario que crea el proyecto.

Tiene las siguientes opciones para crear un proyecto a partir de una plantilla:

* Cree un proyecto a partir de una plantilla en el área Proyectos
* Creación de un proyecto a partir de una plantilla en el nivel de plantilla
* Adjuntar una plantilla a un proyecto existente

  Para obtener más información, consulte [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Cree un proyecto a partir de una plantilla en el área Grupos

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
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Workfront</td> 
   <td> <p>Nuevo: estándar</p>
        <p>o</p>
        <p>Actual: plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Proyectos y Plantillas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos de una plantilla</p> <p>Al crear un proyecto, recibirá automáticamente permisos de administración en el proyecto.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Cree un proyecto a partir de una plantilla en el área Proyectos

Puede crear un proyecto desde el área Proyectos en el menú principal o desde el área Proyectos de un portafolio o programa.

1. Realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda. Clic **Proyectos** y, a continuación, expanda **Nuevo proyecto**.
   * Vaya a un portafolio y amplíe **Nuevo proyecto**.

     >[!TIP]
     >
     >Cuando se crea un proyecto utilizando una plantilla de un portafolio, el campo Portfolio del nuevo proyecto se actualiza para mostrar el portafolio desde el que se eligió crear el proyecto. Esto sobrescribe el campo del Portfolio en la plantilla, si se especifica.

   * Vaya a un programa y expanda **Nuevo proyecto**.

     >[!TIP]
     >
     >Cuando se crea un proyecto con una plantilla de un programa, el campo Programa de los nuevos proyectos se actualiza para mostrar el Programa desde el que se eligió crear el proyecto. El campo Portfolio de la plantilla se actualiza para mostrar el portafolio del programa desde el que eligió crear el proyecto. Esto sobrescribe los campos Programa y Portfolio de la plantilla, si se especifican.

   * Si es administrador de un grupo, también puede crear un proyecto en la sección Proyectos de un grupo que administre. Para obtener más información, consulte [Crear y modificar proyectos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

     >[!TIP]
     >
     >Cuando se crea un proyecto utilizando una plantilla de un grupo, el grupo desde el que se crea el proyecto solo se muestra en el campo Grupo del nuevo proyecto cuando no se especifica el campo Grupo de la plantilla. Si se especifica el campo Grupo de plantilla, el campo Grupo del nuevo proyecto es el de la plantilla.

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![Nuevas opciones de proyecto](assets/new-project-dropdown.png)

1. Haga clic en el nombre de una plantilla en la **Plantillas favoritas** lista.

   ![Seleccionar una plantilla favorita](assets/new-project-from-template-dropdown-with-template-favorites.png)

   O

   Haga lo siguiente:

   1. Seleccionar **Nuevo proyecto a partir de plantilla**.
   1. En el **Buscar plantillas** , empiece a escribir el nombre de una plantilla y haga clic en ella cuando se muestre en la lista.
   1. Revise los detalles de la plantilla a la derecha.

      Los detalles de la plantilla incluyen lo siguiente:

      * Duración de plantilla
      * Propietario de plantilla
      * Número de tareas de nivel superior, que incluye los nombres de las tres tareas principales
      * Número de todas las tareas de la plantilla
      * Nombres de los formularios personalizados de plantilla

   1. (Opcional) Pase el ratón sobre el nombre de una plantilla en el panel izquierdo y haga clic en **Favoritos** **icono** ![](assets/favorites-icon-small.png) para marcarlo como favorito para uso futuro.

      O

      Expanda el **Plantillas favoritas** y seleccione una plantilla de la lista desplegable.

      >[!TIP]
      >
      >Puede tener hasta 40 elementos de Workfront marcados como favoritos. Esto incluye plantillas y otros elementos.

   1. Clic **Usar plantilla** cuando haya seleccionado una plantilla.

      ![Detalles de plantilla](assets/new-project-from-template-small-box-with-template-details-panel.png)

      >[!NOTE]
      >
      >Si ha aplicado la Vista de Hito a la lista de proyectos, haga clic en el nombre de una plantilla en la **Nuevo de la sección Plantilla**.
      >
      >
      >![Vista de hito de la creación de un proyecto a partir de una plantilla](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >

   El **Nuevo proyecto** se abre el cuadro.

   ![Cuadro Nuevo proyecto](assets/new-project-from-template-box.png)

1. Si un campo ya se ha rellenado en la plantilla, el campo se rellena previamente en la **Nuevo proyecto** cuadro. Puede editar los valores rellenados previamente para que coincidan mejor con su proyecto. Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).
1. Clic **Crear proyecto**.

   Todos los detalles definidos en la plantilla se asocian automáticamente al proyecto recién creado si no los ha cambiado en el paso anterior.

## Cree un proyecto a partir de una plantilla en el área Plantillas

En lugar de empezar en el área de Proyectos, puede crear un proyecto a partir de una plantilla empezando por la plantilla.

{{step1-to-templates}}

1. Haga clic en el nombre de la plantilla que desee utilizar.
1. Haga clic en **Más** menú ![](assets/more-icon.png), luego haga clic en **Crear proyecto**.

   ![Crear proyecto a partir de plantilla](assets/project-sharing-on-template.png)

   El **Nuevo proyecto** se abre el cuadro.

1. Introduzca un nombre para el proyecto, revise cada sección y realice los cambios que sean necesarios.

   ![Cuadro Nuevo proyecto](assets/new-project-from-template-box.png)

   Si un campo ya se ha rellenado en la plantilla, el campo se rellena previamente en la **Nuevo proyecto** cuadro. Puede editar los valores rellenados previamente para que coincidan mejor con su proyecto. Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Clic **Crear proyecto**.

   Todos los detalles definidos en la plantilla se asocian automáticamente al proyecto recién creado si no los ha cambiado en el paso anterior.
