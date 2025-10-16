---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Copiar iniciativas en el planificador de escenarios
description: Puede crear iniciativas copiando las existentes. Puede copiar iniciativas en un plan que haya creado o en un plan que alguien comparta con usted.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 88%

---

# Copia de iniciativas en el [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Puede crear iniciativas copiando las existentes. Puede copiar iniciativas en un plan que haya creado o en un plan que alguien comparta con usted.

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

## Copiar iniciativas

Tenga en cuenta lo siguiente al copiar iniciativas:

* Copiar una iniciativa coloca la copia en el mismo plan que la iniciativa original.
* Al copiar una iniciativa se copia y se añade la siguiente información de la iniciativa original a la nueva:

   * [!UICONTROL Duración]
   * [!UICONTROL Funciones]
   * [!UICONTROL Personas] y [!UICONTROL Costes fijos]
   * [!UICONTROL Beneficio planificado]

* Al copiar una iniciativa se puede modificar la siguiente información para el plan, si la información existe en la iniciativa original:

   * Cantidad requerida de funciones
   * [!UICONTROL Costes]
   * [!UICONTROL Utilización del plan]
   * Utilización de funciones
   * [!UICONTROL Valor neto]

* Copiar una iniciativa creada mediante la importación de un proyecto o publicada en un proyecto al menos una vez tiene las siguientes implicaciones:

   * No duplica el proyecto asociado con la iniciativa.
   * No conecta la iniciativa copiada al proyecto.
   * No modifica la sección [!DNL Scenario Planner] del proyecto, para proyectos que hayan sido publicados al menos una vez.

  Para obtener información acerca de cómo publicar iniciativas en proyectos, consulte [Actualizar o crear proyectos mediante la publicación de iniciativas en el [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

  Para obtener información acerca de cómo crear iniciativas importando proyectos, consulte [Importar proyectos a planes en el [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

## Copiar iniciativas

{{step1-to-scenario-planner}}

Se muestra una lista de planes.

1. Haga clic en el nombre de un plan para abrirlo y, a continuación, busque las iniciativas que desee copiar.
1. Seleccione la casilla situada a la izquierda de la iniciativa o iniciativas que desea copiar y, a continuación, haga clic en **[!UICONTROL Copiar]** en el menú que aparece en la parte inferior del plan.

   ![Copiar iniciativa](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] copia las iniciativas inmediatamente y las coloca debajo de la última iniciativa seleccionada.

   El nombre de la iniciativa copiada es *[!UICONTROL Copia de]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >Según el lugar en el que inserte las nuevas iniciativas, el número de iniciativas existentes puede cambiar.

1. Actualice el nombre de la iniciativa copiada.

   >[!TIP]
   >
   >Le recomendamos que siempre actualice el nombre de la iniciativa para evitar confusiones en caso de que desee copiarlas de nuevo.

1. (Opcional) Actualice la prioridad de las iniciativas recién creadas.

   Para obtener información acerca de cómo priorizar iniciativas, consulte [Actualizar prioridades de iniciativas en el [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.
