---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Eliminar planes en el Scenario Planner
description: Puede eliminar los planes que ha creado. No puede eliminar planes que se hayan compartido con usted.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 81%

---

# Eliminar planes en el [!DNL Scenario Planner]

Puede eliminar los planes que ha creado. No puede eliminar planes que se hayan compartido con usted.

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
   <td> <p>Acceso de [!UICONTROL Edit] al [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permisos de objeto </p> </td> 
   <td> <p>Permisos de [!UICONTROL Manage] para un plan</p> </td> 
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
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Eliminar planes

>[!IMPORTANT]
>
>No puede recuperar los planes eliminados.

Puede eliminar un plan o un escenario de un plan.

* [Eliminar planes](#delete-plans)
* [Eliminar escenarios](#delete-scenarios)

### Eliminar planes

>[!IMPORTANT]
>
>Tenga en cuenta lo siguiente al eliminar planes:
>
>* También se elimina toda la información relacionada con el plan. Esto incluye todos los escenarios e iniciativas asociados con el plan, incluida la información sobre las funciones y los costes. Esta información no se puede recuperar.
>* Si el plan contiene un escenario publicado, los proyectos vinculados a las iniciativas eliminadas se conservan y el área [!DNL Scenario Planner] permanece en la sección [!UICONTROL Detalles del proyecto].
>
>  Para obtener información acerca de cómo publicar iniciativas en proyectos, consulte [Actualizar o crear proyectos mediante la publicación de iniciativas en el  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Para suprimir un plan:

{{step1-to-scenario-planner}}

Se muestra una lista de planes.

1. Seleccione el nombre de un plan para abrirlo.
1. Haga clic en el **[!UICONTROL menú Más]** ![menú Más](assets/more-menu.png) que se encuentra a la derecha del nombre del plan y luego haga clic en **[!UICONTROL Eliminar]** > **[!UICONTROL Sí, eliminarlo]**.

   El plan se elimina y usted vuelve a la lista de planes.

### Eliminar escenarios {#delete-scenarios}

>[!IMPORTANT]
>
>Tenga en cuenta lo siguiente al eliminar un escenario:
>
>* Al eliminar un escenario, se eliminan todas las iniciativas y su información. Si se copian en otros escenarios, las iniciativas permanecen en los otros escenarios.
>* Al eliminar un escenario, el escenario posterior toma el número del escenario eliminado y se conserva el orden de recuento. Por ejemplo, si elimina el Escenario 4, el Escenario 5 se convierte en el Escenario 4.
>* Si se publican algunas iniciativas en el escenario, el proyecto vinculado a la iniciativa se conserva y el área del Planificador de escenarios permanece en los proyectos vinculados
>* Si las iniciativas publicadas existen en otro escenario, permanecen en ese escenario, incluido su vínculo al proyecto. La publicación de estas iniciativas desde otros escenarios actualiza los proyectos vinculados con nueva información de esos escenarios.
>
>  Para obtener información acerca de cómo publicar iniciativas en proyectos, consulte [Actualizar o crear proyectos mediante la publicación de iniciativas en [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Para eliminar un escenario:

1. Vaya al plan para el que desea eliminar un escenario.

   De forma predeterminada, se muestra el escenario inicial.

1. Haga clic en **[!UICONTROL Comparar escenarios]**.
1. En la esquina superior derecha de la tarjeta del escenario, haga clic en el menú **[!UICONTROL Más]** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **[!UICONTROL Eliminar]**.

   Se elimina el escenario.

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete initiatives</h2>
<p>(NOTE: moved this section to its own article about deleting initiatives) </p> <note type="important">
<p>Consider the following when deleting initiatives:</p>
<ul>
<li>Deleting an initiative deletes the job roles and cost information from the initiative.</li>
<li><span>When you delete an initiative that is published to a project, the initiative is removed from the scenario but the Scenario Planner area remains in the Project Details section.</span> </li>
<li> <p>If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed. </p> <p>For information about publishing initiatives to projects, see <a href="../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Scenario Planner</a>.</p> </li>
</ul>
</note>
<p>To delete an initiative:</p>
<ol>
<li value="1"> <p> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png">, then click Scenarios.</p> </p> <p>A list of plans displays. </p> </li>
<li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/more-menu.png"> to the right of the initiative name, then click <strong>Delete</strong> > <strong>Yes, delete it</strong>. </p> <p>The initiative is deleted. </p> </li>
<li value="4">Click <strong>Save Plan</strong> to save your changes. </li>
</ol>
</div>
-->


