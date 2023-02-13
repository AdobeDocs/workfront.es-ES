---
title: Aplicar filtros en Análisis mejorado
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Los filtros del área Análisis mejorado le ayudan a centrarse en proyectos específicos o en tipos de datos específicos. Los tipos de filtros que utilice pueden darle una perspectiva sobre - EDITE ME.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1501'
ht-degree: 0%

---

# Aplicar filtros en Análisis mejorado

Los filtros del área Análisis mejorado le ayudan a centrarse en proyectos específicos o en tipos de datos específicos. Los tipos de filtros que utiliza pueden darle una perspectiva sobre:

* Proyectos que posee
* Vistas específicas de portafolio o programa
* Indicadores clave de rendimiento para un período de tiempo específico (semana, trimestre, año fiscal)

Puede agregar y eliminar filtros según sea necesario y Adobe Workfront conserva los filtros que aplica aunque cierre la sesión.

## Requisitos de acceso

Para completar esta tarea, debe tener lo siguiente:

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
  *Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">plan de Workfront</a>*</p> </td> 
   <td>Negocios o superior</td> 
  </tr> 
  <tr> 
   <td> <p><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre las licencias de Adobe Workfront</a>*</p> </td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Nivel de acceso*</b> </td> 
   <td> <p>Ver acceso a Proyectos</p> <p>También debe tener acceso de vista a Tareas, Portfolio y Usuarios para ver las opciones específicas del filtro de campo de proyecto.</p> <p>Nota: Si se seleccionan restricciones en la sección Definir restricciones adicionales del cuadro de diálogo Editar nivel de acceso, es posible que no vea toda la información en los filtros o en la página Análisis mejorado después de aplicar el filtro. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><b>Permisos de objeto</b> </p> </td> 
   <td> <p>Vista</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Requisitos previos

Para conocer los requisitos previos para usar el análisis mejorado, consulte [Requisitos previos](../enhanced-analytics/enhanced-analytics-overview.md#prerequi) en [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Cambiar el filtro de intervalo de fechas {#change-the-date-range-filter}

De forma predeterminada, las visualizaciones del área Análisis mejorado muestran datos de los últimos 60 días y de los próximos 15 días. Puede seleccionar un nuevo intervalo de fechas y aplicarlo a todas las visualizaciones del área Análisis mejorado . Si se aleja de la página, el intervalo de fechas predeterminado se aplica la próxima vez que retroceda.

>[!TIP]
>
>También puede utilizar las teclas del teclado para desplazarse, abrir y seleccionar un intervalo de fechas del widget de calendario.\
>Para obtener más información, consulte la [Métodos abreviados del teclado](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) sección del artículo [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

Para seleccionar un nuevo intervalo de fechas:

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png)y, a continuación, seleccione **Analytics**.
1. En la esquina superior derecha de la pantalla, haga clic en el campo de intervalo de fechas para abrir la vista de calendario.
1. Utilice las flechas encima del calendario para localizar el mes de la fecha de inicio y, a continuación, seleccione la fecha de inicio.

   ![](assets/filters-select-date-range-350x344.png)

1. Utilice las flechas encima del calendario para localizar el mes de la fecha de finalización y, a continuación, seleccione la fecha de finalización.
1. (Opcional) Para acercar un intervalo de fechas más pequeño, arrastre el ratón de una fecha específica a otra en una de las visualizaciones.

   Todas las visualizaciones de la pantalla se actualizan para que coincidan con el marco de tiempo seleccionado y aparece un filtro Intervalo de tiempo junto a los filtros existentes. Este filtro no se conserva si se cierra la sesión o se sale del área de análisis mejorado.

   ![](assets/timeframe-filter-350x220.png)

## Añadir un filtro

Puede agregar filtros basados en campos de proyecto predeterminados, campos de formulario personalizado y equipos principales asignados a proyectos.

>[!TIP]
>
>También puede utilizar teclas en el teclado para desplazarse a un nuevo filtro y agregarlo.\
>Para obtener más información, consulte la [Métodos abreviados del teclado](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) sección del artículo [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

* [Añadir un filtro de campo de proyecto](#add-a-project-field-filter)
* [Añadir un filtro de campo de proyecto](#add-a-project-field-filter)
* [Agregar un filtro de equipo](#add-a-team-filter)

### Añadir un filtro de campo de proyecto {#add-a-project-field-filter}

Los filtros de campo de proyecto permiten filtrar los datos de los proyectos y las tareas en función de los valores introducidos en los campos que se incluyen en los proyectos de forma predeterminada.

Están disponibles los siguientes tipos de filtro de campo de proyecto:

| **Proyecto** | Muestra datos solamente de los proyectos seleccionados |
|---|---|
| **Programar** | Muestra datos solamente para proyectos en los programas seleccionados |
| **Portafolio** | Muestra datos solamente para proyectos del portafolio o portafolios seleccionados |
| **Condición** | Muestra datos solo para proyectos que tuvieron las condiciones seleccionadas más recientemente (como objetivo, en riesgo o en problemas) |
| **Estado** | Muestra datos solo de los proyectos que tuvieron los estados seleccionados más recientemente (completo, actual, en espera, cancelado, etc.) |
| **Patrocinador** | Muestra datos solamente para proyectos con los patrocinadores seleccionados |
| **Propietario del proyecto** | Muestra datos solamente para proyectos con los propietarios del proyecto seleccionado |

{style=&quot;table-layout:auto&quot;}

Los filtros de formulario personalizados funcionan de forma diferente. Para obtener más información, consulte [Añadir un filtro de campo de proyecto](#add-a-project-field-filter).

Para agregar un filtro de campo de proyecto:

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png)y, a continuación, seleccione **Analytics**.
1. En la esquina superior izquierda de la pantalla, haga clic en **Agregar filtro** y, a continuación, seleccione el tipo de filtro que desee.

   >[!NOTE]
   >
   >Los distintos tipos de filtro muestran datos diferentes. Solo se puede utilizar un tipo de filtro en un filtro. Después de seleccionarlo, un tipo de filtro no está disponible para usar en otro filtro de campo de proyecto.

1. Busque los valores para los que desee ver los datos introduciendo al menos 3 caracteres de texto en la variable **Buscar** y, a continuación, seleccione cada valor que desee incluir en el filtro.

   Para seleccionar todos los valores actuales, haga clic en **Seleccionar todo**.

   ![](assets/select-filter-value-350x251.png)

1. Después de seleccionar todos los valores deseados, haga clic en **Aplicar filtro**.\
   El recuento de proyectos en la esquina superior derecha de la página se actualiza para reflejar los filtros aplicados.
1. Repita estos pasos para cada filtro que desee agregar.

   A medida que agrega filtros, aparecen datos en las visualizaciones siguientes de hasta 50 proyectos.

   >[!TIP]
   >
   >Para ver los datos de más de 50 proyectos que se muestran de forma predeterminada, puede:
   >
   >   
   >   
   >   * Utilice las flechas de la esquina inferior izquierda para mostrar los 50 proyectos siguientes en esa visualización.\
      >     ![](assets/pagination-350x118.png)
   >   
   >   * Utilice el menú desplegable Ordenar por de una visualización para ver los proyectos en un orden diferente.\
      >     ![](assets/sort-by-menu-350x247.png)


   Para ajustar el intervalo de fechas, consulte [Cambiar el filtro de intervalo de fechas](#change-the-date-range-filter).

### Agregar un filtro de formulario personalizado de proyecto

El tipo de filtro Formulario personalizado le permite filtrar datos para proyectos y tareas en función de los valores introducidos en los campos Formulario personalizado de los proyectos. A diferencia de otros tipos de filtros de análisis mejorados, puede agregar más de un filtro de formulario personalizado. Cada filtro de formulario personalizado contiene valores introducidos únicamente dentro del campo seleccionado en un formulario personalizado específico.

Para agregar un filtro de formulario personalizado:

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png)y, a continuación, seleccione **Analytics**.
1. En la esquina superior izquierda de la pantalla, haga clic en **Agregar filtro** y, a continuación, seleccione **Formulario personalizado**.

   ![](assets/select-custom-form-filter-350x271.png)

1. Busque el formulario personalizado que desee introduciendo al menos 3 caracteres de texto en la variable **Buscar** y, a continuación, seleccione el formulario personalizado.
1. Seleccione el campo que desee y complete una de las siguientes acciones en función del tipo de campo que agregue al filtro:

   >[!NOTE]
   >
   >No todos los tipos de campo Formulario personalizado se pueden agregar a un filtro. Actualmente, Análisis mejorado solo admite los tipos de campo enumerados arriba.

   * **Casilla de verificación**, **lista desplegable** o **botón de radio**: Seleccione cada valor del campo seleccionado que desee incluir en el filtro o haga clic en el botón **Seleccionar todo** casilla de verificación.\
      ![](assets/custom-form-filter-checkbox-350x255.png)

   * **Fecha**: Utilice las flechas para desplazarse a un mes específico y, a continuación, seleccione la fecha en el campo seleccionado que desee incluir en el filtro.\
      ![](assets/custom-form-filter-date-350x348.png)

   * **Texto**: Introduzca el texto dentro del campo seleccionado que desea incluir en el filtro.\
      ![](assets/custom-form-filter-text-350x90.png)

   * **Número**: Introduzca el número dentro del campo seleccionado que desea incluir en el filtro.\
      ![](assets/custom-form-filter-number-350x93.png)

1. Después de introducir o seleccionar los valores para los que desea filtrar, haga clic en **Aplicar filtro**.

   El recuento de proyectos en la esquina superior derecha de la página se actualiza para reflejar los filtros aplicados.

1. Repita estos pasos para cada filtro que desee agregar.

   A medida que agrega filtros, aparecen datos en las visualizaciones siguientes de hasta 50 proyectos.

   >[!TIP]
   >
   >Para ver los datos de más de 50 proyectos que se muestran de forma predeterminada, puede:
   >
   >   
   >   
   >   * Utilice las flechas de la esquina inferior izquierda para mostrar los 50 proyectos siguientes en esa visualización.\
      >     ![](assets/pagination-350x118.png)
   >   
   >   * Utilice el menú desplegable Ordenar por de una visualización para ver los proyectos en un orden diferente.\
      >     ![](assets/sort-by-menu-350x247.png)


   Para ajustar el intervalo de fechas, consulte [Cambiar el filtro de intervalo de fechas](#change-the-date-range-filter).

### Agregar un filtro de equipo {#add-a-team-filter}

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png)y, a continuación, seleccione **Analytics**.
1. En el panel izquierdo, haga clic en **People**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. En la esquina superior izquierda de la pantalla, haga clic en **Agregar filtro** y, a continuación, seleccione **Equipo** filtro.
1. Busque los equipos para los que desea ver los datos introduciendo al menos 3 caracteres de texto en la variable **Buscar** y, a continuación, seleccione cada equipo que desee incluir en el filtro. Para seleccionar todos los equipos, haga clic en **Seleccionar todo**.

   ![](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >Todos los equipos se incluyen como opciones de filtro, independientemente del nivel de acceso.


1. Después de seleccionar todos los equipos que desee, haga clic en **Aplicar filtro**.

   A medida que agrega filtros, los datos se muestran en las visualizaciones siguientes.

   Para ajustar el intervalo de fechas, consulte [Cambiar el filtro de intervalo de fechas](#change-the-date-range-filter).

## Eliminación de un filtro

Puede quitar un filtro en cualquier momento. Si elimina un filtro, no se mostrará la próxima vez que visite el área de Análisis mejorado .

>[!TIP]
>
>También puede utilizar las teclas del teclado para desplazarse hasta un filtro existente y eliminarlo.\
>Para obtener más información, consulte la [Métodos abreviados del teclado](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) sección del artículo [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

Para quitar un filtro:

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png)y, a continuación, seleccione **Analytics**.
1. Si desea eliminar un filtro de trabajo, permanezca en el **Trabajo** .

   O

   Si desea quitar un filtro Personas, seleccione **People** en el panel izquierdo.

1. Busque el filtro deseado y haga clic en el botón **X** para eliminarlo.

   ![](assets/remove-filter-350x213.png)

   El filtro ya no está activo y no se muestra a menos que lo agregue de nuevo.
