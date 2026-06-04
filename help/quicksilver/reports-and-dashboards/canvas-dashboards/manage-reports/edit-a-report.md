---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Edición de un informe en un panel de lienzo
description: Puede editar un informe de panel de lienzo una vez que se haya creado.
author: Courtney
feature: Reports and Dashboards
exl-id: fd659f56-d67f-4a0f-8735-b214934903ac
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/K9eFg04PjbqHlseDjHQQJXw9uAjNLSGDBu870P-ZCVk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 513
ht-degree: 16%

---

# Edición de un informe en un panel de lienzo

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Póngase en contacto con Atención al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform

Después de agregar informes a un panel de lienzo, puede editar la información del informe para cambiar los datos que se muestran en el panel.

Cualquier cambio realizado en un informe afectará a todos los usuarios que tengan acceso al panel que lo contiene.


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
<p>Estándar</p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td> 
   <td><p>Editar el acceso a Informes, Paneles de control y Calendarios</p>
  </td> 
  </tr>  
        <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td><p>Administración de permisos para el tablero</p>
  </td> 
  </tr>
</tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Requisitos previos

Debe agregar un informe a un panel para poder editarlo.

Para obtener más información, consulte [Crear un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Edición de un informe

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.

1. En la página **Paneles de lienzo**, haga clic en el icono **Más** ![Más icono](assets/more-icon.png) en la esquina superior derecha del informe que desea editar y, a continuación, seleccione **Editar**.

   ![Editar un informe](assets/edit-report-box.png)

1. En el cuadro de diálogo **Configurar**, edite la información en las secciones que aparecen a la izquierda. Estas secciones variarán según el tipo de informe que esté editando.

   >[!TIP]
   >
   >La sección Detalles para todos los tipos de informe incluye la opción **Ejecutar este informe con los derechos de acceso de**. Use esto para especificar un usuario cuyos permisos se utilicen para procesar los datos del informe, asegurándose de que todos los visualizadores de tableros vean los mismos datos. Para obtener más información, vea [Generar un informe KPI](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md), [Generar un informe de gráfico](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md) o [Generar un informe de tabla](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

1. (Opcional) Si edita un informe de KPI, edite la información según sea necesario en las siguientes secciones:

   * **Detalles**
   * **Generar KPI**
   * **Filtros**
   * **Configuración de columna de desglose**
   * **Configuración del grupo de desglose**

   Para obtener más información sobre estas secciones, consulte [Generar un informe de KPI](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md).

1. (Opcional) Si edita un informe de gráfico, edite la información según sea necesario en las siguientes secciones:

   * **Detalles**
   * **Gráfico de compilación**
   * **Filtros**
   * **Configuración de columna de desglose**
   * **Configuración del grupo de desglose**

   Para obtener más información sobre estas secciones, consulte [Crear un informe de gráfico](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

1. (Opcional) Si edita un informe de tabla, edite la información según sea necesario en las siguientes secciones:

   * **Detalles**
   * **Generar tabla**
   * **Filtros**
   * **Configuración de grupo**

   Para obtener más información sobre estas secciones, consulte [Generar un informe de tabla](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

1. Haga clic en **Guardar** para actualizar el informe.

## Editar un informe existente

Al editar un informe existente, los datos del informe que seleccione anularán los datos que se muestran actualmente en el widget. Si desea agregar un informe existente adicional en lugar de reemplazar uno, se recomienda crear un widget de informe independiente.

Para obtener más información, vea [Agregar un informe existente a un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/add-existing-report.md)

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.

1. En la página **Paneles de lienzo**, haga clic en el icono **Más** ![Más icono](assets/more-icon.png) en la esquina superior derecha del informe que desea editar y, a continuación, seleccione **Editar**.

1. En el cuadro **Selección de informe**, haga clic en **Agregar** en línea con el informe con el que desea reemplazar los datos del widget de informe existente.
