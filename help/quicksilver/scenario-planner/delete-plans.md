---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Eliminar planes en el planificador de escenarios
description: Puede eliminar planes que haya creado. No puede eliminar planes que se hayan compartido con usted.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# Eliminar planes en el [!DNL Scenario Planner]

Puede eliminar planes que haya creado. No puede eliminar planes que se hayan compartido con usted.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] o superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licencia*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>Debe adquirir una licencia adicional para [!DNL Adobe Workfront Scenario Planner] para acceder a la funcionalidad descrita en este artículo.</p> <p>Para obtener información sobre cómo obtener la variable [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para usar la variable [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Acceso de [!UICONTROL Edit] o superior a la variable [!DNL Scenario Planner]</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Permisos de [!UICONTROL Administrar] para un plan</p> <p>Para obtener información sobre la solicitud de acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acceso a un plan en la [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Eliminar planes

>[!IMPORTANT]
>
>No se pueden recuperar los planes eliminados.

Puede eliminar un plan o eliminar un escenario de un plan.

* [Eliminar planes](#delete-plans)
* [Eliminar escenarios](#delete-scenarios)

### Eliminar planes

>[!IMPORTANT]
>
>Tenga en cuenta lo siguiente al eliminar planes:
>
>* También se eliminará toda la información relacionada con el plan. Esto incluye todos los escenarios e iniciativas asociados con el plan, incluida la información sobre las funciones y los costos del trabajo. Esta información no se puede recuperar.
>* Si el plan contiene un escenario publicado, los proyectos vinculados a las iniciativas eliminadas se conservan y la variable [!DNL Scenario Planner] permanece en la zona [!UICONTROL Detalles del proyecto] para obtener más información.
>
>  Para obtener información sobre la publicación de iniciativas en proyectos, consulte [Actualice o cree proyectos publicando iniciativas en el [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Para eliminar un plan:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png)y haga clic en [!UICONTROL Situaciones].

   Se muestra una lista de planes.

1. Haga clic en el nombre de un plan para abrirlo.
1. Haga clic en el **[!UICONTROL Más menú]** ![](assets/more-menu.png) a la derecha del nombre del plan, haga clic en **[!UICONTROL Eliminar]** > **[!UICONTROL Sí, elimínelo]**.

   El plan es eliminado y usted vuelve a la lista de planes.

### Eliminar escenarios {#delete-scenarios}

>[!IMPORTANT]
>
>Tenga en cuenta lo siguiente al eliminar un escenario:
>
>* Al eliminar un escenario, se eliminan todas las iniciativas y su información del mismo. Si se copian a otros escenarios, las iniciativas permanecen en los demás escenarios.
>* Al eliminar un escenario, el escenario siguiente toma el número del escenario eliminado y se conserva el orden de recuento. Por ejemplo, si elimina el Escenario 4, el Escenario 5 se convierte en el Escenario 4.
>* Si se publican algunas iniciativas sobre el escenario, se conserva el proyecto vinculado a la iniciativa y el área del planificador del escenario permanece en los proyectos vinculados
>* Si las iniciativas publicadas existen en otro escenario, permanecen en ese escenario, incluido su vínculo al proyecto. La publicación de estas iniciativas desde otros escenarios actualiza los proyectos vinculados con nueva información de esos escenarios.
>
>  Para obtener información sobre la publicación de iniciativas en proyectos, consulte [Actualice o cree proyectos publicando iniciativas en el [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Para eliminar un escenario:

1. Vaya al plan para el que desea eliminar un escenario.

   De forma predeterminada, se muestra el escenario Initial .

1. Haga clic en **[!UICONTROL Comparar escenarios]**.
1. En la esquina superior derecha de la tarjeta de escenario, haga clic en el botón **[!UICONTROL Más]** menú ![](assets/more-menu.png)y haga clic en **[!UICONTROL Eliminar]**.

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


