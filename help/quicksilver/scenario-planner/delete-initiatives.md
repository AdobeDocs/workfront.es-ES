---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Eliminar iniciativas en el planificador de escenarios
description: Puede eliminar iniciativas de un plan que haya creado o de uno que se haya compartido con usted. No es posible recuperar las iniciativas que haya eliminado.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 84%

---

# Eliminar iniciativas en el [!DNL Scenario Planner]

Puede eliminar iniciativas de un plan que haya creado o de uno que se haya compartido con usted. No es posible recuperar las iniciativas que haya eliminado.

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
</table>

*For information, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Eliminar iniciativas

Tenga en cuenta lo siguiente al eliminar iniciativas:

* Al eliminar una iniciativa, se elimina del plan la cantidad necesaria de funciones y la información de costes asociada a la iniciativa.
* Al eliminar una iniciativa creada mediante la importación de un proyecto, no se elimina el proyecto asociado a la iniciativa.
* La eliminación de una iniciativa que se ha publicado en un proyecto al menos una vez resulta en lo siguiente:

   * La iniciativa se eliminará del escenario, pero el área [!DNL Scenario Planner] permanece en la sección [!UICONTROL Detalles del proyecto].
   * Si la iniciativa que elimina es la única publicada en el escenario, también se elimina el indicador de que el plan se ha publicado.

     Para obtener más información sobre cómo publicar iniciativas en proyectos, consulte [Actualizar o crear proyectos mediante la publicación de iniciativas en el [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

     Para obtener más información sobre cómo crear iniciativas mediante la importación de proyectos, consulte [Importar proyectos a planes en el [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

Puede eliminar una iniciativa de una vez o varias por lote.

* [Eliminar una iniciativa](#delete-one-initiative)
* [Eliminar iniciativas por lote](#delete-initiatives-in-bulk)

### Eliminar una iniciativa {#delete-one-initiative}

{{step1-to-scenario-planner}}

Se muestra una lista de planes.

1. Haga clic en el nombre de un plan para abrirlo y busque la iniciativa que desea eliminar.
1. Realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Menú más]** ![Menú más](assets/more-menu.png) a la derecha del nombre de la iniciativa y, a continuación, haga clic en **[!UICONTROL Eliminar]** > **[!UICONTROL Sí, eliminarla]**.

   * Seleccione el cuadro de la izquierda de la iniciativa, haga clic en **[!UICONTROL Eliminar]** en el menú flotante que aparece en la parte inferior del plan y, a continuación, haga clic en **[!UICONTROL Sí, eliminar]**.

   La iniciativa y su información sobre la función y el coste se eliminarán del plan.

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.

### Eliminar iniciativas por lote {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

Se muestra una lista de planes.

1. Haga clic en el nombre de un plan para abrirlo y busque la iniciativa que desea eliminar.
1. Seleccione los cuadros a la izquierda de las iniciativas que desea eliminar, haga clic en **[!UICONTROL Eliminar]** en el menú que aparece en la parte inferior del plan y, a continuación, haga clic en **[!UICONTROL Sí, eliminar]**.

   ![Administrar menú de iniciativa](assets/bottom-manage-initiative-menu-350x45.png)

   Las iniciativas y su información sobre la función y el coste se eliminarán del plan.

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.
