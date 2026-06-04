---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Crear un panel de lienzo
description: Con los paneles de lienzo, puede crear y agregar informes a un panel personalizable para visualizar rápidamente los datos de su cuenta.
author: Courtney
feature: Reports and Dashboards
exl-id: bd31e426-7c4a-4ff8-9432-c95dc8ee3743
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-s26q39f6l5lix-8JuSaHvvdpqeqpw3ve5Gn2ZNnHfM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 384
ht-degree: 21%

---

# Crear un panel de lienzo

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Póngase en contacto con Atención al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform

Con los paneles de lienzo, puede crear y agregar informes a un panel personalizable para visualizar rápidamente los datos de su cuenta.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquiera </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td> 
<p>Estándar </p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td> 
   <td><p>Editar el acceso a Informes, Paneles de control y Calendarios</p>
  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Requisitos previos

Los paneles de lienzo deben habilitarse en la configuración de la plantilla de diseño de los elementos de navegación de la izquierda de la página de los paneles.

## Creación de un panel de control

Los paneles de lienzo ofrecen una amplia variedad de opciones y configuraciones que puede utilizar al crear un panel. En esta sección, le guiaremos por el proceso general de creación de un panel.

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.

1. Haga clic en **Nuevo panel** en la esquina superior derecha.

1. En el cuadro **Crear tablero**,

1. Especifique lo siguiente:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nombre</strong></td>
      <td><p>Escriba un nombre para el tablero. Se recomienda utilizar solo caracteres UTF-8 para evitar problemas de compatibilidad.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descripción (opcional)</strong></td>
      <td>Escriba una descripción del tablero.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>Divisa</strong></td>
      <td>Seleccione el tipo de moneda predeterminado para el panel. <br>
      <br>Los usuarios pueden alternar entre diferentes tipos de moneda al filtrar el panel. Para obtener más información, vea <a href="/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md">Filtrar un panel por tipo de moneda</a>.</td>
     </tr>
    </tbody>
   </table>

1. Haga clic en **Crear**. Se abre **Agregar cuadro de informe**. Desde aquí, puede crear un nuevo informe o agregar uno existente al panel.

## Añadir un informe a un panel de control

Una vez creado un tablero, el siguiente paso es agregarle los informes. Para ello, puede crear un informe desde cero en la sección Paneles de lienzo o agregar uno existente.

Existen tres tipos de informes que puede crear en paneles de lienzo:

* **KPI**: este informe muestra los datos del indicador clave de rendimiento como un número.
Para obtener más información, consulte [Crear un informe de KPI](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md).

* **Gráfico**: este informe muestra los datos en forma de gráfico de barras, columnas, líneas o circulares.
Para obtener más información, consulte [Crear un informe de gráfico](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

* **Tabla**: este informe muestra los datos en formato de tabla.
Para obtener más información, consulte [Generar un informe de tabla](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

Para obtener más información sobre cómo agregar un informe existente a un panel, vea [Agregar un informe existente a un panel](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/add-existing-report.md).
