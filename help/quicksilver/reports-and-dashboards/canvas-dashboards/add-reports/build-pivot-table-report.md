---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Creación de un informe de tabla dinámica en un panel de lienzo
description: Puede agregar un informe de tabla dinámica a un panel de lienzo para ver los totales agregados de los datos en formato de tabla.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 58c5f4a08b2083d7350c19b6c1d8383fa0dbb124
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 9%

---

# Creación de un informe de tabla dinámica en un panel de lienzo

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Contacto con el servicio de asistencia al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform

Puede agregar un informe de tabla dinámica a un panel de lienzo para ver los totales agregados de los datos, como sumas, recuentos y promedios, en formato de tabla. Las tablas dinámicas son útiles cuando se comparan varios valores agregados o recuentos frente a varias dimensiones.

![Ejemplo de informe de tabla dinámica](assets/pivot-table-example.png)

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

Debe crear un tablero para poder crear un informe de tabla dinámica. Para obtener más información, consulte [Crear un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Creación de un informe de tabla dinámica en un panel de lienzo

Hay muchas opciones de configuración disponibles para crear un informe de tabla dinámica. En esta sección, le guiaremos a través del proceso general de creación de uno.

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de lienzo** y, a continuación, haga clic en el nombre del panel al que desee agregar el informe.

1. Haga clic en **Agregar informe** en la esquina superior derecha de la página.

1. En el cuadro **Agregar informe**, seleccione **Crear informe**.

1. En el lado izquierdo, seleccione **Tabla dinámica**.

1. En la esquina superior derecha, haga clic en **Crear informe**.

1. (Opcional) Siga los pasos a continuación para configurar la sección **Detalles**:

   1. Elija **Entidad raíz** para el informe.

      >[!NOTE]
      >
      > La entidad raíz establece el objeto del que provienen los campos. Una vez seleccionados, todos los selectores de campo que utilice más adelante en este informe parten de ese objeto, por lo que puede ir directamente al campo que desee.


   1. Escriba un informe **Nombre**.

   1. Escriba un informe **Descripción**.

   1. (Opcional) En el campo **Ejecutar este informe con los derechos de acceso de**, empiece a escribir el nombre del usuario cuyos permisos desea que utilice el informe y, a continuación, seleccione el usuario cuando aparezca en la lista. Cuando configura un informe para que se ejecute como otro usuario, todos los visualizadores del tablero ven los mismos datos, independientemente de su propio nivel de acceso. Si no selecciona ningún usuario, cada usuario verá los datos en función de sus propios permisos.

      >[!IMPORTANT]
      >
      >Si el usuario seleccionado está desactivado o pierde el acceso a los espacios de trabajo o tipos de registro relevantes, el informe puede mostrar datos incompletos o no procesarse.

1. Siga los pasos a continuación para configurar la sección **Métricas**:

   1. En el panel izquierdo, haga clic en el icono **Mostrar métricas** ![Generar icono de KPI](assets/build-kpi-icon.png).

   1. Haga clic en **Agregar métrica** y, a continuación, seleccione el campo que desee. El campo aparece como una columna en la sección de vista previa a la derecha.

      >[!NOTE]
      >
      > Una métrica (también denominada medida) es un campo numérico que desea sumar o sumar. Por ejemplo, puede sumar todos los costos o contar cuántas tareas hay.


   1. Escriba una **etiqueta de columna**.

   1. En la lista desplegable **Tipo de agregación**, seleccione cómo se acumulan los datos para ese campo. Las opciones de este campo varían según el tipo de campo seleccionado.

   1. Repita los dos pasos anteriores para cada métrica que desee agregar.

1. Siga los pasos a continuación para configurar la sección **Segmentos**:

   1. En el panel izquierdo, haga clic en el icono **Segmentos** ![Icono de grupo de desglose](assets/drilldown-group-icon.png).

   1. Haga clic en **Agregar segmento** y, a continuación, seleccione el segmento que desee. El campo aparece como una columna en la sección de vista previa a la derecha.

      >[!NOTE]
      >
      >Un segmento es la categoría que utiliza para agrupar los datos, como las tareas de agrupación por estado o por propietario. Así es como se ordenan y totalizan sus métricas.


   1. Repita los dos pasos anteriores para añadir hasta dos segmentos.

1. Siga los pasos a continuación para configurar la sección **Filter**:

   1. En el panel izquierdo, haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png).

   1. Seleccione **Editar filtro**.

   1. Haga clic en **Agregar condición** y, a continuación, especifique el campo por el que desea filtrar y el modificador que define qué tipo de condición debe cumplir el campo.

   1. (Opcional) Haga clic en **Añadir grupo de filtros** para añadir otro conjunto de criterios de filtrado. El operador predeterminado entre los conjuntos es Y. Haga clic en el operador para cambiarlo a OR.

1. Siga los pasos a continuación para configurar la sección **Configuración de columna detallada**:

   1. En el panel izquierdo, haga clic en el icono **Columnas de desglose** ![Columnas de desglose](assets/drilldown-column.png).

   1. Haga clic en **Agregar columna** y, a continuación, seleccione el campo que desee mostrar como columna en la tabla de desglose. Repita este proceso para cada columna que desee agregar.

1. Haga clic en **Guardar** para crear el informe y agregarlo al tablero.

## Crear un ejemplo de informe de tabla dinámica

En esta sección, explicaremos los pasos para crear un informe de tabla dinámica que resuma los datos de finalización de las tareas.

{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de lienzo** y, a continuación, haga clic en el nombre del panel al que desee agregar el informe.

1. Haga clic en **Agregar informe** en la esquina superior derecha de la página.

1. En el cuadro **Agregar informe**, seleccione **Crear informe**.

1. En el lado izquierdo, seleccione **Tabla dinámica**.

1. En la esquina superior derecha, haga clic en **Crear informe**.

1. Siga los pasos a continuación para configurar la sección **Detalles**:

   1. Elija **Tarea** como **Entidad raíz**.
   1. Escriba *Tareas planificadas en comparación con horas reales por portafolio y proyecto* en el campo **Nombre**.
   1. Escriba una descripción en el campo **Descripción**.

1. Siga los pasos a continuación para configurar la sección **Métricas**:

   1. En el panel izquierdo, haga clic en el icono **Mostrar métricas** ![Generar icono de KPI](assets/build-kpi-icon.png).
   1. Haga clic en **Agregar métrica** y luego seleccione **Nombre**. Escriba *Task count* en el campo **Column label**. En el menú desplegable **Tipo de agregación**, seleccione **Recuento**.
   1. Haga clic en **Agregar métrica** y luego seleccione **Horas reales**. Escriba *Horas reales* en el campo **Etiqueta de columna**. En la lista desplegable **Tipo de agregación**, seleccione **Suma**.
   1. Haga clic en **Agregar métrica** y luego seleccione **Horas planificadas**. Escriba *Total de horas planificadas* en el campo **Etiqueta de columna**. En la lista desplegable **Tipo de agregación**, seleccione **Suma**.

1. Siga los pasos a continuación para configurar la sección **Segmentos**:

   1. En el panel izquierdo, haga clic en el icono **Segmentos** ![Icono de grupo de desglose](assets/drilldown-group-icon.png).
   1. Haga clic en **Agregar segmento** y luego seleccione **Proyecto** > **Portfolio** > **Nombre**.
   1. Haga clic en **Agregar segmento** y luego seleccione **Proyecto** > **Nombre**.

1. Siga los pasos a continuación para configurar la sección **Filter**:

   1. En el panel izquierdo, haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png).
   1. Seleccione **Editar filtro** y luego **Agregar condición**.
   1. Haga clic en el filtro de condición vacío y luego haga clic en **Elegir un campo**.
   1. Seleccione **Estado**.
   1. Cambie el operador a **Equal** y luego elija *in progress*.

1. Siga los pasos a continuación para configurar la sección **Configuración de columna detallada**:

   1. En el panel izquierdo, haga clic en el icono **Columnas de desglose** ![Columnas de desglose](assets/drilldown-column.png).
   1. Haga clic en **Agregar columna** y luego seleccione **Nombre**.
   1. Haga clic en **Agregar columna** y luego seleccione **Asignado a** > **Nombre**.
   1. Haga clic en **Agregar columna** y luego seleccione **Fecha planificada de finalización**.

1. Haz clic en **Guardar** en la esquina superior derecha de la pantalla.

## Consideraciones al crear un informe de tabla dinámica

### Informes con datos financieros

Los usuarios con acceso de Vista o Edición en los datos financieros en su nivel de acceso seguirán viendo los datos financieros en las visualizaciones del Panel de lienzo, incluso si el permiso de Ver finanzas se elimina en el nivel de tarea o proyecto.

* Los usuarios sin derechos de datos financieros en el nivel de acceso no verán los datos financieros en los informes.
* Los usuarios que sí ven los datos financieros se limitan a registros para los que ya tienen permiso de visualización (proyectos, tareas, problemas, etc.). No verán los valores financieros de los registros a los que no pueden acceder.
* Los creadores de informes deben tener cuidado al incluir datos financieros en los paneles y tener en cuenta con quién los comparten para evitar el acceso no deseado.

Se trata de un límite conocido y tenemos previsto abordarlo en el futuro.

### Uso del selector de campos

La lista desplegable **Secciones** de la sección **Generar tabla dinámica** está diseñada para reducir las opciones de un selector de campo y facilitar la búsqueda de un objeto al crear un informe de tabla dinámica. Para empezar, debe seleccionar un objeto de entidad base.

* **Todas las secciones**: Todos los tipos de objetos en Workfront y Workfront Planning.
* **Objetos Workfront**: objetos Workfront nativos.
* **Tipos de registros de planificación**: tipos de registros personalizados definidos en Workfront Planning.

![Lista desplegable de secciones](assets/sections-dropdown.png)

Una vez seleccionado el objeto de entidad base, la lista desplegable **Secciones** se actualiza con las opciones de tipo de campo aplicables para elegir.

* **Todas las secciones**: campos nativos, campos personalizados y objetos relacionados.
* **Todos los campos**: campos nativos y personalizados (excluye relaciones).
* **Campos personalizados**: campos definidos por el cliente en un formulario personalizado o en un registro de Planning.
* **Campos de Workfront**: Solo campos nativos.
* **Relaciones**: Registros conectados.

![Selección de objetos de informe](assets/reportable-objects-selection.png)

### Referencia a objetos relacionados

Limitamos el acceso a la selección de objetos secundarios como segmentos de una tabla dinámica. Las opciones de segmentos pueden ser atributos del registro en sí o de otros registros relacionados que no representen una relación de 1:many o de varios:many.

También limitamos el acceso a la referencia a cualquier atributo principal o secundario como métrica para reducir el potencial de recuento doble o resumen doble de valores, lo que conduce a una representación incorrecta de los datos reales.

