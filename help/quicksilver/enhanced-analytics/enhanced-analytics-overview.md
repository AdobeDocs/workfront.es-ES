---
title: Resumen de análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: El análisis mejorado es una potente herramienta en Adobe Workfront con visualizaciones prediseñadas que le permite ver los datos del proyecto e identificar tendencias con planificación y finalización. Esta perspectiva de los proyectos le ayuda a administrar su trabajo actual y le permite planificar con mayor precisión para el trabajo futuro.
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 2%

---

# Resumen de análisis mejorado

El análisis mejorado es una potente herramienta en Adobe Workfront con visualizaciones prediseñadas que le permite ver los datos del proyecto e identificar tendencias con planificación y finalización. Esta perspectiva de los proyectos le ayuda a administrar su trabajo actual y le permite planificar con mayor precisión para el trabajo futuro.

Los análisis mejorados pueden ayudarle a identificar:

* La forma en que planifica los proyectos
* Cuándo se agrega trabajo a los proyectos
* La cantidad de trabajo que se está realizando para diferentes proyectos
* Cantidad de horas o días necesarios para completar un proyecto en comparación con las horas o días en los que está programado un equipo local
* La frecuencia con la que los usuarios completan acciones específicas durante un proyecto
* El progreso de los proyectos, así como las tareas individuales dentro de un proyecto

![](assets/nwe-full-screen-analytics-350x222.png)

Para ver casos de uso o obtener más información sobre la administración del trabajo actual y la planificación para el trabajo futuro con Análisis mejorado, consulte [Rutas de aprendizaje de análisis mejoradas](https://one.workfront.com/s/enhanced-analytics-program).

## Requisitos previos

Para acceder al área de Análisis mejorado , debe:

* Tener un plan empresarial o empresarial.

   Para obtener más información, consulte [Planes de Workfront](https://www.workfront.com/plans).

* Pida al administrador de Workfront que añada Análisis mejorado a la plantilla de diseño.

   Para obtener más información, consulte [Análisis mejorado: Adición de análisis a plantillas de diseño](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

Para ver información sobre proyectos y tareas, debe:

* Tenga permiso de vista para las áreas Proyectos y tareas del nivel de acceso.

   Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte [Crear o modificar niveles de acceso personalizados](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Tener permiso Ver para tareas y/o proyectos específicos.

   Para obtener información sobre la solicitud de acceso adicional, consulte [Solicitar acceso a objetos](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## Prácticas recomendadas para análisis mejorado

Para obtener los mejores datos de sus proyectos, utilice plantillas que tengan horas planificadas y días de duración precisos. También debe asegurarse de que los usuarios introduzcan y actualicen los campos siguientes con la mayor precisión posible.

>[!NOTE]
>
>Algunos de los campos siguientes son cálculos que Workfront realiza en función de la información que introducen los usuarios. Estos campos no se pueden actualizar manualmente.

* Horas planificadas

   Este es el campo más importante que se debe rellenar.

   >[!NOTE]
   >
   >Si sus equipos no utilizan horas planificadas, aún puede ver algunos datos en función de la duración del proyecto.\
   >Para obtener más información, consulte la sección [Vista de duración](#duration-view) en este artículo.

* Nombre del proyecto

   El nombre debe ser descriptivo del proyecto.

* Condición del proyecto
* Estado del proyecto
* Fecha de inicio planeada para el proyecto
* Fecha planificada de finalización
* Fecha de inicio real del proyecto
* Fecha de finalización real del proyecto
* Duración del proyecto: horas
* Horas reales del proyecto
* Estado de la tarea (incluye las tareas de marcado completadas).
* Nombre de la tarea
* Porcentaje de tarea completado
* Fecha de inicio planeada para la tarea
* Fecha planificada de finalización de la tarea

>[!IMPORTANT]
>
>Los cambios realizados en tareas y proyectos pueden tardar hasta 24 horas en reflejarse en Análisis mejorado.

## Vista de duración {#duration-view}

De forma predeterminada, las visualizaciones de diagrama de flujo y de proyecto se basan en horas planificadas. Si sus equipos no utilizan horas planificadas, puede ver estas visualizaciones en función de la duración del proyecto.

En Análisis mejorado, la duración de un proyecto se calcula mediante las siguientes fórmulas:

* Plazo de tiempo planificado:

   ```
   Planned Completion Date of the project - Start Date of the project
   ```

* Días trabajados:

   ```
   Planned Duration for tasks completed in the selected date range / Typical hours per work day
   ```

   >[!NOTE]
   >
   >8 horas es el número predeterminado de **Horas habituales por día laborable**. Un administrador de Adobe Workfront puede actualizar el **Horas habituales por día laborable** configurar en **Configuración** > **Preferencias de proyecto** > **Proyectos** > **Líneas de tiempo**.\
   >Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para obtener información sobre la duración prevista, consulte [Descripción general de la duración del proyecto](../manage-work/projects/planning-a-project/project-duration.md).

## Métodos abreviados del teclado

Puede utilizar las siguientes teclas del teclado para desplazarse o completar acciones específicas en el área Análisis mejorado :

| Clave | Acción |
|---|---|
| **Ficha** | Vaya a cada elemento de la página, así como a una tabla con información sobre cada visualización que no se muestre en la página |
| **Entrar** | Abra el widget de calendario, elimine un filtro existente, abra las opciones de adición de filtro, seleccione o anule la selección de valores de filtro, aplique un filtro que haya creado, abra las opciones de exportación de cada visualización, abra los menús desplegables en las visualizaciones Desglose, Tareas en vuelo y Resumen de proyectos |
| **Teclas de flecha** | Vaya a las fechas en el widget de calendario, mediante las opciones de filtro al agregar un filtro y a través de las opciones de todos los menús desplegables de las visualizaciones |
| **Barra espaciadora** | Seleccione fechas en el widget de calendario, seleccione un tipo de filtro al añadir un filtro, seleccione una opción de exportación en el menú desplegable de cada visualización y seleccione opciones en los menús desplegables de las visualizaciones Desglose, Tareas en vuelo y Resumen del proyecto |

{style=&quot;table-layout:auto&quot;}

Si utiliza software de lectura de pantalla o un complemento, el lector de pantalla lee en voz alta la información de la pantalla y describe las acciones que está realizando al utilizar las claves enumeradas anteriormente.

## Vistas y funciones de análisis mejoradas

Para obtener más información sobre los detalles de una función específica dentro de Análisis mejorado, las acciones que puede completar para obtener más información y lo que puede aprender de estos datos, consulte los siguientes artículos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Artículo</th> 
   <th>Explicación</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Aplicar filtros en Análisis mejorado</a> </td> 
   <td> <p>Puede aplicar filtros personalizados, filtros de campo de proyecto o filtros de equipo para ver solo los proyectos que se ajustan a criterios específicos. A medida que agrega filtros, el número de proyectos se actualiza según corresponda.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">Comprender los KPI de análisis mejorados</a> </td> 
   <td> <p>Los indicadores clave de rendimiento (KPI) para todos los proyectos dentro de un lapso de tiempo específico se encuentran en la parte superior de la pantalla.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">Visualización del plan de vuelo en Análisis mejorado</a> </p> </td> 
   <td> <p>La variable <b>Plan de vuelo</b> visualización muestra que la condición ha cambiado durante la vida de un proyecto. La interacción con la visualización proporciona más detalles sobre fechas específicas. Al seleccionar un proyecto, se abren las visualizaciones Desglosar y Tareas en vuelo.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">Visualización de la visualización de Desglose en Análisis mejorado</a> </td> 
   <td> <p>La variable <b>Descarga</b> la visualización muestra la velocidad planeada de un proyecto en comparación con la cantidad real de horas invertidas en un proyecto. La interacción con la visualización proporciona más detalles sobre la condición del proyecto en una fecha específica.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">Ver las tareas en la visualización de vuelo en Análisis mejorado</a> </td> 
   <td> <p>La variable <b>Tareas en vuelo</b> la visualización muestra el estado de cada tarea dentro de un proyecto. La interacción con la visualización le permite realizar cambios rápida y fácilmente en una tarea.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">Ver la visualización de la actividad del proyecto en Análisis mejorado</a> </td> 
   <td> <p>La variable <b>Actividad del proyecto</b> la visualización muestra un mapa de calor del momento en que los usuarios asignados a un proyecto iniciaron sesión en Workfront, cambiaron el estado de la tarea en ese proyecto y completaron las tareas de ese proyecto. La interacción con la visualización le permite ver estos detalles para cada usuario. También puede ver fechas específicas para estas acciones, así como el número de veces que se completó cada acción.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">Ver la visualización del diagrama de árbol del proyecto en Análisis mejorado</a> </td> 
   <td> <p>La variable <b>Gráfico de árbol del proyecto</b> la visualización muestra cuánto tiempo se ha invertido en algunos proyectos en comparación con otros. La interacción con la visualización le proporciona detalles sobre la condición del proyecto, la finalización del proyecto planificada y la finalización real del proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">Visualización de la actividad por equipo en Análisis mejorado</a> </td> 
   <td> <p>La variable <b>Actividad por equipo</b> la visualización muestra un mapa de calor del momento en que los usuarios de un equipo doméstico iniciaron sesión en Workfront, cambiaron el estado de una tarea y completaron una tarea. La interacción con la visualización le permite ver estos detalles para cada usuario individual. También puede ver fechas específicas para estas acciones, así como el número de veces que se completó cada acción.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">Visualización de la capacidad de los recursos en Análisis mejorado</a> </td> 
   <td> <p>La variable <b>Capacidad de los recursos</b> la visualización le muestra qué equipos domésticos tienen la capacidad de realizar más trabajo y qué equipos domésticos tienen más trabajo asignado del que pueden completar. La interacción con la visualización le permite ver más detalles sobre el trabajo completado y las horas disponibles para trabajar más. Al seleccionar un equipo, se abre la visualización Capacidad del equipo .</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">Ver la visualización de capacidad del equipo en Análisis mejorado</a> </td> 
   <td> <p>La variable <b>Capacidad del equipo</b> la visualización muestra un porcentaje del trabajo que un equipo doméstico ha completado de la cantidad de trabajo que se le ha asignado. La interacción con la visualización le permite ver las horas programadas y las horas planificadas para una fecha específica, así como el porcentaje de capacidad y si el equipo de casa terminó, estaba por debajo o a su capacidad en ese día.</p> </td> 
  </tr> 
 </tbody> 
</table>
