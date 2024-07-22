---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Eliminar iniciativas en el Scenario Planner
description: Puede eliminar iniciativas de un plan que haya creado o de un plan que alguien haya compartido con usted. No puede recuperar las iniciativas que ha eliminado.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: ed179058cfec1332384ef76cb04598278109291b
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 1%

---

# Eliminar iniciativas en [!DNL Scenario Planner]

Puede eliminar iniciativas de un plan que haya creado o de un plan que alguien haya compartido con usted. No puede recuperar las iniciativas que ha eliminado.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <p>Actual: [!UICONTROL Empresa] o superior</p>
   <p>Nuevo: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licencia*</p> </td> 
   <td> <p>Nuevo: claro o superior</p> 
   <p>Actual: [!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td>Producto* </td> 
   <td> 
   <p>Para los planes actuales de Workfront: </p>
   <p>Debe adquirir una licencia adicional para la funcionalidad [!DNL Adobe Workfront Scenario Planner] de acceso descrita en este artículo.</p> <p>Para obtener información acerca del acceso y los permisos para [!DNL Workfront Scenario Planner], vea <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para usar [!DNL Scenario Planner]</a>. </p> </td> 
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

## Eliminar iniciativas

Tenga en cuenta lo siguiente al eliminar iniciativas:

* Al eliminar una iniciativa, se elimina del plan la cantidad necesaria de funciones del puesto y la información de costes asociada con la iniciativa.
* Al eliminar una iniciativa creada mediante la importación de un proyecto, no se elimina el proyecto asociado a la iniciativa.
* La eliminación de una iniciativa que se ha publicado en un proyecto al menos una vez resulta en lo siguiente:

   * La iniciativa se eliminará del escenario, pero el área [!DNL Scenario Planner] permanecerá en la sección [!UICONTROL Detalles del proyecto].
   * Si la iniciativa que elimina es la única iniciativa publicada en el escenario, también se elimina el indicador de que el plan se ha publicado.

     Para obtener información acerca de cómo publicar iniciativas en proyectos, vea [Actualizar o crear proyectos mediante la publicación de iniciativas en [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

     Para obtener información acerca de cómo crear iniciativas mediante la importación de proyectos, vea [Importar proyectos a planes en [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

Puede eliminar una iniciativa a la vez o puede eliminar varias iniciativas de forma masiva.

* [Eliminar una iniciativa](#delete-one-initiative)
* [Eliminar iniciativas de forma masiva](#delete-initiatives-in-bulk)

### Eliminar una iniciativa {#delete-one-initiative}

{{step1-to-scenario-planner}}

Se muestra una lista de planes.

1. Haga clic en el nombre de un plan para abrirlo y luego busque la iniciativa que desee eliminar.
1. Realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Menú más]** ![](assets/more-menu.png) a la derecha del nombre de la iniciativa y, a continuación, haga clic en **[!UICONTROL Eliminar]** > **[!UICONTROL Sí, eliminarla]**.

   * Seleccione el cuadro de la izquierda de la iniciativa, luego haga clic en **[!UICONTROL Eliminar]** en el menú flotante que aparece en la parte inferior del plan y luego haga clic en **[!UICONTROL Sí, eliminarla]**.

   La iniciativa y su información de función y coste se eliminan del plan.

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.

### Eliminar iniciativas de forma masiva {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

Se muestra una lista de planes.

1. Haga clic en el nombre de un plan para abrirlo y luego busque la iniciativa que desee eliminar.
1. Seleccione las casillas a la izquierda de las iniciativas que desea eliminar, luego haga clic en **[!UICONTROL Eliminar]** en el menú que aparece en la parte inferior del plan y luego haga clic en **[!UICONTROL Sí, eliminarlas]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   Las iniciativas y su información sobre funciones y costes se eliminan del plan.

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.
