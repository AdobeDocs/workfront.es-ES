---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filtro: Informe de aprobación de pruebas para omitir versiones de pruebas anteriores'
description: En un informe de Aprobación de pruebas, puede usar el filtro Es la versión actual del documento para incluir solamente las versiones actuales de las pruebas que esperan su aprobación.
author: Courtney
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/0K5-65eWGsnej09HOH7yZKBDgANUPN1JThyGnkwt1kM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 378
ht-degree: 49%

---

# Filtro: informe de aprobación de pruebas para omitir versiones de prueba anteriores

<!--Audited: 10/2024-->

En un informe de aprobación de pruebas, puede usar el filtro **Es la versión actual del documento** para incluir solamente las versiones actuales de las pruebas que esperan su aprobación.

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
   <p>Colaborador o solicitud para modificar un filtro </p>
   <p>Estándar o Plan para modificar un informe</p>
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

Puede crear un filtro para un informe de Aprobación de pruebas.

1. Si ya tiene un informe de Aprobación de pruebas, ábralo.

   O

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Para crear su propio informe de aprobación de pruebas, haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha, o en el icono **Menú principal** ![Líneas del menú principal](assets/lines-main-menu.png) en la esquina superior izquierda, si está disponible, y luego haga clic en **Informes** ![Icono de informes](assets/reports-in-main-menu.png).

1. Haga clic en **Nuevo informe**. Se muestra la lista de tipos de objetos.
1. Haga clic en **Aprobación de revisión** en la lista.
Se abre Report Builder.
1. Haga clic en **Filtros** y luego haga clic en **Agregar regla de filtro**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Haga clic dentro del cuadro **Establecer reglas de filtro para el informe** y, a continuación, seleccione **Aprobación de revisión** en la lista.
1. Haga clic en **Es la versión actual del documento** en la lista del objeto **Aprobación de la revisión**.
1. Elija Igual para el modificador de filtro y, a continuación, seleccione Verdadero.
1. Haga clic en **Guardar + Cerrar** en la esquina inferior izquierda de Adobe Workfront y, a continuación, haga clic en **Aplicar** en el cuadro que aparece.

   El informe Aprobación de pruebas muestra solamente las pruebas asociadas con las versiones actuales de cualquier documento, si alguna aprobación de prueba coincide con este criterio de filtrado.
