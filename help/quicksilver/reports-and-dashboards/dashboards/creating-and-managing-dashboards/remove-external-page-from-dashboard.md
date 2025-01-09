---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Eliminación de una página externa de un panel
description: Puede quitar una página externa de un panel si ya no la necesita.
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: a9abbeaa9abd0e905c60000a218eddb85d0389b9
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 26%

---

# Eliminación de una página externa de un panel

<!-- Audited: 1/2025 -->

Puede quitar una página externa de un panel si ya no la necesita.

Sin embargo, no puede eliminar una página externa después de crearla en Adobe Workfront. Solamente puede eliminarsse una página externa mediante la API. Para obtener información acerca de la API de Workfront, consulte [Conceptos básicos de la API](../../../wf-api/general/api-basics.md). Para obtener información sobre cómo crear páginas externas, vea [Incrustar una página web externa en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plan de Adobe Workfront</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront</strong></td> 
   <td> 
      <p>Nuevo:</p>
         <ul>
         <li><p>Estándar</p></li>
         </ul>
      <p>Actual:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>Acceso de Edición a informes, paneles y calendarios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Administrar permisos en el panel</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminación de una página externa de un panel

1. Vaya al panel que contiene la página externa que desea eliminar.

1. Haga clic en **Acciones de panel** y luego haga clic en **Editar**.

   ![](assets/unshimmed-edit-dashboard.png)

1. En el lado derecho de la pantalla, localice la página externa que desee eliminar y haga clic en el icono **Eliminar** ![](assets/delete.png).

   ![](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. Haga clic en **Guardar + Cerrar** en la esquina inferior izquierda.

   Esto elimina la página externa del panel seleccionado. La página externa permanece en Workfront y se puede acceder a ella desde un informe. Para obtener más información, consulte la sección &quot;Ver páginas externas en un informe&quot; en el artículo [Incrustar una página web externa en un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).
