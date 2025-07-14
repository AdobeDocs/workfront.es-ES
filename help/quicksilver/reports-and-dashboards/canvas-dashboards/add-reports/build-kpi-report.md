---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Creación de un informe de KPI
description: Se puede añadir a un panel de lienzo un informe de KPI que muestre de forma destacada un único KPI agregado.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: e1c68ac3-112e-4f9e-b644-f44bb0778b92
source-git-commit: ba9256255905e139c281099555a6d129fc570984
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 12%

---

# Creación de un informe de KPI

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Para obtener más información, consulte [Información beta de paneles de lienzo](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

Puede crear y agregar un informe de KPI a un panel de lienzo que represente visualmente los datos del indicador de rendimiento clave como un número, que puede utilizar para ver el rendimiento de sus proyectos y equipos.

![Ejemplo de informe KPI](assets/kpi-example-main.png)

+++ Amplíe para ver los requisitos de acceso.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront</p></td> 
   <td> 
<p>Cualquiera </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td> 
<p>Actual: plan </p> 
<p>Nuevo: estándar</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td> 
   <td><p>Editar el acceso a Informes, Paneles y Calendarios</p>
  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Requisitos previos

Debe crear un tablero para poder generar un informe de KPI.

## Generar un informe de KPI en un panel de lienzo

Hay muchas opciones de configuración disponibles para crear un informe de KPI. En esta sección, le guiaremos a través del proceso general de creación de uno.

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de lienzo**.

1. Haga clic en **Nuevo panel** en la esquina superior derecha.

1. En el cuadro **Crear tablero**, escriba el **Nombre** y la **Descripción** del tablero.

1. Haga clic en **Crear**.

1. En el cuadro **Agregar informe**, seleccione **Crear informe**.

1. En el lado izquierdo, seleccione **KPI**.

1. En la esquina superior derecha, haga clic en **Crear informe**.

1. Siga los pasos a continuación para configurar la sección **Detalles**:

   1. Escriba un informe **Nombre**.
   1. Escriba un informe **Descripción**.

      >[!NOTE]
      > 
      > La descripción se utilizará como pie de ilustración debajo del valor de KPI. Si no introduce una descripción, se generará un pie de ilustración en función del agregador y el tipo de agregación que seleccione en los pasos siguientes.

1. Siga los pasos a continuación para configurar la sección **Generar KPI**:

   1. En el panel izquierdo, haga clic en el icono **Generar KPI** ![Generar icono de KPI](assets/build-kpi-icon.png).

   1. Haga clic en **Seleccionar campo** y, a continuación, especifique el campo que desee agregar al informe.

   1. En el menú desplegable **Tipo de agregación**, seleccione cómo se acumulan los datos para generar el resultado de KPI. Las opciones de este campo varían en función del tipo de campo seleccionado en el paso anterior.

1. Siga los pasos a continuación para configurar la sección **Filter**:

   1. En el panel izquierdo, haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png).

   1. Seleccione **Editar filtro**.

   1. Haga clic en **Agregar condición** y, a continuación, especifique el campo por el que desea filtrar y el modificador que define qué tipo de condición debe cumplir el campo.

   1. (Opcional) Haga clic en **Agregar grupo de filtros** para agregar otro conjunto de criterios de filtrado. El operador predeterminado entre los conjuntos es Y. Haga clic en el operador para cambiarlo a OR.

1. Siga los pasos a continuación para configurar la sección **Configuración de columna detallada**:

   1. En el panel izquierdo, haga clic en el icono **Columnas de desglose** ![Columnas de desglose](assets/drilldown-column.png). Los campos del gráfico aparecen automáticamente como columnas en la sección de vista previa a la derecha.

   1. (Opcional) Para actualizar cualquiera de las configuraciones de columna existentes, seleccione la columna que desee actualizar en la sección **Columnas actuales** y, a continuación, actualice la información que desee (por ejemplo: etiqueta, estado vinculado y reglas de formato).

   1. Haga clic en **Agregar columna** y, a continuación, seleccione el campo que desee mostrar como columna en la tabla. Repita este proceso para cada columna que desee agregar.

1. Siga los pasos a continuación para configurar la sección **Configuración del grupo de desglose**:

   1. En el panel izquierdo, haga clic en el icono **Configuración de grupo** ![Icono de grupo de desglose](assets/drilldown-group-icon.png).

   1. Haga clic en el botón **Agregar agrupación** y, a continuación, seleccione el campo que desee crear como agrupación.

1. Haga clic en **Guardar** para crear el informe y agregarlo al tablero.


