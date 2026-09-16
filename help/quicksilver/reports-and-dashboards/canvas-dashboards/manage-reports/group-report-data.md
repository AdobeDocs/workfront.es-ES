---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Agrupar datos de informes en un panel de lienzo
description: Organice los resultados de los informes en grupos. La agrupación funciona de forma diferente en función del tipo de informe.
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 375d62fc12af075c2224f979d3ef87cdffdf03ea
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 14%
---
# Agrupar datos de informes en un panel de lienzo

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Contacto con el servicio de asistencia al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform

La agrupación organiza los resultados del informe de modo que los registros relacionados aparezcan juntos. El funcionamiento de la agrupación depende del tipo de informe, por lo que este artículo tiene una sección independiente para cada uno.

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

Debe tener un informe en un tablero o estar generando uno para poder agrupar sus datos. Para obtener más información, consulte [Crear un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Agrupar filas en un informe de tabla

En un informe de tabla, la agrupación organiza las filas del propio informe.

1. En el cuadro de diálogo **Configurar**, haga clic en el icono **Configuración de grupo** en el panel izquierdo.

1. Haga clic en **Agregar agrupación** y, a continuación, seleccione el campo por el que desee agrupar. La agrupación aparece en la vista previa a la derecha.

1. (Opcional) Repita el proceso para agregar más agrupaciones.

## Configurar agrupaciones de desglose en informes de gráficos y KPI

En los informes de gráficos y KPI, no se agrupa la visualización principal. En su lugar, puede configurar cómo se agrupa la tabla de desglose cuando un visor profundiza en un valor.

1. En el cuadro de diálogo **Configurar**, haga clic en el icono **Desglosar configuración de grupo** en el panel izquierdo.

1. Haga clic en **Agregar agrupación** y, a continuación, seleccione el campo por el que desea agrupar la tabla de desglose.

## Configuración de segmentos en un informe de tabla dinámica

Los informes de tabla dinámica no utilizan agrupaciones. En su lugar, puede definir hasta dos segmentos, que son las categorías por las que se agrupan y totalizan las métricas de la tabla dinámica.

1. En el cuadro de diálogo **Configurar**, haga clic en el icono **Segmentos** en el panel izquierdo.

1. Haga clic en **Agregar segmento** y, a continuación, seleccione el campo que desee. El segmento aparece como una columna en la vista previa.

1. (Opcional) Repita el proceso para añadir un segundo segmento. Puede añadir un máximo de dos segmentos.

## Visualización de datos agrupados en un panel

Los visualizadores de informes pueden expandir, contraer y ordenar los datos agrupados. Para obtener más información, consulte [Ver informes con datos agrupados](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md#view-reports-with-grouped-data) en [Usar paneles de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).
