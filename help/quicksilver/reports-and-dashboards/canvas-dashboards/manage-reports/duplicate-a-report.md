---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Copia y movimiento de informes en paneles de lienzo
description: Puede copiar o mover un informe entre paneles de lienzo.
author: Courtney
feature: Reports and Dashboards
exl-id: e0f9d091-bb89-4c5b-a18d-b1e339084e67
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/5ioNl-M-KgnYE0huAbxMmLlE-qIrnwwKp-eeTRRiYLo'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 45491118778279522358f87c1c4185c4cf824829
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 15%
---
# Copia y movimiento de informes en paneles de lienzo

{{highlighted-preview}}

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Contacto con el servicio de asistencia al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform

Puede duplicar un informe de KPI, tabla o gráfico en un panel de lienzo una vez creado. Una vez duplicado, puede editar el informe según sea necesario antes de guardar.


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

Debe agregar un informe a un panel para poder duplicarlo.

Para obtener más información, consulte [Crear un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Duplicación de un informe en producción

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.
1. En la página **Paneles de lienzo**, haga clic en el icono de **Más** ![Más botón](assets/more-icon.png) en la esquina superior derecha del informe que desea duplicar y, a continuación, seleccione **Duplicado**.

   ![Botón duplicado](assets/duplicate-button.png)

1. (Opcional) En el cuadro **Configurar** que aparece, escriba un nuevo informe **Nombre** en la ficha **Detalles**.

1. (Opcional) Realice los ajustes necesarios en las configuraciones utilizando las pestañas del lado izquierdo.

   >[!NOTE]
   >
   >Estas pestañas variarán según si ha duplicado un informe de KPI, tabla o gráfico.  Para obtener más información, consulte [Crear un informe KPI en un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md), [Crear un informe de gráfico en un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md) y [Crear un informe de tabla en un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

1. Haga clic en **Guardar**. El informe duplicado aparecerá en el tablero.

<div class="preview">

## Copiar o mover un informe en vista previa

Puede copiar un informe en el tablero actual, copiarlo en otro tablero o moverlo a otro tablero. Copiar crea un duplicado del informe en el destino; al moverlo, se reubica fuera del panel actual.

>[!IMPORTANT]
>
>* Para copiar un informe, necesita permisos de administración en el panel de destino.
>* Para mover un informe, necesita el acceso de Administración a los paneles de origen y destino.
>* Si el informe tiene configurada una opción Ejecutar como usuario y usted no es administrador del sistema ni el usuario Ejecutar como, podrá copiarlo o moverlo, pero la opción Ejecutar como usuario se eliminará del informe resultante.


Para copiar o mover un informe:

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.
1. Abra el tablero que contiene el informe.
1. Haga clic en el icono **Más** ![Más botón](assets/more-icon.png) en la esquina superior derecha del informe y, a continuación, seleccione **Copiar informe**.

   ![Copiar opción de informe](assets/copy-report-button.png)

1. En el cuadro de diálogo **Copiar informe**, elija una de las siguientes opciones:

   <table>
   <tr>
   <td><strong>Copiar</strong></td>
   <td>Haga clic en <strong>Copiar</strong> en la parte inferior de la pantalla para copiar el informe. El tablero actual está seleccionado de forma predeterminada. Para copiar un informe, es necesario que tenga acceso de Administración al panel.</td>
   </tr>
   <tr>
   <td><strong>Copiar y mover</strong></td>
   <td>Seleccione un tablero de destino diferente para copiar el informe y moverlo a un tablero nuevo. El informe original permanece en el tablero actual.Para copiar y mover un informe, necesita el acceso de Administración al panel de destino. </td>
   </tr>
   <tr>
   <td><strong>Mover</strong></td>
   <td>Seleccione un tablero de destino diferente al que mover el informe. Esto reubica el informe en el panel de destino y lo elimina del panel actual. Para mover un informe, necesita el acceso de Administración a los paneles de origen y destino.</td>
   </tr>
   </table>

   >[!NOTE]
   >
   >Si el informe tiene configurada la opción Ejecutar como usuario y usted no es administrador del sistema o no es el usuario que ha establecido la opción Ejecutar como usuario, podrá copiar o mover el informe. La opción Ejecutar como usuario se elimina del informe resultante.

1. Haga clic en **Guardar**.

   ![copiar y mover](assets/copy-and-move.png)

</div>
