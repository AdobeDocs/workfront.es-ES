---
title: Establecer una condición personalizada como predeterminada para los proyectos
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Si el tipo de condición de un proyecto se establece en Estado de progreso en lugar de en Manual, Adobe Workfront muestra automáticamente una de las tres condiciones predeterminadas integradas en el proyecto (como destino, en riesgo o con problemas) a medida que avanza, como se explica en Información general sobre la condición y el tipo de condición del proyecto.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Establecer una condición personalizada como predeterminada para los proyectos

Si el tipo de condición de un proyecto se establece en estado de progreso en lugar de en manual, Adobe Workfront muestra automáticamente una de las tres condiciones predeterminadas integradas en el proyecto (según el destino, en riesgo o con problemas) a medida que avanza, como se explica en [Información general sobre la condición del proyecto y el tipo de condición](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![](assets/condition-in-project-header-nwe.png)

Puede establecer las condiciones personalizadas como condiciones predeterminadas en lugar de utilizar estas tres condiciones predeterminadas integradas. Por ejemplo, puede cambiar la condición predeterminada En el destino para que se muestre como Bien de seguimiento en todos los proyectos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Establezca una condición personalizada como condición predeterminada para todos los proyectos:

{{step-1-to-setup}}

1. Haga clic en **Preferencias del proyecto** > **Condiciones**.

1. Haga clic en la ficha **Proyecto**.
1. Haga clic en **Establecer condiciones predeterminadas**.
1. En el menú desplegable situado junto a la condición predeterminada que desea cambiar, haga clic en la condición personalizada que desee utilizar en su lugar.
1. Repita el paso anterior para cualquier otra condición predeterminada que desee cambiar.
1. Haga clic en **Guardar**.

Para obtener información acerca de cómo establecer una condición personalizada como condición predeterminada para tareas y problemas, vea [Establecer una condición personalizada como predeterminada para tareas y problemas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Para obtener información acerca de cómo configurar un proyecto de modo que los usuarios puedan actualizar su condición manualmente, vea [Actualizar condición para tareas y problemas](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).

Para obtener información acerca de las condiciones personalizadas, vea [Condiciones personalizadas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
