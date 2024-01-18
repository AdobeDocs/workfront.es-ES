---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
keywords: fusión
navigation-topic: fusion-release-activity
title: "Actividad de la versión de Workfront Fusion: Semana del 30 de noviembre de 2020"
description: Esta página describe todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 30 de noviembre de 2020.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 9621683b-735d-40a6-8d7c-b5bd167cbdd2
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Actividad de la versión de Workfront Fusion: Semana del 30 de noviembre de 2020

Esta página describe todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 30 de noviembre de 2020.

Para ver una lista de todos los cambios recientes, consulte [Actividad de la versión de Adobe Workfront Fusion](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obtener una lista de las correcciones de errores recientes en Workfront Fusion, consulte la [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) y compruebe si hay alguna actualización denominada Actualización de mantenimiento de Workfront Fusion.

## Límite de velocidad para los webhooks de Workfront Fusion 2.0.

Hemos introducido una nueva protección de rendimiento para Workfront Fusion 2.0. Ahora, los webhooks tienen un límite de 100 solicitudes por segundo. Cuando se alcanza este límite, Workfront Fusion 2.0 envía un estado 429 (Demasiadas solicitudes).

Anteriormente, las solicitudes de ganchos web no estaban limitadas.

Para obtener más información, consulte [Protecciones de rendimiento de Adobe Workfront Fusion](../../../../../workfront-fusion/get-started/fusion-performance-guardrails.md).

## Añadir un formulario personalizado a un objeto de Workfront en Workfront Fusion 2.0

Para permitirle agregar formularios personalizados a objetos de Workfront Fusion 2.0, hemos agregado la acción Asignar categorías a Workfront > Varias. Módulo de acción.

Anteriormente, no era posible utilizar un módulo de Workfront Fusion 2.0 para agregar un formulario personalizado a un objeto en Workfront.

Para obtener más información sobre Workfront > Varios. Módulo de acciones, consulte [Módulos de Adobe Workfront](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Jira Server connector and modules now available</h2>
<p>We've added a Jira Server connector to Workfront Fusion. The Jira Server connector offers the same functionality as the current Jira Cloud connector. </p>
<p>With Jira Server modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, modified, or deleted</p> </li>
<li> <p>Create, read, update, or delete a record</p> </li>
<li> <p>List or search records</p> </li>
<li> <p>Download an attachment</p> </li>
<li> <p>Add an issue to a sprint</p> </li>
<li> <p>Make a custom API call</p> </li>
</ul>
<p>Previously, Jira modules were available only for Jira Cloud.</p>
<p>For more information on available Jira modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref" xrefformat="{para}">Jira Software modules</a>.</p>
<h2>Azure DevOps connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Azure DevOps applications. With the Azure DevOps modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, updated, or deleted.</p> </li>
<li> <p>Create or update records.</p> </li>
<li> <p>Get data from existing records.</p> </li>
<li> <p>Download or upload attachments.</p> </li>
<li> <p>Link work items together.</p> </li>
<li> <p>Retrieve a list of work items.</p> </li>
<li> <p>Perform a custom API call.</p> </li>
</ul>
<p>For more information see <a href="../../../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref" xrefformat="{para}">Azure DevOps modules</a>.</p>
<h2>Microsoft Dynamics 365 connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Microsoft Dynamics 365 account. With the Microsoft Dynamics 365 modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when records are added or updated in Microsoft Dynamics 365</p> </li>
<li> <p>Create, read, update, or delete a Microsoft Dynamics 365record</p> </li>
<li> <p>Perform a custom API call</p> </li>
</ul>
<p>For information about available Microsoft Dynamics 365 modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref" xrefformat="{para}">Microsoft Dynamics 365 modules</a>.</p>
</div>
-->
