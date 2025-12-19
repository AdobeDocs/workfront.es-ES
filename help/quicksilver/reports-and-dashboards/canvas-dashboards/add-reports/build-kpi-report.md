---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Generar un informe de KPI en un panel de control de lienzo
description: Se puede añadir a un panel de control de lienzo un informe de KPI que muestre de forma destacada un único KPI agregado.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: e1c68ac3-112e-4f9e-b644-f44bb0778b92
source-git-commit: d7caaa0871263fb8ef4224a9c298778f3ee2454a
workflow-type: tm+mt
source-wordcount: '1260'
ht-degree: 8%

---

# Generar un informe de KPI en un panel de control de lienzo

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Póngase en contacto con Atención al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform

Puede crear y agregar un informe de KPI a un panel de lienzo que represente visualmente los datos del indicador de rendimiento clave como un número, que puede utilizar para ver el rendimiento de sus proyectos y equipos.

![Ejemplo de informe KPI](assets/kpi-example-main.png)

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
</tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Requisitos previos

Debe crear un tablero para poder generar un informe de KPI.

## Generar un informe de KPI en un panel de control de lienzo

Hay muchas opciones de configuración disponibles para crear un informe de KPI. En esta sección, le guiaremos a través del proceso general de creación de uno.

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.

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
      >La descripción se utilizará como pie de ilustración debajo del valor de KPI. Si no introduce una descripción, se generará un pie de ilustración en función del agregador y el tipo de agregación que seleccione en los pasos siguientes.

1. Siga los pasos a continuación para configurar la sección **Generar KPI**:

   1. En el panel izquierdo, haga clic en el icono **Generar KPI** ![Generar icono de KPI](assets/build-kpi-icon.png).

   1. Haga clic en **Seleccionar campo** y, a continuación, especifique el campo que desee agregar al informe.

   1. En el menú desplegable **Tipo de agregación**, seleccione cómo se acumulan los datos para generar el resultado de KPI. Las opciones de este campo varían en función del tipo de campo seleccionado en el paso anterior.

1. Siga los pasos a continuación para configurar la sección **Filter**:

   1. En el panel izquierdo, haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png).

   1. Seleccione **Editar filtro**.

   1. Haga clic en **Agregar condición** y, a continuación, especifique el campo por el que desea filtrar y el modificador que define qué tipo de condición debe cumplir el campo.

   1. (Opcional) Haga clic en **Agregar grupo de filtros** para agregar otro conjunto de criterios de filtrado. El operador predeterminado entre los conjuntos es Y. Haga clic en el operador para cambiarlo a OR.

      Para obtener más información sobre los filtros, consulte [Editar filtros de informe en un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/edit-report-filters.md).

1. Siga los pasos a continuación para configurar la sección **Configuración de columna detallada**:

   1. En el panel izquierdo, haga clic en el icono **Columnas de desglose** ![Columnas de desglose](assets/drilldown-column.png). Los campos del gráfico aparecen automáticamente como columnas en la sección de vista previa a la derecha.

   1. (Opcional) Para actualizar cualquiera de las configuraciones de columna existentes, seleccione la columna que desee actualizar en la sección **Columnas actuales** y, a continuación, actualice la información que desee (por ejemplo: etiqueta, estado vinculado y reglas de formato).

   1. Haga clic en **Agregar columna** y, a continuación, seleccione el campo que desee mostrar como columna en la tabla. Repita este proceso para cada columna que desee agregar.

1. Siga los pasos a continuación para configurar la sección **Configuración del grupo de desglose**:

   1. En el panel izquierdo, haga clic en el icono **Configuración de grupo** ![Icono de grupo de desglose](assets/drilldown-group-icon.png).

   1. Haga clic en el botón **Agregar agrupación** y, a continuación, seleccione el campo que desee crear como agrupación.

1. Haga clic en **Guardar** para crear el informe y agregarlo al tablero.

## Generar un ejemplo de informe de KPI

En esta sección, explicaremos los pasos para crear un informe KPI que muestre las aprobaciones de documentos pendientes.

Para obtener más información sobre ejemplos de informes KPI, consulte [Crear un tablero de informes para revisión y aprobaciones](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.

1. Haga clic en **Nuevo panel** en la esquina superior derecha.

1. En el cuadro **Crear tablero**, escriba el **Nombre** y la **Descripción** del tablero.

1. Haga clic en **Crear**.

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
      ![Ejemplo de filtro de KPI pendiente](assets/pending-kpi-filter.png)
1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.

## Consideraciones al crear un informe de KPI

### Informes con datos financieros

Los usuarios con acceso de Vista o Edición en los datos financieros en su nivel de acceso seguirán viendo los datos financieros en las visualizaciones del Panel de lienzo, incluso si el permiso de Ver finanzas se elimina en el nivel de tarea o proyecto.

* Los usuarios sin derechos de datos financieros en el nivel de acceso no verán los datos financieros en los informes.
* Los usuarios que sí ven datos financieros se limitan a registros para los que ya tienen permiso de visualización (proyectos, tareas, problemas, etc.). No verán los valores financieros de los registros a los que no pueden acceder.
* Los creadores de informes deben tener cuidado al incluir datos financieros en los paneles y tener en cuenta con quién comparten los paneles para evitar el acceso no deseado.

Se trata de un límite conocido y tenemos previsto abordarlo lo antes posible.

### Uso del selector de campos

La lista desplegable **Secciones** de la sección **Generar KPI** se ha diseñado para reducir las opciones de un selector de campo y facilitar la búsqueda de un objeto al crear un informe de tabla. Para empezar, debe seleccionar un objeto de entidad base.

* **Todas las secciones**: Todos los tipos de objetos en Workfront Workflow y Workfront Planning.
* **Objetos Workfront**: objetos nativos de flujo de trabajo de Workfront.
* **Tipos de registros de planificación**: tipos de registros personalizados definidos en Workfront Planning.

![Lista desplegable de secciones](assets/sections-dropdown.png)

Una vez seleccionado el objeto de entidad base, la lista desplegable **Secciones** se actualiza con las opciones de tipo de campo aplicables para elegir.

* **Todas las secciones**: campos nativos, campos personalizados y objetos relacionados.
* **Todos los campos**: campos nativos y personalizados (excluye relaciones).
* **Campos personalizados**: campos definidos por el cliente en un formulario personalizado o en un registro de Planning.
* **Campos de Workfront**: Solo campos nativos.
* **Relaciones**: Registros conectados.

![Selección de objetos de informe](assets/reportable-objects-selection.png)

### Referencia a objetos secundarios

Las relaciones disponibles para columnas adicionales, opciones de filtro y atributos de agrupación generalmente se limitan a objetos superiores en la jerarquía de objetos de Workfront o tienen una sola selección en el objeto de entidad base del informe. Hay algunas excepciones a este respecto, que incluyen las siguientes:

* Proyecto > Tareas
* Aprobación de documento > Fases de aprobación de documento
* Fases de aprobación de documento > Participantes en la fase de aprobación de documento

Al utilizar cualquiera de las relaciones principal-secundario enumeradas anteriormente, verá una fila en la tabla para cada registro secundario conectado al objeto principal.


