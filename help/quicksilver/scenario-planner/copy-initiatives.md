---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Copiar iniciativas en el planificador de escenarios
description: Puede crear iniciativas copiando las existentes. Puede copiar iniciativas en un plan que haya creado o en un plan que alguien comparta con usted.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 1%

---

# Copiar iniciativas en [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Puede crear iniciativas copiando las existentes. Puede copiar iniciativas en un plan que haya creado o en un plan que alguien comparta con usted.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>Nuevo: Ultimate </p></li>
   <p>El Scenario Planner no está disponible para los nuevos planes Workfront Select o Workfront Prime. </p>
   <li><p>Actual: [!UICONTROL Empresa] o superior</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licencia*</p> </td> 
   <td> <p>Nuevo: claro o superior</p> 
   <p>Actual: [!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td>Producto* </td> 
   <td> <ul><li><p>Para los nuevos planes de Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Para los planes actuales de Workfront: </p>
   <p>Adobe Workfront</p> <p>Planificador de escenarios de Adobe Workfront</p></li></ul>

<p>Para obtener más información, consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para utilizar [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Nivel de acceso </td> 
   <td> <p>Acceso de [!UICONTROL Edit] al [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permisos de objeto </p> </td> 
   <td> <p>Permisos de [!UICONTROL Manage] para un plan</p> <p>Para obtener información sobre cómo solicitar acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acceso a un plan en [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso a la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Copiar iniciativas

Tenga en cuenta lo siguiente al copiar iniciativas:

* Copiar una iniciativa coloca la copia en el mismo plan que la iniciativa original.
* Al copiar una iniciativa, se copia y se añade la siguiente información de la iniciativa original a la nueva:

   * [!UICONTROL Duración]
   * [!UICONTROL Funciones del puesto]
   * [!UICONTROL Personas] y [!UICONTROL Costos fijos]
   * [!UICONTROL Beneficio planificado]

* Copiar una iniciativa puede modificar la siguiente información para el plan, si existe en la iniciativa original:

   * Cantidad requerida de funciones del puesto
   * [!UICONTROL Costos]
   * [!UICONTROL Utilización del plan]
   * Utilización de funciones del puesto
   * [!UICONTROL Valor neto]

* Copiar una iniciativa creada mediante la importación de un proyecto o publicada en un proyecto al menos una vez tiene las siguientes implicaciones:

   * No duplica el proyecto asociado con la iniciativa.
   * No conecta la iniciativa copiada al proyecto.
   * No modifica la sección [!DNL Scenario Planner] del proyecto, para proyectos que se han publicado al menos una vez.

  Para obtener información acerca de cómo publicar iniciativas en proyectos, vea [Actualizar o crear proyectos mediante la publicación de iniciativas en [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

  Para obtener información acerca de cómo crear iniciativas importando proyectos, vea [Importar proyectos a planes en [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

## Copiar iniciativas

{{step1-to-scenario-planner}}

Se muestra una lista de planes.

1. Haga clic en el nombre de un plan para abrirlo y, a continuación, busque las iniciativas que desee copiar.
1. Seleccione el cuadro de la izquierda de la iniciativa o iniciativas que desee copiar y luego haga clic en **[!UICONTROL Copiar]** en el menú que aparece en la parte inferior del plan.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] copia las iniciativas inmediatamente y las coloca debajo de la última iniciativa seleccionada.

   El nombre de la iniciativa copiada es *[!UICONTROL Copia de]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >Según el lugar en el que inserte las nuevas iniciativas, el número de iniciativas existentes puede cambiar.

1. Actualice el nombre de la iniciativa copiada.

   >[!TIP]
   >
   >Le recomendamos que siempre actualice el nombre de la iniciativa para evitar confusiones en caso de que desee copiarlos de nuevo.

1. (Opcional) Actualice la prioridad de las iniciativas recién creadas.

   Para obtener información acerca de cómo priorizar iniciativas, vea [Actualizar prioridades de iniciativas en [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.
