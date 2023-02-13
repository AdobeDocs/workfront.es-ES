---
product-area: reporting
navigation-topic: using-built-in-reports
title: Uso de los informes integrados de Adobe Workfront
description: Adobe Workfront tiene una extensa lista de informes integrados que puede utilizar.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2997'
ht-degree: 11%

---

# Uso de los informes integrados de Adobe Workfront

Adobe Workfront tiene una extensa lista de informes integrados que puede utilizar.

Los administradores de Workfront pueden ocultar informes integrados para que los usuarios no tengan acceso a ellos.\
Para obtener más información sobre cómo ocultar informes integrados, consulte [Ocultar informes integrados](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

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
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a filtros, vistas y grupos</p> <p>Ver o tener más acceso a Informes, Tableros y Calendarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe para agregar o editar un filtro en un informe</p> <p>Administrar permisos de un filtro para editarlo en una lista</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Resumen de los informes integrados {#overview-of-built-in-reports}

Puede personalizar un informe integrado y guardarlo como un nuevo informe. Para obtener más información sobre la personalización de informes integrados, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Los siguientes informes incluyen el paquete Workfront . Los informes están disponibles para todos los usuarios que tengan al menos derechos de visualización para los informes integrados en su nivel de acceso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nombre del informe</strong> </th> 
   <th><strong>Descripción del informe</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Costo de portafolio real por programa</td> 
   <td>Informe de proyecto que muestra el costo planeado y el costo real de los proyectos. El informe se agrupa por nombre de programa, se solicita por nombre de Portfolio y contiene un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costo de portafolio real por proyecto</td> 
   <td>Informe de proyecto que muestra el costo planeado y el costo real de los proyectos. El informe se agrupa por nombre del proyecto, lo solicita el nombre del Portfolio y contiene un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio real por programa</td> 
   <td>Informe de proyecto que muestra los ingresos planeados y los ingresos reales de los proyectos. El informe se agrupa por nombre de programa, se solicita por nombre de Portfolio y contiene un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio reales por proyecto</td> 
   <td>Informe de proyecto que muestra los ingresos planeados y los ingresos reales de los proyectos. El informe se agrupa por nombre del proyecto, lo solicita el nombre del Portfolio y contiene un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos reales por compañía</td> 
   <td>Informe de proyecto que muestra los ingresos reales y la empresa de los proyectos. El informe se agrupa por nombre de la empresa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos reales por grupo</td> 
   <td>Informe de proyecto que muestra los ingresos reales y el grupo de los proyectos. El informe se agrupa por Nombre del grupo e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Todas las hojas de horas abiertas</td> 
   <td>Informe de hoja de horas que muestra Hojas de horas abiertas. El informe muestra los campos siguientes: el intervalo de fechas, el nombre del propietario, las horas totales, las horas extraordinarias, el nombre del aprobador y el estado de las hojas de horas.</td> 
  </tr> 
  <tr> 
   <td>Hojas de horas de aprobación (solicitado)</td> 
   <td>Informe de parte de horas que muestra Hojas de horas enviadas o rechazadas con aprobadores. El informe muestra los campos siguientes: el intervalo de fechas, el propietario, las horas totales, las horas extra, el nombre del aprobador y el estado de las hojas de horas. El informe se solicita por: Fecha de inicio del parte de horas, Fecha de finalización del parte de horas, Nombre del aprobador del parte de horas y Nombre de usuario.</td> 
  </tr> 
  <tr> 
   <td>Proyectos en riesgo</td> 
   <td>Informe de proyecto que muestra proyectos actuales y de planificación que tienen una condición de en riesgo o en problemas. El informe muestra los campos siguientes: la descripción, la fecha de finalización planificada, la fecha de finalización prevista, el porcentaje completado, el estado y la prioridad de los proyectos. El informe se agrupa por nombre de Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de facturación por compañía</td> 
   <td>Informe de proyecto que muestra los ingresos de empresa y facturación de los proyectos. El informe se agrupa por nombre de la empresa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de facturación por grupo</td> 
   <td>Informe de proyecto que muestra los ingresos de facturación y el grupo de los proyectos. El informe se agrupa por Nombre del grupo e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de facturación por mes</td> 
   <td>Informe Registro de Facturación que muestra el nombre del proyecto, los ingresos de facturación del proyecto y la fecha de facturación de los registros de facturación. El informe se agrupa por el mes de la fecha de facturación de los registros de facturación e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas resueltos por semana</td> 
   <td>Informe de problemas que muestra la fecha de finalización real de los problemas. El informe se agrupa por la semana de la fecha de finalización real de las emisiones e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas finalizados por semana por usuario</td> 
   <td>Informe de problemas que muestra la fecha de finalización real y las asignaciones de los problemas. El informe se agrupa por el usuario asignado principal y por la semana de la fecha de finalización real de las emisiones, e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos actuales</td> 
   <td>Informe de proyecto que muestra todos los proyectos actuales. El informe muestra los campos siguientes: la descripción, la fecha de finalización planificada, la fecha de finalización prevista, el porcentaje completado, el estado y la prioridad de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Costos por hora por usuario y por mes</td> 
   <td>Un informe de hora de matriz que muestra el número de horas registradas y su coste real. El informe se agrupa por Nombre de propietario y el mes de la fecha de entrada de las horas.</td> 
  </tr> 
  <tr> 
   <td>Horas por usuario</td> 
   <td>Informe de hora que muestra el número de horas registradas. El informe se agrupa por Nombre de propietario e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Horas por usuario y por semana</td> 
   <td>Un informe de hora de matriz que muestra el número de horas registradas en las últimas cuatro semanas y la fecha de entrada de las horas. El informe se solicita mediante la fecha de entrada de las horas y se agrupa por nombre de propietario y el mes de la fecha de entrada de las horas.</td> 
  </tr> 
  <tr> 
   <td>Problemas por estado</td> 
   <td>Informe de problemas que muestra el estado de los problemas. El informe se agrupa por estado de los problemas e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas por estado y proyecto</td> 
   <td>Un informe de problemas de matriz que muestra el estado de los problemas en los proyectos actuales y el nombre del proyecto. El informe se agrupa por Nombre del proyecto y Estado de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Costos de mano de obra contra costos de gastos por portafolio</td> 
   <td>Informe de proyecto que muestra el costo laboral planificado, el costo laboral real, el costo de gastos planeados y el costo real de los proyectos. El informe se agrupa por nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costos de mano de obra contra costos de gastos por programa</td> 
   <td>Informe de proyecto que muestra el costo laboral planificado, el costo laboral real, el costo de gastos planeados y el costo real de los proyectos. El informe se agrupa por nombre de Portfolio y nombre de programa, e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costo planificado de portafolio planificado vs. costo real por proyecto</td> 
   <td>Un informe de proyecto de matriz (datos financieros) que muestra la fecha de asignación, el costo planeado total, el costo real total y la variación de costo total de los proyectos. El informe se agrupa por nombre del proyecto, trimestre y mes de la fecha de asignación.</td> 
  </tr> 
  <tr> 
   <td>Ingresos planificados de portafolio mensual vs. costo real por proyecto</td> 
   <td>Un informe de proyecto de matriz (Datos financieros) que muestra la fecha de asignación, los ingresos planeados totales, los ingresos reales totales y la variación de ingresos totales de los proyectos. El informe se agrupa por nombre del proyecto, trimestre y mes de la fecha de asignación.</td> 
  </tr> 
  <tr> 
   <td>Costos planificados de proyecto mensuales vs. costos reales</td> 
   <td>Un informe de proyecto de matriz (datos financieros) que muestra la fecha de asignación, el costo planeado total, el costo real total y la variación de costo total de los proyectos. El informe se agrupa por nombre del proyecto, trimestre y mes de la fecha de asignación y se solicita por nombre del proyecto.</td> 
  </tr> 
  <tr> 
   <td>Ingresos planificados de proyecto mensuales vs. costos reales</td> 
   <td>Un informe de proyecto de matriz (Datos financieros) que muestra la fecha de asignación, los ingresos planeados totales, los ingresos reales totales y la variación de ingresos totales de los proyectos. El informe se agrupa por nombre del proyecto, trimestre y mes de la fecha de asignación y se solicita por nombre del proyecto.</td> 
  </tr> 
  <tr> 
   <td>Mis documentos</td> 
   <td>Informe de documento que muestra los documentos cargados por el usuario que ha iniciado sesión. El informe muestra los campos siguientes: Nombre del propietario, Fecha de modificación, Tamaño, Recuento de versiones, Origen y Tipo de los documentos.</td> 
  </tr> 
  <tr> 
   <td>Mis favoritos</td> 
   <td>Informe Favoritos que muestra una lista de objetos marcados como favoritos por el usuario que ha iniciado sesión. El informe muestra los campos siguientes: el tipo de objeto y el nombre de los favoritos.</td> 
  </tr> 
  <tr> 
   <td>Mis problemas</td> 
   <td>Informe de problemas que muestra problemas incompletos asignados al usuario que ha iniciado sesión. El informe muestra los campos siguientes: Nombre de origen, Tipo de problema, usuario asignado principal, Fecha de entrada, Estado y Prioridad de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Mis portafolios</td> 
   <td>Informe de Portfolio que muestra Portfolio activos donde el usuario que ha iniciado sesión es el Administrador de Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Mis programas</td> 
   <td>Informe de programa que muestra Programas y su Descripción, donde el usuario que ha iniciado sesión es el Administrador de programas.</td> 
  </tr> 
  <tr> 
   <td>Mis problemas pendientes del proyecto</td> 
   <td>Informe de problemas que muestra problemas incompletos en proyectos cuyo equipo de proyecto incluye al usuario que ha iniciado sesión. El informe muestra los campos siguientes: Nombre de origen, Tipo de problema, usuario asignado principal, Fecha de entrada, Estado y Prioridad de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Mis proyectos</td> 
   <td>Informe de proyecto que muestra los proyectos actuales en los que el equipo de proyecto incluya al usuario que ha iniciado sesión. El informe muestra los campos siguientes: la descripción, la fecha de finalización planificada, la fecha de finalización prevista, el porcentaje completado, el estado y la prioridad de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Mis problemas enviados</td> 
   <td>Informe de problemas que muestra los problemas enviados por el usuario que ha iniciado sesión que se han cerrado en los últimos tres meses o que están abiertos actualmente. El informe muestra los campos siguientes: Nombre de origen, Tipo de problema, Fecha de entrada, Estado y Prioridad de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Mis tareas</td> 
   <td>Informe de tarea que muestra tareas incompletas en Proyectos actuales que están asignadas al usuario que ha iniciado sesión. El informe muestra los campos siguientes: la duración planificada, el nombre del proyecto, el usuario asignado principal, el inicio planificado, la finalización planificada, el porcentaje completado y la prioridad de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Mis hojas de horas</td> 
   <td>Informe de hoja de horas que muestra todas las hojas de horas del usuario que ha iniciado sesión. El informe muestra los campos siguientes: el intervalo de fechas, el nombre del propietario, las horas totales, las horas extraordinarias, el nombre del aprobador y el estado de las hojas de horas.</td> 
  </tr> 
  <tr> 
   <td>Mis problemas sin asignar</td> 
   <td>Informe de problemas que muestra los problemas abiertos asignados a cualquiera de las funciones de trabajo del usuario que ha iniciado sesión y que no están asignados al usuario. El informe muestra los campos siguientes: Nombre de origen, Tipo de problema, Fecha de entrada, Estado y Prioridad de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Mis tareas sin asignación</td> 
   <td>Informe de tarea que muestra tareas incompletas asignadas a cualquiera de las funciones de trabajo del usuario que ha iniciado sesión y que no están asignadas al usuario. El informe muestra los campos siguientes: la duración planeada, el nombre del proyecto, el usuario asignado principal, la fecha de inicio planeada, la fecha de finalización planeada, el porcentaje completado y la prioridad de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Mis próximas tareas</td> 
   <td>Un informe de tareas que muestra tareas incompletas que deberían iniciarse en las dos semanas siguientes, que están en proyectos actuales y que están asignadas al usuario que ha iniciado sesión. El informe muestra los campos siguientes: Nombre del proyecto, Fecha de finalización planificada, Fecha de finalización prevista, Porcentaje completado y Estado de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Abrir hojas de horas (solicitado)</td> 
   <td>Informe de hoja de horas que muestra Hojas de horas abiertas. El informe muestra los campos siguientes: el intervalo de fechas, propietario, horas totales, horas extra, nombre del aprobador, estado de las hojas de horas. El informe se solicita por: Fecha de inicio del parte de horas, Fecha de finalización del parte de horas, Nombre del aprobador del parte de horas y Nombre de usuario.</td> 
  </tr> 
  <tr> 
   <td>Proyecto con presupuesto excedido por portafolio</td> 
   <td>Informe de proyecto que muestra el costo planeado y el costo real de los proyectos. El informe se agrupa por nombre de Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Costo de portafolio planificado por programa</td> 
   <td>Informe de proyecto que muestra el costo planeado y el costo real de los proyectos. El informe se solicita por nombre de Portfolio, se agrupa por nombre de programa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costo de portafolio planificado por proyecto</td> 
   <td>Informe de proyecto que muestra el costo planeado y el costo real de los proyectos. El informe se solicita por nombre de Portfolio, se agrupa por nombre del proyecto e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio planificados por programa</td> 
   <td>Informe de proyecto que muestra los ingresos planeados y los ingresos reales de los proyectos. El informe se solicita por nombre de Portfolio, se agrupa por nombre de programa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio planificados por proyecto</td> 
   <td>Informe de proyecto que muestra los ingresos planeados y los ingresos reales de los proyectos. El informe se solicita por nombre de Portfolio, se agrupa por nombre del proyecto e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costos planificados contra costos reales por portafolio</td> 
   <td>Informe de proyecto que muestra el costo planeado y el costo real de los proyectos por Portfolio. El informe se agrupa por nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costos planificados contra costos reales por programa</td> 
   <td>Informe de proyecto que muestra el costo planeado y el costo real de los proyectos por programa. El informe se agrupa por nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos planificados contra ingresos reales por portafolio</td> 
   <td>Informe de proyecto que muestra los ingresos planeados y los ingresos reales de los proyectos. El informe se agrupa por nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos planificados contra ingresos reales por programa</td> 
   <td>Informe de proyecto que muestra los ingresos planeados y los ingresos reales de los proyectos. El informe se agrupa por Nombre del programa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costos de portafolio agrupados por programa y por mes</td> 
   <td>Un informe de proyecto de matriz que muestra el costo planeado, el costo presupuestado y el costo real de los proyectos. El informe se agrupa por nombre de Portfolio, nombre del programa y mes de la fecha de inicio planeada de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Proyectos de portafolio por estado agrupados por programa</td> 
   <td>Informe de proyecto que muestra el estado de los proyectos. El informe se agrupa por nombre de programa y estado del proyecto, e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos de portafolio agrupados por estado y portafolio</td> 
   <td>Informe de proyecto que muestra el nombre del Portfolio y el estado de los proyectos. El informe se agrupa por nombre de Portfolio y estado de los proyectos, e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio por programa</td> 
   <td>Informe de proyecto que muestra el nombre del Portfolio, el nombre del programa, los ingresos previstos y los ingresos reales de los proyectos. El informe se agrupa por nombre de Portfolio y nombre de programa, e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio agrupados por programa y por mes</td> 
   <td>Un informe de proyecto de matriz que muestra los ingresos planeados, los ingresos reales, el nombre del Portfolio y el nombre del programa. El informe se agrupa por nombre de Portfolio, nombre del programa y mes de la fecha de inicio planeada de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Costos e ingresos de proyecto por estado de tarea</td> 
   <td>Un informe de tarea de matriz que muestra el Coste planeado, Coste real, Ingresos planificados, Ingresos reales y Nombre del proyecto de las tareas. El informe se agrupa por Nombre del proyecto y Estado de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Costos de proyecto contra ingresos por portafolio</td> 
   <td>Informe de proyecto que muestra el nombre del Portfolio, el costo real y los ingresos reales de los proyectos. El informe se agrupa por nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Gastos de proyecto por mes y trimestre</td> 
   <td>Un informe de gastos de matriz que muestra la fecha de entrada, el importe planeado, el importe real y el proyecto de los gastos. El informe se agrupa por nombre del proyecto, trimestre y mes de la fecha de entrada de los gastos.</td> 
  </tr> 
  <tr> 
   <td>Costos por hora de proyecto por tipo de hora y por mes</td> 
   <td>Informe de hora de matriz que muestra los campos siguientes: Horas, Fecha de entrada, Coste real de los proyectos, Tipo de hora, Nombre del proyecto. El informe se agrupa por nombre del proyecto, mes de la fecha de entrada de las horas y tipo de hora.</td> 
  </tr> 
  <tr> 
   <td>Costos de mano de obra y gastos de proyecto por mes y trimestre</td> 
   <td>Un informe de proyecto de matriz que muestra el costo laboral planificado, el costo laboral real, el costo de costo planeado y el costo real de los proyectos. El informe se agrupa por nombre del proyecto y por trimestre y mes de la fecha de inicio real de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Rendimiento del proyecto</td> 
   <td>Un informe de proyecto que muestra los siguientes campos de proyectos actuales: la Fecha de Vencimiento, CPI, SPI, CSI, Coste, Presupuesto, EAC y Gastos de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Solicitudes de proyecto</td> 
   <td>Informe de proyecto que muestra los proyectos solicitados. El informe muestra los campos siguientes: la descripción, la fecha de finalización planificada, la fecha de finalización prevista, el porcentaje completado, el estado y la prioridad de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Proyectos por condición</td> 
   <td>Informe de proyecto que muestra la condición de los proyectos. El informe se agrupa por condición e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos por condición de grupo</td> 
   <td>Informe de proyecto que muestra el estado de progreso y el grupo de los proyectos. El informe se agrupa por Nombre del grupo y Estado de progreso, e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos por prioridad</td> 
   <td>Informe de proyecto que muestra la prioridad de los proyectos. El informe se agrupa por prioridad e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos por estado de progreso</td> 
   <td>Informe de proyecto que muestra el estado de progreso de los proyectos. El informe se agrupa por estado de progreso e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Tareas por estado de progreso</td> 
   <td>Informe de tarea que muestra el estado de progreso de todas las tareas de los proyectos actuales. El informe se agrupa por estado de progreso e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Tareas por estado</td> 
   <td>Informe de tarea que muestra el estado de todas las tareas. El informe se agrupa por estado e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Hojas de horas para revisar</td> 
   <td>Informe de parte de horas que muestra las hojas de horas enviadas y rechazadas cuyo aprobador es el usuario que ha iniciado sesión. El informe muestra los campos siguientes: el intervalo de fechas, propietario, horas totales, horas extra, nombre del aprobador y estado de las hojas de horas.</td> 
  </tr> 
  <tr> 
   <td>Tarea con problemas</td> 
   <td>Informe de tarea que muestra tareas incompletas con un estado de progreso de atrasado o retrasado, una fecha de entrega antes de mañana y donde el usuario que ha iniciado sesión forma parte del equipo de proyecto del proyecto en el que están las tareas. El informe muestra los campos siguientes: Duración planeada, Nombre del proyecto, Usuario asignado principal, Inicio planificado, Finalización planificada, Porcentaje completado y Prioridad de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Inicios de sesión del usuario</td> 
   <td>Informe de usuario que muestra los campos siguientes: ID único, Recuento de inicio de sesión (el número de veces que el usuario ha iniciado sesión desde que se inicia con Workfront) y Fecha de último inicio de sesión de los usuarios. El informe se agrupa por nivel de acceso de los usuarios.</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## Acceso a informes integrados

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.
1. Haga clic en **Informes**.
1. Haga clic en **Todos los informes**.
1. Expanda el **Filtro** menú desplegable y seleccione **Nuevo filtro**.

1. Haga clic en **Agregar una regla de filtro**.
1. En el **Empezar a escribir el nombre del campo** campo, empezar a escribir **ID global**.

1. En el **Informe** objeto, seleccionar **ID global**.

1. En el menú desplegable del modificador de filtro, seleccione **No está en blanco**.\
   ![](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Haga clic en **Guardar filtro**.\
   La lista de informes solo muestra los informes integrados.\
   Para obtener más información sobre los informes integrados disponibles, consulte [Resumen de los informes integrados](#overview-of-built-in-reports).
