---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Eliminar iniciativas en el planificador de escenarios
description: Puede eliminar iniciativas en un plan que haya creado o en un plan que alguien haya compartido con usted. No puede recuperar iniciativas que eliminó.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# Elimine iniciativas en [!DNL Scenario Planner]

Puede eliminar iniciativas en un plan que haya creado o en un plan que alguien haya compartido con usted. No puede recuperar iniciativas que eliminó.

## Requisitos de acceso

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
   <td> <p>Debe adquirir una licencia adicional para [!DNL Adobe Workfront Scenario Planner] para acceder a la funcionalidad descrita en este artículo. </p> <p>Para obtener información sobre cómo obtener la variable [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Se necesita acceso para utilizar el [!UICONTROL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Acceso de [!UICONTROL Edit] o superior a la variable [!DNL Scenario Planner]</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Permisos de [!UICONTROL Administrar] para un plan</p> <p>Para obtener información sobre la solicitud de acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acceso a un plan en la [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Eliminar iniciativas

Tenga en cuenta lo siguiente al eliminar iniciativas:

* Al eliminar una iniciativa, se elimina del plan la cantidad necesaria de funciones de trabajo y la información de coste asociada con ella.
* Al eliminar una iniciativa que se creó mediante la importación de un proyecto, no se elimina el proyecto asociado a la iniciativa.
* Al eliminar una iniciativa que se ha publicado en un proyecto al menos una vez, se obtiene lo siguiente:

   * La iniciativa se borra del escenario, pero el [!DNL Scenario Planner] permanece en la zona [!UICONTROL Detalles del proyecto] para obtener más información.
   * Si la iniciativa que borra es la única iniciativa publicada en el escenario, también se elimina el indicador de que el plan ha sido publicado.

      Para obtener información sobre la publicación de iniciativas en proyectos, consulte [Actualice o cree proyectos publicando iniciativas en el [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

      Para obtener información sobre la creación de iniciativas mediante la importación de proyectos, consulte [Importar proyectos a planes en el [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

Puede eliminar una iniciativa a la vez o varias iniciativas de forma masiva.

* [Eliminar una iniciativa](#delete-one-initiative)
* [Eliminar iniciativas de forma masiva](#delete-initiatives-in-bulk)

### Eliminar una iniciativa {#delete-one-initiative}

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png)y haga clic en [!UICONTROL Situaciones].

   Se muestra una lista de planes.

1. Haga clic en el nombre de un plan para abrirlo y, a continuación, busque la iniciativa que desee eliminar.
1. Realice una de las siguientes acciones:

   * Haga clic en el **[!UICONTROL Más menú]** ![](assets/more-menu.png) a la derecha del nombre de la iniciativa, haga clic en **[!UICONTROL Eliminar]** > **[!UICONTROL Sí, elimínelo]**.

   * Seleccione el cuadro de la izquierda de la iniciativa y haga clic en **[!UICONTROL Eliminar]** en el menú flotante que aparece en la parte inferior del plan, haga clic en **[!UICONTROL Sí, elimínelo]**.

   La iniciativa y su función de trabajo y la información sobre los costos se eliminan del plan.

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.

### Eliminar iniciativas de forma masiva {#delete-initiatives-in-bulk}

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png)y haga clic en [!UICONTROL Situaciones].

   Se muestra una lista de planes.

1. Haga clic en el nombre de un plan para abrirlo y, a continuación, busque la iniciativa que desee eliminar.
1. Seleccione los cuadros a la izquierda de las iniciativas que desea eliminar y haga clic en **[!UICONTROL Eliminar]** en el menú que aparece en la parte inferior del plan, haga clic en **[!UICONTROL Sí, elimínelos]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   Las iniciativas y su función de trabajo y la información sobre los costos se eliminan del plan.

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.
