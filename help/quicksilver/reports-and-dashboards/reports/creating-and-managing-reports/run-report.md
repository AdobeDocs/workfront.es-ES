---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Ejecutar un informe
description: Puede ejecutar cualquier informe al que tenga acceso Ver.
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---


# Ejecutar un informe

Puede ejecutar cualquier informe al que tenga acceso Ver.

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso a informes, tableros y calendarios</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ejecutar un informe

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y luego haga clic en **Informes**.

1. Seleccione entre las siguientes opciones:

   * **Mis informes:** informes que ha creado.
   * **Compartido conmigo:** Informes que otros usuarios han compartido con usted.
   * **Todos los informes:** Todos los informes del sistema al que tiene acceso.

1. Haga clic en el nombre del informe que desee ejecutar.\
   O\
   Si el informe se creó con indicaciones, seleccione la información adecuada en los menús desplegables y, a continuación, haga clic en **Ejecutar informe**.\
   Para obtener más información sobre las solicitudes, vea [Agregar una solicitud a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   El contenido del informe se muestra con una marca de tiempo en la esquina superior derecha del informe que incluye la fecha, la hora y la zona horaria en que se ejecutó el informe desde el contexto del usuario que lo ejecutó.

1. (Opcional) Haga clic en el **icono Recargar** ![](assets/qs-report-refresh-icon.png) para actualizar los resultados de un informe si este se ha mostrado en el explorador durante un tiempo.

1. (Condicional) Si el informe usa filtros o indicadores, haga clic en **Mostrar filtros e indicadores** para mostrar una lista de los filtros y los indicadores que se están usando en el informe que está viendo. Si el informe solo contiene filtros o indicadores, **Mostrar filtros** o **Mostrar indicadores** aparecerán en su lugar.

   ![Mostrar filtros e indicadores](assets/qs-reports-showfiltersandprompts-2022-350x136.png)

   La información se muestra debajo del nombre del informe en la parte izquierda de la página. En el caso de las solicitudes, se trata de información sobre las selecciones de solicitudes realizadas en el momento de ejecutar el informe, tal como se describe en el paso 4.

1. Si utiliza indicadores personalizados, no se mostrarán. Sólo se muestran las indicaciones del sistema. Los filtros personalizados siempre se muestran.

## Ver un informe almacenado en caché

Es posible que el informe se almacene en caché si se ha mostrado en el explorador durante un tiempo. Puede forzar que un informe almacenado en caché se vuelva a cargar cuando realice cualquiera de las siguientes acciones:

* Edite la configuración del informe y guárdelo.
* Cambiar la vista, el grupo o el filtro.
* Haga clic en el **icono Recargar**
Esta opción está disponible en la esquina superior derecha de la página, dentro del cuadro de mensaje que indica la hora en que se guardó el informe, o bien está disponible en la esquina superior derecha del panel en el que se coloca el informe. Para obtener más información acerca de cómo volver a cargar los paneles, vea la sección &quot;Mostrar paneles&quot; en el artículo [Introducción a los paneles](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* Para acceder a cualquier página del informe que no sea la primera página, vaya a las pestañas Resumen, Matriz o Gráfico.
