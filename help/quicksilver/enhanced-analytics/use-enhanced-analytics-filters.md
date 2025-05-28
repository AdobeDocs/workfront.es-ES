---
title: Aplicar filtros en Análisis mejorado
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Los filtros del área de Análisis mejorado de Adobe Workfront le ayudan a centrarse en proyectos específicos o tipos específicos de datos.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '1525'
ht-degree: 97%

---

# Aplicar filtros en Análisis mejorado

>[!IMPORTANT]
>
>El análisis mejorado se eliminó de Workfront el 27 de mayo. Workfront Data Connect es una nueva solución alternativa que se puede utilizar para replicar las visualizaciones de Analytics mejoradas que utilice actualmente. <br>Consulte la guía de [Desaprobación mejorada de Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) para obtener más información.


<!-- Audited: 12/2023 -->

Los filtros del área de Análisis mejorado de Adobe Workfront le ayudan a centrarse en proyectos específicos o tipos específicos de datos. Los tipos de filtros que utiliza pueden proporcionarle información sobre lo siguiente:

* Proyecto de su propiedad
* Vistas específicas de portafolios o programas
* Indicadores de rendimiento clave para un lapso de tiempo específico (semana, trimestre, año fiscal)

Puede añadir y eliminar filtros según sea necesario, y Workfront conserva los filtros que aplica aunque cierre la sesión.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>
      <p>Nuevo: cualquiera</p>
      <p>o</p>
      <p>Actual: empresa o superior</p></td> 
  </tr>
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
      <p>Nuevo: Light o superior</p>
      <p>o</p>
      <p>Actual: revisión o superior</p>
   </td> 
  </tr>
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Ver acceso a proyectos</p> <p>También debe tener acceso de visualización a tareas, portafolios y usuarios para ver opciones específicas de filtrado de campos del proyecto.</p> <p>Nota: Si se seleccionan restricciones en la sección <strong>Establecer restricciones adicionales</strong> del cuadro de diálogo Editar nivel de acceso, es posible que no vea toda la información en los filtros o en la página Análisis mejorado después de aplicar el filtro.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permisos de objeto </p> </td> 
   <td> <p>Ver</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para conocer los requisitos previos para usar el análisis mejorado, consulte [Requisitos previos](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites) en [Información general de Análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Cambiar el filtro de intervalo de fechas {#change-the-date-range-filter}

De forma predeterminada, las visualizaciones del área de Análisis mejorado muestran datos de los últimos 60 días y los siguientes 15 días. Puede seleccionar un nuevo intervalo de fecha y aplicarlo a todos los gráficos mientras utiliza el área Análisis mejorado. Si sale de la página, el intervalo de fecha predeterminado se aplica la próxima vez que vuelva a la página.

>[!TIP]
>
>También puede utilizar las teclas del teclado para desplazarse, abrir y seleccionar un intervalo de fecha del widget de calendario.\
>Para obtener más información, consulte la sección [Métodos abreviados de teclado](../enhanced-analytics/enhanced-analytics-overview.md#keyboard-shortcuts) en el artículo [Información general de Análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

Para seleccionar un nuevo intervalo de fecha, haga lo siguiente:

{{step1-to-analytics}}

1. En la parte superior derecha, haga clic en el campo de intervalo de fecha para abrir la vista de calendario.
1. Utilice las flechas situadas encima del calendario para localizar el mes de la fecha de inicio y, a continuación, seleccione la fecha de inicio.

   ![Seleccionar intervalo de fecha](assets/filters-select-date-range-350x344.png)

1. Utilice las flechas situadas encima del calendario para localizar el mes de la fecha de finalización y, a continuación, seleccione la fecha de finalización.
1. (Opcional) Para ampliar un intervalo de fecha más pequeño, arrastre el ratón de una fecha específica a otra en una de las visualizaciones.

   Todas las visualizaciones de la pantalla se actualizarán para que coincidan con el periodo de tiempo seleccionado, y aparecerá un filtro de periodo de tiempo junto a los filtros existentes. Este filtro no se conserva si cierra la sesión o sale del área de Análisis mejorado.

   ![Filtro de período de tiempo](assets/timeframe-filter-350x220.png)

## Añadir un filtro

Puede añadir filtros basados en campos de proyecto predeterminados, campos de formulario personalizados y equipos de inicio asignados a proyectos.

>[!TIP]
>
>También puede utilizar las teclas del teclado para navegar hasta un nuevo filtro y añadirlo.\
>Para obtener más información, consulte la sección [Métodos abreviados de teclado](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) en el artículo [Información general de Análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

* [Añadir un filtro de campo de proyecto](#add-a-project-field-filter)
* [Añadir un filtro de formulario personalizado de proyecto](#add-a-project-custom-form-filter)
* [Añadir un filtro de equipo](#add-a-team-filter)

### Añadir un filtro de campo de proyecto {#add-a-project-field-filter}

Los filtros de campos de proyectos permiten filtrar los datos de los proyectos y de las tareas en función de los valores introducidos en los campos que se incluyen en los proyectos de forma predeterminada.

Están disponibles los tipos de filtros de campos de proyectos siguientes:

| Campo | Datos mostrados |
|---|---|
| **Proyecto** | Muestra datos solo de los proyectos seleccionados |
| **Programa** | Muestra datos solamente de los proyectos en los programas seleccionados |
| **Portafolio** | Muestra datos solamente de los proyectos en los portafolios seleccionados |
| **Condición** | Muestra datos solamente de los proyectos que han tenido recientemente las condiciones seleccionadas (en destino, en riesgo o con problemas) |
| **Estado** | Muestra datos solamente de los proyectos que han tenido los estados seleccionados más recientemente (completado, actual, en espera, cancelado, etc.) |
| **Patrocinador** | Muestra datos solamente de los proyectos con los patrocinadores seleccionados |
| **Propietario del proyecto** | Muestra datos solamente de los proyectos con los propietarios de proyectos seleccionados |

Los filtros de formularios personalizados funcionan de forma diferente. Para obtener más información, consulte [Añadir un filtro de formulario personalizado de proyecto](#add-a-project-custom-form-filter).

Para añadir un filtro de campo de proyecto:

{{step1-to-analytics}}

1. En la parte superior izquierda, haga clic en **Añadir filtro** y luego seleccione el tipo de filtro que desee.

   >[!NOTE]
   >
   >Los distintos tipos de filtros muestran datos diferentes. Solo se puede utilizar un tipo de filtro en un filtro. Tras seleccionarlo, no hay ningún tipo de filtro disponible para usar en otro filtro de campo de proyecto.

1. Busque los valores cuyos datos desea ver escribiendo al menos tres caracteres de texto en el campo **Buscar** y, a continuación, seleccione cada valor que desee incluir en el filtro.

   Para seleccionar todos los valores actuales, haga clic en **Seleccionar todo**.

   ![Seleccionar valor de filtro](assets/select-filter-value-350x251.png)

1. Después de seleccionar todos los valores deseados, haga clic en **Aplicar filtro**.

   El recuento de proyectos en la parte superior derecha se actualiza para reflejar los filtros aplicados.

1. Repita estos pasos para cada filtro que desee añadir.

   A medida que añada filtros, los datos se muestran en las visualizaciones siguientes para un máximo de 50 proyectos.

   >[!TIP]
   >
   >Para ver los datos de más de 50 proyectos que se muestran de forma predeterminada, puede hacer lo siguiente:
   >
   >   * Usar las flechas de la parte inferior izquierda para mostrar los 50 proyectos siguientes en esa visualización.\
   >     ![Flecha de paginación](assets/pagination-350x118.png)
   >   
   >   * Usar el menú desplegable **Ordenar por** de una visualización para ver los proyectos en un orden diferente.\
   >     ![Ordenar por menú](assets/sort-by-menu-350x247.png)

   Para ajustar el intervalo de fecha, consulte [Cambiar el filtro del intervalo de fecha](#change-the-date-range-filter).

### Añadir un filtro de formulario personalizado de proyecto

El tipo de filtro de formulario personalizado permite filtrar los datos de los proyectos y de las tareas en función de los valores introducidos en los campos de formularios personalizados de los proyectos. A diferencia de otros tipos de filtros de análisis mejorado, puede añadir más de un filtro de formulario personalizado. Cada filtro de formulario personalizado contiene valores introducidos solo dentro del campo seleccionado en un formulario personalizado específico.

Para añadir un filtro de formulario personalizado, haga lo siguiente:

{{step1-to-analytics}}

1. En la esquina superior izquierda de la pantalla, haga clic en **Añadir filtro** y, a continuación, seleccione **Formulario personalizado**.

   ![Seleccionar filtro de formulario personalizado](assets/select-custom-form-filter-350x271.png)

1. Busque el formulario personalizado que desee escribiendo al menos tres caracteres de texto en el campo **Buscar** y, a continuación, seleccione el formulario personalizado.
1. Seleccione el campo que desee y, a continuación, complete una de las siguientes acciones en función del tipo de campo que esté añadiendo al filtro:

   >[!NOTE]
   >
   >No todos los tipos de campos de formularios personalizados se pueden añadir a un filtro. Actualmente, el análisis mejorado solo admite los tipos de campo enumerados a continuación.

   * **Casilla de verificación**, **lista desplegable** o **botón de radio**: seleccione cada valor del campo que desee incluir en el filtro o haga clic en la casilla de verificación **Seleccionar todo**.\
     ![Valores de casilla de verificación](assets/custom-form-filter-checkbox-350x255.png)

   * **Fecha**: utilice las flechas para ir a un mes específico y, a continuación, seleccione la fecha en el campo que desee incluir en el filtro.\
     ![Valor de la fecha](assets/custom-form-filter-date-350x348.png)

   * **Texto**: introduzca el texto dentro del campo que desea incluir en el filtro.\
     ![Valor de texto](assets/custom-form-filter-text-350x90.png)

   * **Número**: introduzca el número dentro del campo que desea incluir en el filtro.\
     ![Valor numérico](assets/custom-form-filter-number-350x93.png)

1. Después de especificar o seleccionar los valores que desea filtrar, haga clic en **Aplicar filtro**.

   El recuento de proyectos en la parte superior derecha se actualiza para reflejar los filtros aplicados.

1. Repita estos pasos para cada filtro que desee añadir.

   A medida que añada filtros, los datos se muestran en las visualizaciones siguientes para un máximo de 50 proyectos.

   >[!TIP]
   >
   >Para ver los datos de más de 50 proyectos que se muestran de forma predeterminada, puede hacer lo siguiente:
   >  
   >   * Usar las flechas de la parte inferior izquierda para mostrar los 50 proyectos siguientes en esa visualización.\
   >     ![Flechas de paginación](assets/pagination-350x118.png)
   >   
   >   * Utilice el menú desplegable **Ordenar por** de una visualización para ver los proyectos en un orden diferente.\
   >     ![Ordenar por menú](assets/sort-by-menu-350x247.png)

   Para ajustar el intervalo de fecha, consulte [Cambiar el filtro del intervalo de fecha](#change-the-date-range-filter).

### Añadir un filtro de equipo {#add-a-team-filter}

{{step1-to-analytics}}

1. En el panel izquierdo, haga clic en **Personas**.

   ![Seleccionar personas](assets/people-area-cropped-qs-350x276.png)

1. En la parte superior izquierda de la pantalla, haga clic en **Añadir filtro** y, a continuación, seleccione el filtro **Equipo**.
1. Busque los equipos cuyos datos desea ver escribiendo al menos tres caracteres de texto en el campo **Buscar** y, a continuación, seleccione cada equipo que desee incluir en el filtro. Para seleccionar todos los equipos, haga clic en **Seleccionar todo**.

   ![Seleccionar equipos](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >Todos los equipos se incluyen como opciones de filtro, independientemente del nivel de acceso.

1. Después de seleccionar todos los equipos deseados, haga clic en **Aplicar filtro**.

   A medida que añades filtros, los datos se muestran en las siguientes visualizaciones.

   Para ajustar el intervalo de fecha, consulte [Cambiar el filtro del intervalo de fecha](#change-the-date-range-filter).

## Quitar un filtro

Puede quitar un filtro en cualquier momento. Si quita un filtro, no se mostrará la próxima vez que visite el área de Análisis mejorado.

>[!TIP]
>
>También puede utilizar las teclas del teclado para desplazarse a un filtro existente y quitarlo.\
>Para obtener más información, consulte la sección [Métodos abreviados de teclado](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) en el artículo [Información general de Análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

Para quitar un filtro, haga lo siguiente:

{{step1-to-analytics}}

1. Si desea quitar un campo de proyecto o un filtro de formulario personalizado, permanezca en el área **Trabajo**.

   O

   Si desea quitar un filtro de equipo, seleccione **Personas** en el panel izquierdo.

1. Busque el filtro que desee y haga clic en la **X** para quitarlo.

   ![Quitar](assets/remove-filter-350x213.png)

   El filtro ya no está activo y no se muestra a menos que lo vuelva a añadir.
