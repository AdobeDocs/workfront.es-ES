---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filtro: Informe de aprobación de pruebas para omitir versiones de pruebas anteriores'
description: En un informe de Aprobación de pruebas, puede usar el filtro Es la versión actual del documento para incluir solamente las versiones actuales de las pruebas que esperan su aprobación.
author: Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 50%

---

# Filtro: informe de aprobación de pruebas para omitir las versiones de prueba anteriores

<!--Audited: 10/2024-->

En un informe de aprobación de pruebas, puede usar el filtro **Es la versión actual del documento** para incluir solamente las versiones actuales de las pruebas que esperan su aprobación.

Esto resulta útil, por ejemplo, si se le ha pedido que apruebe pruebas que tienen varias versiones. Cuando se ejecuta el informe de aprobación de pruebas con el filtro Es la versión del documento actual, el informe muestra solamente la versión actual de cada prueba en espera de aprobación, omitiendo las versiones anteriores en las que ya no es necesario trabajar.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
    <p>Nuevo:</p>
   <ul><li><p>Colaborador para modificar un filtro </p></li>
   <li><p>Estándar para modificar un informe</p></li> </ul>

<p>Actual:</p>
   <ul><li><p>Solicitud para modificar un filtro </p></li>
   <li><p>Plan para modificar un informe</p></li> </ul></td> 
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

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
