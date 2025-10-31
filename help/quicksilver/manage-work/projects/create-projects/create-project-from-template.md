---
product-area: projects;templates
navigation-topic: create-projects
title: Crear un proyecto a partir de una plantilla
description: Puede utilizar las plantillas como un marco de trabajo para crear proyectos en Adobe Workfront. Si tiene proyectos que se repiten con frecuencia, el uso de plantillas para el nuevo proyecto evita tener que generar los mismos proyectos repetidamente.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 84%

---

# Crear un proyecto a partir de una plantilla

<!-- Audited: 10/2025 -->

Puede utilizar las plantillas como un marco de trabajo para crear proyectos en Adobe Workfront. Si tiene proyectos que se repiten con frecuencia, el uso de plantillas para la cronología general del nuevo proyecto evita tener que generar los mismos proyectos repetidamente.

Las plantillas le proporcionan una forma de capturar procesos, información y configuraciones repetibles asociados a sus proyectos. La información asociada con una plantilla se transfiere al proyecto. Esto incluye tareas, asignaciones, duraciones, documentos, detalles financieros, riesgos y formularios personalizados.

>[!TIP]
>
>Workfront define el Grupo y el Estado del nuevo proyecto de la siguiente manera:
>
>* El estado predeterminado de un nuevo proyecto creado a partir de una plantilla corresponde al estado definido por el administrador de Workfront en el área principal Preferencias de proyecto, o por un administrador de grupo (o administrador de Workfront) en el área Preferencias de proyecto para un grupo. Para obtener información acerca de cómo configurar las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Configurar las preferencias de proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* El Grupo del nuevo proyecto es el Grupo de la plantilla. Si la plantilla no está asociada a un Grupo, el Grupo del proyecto es el Grupo de inicio del usuario que crea el proyecto.
>
>* Los estados disponibles para un nuevo proyecto coinciden con los estados del Grupo del proyecto, que es el Grupo de la plantilla o el Grupo de inicio del usuario que crea el proyecto.

Tiene las siguientes opciones para crear un proyecto a partir de una plantilla:

* Crear un proyecto a partir de una plantilla en el área Proyectos
* Crear un proyecto a partir de una plantilla en el nivel de plantilla
* Adjuntar una plantilla a un proyecto existente

  Para obtener información, consulte [Adjuntar una plantilla a un proyecto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Crear un proyecto a partir de una plantilla en el área Grupos

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
   <td role="rowheader">Licencia de Workfront</td> 
   <td> <p>Estándar</p>
        <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuración de nivel de acceso</td> 
   <td> <p>Editar el acceso a Proyectos y Plantillas</p>
   <p>Editar el acceso a Portafolios y Programas, si la plantilla utilizada contiene un Portfolio y un Programa</p>  
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos de una plantilla</p> 
  <p>Si la plantilla que utiliza contiene un Portafolio y un Programa, debe tener permisos de administración en el portafolio y el programa para crear el proyecto </p> 
   <p>Al crear un proyecto, recibirá automáticamente permisos de Administración en el proyecto.</p></td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects and to Templates</p>
   
   <p>edit access to Portfolios and Programs, if the template you use contains a Portfolio and a Program</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> 
  <p>If the template you use contains a Portfolio and a Program, you must have Manage permissions to the portfolio and program to create the project </p> 
   <p>When you create a project, you automatically receive Manage permissions to the project.</p></td> 
  </tr> 
 </tbody> 
</table>-->

## Crear un proyecto a partir de una plantilla en el área Proyectos

Puede crear un proyecto desde el área Proyectos del menú principal o desde el área Proyectos de un portafolio o programa.

>[!NOTE]
>
>El administrador del sistema o del grupo puede modificar la interfaz mediante una plantilla de diseño. En este caso, algunos de los nombres de las secciones y áreas a las que se hace referencia en los pasos siguientes podrían ser diferentes en su instancia de Workfront.

1. Realice una de las siguientes acciones:

   * Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda, o en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, si está disponible, luego haga clic en **Proyectos** y expanda **Nuevo proyecto**.
   * Vaya a un portafolio y expanda **Nuevo proyecto**.

     >[!TIP]
     >
     >Cuando se crea un proyecto utilizando una plantilla de un portafolio, el campo Portafolio del nuevo proyecto se actualiza para mostrar el portafolio desde el que se eligió crear el proyecto. Esto sobrescribe el campo del Portafolio en la plantilla, si se especifica.

   * Vaya a un programa y expanda **Nuevo proyecto**.

     >[!TIP]
     >
     >Cuando se crea un proyecto con una plantilla desde un programa, el campo Programa de los nuevos proyectos se actualiza para mostrar el Programa desde el que se eligió crear el proyecto. El campo Portafolio de la plantilla se actualiza para mostrar el portafolio del programa desde el que eligió crear el proyecto. Esto sobrescribe los campos Programa y Portafolio de la plantilla, si se especifican.

   * Si es administrador de un grupo, también puede crear un proyecto en la sección Proyectos de un grupo que administre. Para obtener más información, consulte [Crear y modificar proyectos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

     >[!TIP]
     >
     >Cuando se crea un proyecto utilizando una plantilla de un grupo, el grupo desde el que se crea el proyecto solo se muestra en el campo Grupo del nuevo proyecto cuando no se especifica el campo Grupo de la plantilla. Si se especifica el campo Grupo de plantilla, el campo Grupo del nuevo proyecto es el de la plantilla.

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![Nuevas opciones de Proyecto](assets/new-project-dropdown.png)

1. Haga clic en el nombre de una plantilla en la lista **Plantillas favoritas**.

   ![Seleccionar una plantilla favorita](assets/new-project-from-template-dropdown-with-template-favorites.png)

   O

   Haga lo siguiente:

   1. Haga clic en **Nuevo proyecto a partir de plantilla**
   1. En el campo **Buscar plantillas**, empiece a escribir el nombre de una plantilla y haga clic en ella cuando se muestre en la lista.
   1. Revise los detalles de la plantilla a la derecha.

      Los detalles de la plantilla incluyen lo siguiente:

      * Duración de la plantilla
      * Propietario de la plantilla
      * Número de tareas de nivel superior, que incluye los nombres de las tres tareas principales
      * Número de todas las tareas de la plantilla
      * Nombres de los formularios personalizados de plantilla

   1. (Opcional) Pase el ratón sobre el nombre de una plantilla en el panel izquierdo y haga clic en el **icono de Favoritos** **icono** ![Favoritos](assets/favorites-icon-small.png) para marcarla como favorita para uso futuro.

      O

      Expanda la lista **Plantillas favoritas** y seleccione una plantilla de la lista desplegable.

      >[!TIP]
      >
      >Puede tener hasta 40 elementos de Workfront marcados como favoritos. Esto incluye plantillas y otros elementos.

   1. Haga clic en **Usar plantilla** cuando haya seleccionado una plantilla.

      ![Detalles sobre la plantilla](assets/new-project-from-template-small-box-with-template-details-panel.png)

      <!--no longer available, after unshimming - Oct 2025:
      >[!NOTE]
      >
      >If you have the Milestone View applied to the list of projects, click the name of a template in the **New from Template section**.
      >
      >
      >![Milestone view of creating a project from a template](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >
      -->

   Se abre el cuadro **Nuevo proyecto**.

   ![Cuadro Nuevo proyecto](assets/new-project-from-template-box.png)

1. (Condicional) Si un campo ya se ha rellenado en la plantilla, ya se ha rellenado en el cuadro **Nuevo proyecto**.

   Edite los valores rellenados previamente para que coincidan mejor con el proyecto.

   Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).
1. Haga clic en **Crear proyecto**.

   Todos los detalles definidos en la plantilla se asocian automáticamente al proyecto recién creado si no los ha cambiado en el paso anterior.

## Cree un proyecto a partir de una plantilla en el área Plantillas

En lugar de empezar en el área de Proyectos, puede crear un proyecto a partir de una plantilla empezando por la plantilla.

{{step1-to-templates}}

1. Haga clic en el nombre de la plantilla que desee utilizar.
1. Haga clic en el icono **Más** del menú ![Más](assets/more-icon.png) a la derecha del nombre de la plantilla en el encabezado, luego haga clic en **Crear proyecto**.

   ![Crear proyecto a partir de plantilla](assets/project-sharing-on-template.png)

   Se abre el cuadro **Nuevo proyecto**.

1. Escriba un nombre para el proyecto. Workfront utiliza el nombre de la plantilla para asignar un nombre al nuevo proyecto.

1. Revise cada sección del cuadro **Nuevo proyecto** y realice los cambios que sean necesarios.

   ![Cuadro Nuevo proyecto](assets/new-project-from-template-box.png)

   Si un campo ya se ha rellenado en la plantilla, el campo ya se ha rellenado previamente en el cuadro **Nuevo proyecto**. Puede editar los valores rellenados previamente para que coincidan mejor con su proyecto.

   Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Haga clic en **Crear proyecto**.

   Todos los detalles definidos en la plantilla se asocian automáticamente al proyecto recién creado si no los ha cambiado en el paso anterior.
