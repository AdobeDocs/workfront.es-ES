---
title: Vea la visualización Actividad por equipo en el análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualización Actividad por equipo muestra las actividades que se producen durante un lapso de tiempo específico para un equipo en casa, lo que le permite comprender cómo los distintos equipos en casa invierten su tiempo en Adobe Workfront. Según la configuración de su equipo de inicio en Workfront, esta visualización puede ofrecerle diferentes perspectivas y responder a diferentes preguntas.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 59e021aa3ae66e4fc8d9ce9eb57616f948e6cd90
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 37%

---

# Vea la visualización Actividad por equipo en el análisis mejorado

>[!IMPORTANT]
>
>El análisis mejorado se eliminará de Workfront la semana del 26 de mayo. Workfront Data Connect es una nueva solución alternativa que se puede utilizar para replicar las visualizaciones de Analytics mejoradas que utilice actualmente. <br>Consulte la guía de [Desaprobación mejorada de Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) para obtener más información.



<!-- Audited: 12/2023 -->

La visualización Actividad por equipo muestra las actividades que se producen durante un lapso de tiempo específico para un equipo en casa, lo que le permite comprender cómo los distintos equipos en casa invierten su tiempo en Adobe Workfront. Según la configuración de su equipo de inicio en Workfront, esta visualización puede ofrecerle diferentes perspectivas y responder a diferentes preguntas.

>[!NOTE]
>
>La visualización de la actividad del proyecto es similar a esta visualización, pero muestra la actividad en función de las personas asignadas a proyectos, en lugar de las personas asignadas a un equipo de inicio.\
>Para obtener información sobre la visualización de la actividad del proyecto, consulte [Ver la visualización de la actividad del proyecto en el análisis mejorado](../enhanced-analytics/project-activity-overview.md).

![Actividad por equipo](assets/activity-by-team-350x113.png){width="700"}

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Plan de Workfront</a></td> 
   <td> <p>Business o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre licencias de Adobe Workfront</a></td> 
   <td>
      <p>Nuevo:</p> 
         <ul><li>Light o superior</li></ul>
      <p>Actual:</p>
         <ul><li>Revisión o superior</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Ver acceso a proyectos</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para conocer los requisitos previos para usar el análisis mejorado, consulte la sección “Requisitos previos” en [Información general de Análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprender la visualización Actividad por equipo

Las diferentes actividades se muestran en diferentes colores para resumir eventos específicos durante el período de tiempo filtrado:

* **Usuarios que iniciaron sesión**: Los cuadros morados muestran que las personas del equipo de inicio iniciaron sesión ese día. Un tono más oscuro indica un número mayor de personas que iniciaron sesión.

  ![Usuarios que iniciaron sesión](assets/project-activity-users-logged-in.png)

* **Cambio de estado de la tarea**: los cuadros rosas muestran que las personas del equipo de inicio cambiaron el estado de una tarea en ese día. Un sombreado más oscuro indica que se ha cambiado un número mayor de estados de tarea.

  ![Cambios de estado de la tarea](assets/project-activity-task-status-changes.png)

* **Tareas completadas**: Los cuadros azules muestran que las personas del equipo de inicio completaron una tarea ese día. Un tono más oscuro indica que se está completando un número mayor de tareas.

  ![Tareas completadas](assets/project-activity-tasks-completed.png)

Al pasar el puntero por encima de una casilla, se muestra el número exacto de veces que se completó la acción en un día determinado. Puede seleccionar un equipo para ver un desglose de estas actividades por cada persona del equipo de inicio.

Ver esta información le ayuda a determinar lo siguiente:

* Qué actividades se están produciendo dentro de un equipo local y a qué ritmo.
* Qué equipos de inicio están sobrecargados de trabajo o están usando más el sistema.
* Si la distribución del trabajo es adecuada para el equipo local.

Para obtener los mejores datos para esta visualización, consulte [Información general sobre el Análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualización de la actividad por equipo

1. Haga clic en el icono del menú principal ![icono del menú principal](assets/main-menu-icon-16x12.png) y, a continuación, seleccione **Analytics**.
1. En el panel izquierdo, seleccione **Personas**.

   ![Área de personas](assets/people-area-cropped-qs-350x276.png)

1. (Opcional) Para utilizar un intervalo de fecha diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fecha.

   ![Seleccionar intervalo de fecha](assets/filters-select-date-range-350x344.png)

   Para obtener más información sobre el uso del filtro de intervalo de fecha, consulte [Aplicar filtros en el Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Si no ha establecido el filtro Equipo, agregue el filtro Equipo y seleccione cada equipo cuyos datos desee ver.

   Para obtener más información sobre cómo añadir filtros en Análisis mejorado, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de añadir filtros, se muestran los datos de hasta 50 proyectos y los filtros permanecen activos incluso después de salir de la página o cerrar la sesión de Workfront.

1. (Opcional) Para acercar un intervalo de fecha, seleccione un punto en la visualización para el inicio del intervalo de fecha y arrastre hasta el final del intervalo de fecha.

   Todas las demás visualizaciones se actualizan al mismo intervalo de fecha y se crea un filtro de periodo de tiempo.

   ![Filtro de período de tiempo](assets/timeframe-filter-350x220.png)

1. Haga clic en un nombre de equipo

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   para ver más detalles de las actividades completadas por el equipo de inicio.

   La lista se expande para mostrar las actividades de cada persona asignada al equipo de inicio.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. Pase el ratón sobre un cuadro de color para ver la fecha en la que los usuarios completaron una acción, así como el número de veces que la acción se completó ese día.

   Los colores más oscuros indican una mayor actividad.

   ![Actividad por equipo](assets/activity-by-team-activity-pop-up-350x155.png)

1. (Opcional) Para exportar los datos de visualización, haga clic en el icono Exportar ![Icono de exportación](assets/export.png) en la esquina superior derecha de la visualización y, a continuación, seleccione el formato de exportación:

   * **Gráfico (PNG)**
   * **Tabla de datos (XLSX)**

