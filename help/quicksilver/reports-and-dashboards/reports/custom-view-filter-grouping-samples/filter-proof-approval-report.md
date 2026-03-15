---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filter: Proof Approval Report to Omit Previous Proof Versions'
description: En un informe de Aprobación de pruebas, puede usar el filtro Es la versión actual del documento para incluir solamente las versiones actuales de las pruebas que esperan su aprobación.
author: Courtney
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 48%

---

# Filtro: informe de aprobación de pruebas para omitir versiones de prueba anteriores

<!--Audited: 10/2024-->

On a Proof Approval report, you can use the **Is Current Document Version** filter to include only the current versions of proofs waiting for your approval.

Esto resulta útil, por ejemplo, si se le ha pedido que apruebe pruebas que tienen varias versiones. Cuando se ejecuta el informe de aprobación de pruebas con el filtro Es la versión del documento actual, el informe muestra solamente la versión actual de cada prueba en espera de aprobación, omitiendo las versiones anteriores en las que ya no es necesario trabajar.

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
   <p>Contributor or Request to modify a filter </p>
   <p>Standard or Plan to modify a report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Acceso de edición a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrar informe de aprobación de pruebas para omitir versiones de pruebas anteriores

You can create a filter for a Proof Approval report.

1. Si ya tiene un informe de Aprobación de pruebas, ábralo.

   O

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   To create your own Proof Approval report, click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, or the **Main Menu** icon ![Main Menu lines](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Reports** ![Reports icon](assets/reports-in-main-menu.png).

1. Click **New Report**. The list of object types displays.
1. Click **Proof Approval** in the list.
The report builder opens.
1. Haga clic en **Filtros** y luego haga clic en **Agregar regla de filtro**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Click inside the **Set Filter Rules for your Report** box, then select **Proof Approval** from the list.
1. Click **Is Current Document Version** in the list under the **Proof Approval** object.
1. Choose Equal for your filter modifier, then select True.
1. Click **Save + Close** in the lower-left corner of Adobe Workfront, then click **Apply** in the box that appears.

   The Proof Approval report displays only proofs associated with the current versions of any document, if any proof approvals match this filtering criteria.
