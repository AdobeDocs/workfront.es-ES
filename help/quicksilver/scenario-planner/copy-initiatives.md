---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Copiar iniciativas en el planificador de escenarios
description: Puede crear iniciativas copiando las existentes. Puede copiar iniciativas en un plan que haya creado o en un plan que alguien comparta con usted.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Copiar iniciativas en [!DNL Scenario Planner]

Puede crear iniciativas copiando las existentes. Puede copiar iniciativas en un plan que haya creado o en un plan que alguien comparta con usted.

## Requisitos de acceso

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Empresa] o superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licencia</b>*</p> </td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Producto</b> </td> 
   <td> <p>Debe adquirir una licencia adicional para la funcionalidad [!DNL Adobe Workfront Scenario Planner] de acceso descrita en este artículo.</p> <p>Para obtener información acerca de cómo obtener [!DNL Workfront Scenario Planner], vea <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para usar [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>[!UICONTROL Edit] acceso o superior a [!DNL Scenario Planner]</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede cambiar su nivel de acceso, vea <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Permisos de [!UICONTROL Manage] para un plan</p> <p>Para obtener información sobre cómo solicitar acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acceso a un plan en [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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

  Para obtener información acerca de cómo crear iniciativas mediante la importación de proyectos, vea [Importar proyectos a planes en [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

## Copiar iniciativas

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) y luego haga clic en [!UICONTROL Escenarios].

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
