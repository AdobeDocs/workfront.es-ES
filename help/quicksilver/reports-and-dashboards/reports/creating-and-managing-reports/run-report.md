---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Ejecutar un informe
description: Puede ejecutar cualquier informe al que tenga acceso de visualización.
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 85%

---


# Ejecutar un informe

Puede ejecutar cualquier informe al que tenga acceso de visualización.

<!-- Audited: 11/2024 -->

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
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
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de visualización a informes, paneles de control y calendarios</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización para un informe</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ejecutar un informe

1. Haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Informes]**.

1. Seleccione entre las siguientes opciones:

   * **Mis informes:** informes que ha creado.
   * **Compartido conmigo:** informes que otros usuarios han compartido con usted.
   * **Todos los informes:** todos los informes del sistema al que tiene acceso.

1. Haga clic en el nombre del informe que desee ejecutar.\
   O\
   Si el informe se creó con solicitudes, seleccione la información adecuada en los menús desplegables y, a continuación, haga clic en **Ejecutar informe**.\
   Para obtener más información sobre las solicitudes, consulte [Añadir una solicitud a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   El contenido del informe se muestra con una marca de tiempo en la esquina superior derecha del informe que incluye la fecha, la hora y la zona horaria en que se ejecutó el informe desde el contexto del usuario que lo ejecutó.

1. (Opcional) Haga clic en el **icono Recargar** ![Icono Recargar](assets/unshimmed-report-refresh-icon.png) para actualizar los resultados de un informe si este se ha mostrado en el explorador durante un tiempo.

1. (Condicional) Si el informe usa filtros o solicitudes, haga clic en **Mostrar filtros y solicitudes** para mostrar una lista de los filtros y las solicitudes que se están usando en el informe que está viendo. Si el informe solo contiene filtros o solicitudes, **Mostrar filtros** o **Mostrar solicitudes** aparecerán en su lugar.

   ![Mostrar filtros y solicitudes](assets/unshimmed-show-filters-and-prompts.png)

   La información se muestra debajo del nombre del informe en la parte izquierda de la página. En el caso de las solicitudes, se trata de información sobre las selecciones de solicitudes realizadas en el momento de ejecutar el informe, tal como se describe en el paso 3.

1. Si utiliza solicitudes personalizadas, no se mostrarán. Solo se muestran las solicitudes del sistema. Los filtros personalizados siempre se muestran.

## Ver un informe almacenado en caché

Es posible que el informe se almacene en caché si se ha mostrado en el explorador durante un tiempo. Puede forzar que un informe almacenado en caché se vuelva a cargar cuando realice cualquiera de las siguientes acciones:

* Edite la configuración del informe y guárdelo.
* Cambie la vista, el grupo o el filtro.
* Haga clic en el **icono Recargar** ![icono Recargar](assets/unshimmed-report-refresh-icon.png)
Esta opción está disponible en la esquina superior derecha de la página, dentro del cuadro de mensaje que indica la hora en que se guardó el informe, o bien está disponible en la esquina superior derecha del panel en el que se coloca el informe. Para obtener más información sobre cómo volver a cargar los paneles, consulte la sección &quot;Mostrar paneles&quot; en el artículo [Introducción a los paneles](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* Para acceder a cualquier página del informe que no sea la primera página, vaya a las pestañas Resumen, Matriz o Gráfico.
