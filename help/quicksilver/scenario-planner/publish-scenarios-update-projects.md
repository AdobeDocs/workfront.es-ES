---
product-area: enterprise-scenario-planner-product-area
keywords: publicar,planes,proyectos,escenario,escenarios
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Actualizar o crear proyectos publicando iniciativas en el Scenario Planner
description: Puede crear proyectos a partir de iniciativas existentes, así como actualizar proyectos previamente vinculados a iniciativas mediante la publicación de escenarios en el Scenario Planner de Adobe Workfront.
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: 9babe17ad862925440e555f881bf753fb443b67d
workflow-type: tm+mt
source-wordcount: '1722'
ht-degree: 0%

---

# Actualice o cree proyectos publicando iniciativas en [!DNL Scenario Planner]

Publicación de un escenario desde [!DNL Adobe Workfront Scenario Planner] logra lo siguiente:

* Crea proyectos a partir de las iniciativas del escenario y los vincula juntos.
* Actualiza los proyectos ya vinculados a iniciativas en el escenario con información de la iniciativa vinculada. Los proyectos también se pueden vincular a iniciativas cuando se importan en un plan. Para obtener más información, consulte [Proyectos importados a planes en [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td>[!UICONTROL Empresa] o superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licencia*</p> </td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td>Product </td> 
   <td> <p>Debe adquirir una licencia adicional para el [!DNL Adobe Workfront Scenario Planner] para acceder a la funcionalidad descrita en este artículo.</p> <p>Para obtener información sobre la obtención de [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para utilizar [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p></p> <p>Nivel de acceso*</p> </td> 
   <td> 
    <ul> 
    <li>Acceso a [!UICONTROL Edit] para [!DNL Scenario Planner] y proyectos</li></ul>

<p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede cambiar su nivel de acceso. Consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permisos de objeto</p> </td> 
   <td> 
    <ul> 
     <li>Permisos de [!UICONTROL Manage] para el plan </li> 
     <li>Permisos de [!UICONTROL Manage] para proyectos publicados</li> 
    </ul> <p>Para obtener información sobre cómo solicitar acceso adicional a los proyectos, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> <p>Para obtener información sobre cómo solicitar acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicite acceso a un plan en el [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener más información sobre el acceso a [!DNL Workfront Scenario Planner], consulte [Acceso necesario para utilizar [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

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
  >Cuando un proyecto existe en varios planes y publica información en el proyecto desde todos los planes, la última publicación sobrescribe la existente [!DNL Scenario Planner] información sobre el proyecto.

* Si se han creado iniciativas en el plan importando proyectos a este, al publicar la iniciativa también se actualizan los proyectos vinculados con información de la iniciativa.

  >[!TIP]
  >
  >Puede importar el mismo proyecto en varios planes. La publicación puede sobrescribir la información de la iniciativa en un proyecto vinculado a varias iniciativas.

  Para obtener información sobre la creación de iniciativas mediante la importación de proyectos, consulte [Proyectos importados a planes en [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Los cambios realizados en el proyecto no se transfieren a la iniciativa vinculada.



## Publicar iniciativas

>[!IMPORTANT]
>
>Si realiza cambios en las iniciativas del plan, incluida la resolución de conflictos, debe volver a publicar la iniciativa para que la nueva información sea visible en el proyecto. Esta información se muestra en los proyectos vinculados a iniciativas únicamente cuando publica la iniciativa correspondiente. Para obtener información sobre la resolución de conflictos entre iniciativas, consulte [Resolución de conflictos de iniciativas en [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **[!UICONTROL Escenarios]**
1. (Opcional y condicional) Si desea publicar desde un plan existente, haga clic en **[!UICONTROL Filtrar]** icono ![](assets/filter-nwepng.png) en la esquina superior derecha del plan, seleccione una de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Todo]</td> 
      <td>Muestra todos los planes que posee o que han compartido con usted. Esta es la opción predeterminada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Mis planes]</td> 
      <td>Muestra los planes creados.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL compartido conmigo]</td> 
      <td> <p>Muestra los planes que no creó pero que compartió con usted.</p> <p>Importante: Debe tener permisos de [!UICONTROL Manage] en planes compartidos con usted para poder publicarlos. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Opcional) Haga clic en **[!UICONTROL Buscar]** icono ![](assets/search-icon.png) y empiece a escribir el nombre de un plan para encontrarlo rápidamente en la lista.
1. (Condicional) Para publicar desde un plan nuevo, cree un plan.

   Para obtener información sobre la creación de planes, consulte [Crear y editar planes en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) .

1. (Opcional) Haga clic en el nombre de un plan existente y cree nuevos escenarios para el plan.

   Para obtener información sobre la creación de escenarios para un plan, consulte [Cree y compare escenarios de plan en la [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Opcional) Actualice las iniciativas de un plan existente o nuevo, o cree otros nuevos.

   Para obtener información sobre la creación de iniciativas, consulte [Cree y edite iniciativas en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. Clic **[!UICONTROL Guardar plan]**.
1. Seleccione el escenario que desee publicar en **[!UICONTROL Escenario inicial]** y, a continuación, haga clic en **[!UICONTROL Ir a Publicar]** ![](assets/go-to-publish-button-icon.png) en la esquina superior derecha.

   O

   Clic **[!UICONTROL Comparar escenarios]**, pase el ratón sobre la tarjeta del escenario desde la que quiera publicar y haga clic en **[!UICONTROL Ir a Publicar]** ![](assets/go-to-publish-button-icon.png).

   El [!UICONTROL Publicar iniciativas] Se muestra la página con una lista de todas las iniciativas del escenario. Si alguna de las iniciativas se publicó anteriormente, el icono del proyecto ![](assets/project-icon-sp.png) se muestra después de su nombre y la etiqueta **[!UICONTROL Última publicación]** La fecha se rellena en la lista.

   >[!TIP]
   >
   >Las iniciativas creadas mediante la importación de proyectos también muestran el icono de proyecto ![](assets/project-icon-sp.png) a la derecha de su nombre

   ![](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. (Opcional y condicional) Si desea publicar desde un plan existente, haga clic en **[!UICONTROL Filtrar]** icono ![](assets/filter-nwepng.png) en la esquina superior derecha del plan, seleccione una de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Todo]</td> 
      <td>Muestra todas las iniciativas del escenario seleccionado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Publicado]</td> 
      <td>Muestra las iniciativas que usted u otro usuario han publicado anteriormente. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Sin publicar]</td> 
      <td> <p>Muestra las iniciativas sin publicar. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. (Opcional) Haga clic en **[!UICONTROL Buscar]** icono ![](assets/search-icon.png) y empiece a escribir el nombre de una iniciativa para encontrarla rápidamente en la lista.
1. Seleccione una o varias iniciativas para publicarlas, crear o actualizar proyectos a partir de ellas y haga clic en **[!UICONTROL Publicar iniciativas]**.

   Esto crea un nuevo proyecto a partir de cada iniciativa seleccionada o actualiza los proyectos conectados existentes, si las iniciativas publicadas ya estaban vinculadas a un proyecto.

   >[!TIP]
   >
   >Los nuevos proyectos tienen el mismo nombre que las iniciativas publicadas.

1. (Condicional) Realice una de las siguientes acciones:

   * Si ha publicado una iniciativa, haga clic en **[!UICONTROL Ver proyecto asociado]** para abrir el proyecto creado o actualizado a partir de la iniciativa.
   * Si ha publicado más de una iniciativa, haga clic en **[!UICONTROL Ver proyectos asociados]** para abrir una lista de proyectos publicados a partir de iniciativas. [!DNL Workfront] aplica el [!DNL Scenario Planner] Proyectos filtra a la lista de proyectos de forma predeterminada. Los proyectos publicados más recientemente se muestran en la parte superior de la lista.

     ![](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. Vaya a las siguientes áreas para ver información de la iniciativa sobre el proyecto:

   * **El [!UICONTROL Actualizaciones] sección**: Se publica una actualización para indicar que el proyecto se creó o actualizó a partir de la iniciativa. La actualización contiene el nombre de la iniciativa que ha creado o actualizado el proyecto y el nombre vinculado del plan que contiene la iniciativa. Puede hacer clic en el nombre del plan en la actualización para abrirlo en [!DNL Scenario Planner].

     ![](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **El [!UICONTROL Información general] área de la [!UICONTROL Detalles del proyecto] sección**: Un nuevo [!DNL Scenario Planner] se crea en esta área que contiene información de la iniciativa vinculada.

     ![](assets/scenario-planner-on-project-details-350x135.png)

     La siguiente información sobre la iniciativa se publica en el [!DNL Scenario Planner] área de la [!UICONTROL Detalles del proyecto] sección:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Duración de la iniciativa]</span> </td> 
        <td><span>La duración de la iniciativa correspondiente cuando el proyecto está vinculado a una iniciativa. Este campo no se puede editar.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Última fecha de publicación]</span> </td> 
        <td><span>La fecha en la que se publicó por última vez el proyecto a partir de una iniciativa correspondiente.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Fecha de inicio de la iniciativa]</span> </td> 
        <td><span>El primer día del mes de inicio de la iniciativa, cuando el proyecto está vinculado a una iniciativa.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Fecha de finalización de la iniciativa]</span> </td> 
        <td><span>Último día del mes de finalización de la iniciativa, cuando el proyecto está vinculado a una iniciativa. </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>Funciones del puesto de la iniciativa [!UICONTROL en jornadas completas y horas]</span> </td> 
        <td> <p>Información sobre las funciones del puesto asociadas y sus asignaciones de tiempo para la iniciativa. Esto incluye:</p> 
         <ul> 
          <li>Nombre del rol</li> 
          <li>Número de ETC</li> 
          <li> <p>Número de horas para todos los ETC</p> <p>Puede calcular la cantidad de funciones del puesto necesarias para su plan o iniciativa mediante horas o jornadas completas.</p> <p>Para obtener más información, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Crear y editar planes en el Scenario Planner</a>. </p> </li> 
         </ul> 
      <p><b>SUGERENCIA</b>

     Si el número de funciones del puesto es diferente cada mes en la iniciativa, este campo muestra la cantidad máxima de funciones necesarias para la iniciativa. Por ejemplo, si necesita 1 consultor para enero y 2 para febrero, la columna muestra 2 FTE y la cantidad correspondiente de horas para 2 FTE para todos los meses.</p> </td>
     </tr> 
      </tbody> 
     </table>

     >[!NOTE]
     >
     >Todos los usuarios con [!UICONTROL Ver] acceso al proyecto puede ver el [!DNL Scenario Planner] de la sección [!UICONTROL Información general] área. Puede controlar si esta área se muestra en la [!UICONTROL Detalles] mediante una plantilla de diseño. Si los usuarios no tienen asociada una plantilla de diseño, esta área se muestra de forma predeterminada.
     >
     >   
     >   
     >   * Para obtener información acerca de cómo agregar o quitar áreas en la [!UICONTROL Detalles] sección con una plantilla de diseño, consulte [Personalización de [!UICONTROL Detalles] ver mediante una plantilla de diseño](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
     >   * Para obtener más información sobre la visualización de información en [!UICONTROL Información general] área de la [!UICONTROL Detalles del proyecto], consulte [[!UICONTROL Administrar] información en el proyecto [!UICONTROL Información general] área](../manage-work/projects/manage-projects/understand-project-overview-area.md).
     >   
     >

   * **El [!UICONTROL Asignación de funciones] panel en el [!UICONTROL Distribuidor de cargas de trabajo] o la lista de tareas del proyecto**: la información sobre la asignación de funciones en la iniciativa se rellena en esta área, además de las asignaciones de funciones en el proyecto.

     Para obtener más información, consulte [Resumen de la conciliación de asignaciones de recursos entre proyectos e iniciativas](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

     ![](assets/role-allocation-panel-350x174.png)

     Los cambios en las fechas o recursos del proyecto no afectan a la iniciativa correspondiente ni a ninguna de las áreas del proyecto que contengan información de la iniciativa.

   * **El [!UICONTROL Presupuestación de recursos] área de la [!UICONTROL Caso comercial] del proyecto**: una nueva opción para administrar recursos de proyecto mediante [!DNL Scenario Planner] La información de se agrega en [!UICONTROL Presupuestación de recursos] área de la [!UICONTROL Caso comercial] del proyecto.

     Para obtener más información, consulte [Recursos de presupuesto en [!UICONTROL Caso comercial] uso del [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     ![](assets/sp-in-business-case-selected-350x110.png)

1. (Opcional) Revise la siguiente información en la [!DNL Scenario Planner] después de publicar un escenario:

   * El escenario publicado se convierte en el primero después de publicar iniciativas a partir de él.
   * No puede publicar desde ningún otro escenario después de haber publicado un escenario al menos una vez.
   * El [!UICONTROL Ir a Publicar] se elimina de todos los demás escenarios después de que se haya publicado al menos una iniciativa de un escenario.
   * Aparece un indicador verde junto a los iconos de proyecto de las iniciativas publicadas en el plan.

     ![](assets/indicator-for-published-initiative-icon-350x119.png)

   * Un indicador verde &quot;Publicado&quot; se muestra en la parte superior del escenario y en la tarjeta Escenario, y el campo Publicado se rellena en la tarjeta Escenario indicando el número de iniciativas del escenario que se han publicado.

     ![](assets/published-scenario-highlighted-350x632.png)

     >[!TIP]
     >
     >Si se eliminan todos los proyectos publicados a partir de las iniciativas del escenario, se elimina la indicación de que el escenario se ha publicado. Para obtener más información, consulte [Eliminar proyectos](../manage-work/projects/manage-projects/delete-projects.md).

1. (Opcional) Actualice la información sobre la iniciativa y repita el proceso descrito anteriormente para volver a publicar la iniciativa y actualizar la información de la iniciativa en el proyecto vinculado.

   Para obtener información sobre la edición de iniciativas, consulte [Cree y edite iniciativas en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).


