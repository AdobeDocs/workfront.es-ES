---
title: Visualización de la actividad por equipo en Análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualización Actividad por equipo muestra las actividades que se producen durante un intervalo de tiempo específico para un equipo de casa, lo que le permite comprender cómo los distintos equipos de casa pasaron su tiempo en Adobe Workfront. En función de cómo esté configurado el equipo de inicio en Workfront, esta visualización puede ofrecerle diferentes perspectivas y responder a preguntas diferentes.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Visualización de la actividad por equipo en Análisis mejorado

La visualización Actividad por equipo muestra las actividades que se producen durante un intervalo de tiempo específico para un equipo de casa, lo que le permite comprender cómo los distintos equipos de casa pasaron su tiempo en Adobe Workfront. En función de cómo esté configurado el equipo de inicio en Workfront, esta visualización puede ofrecerle diferentes perspectivas y responder a preguntas diferentes.

>[!NOTE]
>
>La visualización de actividad del proyecto es similar a esta visualización, pero muestra la actividad en función de las personas asignadas a proyectos en lugar de las personas asignadas a un equipo local.\
>Para obtener información sobre la visualización de la actividad del proyecto, consulte [Ver la visualización de la actividad del proyecto en Análisis mejorado](../enhanced-analytics/project-activity-overview.md).

![](assets/activity-by-team-350x113.png)

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plan de Workfront</a>*</td> 
   <td> <p>Negocios o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre las licencias de Adobe Workfront</a>*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso a Proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso.<br>Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Vista</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Para conocer los requisitos previos para usar el análisis mejorado, consulte la sección &quot;Requisitos previos&quot; en [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprender la visualización Actividad por equipo

Las distintas actividades se muestran en colores diferentes para resumir eventos específicos durante el período de tiempo filtrado:

* **Usuarios con sesión iniciada**: Los cuadros morados muestran que las personas del equipo de casa iniciaron sesión ese día. Un tono más oscuro indica un número mayor de personas que inician sesión.

   ![](assets/project-activity-users-logged-in.png)

* **Cambio de estado de la tarea**: Los cuadros rosas muestran que las personas del equipo de casa cambiaron el estado de una tarea ese día. Un sombreado más oscuro indica que se ha cambiado un número mayor de estados de tarea.

   ![](assets/project-activity-task-status-changes.png)

* **Tareas completadas**: Los cuadros azules muestran que las personas del equipo de casa completaron una tarea ese día. Un tono más oscuro indica un número mayor de tareas que se están completando.

   ![](assets/project-activity-tasks-completed.png)

Al pasar el ratón por encima de un cuadro, se muestra la cantidad exacta de veces que la acción se completó en un día determinado. Puede seleccionar un equipo para ver un desglose de estas actividades por cada persona del equipo de inicio.

Ver esta información le ayuda a determinar:

* Qué actividades están ocurriendo dentro de un equipo doméstico y a qué ritmo.
* ¿Qué equipos domésticos se están sobrecargando de trabajo o están utilizando más el sistema?
* Si la distribución del trabajo es adecuada para el equipo de origen.

Para obtener información sobre cómo obtener los mejores datos para esta visualización, consulte [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualización de la actividad por equipo

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png)y, a continuación, seleccione **Analytics**.
1. En el panel izquierdo, seleccione **People**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Opcional) Para utilizar un intervalo de fechas diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fechas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fechas, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Si no ha establecido el filtro Equipo , agregue el filtro Equipo y seleccione cada equipo para el que desee ver los datos.

   Para obtener más información sobre la adición de filtros en Análisis mejorado, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de agregar filtros, se muestran datos de hasta 50 proyectos y los filtros permanecen activos incluso después de abandonar la página o cerrar la sesión de Workfront.

1. (Opcional) Para acercar un intervalo de fechas, seleccione un punto en la visualización para el inicio del intervalo de fechas y arrastre hasta el final del intervalo de fechas.

   Todas las demás visualizaciones se actualizan al mismo intervalo de fechas y se crea un filtro de intervalo de tiempo.

   ![](assets/timeframe-filter-350x220.png)

1. Haga clic en un nombre de equipo

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   para ver más detalles sobre las actividades completadas por el equipo principal.

   La lista se expande para mostrar las actividades de cada persona asignada al equipo principal.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. Pase el ratón sobre un cuadro de color para ver la fecha en la que los usuarios completaron una acción, así como el número de veces que se completó la acción ese día.

   Los colores más oscuros indican una mayor actividad.

   ![](assets/activity-by-team-activity-pop-up-350x155.png)

1. (Opcional) Para exportar los datos de visualización, haga clic en el icono Exportar ![](assets/export.png) en la esquina superior derecha de la visualización, seleccione el formato de exportación:

   * **Gráfico (PNG)**
   * **Tabla de datos (XSLX)**

