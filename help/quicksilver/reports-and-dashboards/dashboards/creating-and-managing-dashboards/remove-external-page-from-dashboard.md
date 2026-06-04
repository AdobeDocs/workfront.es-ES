---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Eliminación de una página externa de un panel
description: Puede quitar una página externa de un panel de control si ya no es necesaria.
author: Courtney
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/7uIQfoO7cP-2ouFCg9lm1EKctxkZIUtpP-SfWL34HeE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 251
ht-degree: 45%

---

# Eliminación de una página externa de un panel

<!-- Audited: 1/2025 -->

Puede quitar una página externa de un panel de control si ya no es necesaria.

Sin embargo, no puede eliminar una página externa después de crearla en Adobe Workfront. Solamente puede eliminarsse una página externa mediante la API. Para obtener más información sobre la API de Workfront, consulte [Conceptos básicos de la API](../../../wf-api/general/api-basics.md). Para obtener información sobre cómo crear páginas externas, vea [Incrustar una página web externa en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
      <p>Estándar</p>
      <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en el panel de control</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminación de una página externa de un panel

1. Vaya al panel que contiene la página externa que desea eliminar.

1. Haga clic en **Acciones de panel** y luego haga clic en **Editar**.

   ![Editar tablero](assets/unshimmed-edit-dashboard.png)

1. En el lado derecho de la pantalla, localice la página externa que desee eliminar y haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete.png).

   ![Eliminar icono de página externa dentro del panel](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. Haga clic en **Guardar + Cerrar** en la esquina inferior izquierda.

   Esto elimina la página externa del panel seleccionado. La página externa permanece en Workfront y se puede acceder a ella desde un informe. Para obtener más información, consulte la sección &quot;Ver páginas externas en un informe&quot; en el artículo [Incrustar una página web externa en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).
