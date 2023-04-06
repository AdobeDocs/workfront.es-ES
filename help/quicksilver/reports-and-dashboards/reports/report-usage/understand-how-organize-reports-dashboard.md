---
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
title: Cómo organizar informes en un tablero
description: Puede ver si un informe se agrega a un tablero en Adobe Workfront. Esto puede resultar útil a la hora de decidir qué informes se pueden conservar y cuáles se pueden eliminar del sistema. Si los informes se encuentran en tableros, es posible que los usuarios sigan confiando en ellos. Se recomienda no eliminar los informes que aparecen en los tableros que utilizan los usuarios. Para obtener más información sobre cómo agregar informes a tableros, consulte el artículo Agregar un informe a un tablero .
author: Nolan
feature: Reports and Dashboards
exl-id: ce00c307-9e64-49f5-997b-f7fc461c960c
source-git-commit: d738ef3f6642d5b1a646f58896575a2971bbc06a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Cómo organizar informes en un tablero

## Acceder a la información del tablero en una lista de informes

Puede ver si un informe se agrega a un tablero en Adobe Workfront. Esto puede resultar útil a la hora de decidir qué informes se pueden conservar y cuáles se pueden eliminar del sistema. Si los informes se encuentran en tableros, es posible que los usuarios sigan confiando en ellos. Se recomienda no eliminar los informes que aparecen en los tableros que utilizan los usuarios.\
Para obtener más información sobre cómo agregar informes a tableros, consulte el artículo [Agregar un informe a un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

Puede ver si un informe se agrega a un tablero haciendo una de las siguientes acciones:

* Creación de una vista para una lista de informes e inclusión de información de tablero en las columnas
* Filtrado de una lista de informes por uno o varios tableros específicos que sabe que se están utilizando activamente
* Creación de un informe para el objeto de informe y uso de una vista o un filtro que incluya información del tablero

Cualquier persona puede crear una vista o un filtro, pero debe tener acceso de edición a los informes en el nivel de acceso para crear un informe.\
Para obtener más información sobre el acceso a los informes, consulte el artículo [Conceder acceso a informes, tableros y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).\
Para obtener más información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Mostrar la información del tablero en la Vista de una lista de informes

>[!WARNING]
>
>Incluir la columna Tableros en una lista de informes puede aumentar significativamente los tiempos de carga, especialmente para listas de informes largas.

Para crear una vista con información de tablero para una lista de informes:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Informes**.
1. En la lista de informes, haga clic en el botón **Ver** menú desplegable.
1. Haga clic en **Nueva vista**.
1. Haga clic en **Agregar columna**.
1. Empiece a escribir &quot;Tableros&quot; en la sección **Empezar a escribir el nombre del campo** campo .
1. En el **Informe** objeto, seleccionar **Tableros**.

1. Haga clic en **Guardar vista**.\
   Los tableros en los que aparece un informe se muestran en la columna Tableros de la lista de informes.\
   ![](assets/qs-dashboards-in-report-view.png)

## Filtrar una lista de informes por información del tablero

Para filtrar una lista de informes por información de tablero:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Informes**.

1. En la lista de informes, haga clic en el botón **Filtro** menú desplegable.
1. Haga clic en **Nuevo filtro** y haga clic en **Agregar una regla de filtro**.

1. Empiece a escribir &quot;Tableros&quot; en la sección **Empezar a escribir el nombre del campo** campo .

1. En el **Tableros** objeto, seleccionar **Nombre**.

1. Select **Igual** en el menú desplegable del modificador , empiece a escribir el nombre del tablero por el que desea filtrar. Puede seleccionar varios tableros para el filtro.\
   ![](assets/qs-dashboards-in-report-filters-350x143.png)

1. Haga clic en **Guardar + Cerrar**.\
   Esto muestra una lista de informes que aparecen solo en los tableros especificados.\
   También puede crear un informe para el objeto de informe y utilizar este filtro en el informe.
