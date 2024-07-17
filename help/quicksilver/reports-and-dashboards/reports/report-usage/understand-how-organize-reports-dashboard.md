---
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
title: Obtenga información sobre cómo organizar informes en un tablero
description: Puede ver si un informe se agrega a un panel en Adobe Workfront. Esto puede resultar útil a la hora de decidir qué informes se pueden conservar y cuáles se pueden eliminar del sistema. Si los informes están en los paneles, es posible que los usuarios sigan dependiendo de ellos. Se recomienda no eliminar los informes que se enumeran en los paneles que utilizan los usuarios. Para obtener más información sobre cómo agregar informes a los paneles, consulte el artículo Agregar un informe a un panel.
author: Nolan
feature: Reports and Dashboards
exl-id: ce00c307-9e64-49f5-997b-f7fc461c960c
source-git-commit: d738ef3f6642d5b1a646f58896575a2971bbc06a
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 1%

---

# Obtenga información sobre cómo organizar informes en un tablero

## Acceso a información de tablero en una lista de informes

Puede ver si un informe se agrega a un panel en Adobe Workfront. Esto puede resultar útil a la hora de decidir qué informes se pueden conservar y cuáles se pueden eliminar del sistema. Si los informes están en los paneles, es posible que los usuarios sigan dependiendo de ellos. Se recomienda no eliminar los informes que se enumeran en los paneles que utilizan los usuarios.\
Para obtener más información acerca de cómo agregar informes a los paneles, vea el artículo [Agregar un informe a un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

Puede ver si un informe se agrega a un tablero mediante uno de los procedimientos siguientes:

* Crear una vista para una lista de informes e incluir información del panel en las columnas
* Filtrado de una lista de informes por uno o varios paneles específicos que sabe que se están utilizando activamente
* Creación de un informe para el objeto de informe y uso de una vista o un filtro que incluya información del panel

Cualquiera puede crear una vista o un filtro, pero debe tener acceso de edición a los informes en su nivel de acceso para crear un informe.\
Para obtener más información acerca del acceso a los informes, vea el artículo [Conceder acceso a informes, paneles y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).\
Para obtener más información sobre cómo generar un informe, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Mostrar información de tablero en la lista Vista de un informe

>[!WARNING]
>
>Incluir la columna Paneles en una lista de informes puede aumentar significativamente los tiempos de carga, especialmente en el caso de listas de informes largas.

Para crear una vista con información del tablero para una lista de informes:

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront y luego haga clic en **Informes**.
1. En la lista de informes, haga clic en el menú desplegable **Ver**.
1. Haga clic en **Nueva vista**.
1. Haga clic en **Añadir columna**.
1. Empiece a escribir &quot;Paneles&quot; en el campo **Empiece a escribir el nombre del campo**.
1. En el objeto **Informe**, seleccione **Paneles**.

1. Pulse **Guardar vista**.\
   Los paneles en los que aparece un informe se muestran en la columna Paneles de la lista de informes.\
   ![](assets/qs-dashboards-in-report-view.png)

## Filtrado de una lista de informes por información de panel

Para filtrar una lista de informes por información de panel:

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront y luego haga clic en **Informes**.

1. En la lista de informes, haga clic en el menú desplegable **Filtro**.
1. Haga clic en **Nuevo filtro** y luego haga clic en **Agregar una regla de filtro**.

1. Empiece a escribir &quot;Paneles&quot; en el campo **Empiece a escribir el nombre del campo**.

1. En el objeto **Paneles**, seleccione **Nombre**.

1. Seleccione **Equal** en el menú desplegable de modificadores y, a continuación, empiece a escribir el nombre del panel por el que desea filtrar. Puede seleccionar varios paneles para el filtro.\
   ![](assets/qs-dashboards-in-report-filters-350x143.png)

1. Haga clic en **Guardar + Cerrar**.\
   Esto muestra una lista de informes que solo se enumeran en los paneles especificados.\
   También puede crear un informe para el objeto de informe y utilizar este filtro en el informe.
