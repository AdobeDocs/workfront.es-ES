---
product-area: enterprise-scenario-planner-product-area
keywords: publicar,planes,proyectos,escenario,escenarios
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Actualizar o crear proyectos publicando iniciativas en el Scenario Planner
description: Puede crear proyectos a partir de iniciativas existentes, así como actualizar proyectos previamente vinculados a iniciativas mediante la publicación de escenarios en el Planificador de escenarios de Adobe Workfront.
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '1696'
ht-degree: 82%

---

# Actualizar o crear proyectos mediante la publicación de iniciativas en el [!DNL Scenario Planner]

Al publicar un escenario desde [!DNL Adobe Workfront Scenario Planner] se logra lo siguiente:

* Crea proyectos a partir de las iniciativas del escenario y los vincula.
* Actualiza los proyectos ya vinculados a iniciativas en el escenario con información de la iniciativa vinculada. Los proyectos también se pueden vincular a iniciativas cuando se importan en un plan. Para obtener más información, consulte [Importar proyectos a planes en  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] paquete</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTA</b></p>
<p>Hable con su representante de Workfront si tiene un paquete de Workfront diferente.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licencia</p> </td> 
   <td> <p>[!UICONTROL Light] o superior</p> 
   <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
    <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de [!UICONTROL Edit] para [!DNL Scenario Planner] y [!UICONTROL Projects]</p></td> 
  </tr> 
  <tr> 
   <td> <p>Permisos de objeto </p> </td> 
   <td> <ul> 
     <li>Permisos de [!UICONTROL Manage] para el plan </li> 
     <li>Permisos de [!UICONTROL Manage] para proyectos publicados</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el acceso al Scenario Planner, consulte [Acceso necesario para usar el [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Para obtener información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso a la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access for the [!DNL Scenario Planner] and [!UICONTROL Projects]</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td>  <ul> 
     <li>[!UICONTROL Manage] permissions for the plan </li> 
     <li>[!UICONTROL Manage] permissions for published projects</li> 
    </ul> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->


## Requisitos previos

Antes de empezar:

* Debe crear y guardar un plan para poder publicar iniciativas a partir de él.
* La opción Permitir que los usuarios creen proyectos sin usar una plantilla debe estar habilitada en el área Preferencias de proyecto de Configuración. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Consideraciones sobre la publicación de iniciativas en proyectos

* Solo puede publicar un escenario a partir de un plan.
* Una iniciativa solo se puede vincular a un proyecto.
* Un proyecto puede vincularse a más de una iniciativa cuando las iniciativas pertenecen a planes diferentes.

  >[!TIP]
  >
  >Cuando existe un proyecto en varios planes y publica información en el proyecto desde todos los planes, la última publicación sobrescribe la información existente de [!DNL Scenario Planner] en el proyecto.

* Si se han creado iniciativas en el plan importando proyectos a este, al publicar la iniciativa también actualiza los proyectos vinculados con información de la iniciativa.

  >[!TIP]
  >
  >Puede importar el mismo proyecto en varios planes. La publicación puede sobrescribir la información de la iniciativa en un proyecto vinculado a varias iniciativas.

  Para obtener información acerca de cómo crear iniciativas importando proyectos, consulte [Importar proyectos a planes en  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Los cambios realizados en el proyecto no se transfieren a la iniciativa vinculada.



## Publicar iniciativas

>[!IMPORTANT]
>
>Si realiza cambios en las iniciativas del plan, incluida la resolución de conflictos, debe volver a publicar la iniciativa para que la nueva información sea visible en el proyecto. Esta información se muestra en los proyectos vinculados a iniciativas únicamente cuando publica la iniciativa correspondiente. Para obtener información sobre la resolución de conflictos entre iniciativas, consulte [Resolver conflictos de iniciativas en  [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

{{step1-to-scenario-planner}}

1. (Opcional y condicional) Si desea publicar desde un plan existente, haga clic en el icono **[!UICONTROL Filtro]** ![Icono de filtro](assets/filter-nwepng.png) en la esquina superior derecha del plan y seleccione una de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>Muestra todos los planes que posee o que han compartido con usted. Es la opción predeterminada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL My plans]</td> 
      <td>Muestra los planes creados.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Shared with me]</td> 
      <td> <p>Muestra los planes que no ha creado, pero que se han compartido con usted.</p> <p>Importante: Debe tener permisos de [!UICONTROL Manage] sobre los planes compartidos para poder publicarlos. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![Opciones desplegables de filtro](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Opcional) Haga clic en el icono **[!UICONTROL Buscar]** ![icono de búsqueda](assets/search-icon.png) y empiece a escribir el nombre de un plan para encontrarlo rápidamente en la lista.
1. (Condicional) Para publicar desde un plan nuevo, cree un plan.

   Para obtener información sobre la creación de planes, consulte [Crear y editar planes en el  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) .

1. (Opcional) Haga clic en el nombre de un plan existente y cree nuevos escenarios para el plan.

   Para obtener información sobre la creación de escenarios de un plan, consulte [Crear y comparar escenarios de plan en el  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Opcional) Actualice las iniciativas de un plan existente o nuevo, o cree otras nuevas.

   Para obtener información sobre la creación de iniciativas, consulte [Crear y editar iniciativas en el  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. Haga clic en **[!UICONTROL Guardar plan]**.
1. Seleccione el escenario que desea publicar en el menú desplegable **[!UICONTROL Escenario inicial]** y, a continuación, haga clic en **[!UICONTROL Ir a publicar]** ![Ir a publicar](assets/go-to-publish-button-icon.png) en la esquina superior derecha.

   O

   Haga clic en **[!UICONTROL Comparar escenarios]**, pase el ratón sobre la tarjeta de escenario desde la que desee publicar y, a continuación, haga clic en **[!UICONTROL Ir a publicar]** ![Ir a publicar](assets/go-to-publish-button-icon.png).

   Se mostrará la página [!UICONTROL Publicar iniciativas] con una lista de todas las iniciativas del escenario. Si alguna de las iniciativas se publicó anteriormente, el icono del proyecto ![Icono del proyecto](assets/project-icon-sp.png) se muestra después de su nombre y la fecha de **[!UICONTROL Última publicación]** se rellena en la lista.

   >[!TIP]
   >
   >Las iniciativas que se han creado importando proyectos también muestran el icono del proyecto ![Icono del proyecto](assets/project-icon-sp.png) a la derecha de su nombre

   ![Icono de proyecto y fecha de última publicación](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. (Opcional y condicional) Si desea publicar desde un plan existente, haga clic en el icono **[!UICONTROL Filtro]** ![Icono de filtro](assets/filter-nwepng.png) en la esquina superior derecha del plan y seleccione una de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>Muestra todas las iniciativas del escenario seleccionado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Published]</td> 
      <td>Muestra las iniciativas que ha publicado o que otro usuario ha publicado anteriormente. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unpublished]</td> 
      <td> <p>Muestra las iniciativas sin publicar. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![Filtro de iniciativas](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. (Opcional) Haga clic en el icono **[!UICONTROL Buscar]** ![Icono de búsqueda](assets/search-icon.png) y empiece a escribir el nombre de una iniciativa para encontrarla rápidamente en la lista.
1. Seleccione una o varias iniciativas para publicar, cree o actualice proyectos a partir de estas, y haga clic en **[!UICONTROL publicar iniciativas]**.

   Esta acción creará un nuevo proyecto a partir de cada iniciativa seleccionada o actualizará los proyectos conectados existentes, si las iniciativas publicadas ya estaban vinculadas a un proyecto.

   >[!TIP]
   >
   >Los nuevos proyectos tienen el mismo nombre que las iniciativas publicadas.

1. (Condicional) Realice una de las siguientes acciones:

   * Si ha publicado una iniciativa, haga clic en **[!UICONTROL ver proyectos vinculados]** para abrir el proyecto creado o actualizado a partir de la iniciativa.
   * Si ha publicado más de una iniciativa, haga clic en **[!UICONTROL ver proyectos vinculados]** para abrir una lista de proyectos publicados a partir de iniciativas. [!DNL Workfront] aplica el filtro de proyectos del [!DNL Scenario Planner] a la lista de proyectos de forma predeterminada. Los proyectos publicados más recientemente se muestran en la parte superior de la lista.

     ![Planificador de escenarios después de publicar iniciativas](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. Vaya a las siguientes áreas para ver información sobre la iniciativa del proyecto:

   * **La sección [!UICONTROL actualizaciones]**: se publica una actualización para indicar que el proyecto se ha creado o actualizado a partir de la iniciativa. La actualización contiene el nombre de la iniciativa que ha creado o actualizado el proyecto y el nombre vinculado del plan que contiene la iniciativa. Puede hacer clic en el nombre del plan de la actualización para abrir el plan en el [!DNL Scenario Planner].

     ![Actualizar confirmación de flujo de publicación](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **El área [!UICONTROL información general] de la sección [!UICONTROL Detalles del proyecto]**: se crea una nueva sección [!DNL Scenario Planner] en esta área que contiene información de la iniciativa vinculada.

     ![Planificador de escenarios en los detalles del proyecto](assets/scenario-planner-on-project-details-350x135.png)

     La siguiente información de la iniciativa se publica en el área [!DNL Scenario Planner] de la sección [!UICONTROL Detalles del proyecto]:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Duration]</span> </td> 
        <td><span>Duración de la iniciativa correspondiente cuando el proyecto está vinculado a una iniciativa. Este campo no se puede editar.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Last Published Date]</span> </td> 
        <td><span>Fecha en la que se publicó por última vez el proyecto a partir de una iniciativa correspondiente.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Start Date]</span> </td> 
        <td><span>Primer día del mes de inicio de la iniciativa, cuando el proyecto está vinculado a una iniciativa.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative End Date]</span> </td> 
        <td><span>El último día del mes de finalización de la iniciativa, en caso de que el proyecto esté vinculado a una. </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Job Roles in FTEs and Hours]</span> </td> 
        <td> <p>Información sobre las funciones asociadas y sus asignaciones de tiempo para la iniciativa. Esto incluye:</p> 
         <ul> 
          <li>Nombre de la función</li> 
          <li>Número de jornadas completas</li> 
          <li> <p>Número de horas para todas las jornadas completas</p> <p>Puede calcular la cantidad de funciones necesarias para su plan o iniciativa mediante horas o jornadas completas.</p> <p>Para obtener más información, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Crear y editar planes en el Planificador de escenarios</a>. </p> </li> 
         </ul> 
      <p><b>Sugerencia</b>

     Si el número de funciones es diferente para cada mes de la iniciativa, este campo muestra la cantidad máxima de funciones necesarias para esta. Por ejemplo, si necesita un consultor para enero y dos para febrero, la columna muestra dos jornadas completas y la cantidad de horas que les corresponden para todos los meses.</p> </td>
     </tr> 
      </tbody> 
     </table>

     >[!NOTE]
     >
     >Los usuarios con acceso para [!UICONTROL Ver] en el proyecto pueden visualizar la sección [!DNL Scenario Planner] en el área de [!UICONTROL Información general]. Puede controlar si esta área se muestra en la sección [!UICONTROL Detalles] mediante una plantilla de diseño. Si el usuario no tiene asociada una plantilla de diseño, esta área se muestra de forma predeterminada.
     >
     >   
     >   
     >   * Para obtener más información sobre cómo añadir o quitar áreas en la sección [!UICONTROL Detalles] mediante una plantilla de diseño, consulte [Personalizar la vista de [!UICONTROL Detalles] mediante una plantilla de diseño](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
     >   * Para obtener más información en el área [!UICONTROL Información general] de [!UICONTROL Detalles del proyecto], consulte [[!UICONTROL Administrar] en el área [!UICONTROL Información general] del proyecto](../manage-work/projects/manage-projects/understand-project-overview-area.md).
     >   
     >

   * **El panel [!UICONTROL Asignación de funciones] en el [!UICONTROL Distribuidor de cargas de trabajo] o la lista de tareas del proyecto**: la información sobre la asignación de funciones en la iniciativa y en el proyecto se rellena en esta área.

     Para obtener más información, consulte [Información general sobre la conciliación de asignaciones de recursos entre proyectos e iniciativas](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

     ![Panel de asignación de funciones](assets/role-allocation-panel-350x174.png)

     Los cambios en las fechas o los recursos del proyecto no afectan a la iniciativa correspondiente ni a ninguna de las áreas del proyecto que contengan información sobre la iniciativa.

   * **El área de [!UICONTROL Presupuestación de recursos] del [!UICONTROL Caso empresarial] del proyecto**: se añade una nueva opción para la administración de recursos del proyecto mediante la información de [!DNL Scenario Planner] en el área de [!UICONTROL Presupuestación de recursos] del [!UICONTROL Caso empresarial] del proyecto.

     Para obtener más información, consulte [Recursos presupuestarios en el [!UICONTROL Caso empresarial] con [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     ![Planificador de escenarios en caso empresarial](assets/sp-in-business-case-selected-350x110.png)

1. (Opcional) Revise la siguiente información en [!DNL Scenario Planner] después de publicar un escenario:

   * El escenario publicado se convierte en el primero después de publicar iniciativas a partir de este.
   * No es posible publicar desde ningún otro escenario después de haber publicado uno al menos una vez.
   * La opción [!UICONTROL Ir a publicar] se ha eliminado de los demás escenarios después de que al menos una iniciativa se haya publicado a partir de un escenario.
   * Aparece un indicador verde junto a los iconos de proyecto de las iniciativas publicadas en el plan.

     ![Indicador de la iniciativa publicada](assets/indicator-for-published-initiative-icon-350x119.png)

   * En la parte superior del escenario y en la tarjeta de escenario aparece un indicador verde de “Publicado”. El campo Publicado se rellena en la tarjeta de escenario indicando el número de iniciativas del escenario que se han publicado.

     ![Escenario publicado](assets/published-scenario-highlighted-350x632.png)

     >[!TIP]
     >
     >Si se eliminan todos los proyectos publicados a partir de las iniciativas del escenario, desaparecerá la indicación de que el escenario se ha publicado. Para obtener más información, consulte [Eliminar proyectos](../manage-work/projects/manage-projects/delete-projects.md).

1. (Opcional) Actualice la información sobre la iniciativa y repita el proceso descrito anteriormente para volver a publicarla y actualizar la información relativa a esta en el proyecto vinculado.

   Para obtener más información sobre la edición de iniciativas, consulte [Crear y editar iniciativas en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).


