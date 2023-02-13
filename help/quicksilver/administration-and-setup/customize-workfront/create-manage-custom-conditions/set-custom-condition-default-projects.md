---
title: Establecer una condición personalizada como predeterminada para los proyectos
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Si el tipo de condición de un proyecto se establece en Estado de progreso en lugar de en Manual, Adobe Workfront muestra automáticamente una de las tres condiciones predeterminadas integradas en el proyecto (Segmentación, En riesgo o En problemas) a medida que avanza, tal como se explica en Información general sobre la condición del proyecto y el tipo de condición.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Establecer una condición personalizada como predeterminada para los proyectos

Si el tipo de condición de un proyecto se establece en Estado de progreso en lugar de en Manual, Adobe Workfront muestra automáticamente una de las tres condiciones predeterminadas integradas en el proyecto (Segmentación, En riesgo o En problemas) a medida que avanza, tal como se explica en [Descripción general de la condición y el tipo de condición del proyecto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![](assets/condition-in-project-header-nwe.png)

Puede establecer las condiciones personalizadas como condiciones predeterminadas en lugar de usar estas tres condiciones predeterminadas integradas. Por ejemplo, puede cambiar la condición predeterminada On Target para que se muestre como Tracking Well en todos los proyectos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Establezca una condición personalizada como condición predeterminada para todos los proyectos:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Preferencias de proyecto** > **Condiciones**.

1. Haga clic en el **Proyecto** pestaña .
1. Haga clic en **Establecer condiciones predeterminadas**.
1. En el menú desplegable situado junto a la condición predeterminada que desea cambiar, haga clic en la condición personalizada que desee usar en su lugar.
1. Repita el paso anterior para cualquier otra condición predeterminada que desee cambiar.
1. Haga clic en **Guardar**.

Para obtener información sobre la configuración de una condición personalizada como condición predeterminada para tareas y problemas, consulte [Establecer una condición personalizada como predeterminada para tareas y problemas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Para obtener información sobre la configuración de un proyecto para que los usuarios puedan actualizar su condición manualmente, consulte [Actualizar condición para tareas y problemas](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).

Para obtener información sobre las condiciones personalizadas, consulte [Condiciones personalizadas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
