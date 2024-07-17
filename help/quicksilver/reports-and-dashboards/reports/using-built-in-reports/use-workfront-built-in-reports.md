---
product-area: reporting
navigation-topic: using-built-in-reports
title: Uso de informes integrados de Adobe Workfront
description: Adobe Workfront tiene una extensa lista de informes integrados que están listos para usar. Los administradores de Workfront pueden ocultar los informes integrados para que los usuarios no tengan acceso a ellos.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: f2b6f0fb8a24723fec60c6fc1a99e1b8f9cf39c7
workflow-type: tm+mt
source-wordcount: '2953'
ht-degree: 10%

---

# Uso de informes integrados de Adobe Workfront

<!--Audited: 07/2024-->

Adobe Workfront tiene una extensa lista de informes integrados que puede utilizar.

Los administradores de Workfront pueden ocultar los informes integrados para que los usuarios no tengan acceso a ellos.

Para obtener más información acerca de cómo ocultar informes integrados, vea [Ocultar informes integrados](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: Colaborador o superior</p>  
   <p>Actual: Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Acceso de visualización o superior a informes, tableros, calendarios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe para agregar o editar un filtro en un informe</p> <p>Administración de permisos de un filtro para editarlo en una lista</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Información general sobre los informes integrados {#overview-of-built-in-reports}

Puede personalizar un informe integrado y guardarlo como un informe nuevo. Para obtener más información sobre cómo personalizar informes integrados, vea [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Los siguientes informes se incluyen con el paquete Workfront. Los informes están disponibles para todos los usuarios que tengan al menos derechos de visualización de informes integrados en su nivel de acceso.

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
   <td>Informe de proyecto que muestra el costo planificado y el costo real de los proyectos. El informe se agrupa por Nombre de programa, se solicita por Nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costo de portafolio real por proyecto</td> 
   <td>Informe de proyecto que muestra el costo planificado y el costo real de los proyectos. El informe se agrupa por Nombre de proyecto, se solicita por Nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio real por programa</td> 
   <td>Informe de proyecto que muestra los ingresos planificados y los ingresos reales de los proyectos. El informe se agrupa por Nombre de programa, se solicita por Nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio reales por proyecto</td> 
   <td>Informe de proyecto que muestra los ingresos planificados y los ingresos reales de los proyectos. El informe se agrupa por Nombre de proyecto, se solicita por Nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos reales por compañía</td> 
   <td>Informe de proyecto que muestra los ingresos reales y la compañía de los proyectos. El informe se agrupa por Nombre de la empresa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos reales por grupo</td> 
   <td>Informe de proyecto que muestra los ingresos reales y el grupo de los proyectos. El informe se agrupa por nombre de grupo e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Todas las hojas de horas abiertas</td> 
   <td>Informe de hoja de horas que muestra las hojas de horas abiertas. El informe muestra los campos siguientes: Intervalo de fechas, Nombre del propietario, Horas totales, Horas extra, Nombre del aprobador y Estado de las hojas de horas.</td> 
  </tr> 
  <tr> 
   <td>Hojas de horas de aprobación (solicitado)</td> 
   <td>Informe de hoja de horas que muestra las hojas de horas enviadas o rechazadas con los aprobadores. El informe muestra los campos siguientes: Intervalo de fechas, Propietario, Horas totales, Horas extra, Nombre del aprobador y Estado de las hojas de horas. El informe se solicita mediante: Fecha de inicio de la hoja de horas, Fecha de finalización de la hoja de horas, Nombre del aprobador de la hoja de horas y Nombre de usuario.</td> 
  </tr> 
  <tr> 
   <td>Proyectos en riesgo</td> 
   <td>Informe de proyecto que muestra los proyectos actuales y planificados que tienen la condición de en riesgo o con problemas. El informe muestra los campos siguientes: la descripción, la fecha planificada de finalización, la fecha proyectada de finalización, el porcentaje completado, el estado y la prioridad de los proyectos. El informe se agrupa por Nombre de Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de facturación por compañía</td> 
   <td>Informe de proyecto que muestra la compañía y los ingresos de facturación de los proyectos. El informe se agrupa por Nombre de la empresa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de facturación por grupo</td> 
   <td>Informe de proyecto que muestra los ingresos de facturación y el grupo de los proyectos. El informe se agrupa por nombre de grupo e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de facturación por mes</td> 
   <td>Informe de registro de facturación que muestra el nombre del proyecto, los ingresos de facturación del proyecto y la fecha de facturación de los registros de facturación. El informe se agrupa por el mes de la fecha de facturación de los registros de facturación e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas resueltos por semana</td> 
   <td>Informe de problema que muestra la fecha real de finalización de los problemas. El informe se agrupa por la semana de la fecha real de finalización de los problemas e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas finalizados por semana por usuario</td> 
   <td>Informe de problema que muestra la fecha real de finalización y las asignaciones de los problemas. El informe se agrupa por el usuario asignado principal y por la semana de la fecha real de finalización de los problemas e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos actuales</td> 
   <td>Informe de proyecto que muestra todos los proyectos actuales. El informe muestra los campos siguientes: la descripción, la fecha planificada de finalización, la fecha proyectada de finalización, el porcentaje completado, el estado y la prioridad de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Costos por hora por usuario y por mes</td> 
   <td>Informe de hora en matriz que muestra la cantidad de horas registradas y el costo real correspondiente. El informe se agrupa por nombre de propietario y el mes de la fecha de entrada de las horas.</td> 
  </tr> 
  <tr> 
   <td>Horas por usuario</td> 
   <td>Informe de hora que muestra la cantidad de horas registradas. El informe se agrupa por Nombre de propietario e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Horas por usuario y por semana</td> 
   <td>Informe de hora en matriz que muestra la cantidad de horas registradas en las últimas cuatro semanas y la fecha de entrada de las horas. El informe se solicita mediante la fecha de entrada de las horas y se agrupa por nombre de propietario y el mes de la fecha de entrada de las horas.</td> 
  </tr> 
  <tr> 
   <td>Problemas por estado</td> 
   <td>Informe de problema que muestra el estado de los problemas. El informe se agrupa por estado de los problemas e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas por estado y proyecto</td> 
   <td>Informe de problema en matriz que muestra el estado de los problemas de los proyectos actuales y el nombre del proyecto. El informe se agrupa por nombre de proyecto y estado de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Costos de mano de obra contra costos de gastos por portafolio</td> 
   <td>Informe de proyecto que muestra el costo de mano de obra planificado, el costo de mano de obra real, el costo de gasto planificado y el costo de gasto real de los proyectos. El informe se agrupa por Nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costos de mano de obra contra costos de gastos por programa</td> 
   <td>Informe de proyecto que muestra el costo de mano de obra planificado, el costo de mano de obra real, el costo de gasto planificado y el costo de gasto real de los proyectos. El informe se agrupa por nombre de Portfolio y nombre de programa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costo planificado de portafolio planificado vs. costo real por proyecto</td> 
   <td>Informe de proyecto en matriz (datos financieros) que muestra la fecha de asignación, el costo total planificado, el costo real total y la desviación de costo total de los proyectos. El informe se agrupa por nombre de proyecto, trimestre y mes de la fecha de asignación.</td> 
  </tr> 
  <tr> 
   <td>Ingresos planificados de portafolio mensual vs. costo real por proyecto</td> 
   <td>Informe de proyecto en matriz (datos financieros) que muestra la fecha de asignación, los ingresos totales planificados, los ingresos reales totales y la desviación de ingresos totales de los proyectos. El informe se agrupa por nombre de proyecto, trimestre y mes de la fecha de asignación.</td> 
  </tr> 
  <tr> 
   <td>Costos planificados de proyecto mensuales vs. costos reales</td> 
   <td>Informe de proyecto en matriz (datos financieros) que muestra la fecha de asignación, el costo total planificado, el costo real total y la desviación de costo total de los proyectos. El informe se agrupa por nombre de proyecto, trimestre y mes de la fecha de asignación y se le solicita mediante nombre de proyecto.</td> 
  </tr> 
  <tr> 
   <td>Ingresos planificados de proyecto mensuales vs. costos reales</td> 
   <td>Informe de proyecto en matriz (datos financieros) que muestra la fecha de asignación, los ingresos totales planificados, los ingresos reales totales y la desviación de ingresos totales de los proyectos. El informe se agrupa por nombre de proyecto, trimestre y mes de la fecha de asignación y se le solicita mediante nombre de proyecto.</td> 
  </tr> 
  <tr> 
   <td>Mis documentos</td> 
   <td>Informe de documento que muestra los documentos cargados por el usuario que ha iniciado sesión. El informe muestra los campos siguientes: Nombre del propietario, Fecha de modificación, Tamaño, Recuento de versiones, Source y Tipo de los documentos.</td> 
  </tr> 
  <tr> 
   <td>Mis favoritos</td> 
   <td>Informe de favoritos que muestra una lista de los objetos marcados como favoritos por el usuario que ha iniciado sesión. El informe muestra los campos siguientes: Tipo de objeto y Nombre de los favoritos.</td> 
  </tr> 
  <tr> 
   <td>Mis problemas</td> 
   <td>Informe de problema que muestra los problemas no resueltos asignados al usuario que ha iniciado sesión. El informe muestra los campos siguientes: Nombre de Source, Tipo de problema, Usuario asignado principal, Fecha de entrada, Estado y Prioridad de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Mis portafolios</td> 
   <td>Informe de Portfolio que muestra los Portfolio activos en los que el usuario que ha iniciado sesión es el administrador de Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Mis programas</td> 
   <td>Informe de programa que muestra los programas y su descripción en los que el usuario que ha iniciado sesión es el administrador de programas.</td> 
  </tr> 
  <tr> 
   <td>Mis problemas pendientes del proyecto</td> 
   <td>Informe de problema que muestra los problemas no resueltos de los proyectos en los que el equipo de proyecto incluya al usuario que ha iniciado sesión. El informe muestra los campos siguientes: Nombre de Source, Tipo de problema, Usuario asignado principal, Fecha de entrada, Estado y Prioridad de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Mis proyectos</td> 
   <td>Informe de proyecto que muestra los proyectos actuales en los que el equipo de proyecto incluya al usuario que ha iniciado sesión. El informe muestra los campos siguientes: la descripción, la fecha planificada de finalización, la fecha proyectada de finalización, el porcentaje completado, el estado y la prioridad de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Mis problemas enviados</td> 
   <td>Informe de problema que muestra los problemas enviados por el usuario que ha iniciado sesión y que se han cerrado en los últimos tres meses o que se encuentran abiertos. El informe muestra los campos siguientes: Nombre de Source, Tipo de problema, Fecha de entrada, Estado y Prioridad de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Mis tareas</td> 
   <td>Informe de tarea que muestra las tareas no terminadas de los proyectos actuales asignados al usuario que ha iniciado sesión. El informe muestra los campos siguientes: Duración planificada, Nombre del proyecto, Usuario asignado principal, Inicio planificado, Finalización planificada, Porcentaje completado y Prioridad de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Mis hojas de horas</td> 
   <td>Informe de hoja de horas que muestra todas las hojas de horas del usuario que ha iniciado sesión. El informe muestra los campos siguientes: Intervalo de fechas, Nombre del propietario, Horas totales, Horas extra, Nombre del aprobador y Estado de las hojas de horas.</td> 
  </tr> 
  <tr> 
   <td>Mis problemas sin asignar</td> 
   <td>Informe de problema que muestra los problemas pendientes asignados a cualquiera de los roles del usuario que ha iniciado sesión y que no están asignados a ese usuario. El informe muestra los campos siguientes: Nombre de Source, Tipo de problema, Fecha de entrada, Estado y Prioridad de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Mis tareas sin asignación</td> 
   <td>Informe de tarea que muestra las tareas no terminadas asignadas a cualquiera de los roles del usuario que ha iniciado sesión y que no están asignadas a ese usuario. El informe muestra los campos siguientes: Duración planificada, Nombre del proyecto, Usuario asignado principal, Fecha planificada de inicio, Fecha planificada de finalización, Porcentaje completado y Prioridad de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Mis próximas tareas</td> 
   <td>Informe de tarea que muestra las tareas no terminadas que deberían comenzarse en las próximas dos semanas, que se encuentran en proyectos actuales y que se han asignado al usuario que inició sesión. El informe muestra los campos siguientes: Nombre del proyecto, Fecha planificada de finalización, Fecha proyectada de finalización, Porcentaje completado y Estado de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Abrir hojas de horas (solicitado)</td> 
   <td>Informe de hoja de horas que muestra las hojas de horas abiertas. El informe muestra los campos siguientes: Intervalo de fechas, Propietario, Horas totales, Horas extra, Nombre del aprobador y Estado de las hojas de horas. El informe se solicita mediante: Fecha de inicio de la hoja de horas, Fecha de finalización de la hoja de horas, Nombre del aprobador de la hoja de horas y Nombre de usuario.</td> 
  </tr> 
  <tr> 
   <td>Proyecto con presupuesto excedido por portafolio</td> 
   <td>Informe de proyecto que muestra el costo planificado y el costo real de los proyectos. El informe se agrupa por Nombre de Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Costo de portafolio planificado por programa</td> 
   <td>Informe de proyecto que muestra el costo planificado y el costo real de los proyectos. El informe se solicita mediante Nombre de Portfolio, agrupado por Nombre de programa, e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costo de portafolio planificado por proyecto</td> 
   <td>Informe de proyecto que muestra el costo planificado y el costo real de los proyectos. El informe se solicita mediante Nombre de Portfolio, agrupado por Nombre de proyecto, e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio planificados por programa</td> 
   <td>Informe de proyecto que muestra los ingresos planificados y los ingresos reales de los proyectos. El informe se solicita mediante Nombre de Portfolio, agrupado por Nombre de programa, e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio planificados por proyecto</td> 
   <td>Informe de proyecto que muestra los ingresos planificados y los ingresos reales de los proyectos. El informe se solicita mediante Nombre de Portfolio, agrupado por Nombre de proyecto, e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costos planificados contra costos reales por portafolio</td> 
   <td>Informe de proyecto que muestra el costo planificado y el costo real de los proyectos por Portfolio. El informe se agrupa por Nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costos planificados contra costos reales por programa</td> 
   <td>Informe de proyecto que muestra el costo planificado y el costo real de los proyectos por programa. El informe se agrupa por Nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos planificados contra ingresos reales por portafolio</td> 
   <td>Informe de proyecto que muestra los ingresos planificados y los ingresos reales de los proyectos. El informe se agrupa por Nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos planificados contra ingresos reales por programa</td> 
   <td>Informe de proyecto que muestra los ingresos planificados y los ingresos reales de los proyectos. El informe se agrupa por Nombre de programa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costos de portafolio agrupados por programa y por mes</td> 
   <td>Informe de proyecto en matriz que muestra el costo planificado, el costo presupuestado y el costo real de los proyectos. El informe se agrupa por nombre de Portfolio, nombre de programa y el mes de la fecha planificada de inicio de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Proyectos de portafolio por estado agrupados por programa</td> 
   <td>Informe de proyecto que muestra el estado de los proyectos. El informe se agrupa por nombre de programa y estado de proyecto e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos de portafolio agrupados por estado y portafolio</td> 
   <td>Informe de proyecto que muestra el nombre del Portfolio y el estado de los proyectos. El informe se agrupa por el nombre del Portfolio y el estado de los proyectos e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio por programa</td> 
   <td>Informe de proyecto que muestra el nombre del Portfolio, el nombre del programa, los ingresos planificados y los ingresos reales de los proyectos. El informe se agrupa por el nombre del Portfolio y el nombre del programa, e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio agrupados por programa y por mes</td> 
   <td>Informe de proyecto en matriz que muestra los ingresos planificados, los ingresos reales, el nombre del Portfolio y el nombre del programa. El informe se agrupa por nombre de Portfolio, nombre de programa y el mes de la fecha planificada de inicio de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Costos e ingresos de proyecto por estado de tarea</td> 
   <td>Informe de tarea en matriz que muestra el costo planificado, el costo real, los ingresos planificados, los ingresos reales y el nombre del proyecto de las tareas. El informe se agrupa por Nombre de proyecto y Estado de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Costos de proyecto contra ingresos por portafolio</td> 
   <td>Informe de proyecto que muestra el nombre del Portfolio, el costo real y los ingresos reales de los proyectos. El informe se agrupa por Nombre de Portfolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Gastos de proyecto por mes y trimestre</td> 
   <td>Informe de gasto en matriz que muestra la fecha de entrada, el importe planificado, el importe real y el proyecto de los gastos. El informe se agrupa por el nombre del proyecto, el trimestre y el mes de la fecha de entrada de los gastos.</td> 
  </tr> 
  <tr> 
   <td>Costos por hora de proyecto por tipo de hora y por mes</td> 
   <td>Informe de hora en matriz que muestra los campos siguientes: Horas, Fecha de entrada, Costo real de los proyectos, Tipo de hora, Nombre del proyecto. El informe se agrupa por nombre de proyecto, mes de la fecha de entrada de las horas y tipo de hora.</td> 
  </tr> 
  <tr> 
   <td>Costos de mano de obra y gastos de proyecto por mes y trimestre</td> 
   <td>Informe de proyecto en matriz que muestra el costo de mano de obra planificado, el costo de mano de obra real, el costo de gasto planificado y el costo de gasto real de los proyectos. El informe se agrupa por nombre de proyecto, trimestre y mes de la fecha real de inicio de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Rendimiento del proyecto</td> 
   <td>Informe de proyecto que muestra los campos siguientes de los proyectos actuales: fecha de vencimiento, CPI, SPI, CSI, costo planificado, presupuesto, EAC y gastos.</td> 
  </tr> 
  <tr> 
   <td>Solicitudes de proyecto</td> 
   <td>Informe de proyecto que muestra los proyectos solicitados. El informe muestra los campos siguientes: la descripción, la fecha planificada de finalización, la fecha proyectada de finalización, el porcentaje completado, el estado y la prioridad de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Proyectos por condición</td> 
   <td>Informe de proyecto que muestra la condición de los proyectos. El informe se agrupa por Condición e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos por condición de grupo</td> 
   <td>Informe de proyecto que muestra el estado de progreso y el grupo de los proyectos. El informe se agrupa por nombre de grupo y estado de progreso e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos por prioridad</td> 
   <td>Informe de proyecto que muestra la prioridad de los proyectos. El informe se agrupa por Prioridad e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos por estado de progreso</td> 
   <td>Informe de proyecto que muestra el estado de progreso de los proyectos. El informe se agrupa por el estado de progreso e incluye un gráfico.</td> 
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
   <td>Informe de hoja de horas que muestra las hojas de horas enviadas y rechazadas, cuyo aprobador sea el usuario que ha iniciado sesión. El informe muestra los campos siguientes: Intervalo de fechas, Propietario, Horas totales, Horas extra, Nombre del aprobador y Estado de las hojas de horas.</td> 
  </tr> 
  <tr> 
   <td>Tarea con problemas</td> 
   <td>Informe de tarea que muestra las tareas no terminadas con un estado de progreso de Retrasado, con una fecha de transferencia anterior a la de mañana y en las que el usuario que ha iniciado sesión forme parte del equipo del proyecto en el que se encuentran las tareas. El informe muestra los campos siguientes: Duración planificada, Nombre del proyecto, Usuario asignado principal, Inicio planificado, Finalización planificada, Porcentaje completado y Prioridad de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Inicios de sesión del usuario</td> 
   <td>Informe de usuario que muestra los campos siguientes: el ID único, el recuento de inicio de sesión (el número de veces que el usuario inició sesión desde que comenzó con Workfront) y la fecha del último inicio de sesión de los usuarios. El informe se agrupa por el nivel de acceso de los usuarios.</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## Acceso a informes integrados

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

{{step1-click-main-menu}}

1. Haga clic en **Informes**.
1. Haga clic en **Todos los informes**.
1. Expanda el menú desplegable **Filtro** y seleccione **Nuevo filtro**.

1. Haga clic en **Agregar una regla de filtro**.
1. En el campo **Empiece a escribir el nombre del campo**, empiece a escribir **Id. global**.

1. En el objeto **Informe**, seleccione **Identificador global**.

1. En el menú desplegable del modificador de filtro, seleccione **No está en blanco**.\
   ![](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Haga clic en **Guardar filtro**.\
   La lista de informes solo muestra los informes integrados.\
   Para obtener más información sobre los informes integrados disponibles, consulte la sección [Información general sobre los informes integrados](#overview-of-built-in-reports) en este artículo.
