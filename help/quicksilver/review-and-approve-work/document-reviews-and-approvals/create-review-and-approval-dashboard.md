---
product-area: documents
navigation-topic: approvals
title: Crear un panel de revisión y aprobación
description: Puede revisar las métricas de aprobaciones en los paneles del lienzo.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 48f8605b-c342-493b-96e7-f73248e34b35
source-git-commit: 0b4884d6c9a88c096b15af65a2aff0a54ca66811
workflow-type: tm+mt
source-wordcount: '2520'
ht-degree: 1%

---

# Creación de un tablero de informes para revisión y aprobaciones

Puede crear un tablero de informes en el área de Paneles de lienzo para mostrar información de alto nivel y detallada acerca de las revisiones y aprobaciones con la funcionalidad de Aprobaciones unificadas.

>[!IMPORTANT]
>
>Esta funcionalidad solo está disponible para clientes que utilizan el servicio de aprobaciones unificadas e inscritos en la versión beta de paneles de lienzo. Para obtener más información, consulte [Información beta de paneles de lienzo](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).


![tablero de ejemplo](assets/whole-dashboard.png)

## Creación de un panel

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de lienzo**.
1. Haga clic en **Nuevo panel**.
1. Asigne un nombre al tablero.
1. (Opcional) Añada una descripción.
1. Haga clic en **Crear**.
   ![agregar nombre y descripción de panel](assets/create-a-dashboard.png)

Una vez creado un panel, puede empezar a agregar KPI, gráficos y tablas. Consulte las secciones siguientes para obtener más información:

* [Agregar información de revisión y aprobación de alto nivel con KPI y gráficos](#add-high-level-review-and-approval-information-with-kpis-and-charts)
* [Agregar información detallada de revisión y aprobación con tablas](#add-detailed-review-and-approval-information-with-tables)

## Agregar información de revisión y aprobación de alto nivel con KPI y gráficos

Puede ver información de alto nivel sobre aprobaciones de documentos con KPI y gráficos.

Para obtener más información, consulte [Generar un informe de KPI](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md) y [Crear un informe de gráfico](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

### KPI

![ejemplos de KPI](assets/kpi-dashboard.png)

#### Aprobaciones pendientes

1. [Cree un tablero](#create-a-dashboard) tal como se describe en la sección anterior.
1. En la esquina superior derecha de la página de detalles del panel, haga clic en **Agregar informe**.

1. En el cuadro **Agregar informe**, seleccione **Crear informe**.

1. En el lado izquierdo, seleccione **KPI**.

1. En la esquina superior derecha, haga clic en **Crear informe**.

1. Siga los pasos a continuación para configurar la sección **Detalles**:

   1. Escriba *Pending* en el campo **Name**.
   1. Escriba *aprobaciones pendientes* en el campo **Descripción**. Esto se muestra como un pie de ilustración debajo del valor de KPI.

1. Siga los pasos a continuación para configurar la sección **Generar KPI**:

   1. En el panel izquierdo, haga clic en el **KPI de compilación** ![icono de KPI de compilación](assets/build-kpi-icon.png).

   1. Haga clic en **Seleccionar campo**.

   1. Busque y seleccione la carpeta **Aprobación de documento**.

   1. Seleccione **Estado**.

   1. En el menú desplegable **Tipo de agregación**, seleccione **Recuento**.

1. Siga los pasos a continuación para configurar la sección **Filter**:

   1. En el panel izquierdo, haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png).

   1. Seleccione **Editar filtro**.

   1. Haga clic en **Agregar condición**.

   1. Haga clic en el filtro de condición vacío, haga clic en **Elegir un campo** y, a continuación, elija **Estado**.
   1. Deje el operador como **Equal** y, a continuación, escriba _pending review_ en el cuadro de texto.
      ![ejemplo de filtro kpi pendiente](assets/pending-kpi-filter.png)
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.


#### Aprobaciones vencidas

1. [Cree un tablero](#create-a-dashboard) tal como se describe en la sección anterior.
1. En la esquina superior derecha de la página de detalles del panel, haga clic en **Agregar informe**.

1. En el cuadro **Agregar informe**, seleccione **Crear informe**.

1. En el lado izquierdo, seleccione **KPI**.

1. En la esquina superior derecha, haga clic en **Crear informe**.

1. Siga los pasos a continuación para configurar la sección **Detalles**:

   1. Escriba _Vencido_ en el campo **Nombre**.
   1. Escriba _Plazo límite de la fase de aprobación en el último_ en el campo **Descripción**. Esta descripción se muestra como un pie de ilustración debajo del valor de KPI.

1. Siga los pasos a continuación para configurar la sección **Generar KPI**:

   1. En el panel izquierdo, haga clic en el **KPI de compilación** ![icono de KPI de compilación](assets/build-kpi-icon.png).

   1. Haga clic en **Seleccionar campo**.

   1. Busque y seleccione la carpeta **Aprobación de documento**.

   1. Seleccione **Estado**.

   1. En el menú desplegable **Tipo de agregación**, seleccione **Recuento**.

1. Siga los pasos a continuación para configurar la sección **Filter**:

   1. En el panel izquierdo, haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png).

   1. Seleccione **Editar filtro**.

   1. Haga clic en **Agregar condición**.

   1. Haga clic en el filtro de condición vacío y luego haga clic en **Elegir un campo**.

   1. Seleccione **Fase de aprobación** > **Plazo**.
   1. Cambie el operador a **Less Than**.
   1. Cambie **Establecer fecha relativa** en **EL** y, a continuación, escriba _$$HOY_ en el cuadro de texto.
      ![ejemplo de filtro de kpi vencido](assets/overdue-kpi-filter.png)
   1. Haga clic en **Agregar condición**.
   1. Haga clic en el filtro de condición vacío y luego haga clic en **Elegir un campo**.
   1. Seleccione **Estado**.
   1. Cambie el operador a **No contiene** y, a continuación, escriba _aprobado_ en el cuadro de texto.
      ![ejemplo de filtro kpi vencido 2](assets/overdue-kpi-filter-2.png)
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.


#### Aprobaciones completadas


1. [Cree un tablero](#create-a-dashboard) tal como se describe en la sección anterior.
1. En la esquina superior derecha de la página de detalles del panel, haga clic en **Agregar informe**.

1. En el cuadro **Agregar informe**, seleccione **Crear informe**.

1. En el lado izquierdo, seleccione **KPI**.

1. En la esquina superior derecha, haga clic en **Crear informe**.

1. Siga los pasos a continuación para configurar la sección **Detalles**:

   1. Escriba _Completed_ en el campo **Name**.
   1. Escriba _Recuento de estado de aprobación_ en el campo **Descripción**. Esta descripción se muestra como un pie de ilustración debajo del valor de KPI.

1. Siga los pasos a continuación para configurar la sección **Generar KPI**:

   1. En el panel izquierdo, haga clic en el **KPI de compilación** ![icono de KPI de compilación](assets/build-kpi-icon.png).

   1. Haga clic en **Seleccionar campo**.

   1. Busque y seleccione la carpeta **Aprobación de documento**.

   1. Seleccione **Estado**.

   1. En el menú desplegable **Tipo de agregación**, seleccione **Recuento**.

1. Siga los pasos a continuación para configurar la sección **Filter**:

   1. En el panel izquierdo, haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png).

   1. Seleccione **Editar filtro**.

   1. Haga clic en **Agregar condición**.

   1. Haga clic en el filtro de condición vacío y luego haga clic en **Elegir un campo**.

   1. Seleccione **Estado**.

   1. Cambie el operador a **Contains** y escriba _approved_ en el cuadro de texto.
      ![ejemplo de filtro kpi completado](assets/completed-kpi-filter.png)
   1. Haga clic en **Agregar condición**.
   1. Haga clic en **Y** para cambiarlo a **O**.
   1. Haga clic en el filtro de condición vacío y luego haga clic en **Elegir un campo**.
   1. Seleccione **Estado**.
   1. Cambie el operador a **Equal** y, a continuación, escriba _review_ en el cuadro de texto.
      ![ejemplo de filtro kpi completado](assets/completed-kpi-filter-2.png)
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.

#### Aprobaciones abandonadas

1. [Cree un tablero](#create-a-dashboard) tal como se describe en la sección anterior.
1. En la esquina superior derecha de la página de detalles del panel, haga clic en **Agregar informe**.

1. En el cuadro **Agregar informe**, seleccione **Crear informe**.

1. En el lado izquierdo, seleccione **KPI**.

1. En la esquina superior derecha, haga clic en **Crear informe**.

1. Siga los pasos a continuación para configurar la sección **Detalles**:

   1. Escriba _Abandonado_ en el campo **Nombre**.
   1. Escriba _Plazo de aprobación de más de 2 semanas después de_ en el campo **Descripción**. Esta descripción se muestra como un pie de ilustración debajo del valor de KPI.

1. Siga los pasos a continuación para configurar la sección **Generar KPI**:

   1. En el panel izquierdo, haga clic en el **KPI de compilación** ![icono de KPI de compilación](assets/build-kpi-icon.png).

   1. Haga clic en **Seleccionar campo**.

   1. Busque y seleccione la carpeta **Fase de aprobación del documento**.

   1. Seleccione **Plazo**.

   1. En el menú desplegable **Tipo de agregación**, seleccione **Recuento**.

1. Siga los pasos a continuación para configurar la sección **Filter**:

   1. En el panel izquierdo, haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png).

   1. Seleccione **Editar filtro**.

   1. Haga clic en **Agregar condición**.

   1. Haga clic en el filtro de condición vacío y luego en **Elegir un campo**.

   1. Seleccione **Estado**.

   1. Cambie el operador a **No contiene** y escriba _aprobado_ en el cuadro de texto.
      ![ejemplo de filtro kpi abandonado](assets/abandoned-kpi-filter.png)
   1. Haga clic en **Agregar condición**.
   1. Haga clic en el filtro de condición vacío y luego haga clic en **Elegir un campo**.
   1. Seleccione **Plazo**.
   1. Cambie el operador a **Less Than** y luego cambie **Set relative date** a **ON**.
   1. Escriba _$$TODAY-2w_ en el cuadro de texto.
      ![ejemplo de filtro kpi abandonado](assets/abandoned-kpi-filter-2.png)
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.

### Gráficos

![Ejemplos de gráficos](assets/chart-dashboard.png)

#### Gráfico de barras de decisión de aprobaciones

1. [Cree un tablero](#create-a-dashboard) tal como se describe en la sección anterior.
1. En la esquina superior derecha de la página de detalles del panel, haga clic en **Agregar informe**.

1. En el cuadro **Agregar informe**, seleccione **Crear informe**.

1. En el lado izquierdo, seleccione **Gráfico**.

1. En la esquina superior derecha, haga clic en **Crear informe**.

1. Siga los pasos a continuación para configurar la sección **Detalles**:

   1. Escriba _Aprobaciones por decisión_ en el campo **Nombre**.
   1. (Opcional) Escriba una descripción en el campo **Descripción**. Este texto se muestra como información de objeto junto al nombre del gráfico.
1. Siga los pasos a continuación para configurar la sección **Gráfico de generación**:

   1. En el panel izquierdo, haga clic en el icono **Crear gráfico** ![Crear gráfico](assets/build-chart-icon.png).

   1. En el menú desplegable **Tipo de gráfico**, deje seleccionado **Barra**.
   1. En el menú desplegable **Tipo de barra**, deje seleccionado **Simple**.
   1. Haga clic en **Actualizar campo** para el **eje inferior (X)** y, a continuación, seleccione **Aprobación de documento** > **Estado**.
   1. Establezca **Aggregation type** en **Count**.
   1. Haga clic en **Actualizar campo** para el **eje izquierdo (Y)** y, a continuación, seleccione **Estado**.
1. Siga los pasos a continuación para configurar la sección **Filter**:
   1. En el panel izquierdo, haga clic en el icono **Filtrar** ![icono de ficha de filtro](assets/filter-tab.png).
   1. Haga clic en **Editar filtro** y luego en **Agregar condición**.
   1. Haga clic en el filtro de condición vacío y luego haga clic en **Elegir un campo**.
   1. Seleccione **Versión del documento** > **Versión**.
   1. Cambiar el operador a **No es nulo**.
      ![ejemplo de filtro](assets/approvals-by-decision-chart-filter.png)
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.


#### Gráfico de barras de revisiones

1. [Cree un tablero](#create-a-dashboard) tal como se describe en la sección anterior.
1. En la esquina superior derecha de la página de detalles del panel, haga clic en **Agregar informe**.

1. En el cuadro **Agregar informe**, seleccione **Crear informe**.

1. En el lado izquierdo, seleccione **Gráfico**.

1. En la esquina superior derecha, haga clic en **Crear informe**.

1. Siga los pasos a continuación para configurar la sección **Detalles**:

   1. Escriba _Revisiones_ en el campo **Nombre**.
   1. Escriba _Número de revisiones de documentos con decisiones incompletas planeadas antes de que finalice este mes_ en el campo **Descripción**. Este texto se muestra como información de objeto junto al nombre del gráfico.

1. Siga los pasos a continuación para configurar la sección **Gráfico de generación**:

   1. En el panel izquierdo, haga clic en el icono **Crear gráfico** ![Crear gráfico](assets/build-chart-icon.png).

   1. En el menú desplegable **Tipo de gráfico**, deje seleccionado **Barra**.
   1. En el menú desplegable **Tipo de barra**, deje seleccionado **Simple**.
   1. Haga clic en **Actualizar campo** para el **eje inferior (X)** y, a continuación, seleccione **Aprobación de documento** > **Versión de documento** > **Versión**.
   1. Establezca **Aggregation type** en **Count**.
   1. Haga clic en **Actualizar campo** para el **eje izquierdo (Y)** y, a continuación, seleccione **Aprobación de documento** > **Versión de documento** > **Documento** > **Nombre**.

1. Siga los pasos a continuación para configurar la sección **Filter**:
   1. En el panel izquierdo, haga clic en el icono **Filtrar** ![icono de ficha de filtro](assets/filter-tab.png).
   1. Haga clic en **Editar filtro** y luego en **Agregar condición**.
   1. Haga clic en el filtro de condición vacío y luego haga clic en **Elegir un campo**.

   1. Seleccione **fase de aprobación** > **participantes en la fase de aprobación** > **Fecha de decisión**.

   1. Cambie el operador a **Is Null**.
      ![ejemplo de filtro de gráfico de revisiones](assets/revision-chart-filter.png)
   1. Haga clic en **Agregar condición**.
   1. Haga clic en el filtro de condición vacío y luego haga clic en **Elegir un campo**.
   1. Seleccione **Fase de aprobación** > **Plazo**.
   1. Cambie el operador a **Menor o igual que**, luego cambie **Establecer fecha relativa** a **ON**.
   1. Escriba _$$TODAYem_ en el cuadro de texto.
      ![Ejemplo de filtro de gráfico de revisiones](assets/revision-chart-filter-2.png)
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.

## Agregar información detallada de revisión y aprobación con tablas

Para obtener más información sobre cómo generar un informe de tabla, consulte [Generar un informe de tabla](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

![ejemplo de tabla](assets/table-dashboard.png)

### Lista de aprobaciones pendientes

1. [Cree un tablero](#create-a-dashboard) tal como se describe en la sección anterior.
1. En la esquina superior derecha de la página de detalles del panel, haga clic en **Agregar informe**.

1. En el cuadro **Agregar informe**, seleccione **Crear informe**.

1. En el lado izquierdo, seleccione **Tabla**.

1. En la esquina superior derecha, haga clic en **Crear informe**.

1. Siga los pasos a continuación para configurar la sección **Detalles**:

   1. Escriba _aprobaciones pendientes_ en el campo **Nombre**.
   1. Escriba una descripción en el campo **Descripción**. Este texto se muestra como información de objeto junto al nombre del gráfico.

1. Siga los pasos a continuación para configurar la sección **Generar tabla**:

   1. En el panel izquierdo, haga clic en el icono **Columnas de tabla** ![Icono de columnas de tabla](assets/drilldown-column.png).
   1. Haga clic en **Agregar columna**.
   1. Desplácese hacia abajo y seleccione **Aprobaciones de documentos** > **Estado**.
   1. Añada las siguientes columnas:

   <table>
    <tr>
    <td><strong>Nombre del proyecto</strong></td>
    <td>Versión del documento &gt; Documento &gt; Proyecto &gt; Nombre</td>
    </tr>
    <tr>
    <td><strong>Nombre de documento</strong></td>
    <td>Versión del documento &gt; Documento &gt; escriba <em>Nombre</em> en el cuadro de búsqueda.</td>
    </tr>
    <tr>
    <td><strong>Versión del documento</strong></td>
    <td>Versión del documento &gt; Documento &gt; Versión</td>
    </tr>
    <tr>
    <td><strong>Fecha límite</strong></td>
    <td>Aprobación de documento &gt; Fase de aprobación &gt; Plazo</td>
    </tr>
    <tr>
    <td><strong>Solicitado por</strong></td>
    <td>Aprobación de documento &gt; Fase de aprobación &gt; Participantes en la fase de aprobación* &gt; Solicitante &gt; escriba <em>Nombre</em> en el cuadro de búsqueda.</td>
    </tr>
    <tr>
    <td><strong>Fecha de solicitud</strong></td>
    <td>Aprobación de documento &gt; Fase de aprobación &gt; Participantes de fase de aprobación* &gt; Creado en</td>
    </tr>
    <tr>
    <td><strong>Aprobador</strong></td>
    <td>Aprobación de documento &gt; Fase de aprobación &gt; Participantes en la fase de aprobación* &gt; Usuario participante &gt; escriba <em>Nombre</em> en el cuadro de búsqueda.</td>
    </tr>
    </table>


   *Los participantes de la fase de aprobación se truncan a _fase de aprobación Pa.._


1. Siga los pasos a continuación para configurar la sección **Filter**:
   1. En el panel izquierdo, haga clic en el icono **Filtrar** ![icono de ficha de filtro](assets/filter-tab.png).
   1. Haga clic en **Editar filtro** y luego en **Agregar condición**.
   1. Haga clic en el filtro de condición vacío y luego haga clic en **Elegir un campo**.
   1. Seleccione **Estado**.
   1. Cambie el operador a **Equal** y, a continuación, escriba _pending approval_ en el cuadro de texto.
      ![ejemplo de filtro de tabla de aprobación pendiente](assets/pending-approval-table-filter.png)
   1. (Opcional) Agregue filtros adicionales como se describe en la sección **Filtros opcionales** a continuación.
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.


**Filtros opcionales**

Para ver información más específica según el caso de uso, puede añadir condiciones de filtro adicionales. Es posible que desee volver a crear la tabla y agregar nuevas condiciones de filtro por caso de uso.

+++ Expandir para ver opciones de filtro adicionales

**Mis proyectos**

1. Haga clic en **Editar filtro** > **Agregar condición**:
   1. Haga clic en el filtro de condición vacío y luego haga clic en **Elegir un campo**.
   1. Seleccione **Versión del documento** > **Documento** > **Proyecto** > **Propietario** > escriba _Nombre_ en el cuadro de búsqueda.
   1. Cambie el operador a **Equal** y, a continuación, elija **Me (Logged in user)** para mostrar los proyectos en Workfront donde esté marcado como propietario del proyecto.
      ![ejemplo de filtro de tabla de aprobación pendiente](assets/pending-approvals-my-project-filter.png)
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.

**Aprobaciones enviadas**

1. Haga clic en **Editar filtro** > **Agregar condición**:
   1. Haga clic en el filtro de condición vacío y luego en **Elegir un campo**.
   1. Seleccione **Fase de aprobación** > **Participantes en la fase de aprobación** > **Solicitante** > escriba _Nombre_ en el cuadro de búsqueda.
   1. Cambie el operador a **Equal** y, a continuación, elija **Me (Logged in user)** para mostrar los proyectos en Workfront donde esté marcado como propietario del proyecto.
      ![ejemplo de filtro de tabla de aprobación pendiente](assets/pending-approvals-my-project-filter.png)
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.

+++

### Lista de aprobaciones vencidas

1. [Cree un tablero](#create-a-dashboard) tal como se describe en la sección anterior.

1. En la esquina superior derecha de la página de detalles del panel, haga clic en **Agregar informe**.

1. En el cuadro **Agregar informe**, seleccione **Crear informe**.

1. En el lado izquierdo, seleccione **Tabla**.

1. En la esquina superior derecha, haga clic en **Crear informe**.

1. Siga los pasos a continuación para configurar la sección **Detalles**:

   1. Escriba _aprobaciones vencidas_ en el campo **Nombre**.
   1. (Opcional) Escriba una descripción en el campo **Descripción**. Este texto se muestra como información de objeto junto al nombre del gráfico.

1. Siga los pasos a continuación para configurar la sección **Generar tabla**:

   1. En el panel izquierdo, haga clic en el icono **Columnas de tabla** ![Icono de columnas de tabla](assets/drilldown-column.png).
   1. Haga clic en **Agregar columna**.
   1. Desplácese hacia abajo y seleccione **Aprobaciones de documentos** > **Estado**.
   1. Añada las siguientes columnas:

      <table>
        <tr>
        <td><strong>Nombre del proyecto</strong></td>
        <td>Versión del documento &gt; Documento &gt; Proyecto &gt; Nombre</td>
        </tr>
        <tr>
        <td><strong>Nombre de documento</strong></td>
        <td>Versión del documento &gt; Documento &gt; escriba <em>Nombre</em> en el cuadro de búsqueda.</td>
        </tr>
        <tr>
        <td><strong>Versión del documento</strong></td>
        <td>Versión del documento &gt; Documento &gt; Versión</td>
        </tr>
        <tr>
        <td><strong>Fecha límite</strong></td>
        <td>Documento &gt; Fase de aprobación &gt; Plazo</td>
        </tr>
        <tr>
        <td><strong>Solicitado por</strong></td>
        <td>Documento &gt; Fase de aprobación &gt; Participantes en la fase de aprobación* &gt; Solicitante &gt; escriba <em>Nombre</em> en el cuadro de búsqueda.</td>
        </tr>
        <tr>
        <td><strong>Fecha de solicitud</strong></td>
        <td>Documento &gt; Fase de aprobación &gt; Participantes de la fase de aprobación* &gt; Creado en</td>
        </tr>
        <tr>
        <td><strong>Aprobador</strong></td>
        <td>Documento &gt; Fase de aprobación &gt; Participantes en la fase de aprobación* &gt; Usuario participante &gt; escriba <em>Nombre</em> en el cuadro de búsqueda.</td>
        </tr>
        </table>

      *Los participantes de la fase de aprobación se truncan a _fase de aprobación Pa.._

1. Siga los pasos a continuación para configurar la sección **Filter**:
   1. En el panel izquierdo, haga clic en el icono **Filtrar** ![icono de ficha de filtro](assets/filter-tab.png).
   1. Haga clic en **Editar filtro** y luego en **Agregar condición**.
   1. Haga clic en el filtro de condición vacío y luego haga clic en **Elegir un campo**.
   1. Seleccione **Fase de aprobación** > **Plazo**.
   1. Cambie el operador a **Less than** y luego cambie **Set relative date** a **ON**.
   1. Escriba _$$TODAY_ en el campo de texto.
      ![ejemplo de filtro de tabla de aprobación vencida](assets/overdue-approval.png)
   1. (Opcional) Agregue filtros adicionales como se describe en la sección **Filtros opcionales** a continuación.
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.



**Filtros opcionales**

Para ver información más específica según el caso de uso, puede añadir condiciones de filtro adicionales. Es posible que desee volver a crear la tabla y agregar nuevas condiciones de filtro opcionales por caso de uso.

+++ Expandir para ver opciones de filtro adicionales

**Mis proyectos**

1. Haga clic en **Editar filtro** > **Agregar condición**:
   1. Haga clic en el filtro de condición vacío y luego en **Elegir un campo**.
   1. Seleccione **Versión del documento** > **Documento** > **Proyecto** > **Propietario** > escriba _Nombre_ en el cuadro de búsqueda.
   1. Cambie el operador a **Equal** y, a continuación, elija **Me (usuario conectado)** para mostrar los proyectos en Workfront en los que esté marcado como propietario del proyecto.
      ![ejemplo de filtro de tabla de aprobación pendiente](assets/pending-approvals-my-project-filter.png)
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.

**Aprobaciones enviadas**

1. Haga clic en **Editar filtro** > **Agregar condición**:
   1. Haga clic en el filtro de condición vacío y luego en **Elegir un campo**.
   1. Seleccione **Fase de aprobación** > **Participantes en la fase de aprobación** > **Solicitante** > escriba _Nombre_ en el cuadro de búsqueda.
   1. Cambie el operador a **Equal** y, a continuación, elija **Me (usuario conectado)** para mostrar los proyectos en Workfront en los que esté marcado como propietario del proyecto.
      ![ejemplo de filtro de tabla de aprobación pendiente](assets/pending-approvals-my-project-filter.png)
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.

**Mi equipo**

1. Haga clic en **Editar filtro** > **Agregar condición**:
   1. Haga clic en el filtro de condición vacío y luego en **Elegir un campo**.
   1. Seleccione **Fase de aprobación** > **Participantes en la fase de aprobación** > **Equipo de participantes** > escriba _Nombre_ en el cuadro de búsqueda.
   1. Cambie el operador a **Equal** y, a continuación, elija **Mis equipos predeterminados (Usuario con sesión iniciada)** o **Mis otros equipos (Usuario con sesión iniciada)** para mostrar los proyectos asignados a su equipo predeterminado o a otros equipos en los que esté.
      ![ejemplo de filtro de tabla de aprobación pendiente](assets/approvals-ive-submitted-filter.png)
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.
+++
