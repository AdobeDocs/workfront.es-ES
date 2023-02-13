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
ht-degree: 1%

---

# Copiar iniciativas en la [!DNL Scenario Planner]

Puede crear iniciativas copiando las existentes. Puede copiar iniciativas en un plan que haya creado o en un plan que alguien comparta con usted.

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
   <td> <p>[!DNL Adobe Workfront]<b> licencia</b>*</p> </td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>Debe adquirir una licencia adicional para [!DNL Adobe Workfront Scenario Planner] para acceder a la funcionalidad descrita en este artículo.</p> <p>Para obtener información sobre cómo obtener la variable [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para usar la variable [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Acceso de [!UICONTROL Edit] o superior a la variable [!DNL Scenario Planner]</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Permisos de [!UICONTROL Administrar] para un plan</p> <p>Para obtener información sobre la solicitud de acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acceso a un plan en la [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Copiar iniciativas

Tenga en cuenta lo siguiente al copiar iniciativas:

* Al copiar una iniciativa, la copia se sitúa en el mismo plan que la iniciativa original.
* Copiar una iniciativa copia y agrega la siguiente información de la iniciativa original a la nueva iniciativa:

   * [!UICONTROL Duración]
   * [!UICONTROL Roles]
   * [!UICONTROL People] y [!UICONTROL Costes fijos]
   * [!UICONTROL Beneficio planificado]

* Copiar una iniciativa puede modificar la siguiente información para el plan, si existe información sobre la iniciativa original:

   * Cantidad requerida de funciones de trabajo
   * [!UICONTROL Costes]
   * [!UICONTROL Uso del plan]
   * Utilización de la función del trabajo
   * [!UICONTROL Valor neto]

* La copia de una iniciativa creada mediante la importación de un proyecto o publicada en un proyecto al menos una vez tiene las siguientes implicaciones:

   * No duplica el proyecto asociado con la iniciativa.
   * No conecta la iniciativa copiada con el proyecto.
   * No modifica la variable [!DNL Scenario Planner] del proyecto, para proyectos que se hayan publicado al menos una vez.

   Para obtener información sobre la publicación de iniciativas en proyectos, consulte [Actualice o cree proyectos publicando iniciativas en el [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

   Para obtener información sobre la creación de iniciativas mediante la importación de proyectos, consulte [Importar proyectos a planes en el [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

## Copiar iniciativas

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png)y haga clic en [!UICONTROL Situaciones].

   Se muestra una lista de planes.

1. Haga clic en el nombre de un plan para abrirlo y, a continuación, busque las iniciativas que desee copiar.
1. Seleccione el cuadro a la izquierda de la iniciativa o iniciativas que desee copiar y, a continuación, haga clic en **[!UICONTROL Copiar]** en el menú que aparece en la parte inferior del plan.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] copia las iniciativas inmediatamente y las coloca debajo de la última iniciativa seleccionada.

   El nombre de la iniciativa copiada es *[!UICONTROL Copia de]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >Dependiendo de dónde inserte las nuevas iniciativas, el número de iniciativas existentes puede cambiar.

1. Actualice el nombre de la iniciativa copiada.

   >[!TIP]
   >
   >Le recomendamos que siempre actualice el nombre de la iniciativa para evitar confusiones en caso de que desee volver a copiarlos.

1. (Opcional) Actualice la prioridad de las iniciativas recién creadas.

   Para obtener información sobre cómo priorizar iniciativas, consulte [Actualizar las prioridades de la iniciativa en el [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.
