---
product-area: reporting
navigation-topic: using-built-in-reports
title: Uso de informes integrados de Adobe Workfront
description: Adobe Workfront tiene una extensa lista de informes integrados que están listos para usar. Los administradores de Workfront pueden ocultar los informes integrados para que los usuarios no tengan acceso a ellos.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '2970'
ht-degree: 99%

---

# Uso de informes integrados de Adobe Workfront

<!--Audited: 11/2024-->

Adobe Workfront tiene una extensa lista de informes integrados que puede utilizar.

Los administradores de Workfront pueden ocultar los informes integrados para que los usuarios no tengan acceso a ellos.

Para obtener más información sobre cómo ocultar informes integrados, consulte [Ocultar informes integrados](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
      <p>Nuevo:</p>
         <ul>
         <li><p>Colaborador o superior</p></li>
         </ul>
      <p>Actual:</p>
         <ul>
         <li><p>Solicitud o superior</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a filtros, vistas y agrupaciones</p> <p>Acceso de visualización o superior a informes, paneles de control y calendarios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración de un informe para añadir o editar un filtro en un informe</p> <p>Permisos de administración de un filtro para editarlo en una lista</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Información general sobre informes integrados {#overview-of-built-in-reports}

Puede personalizar un informe integrado y guardarlo como un informe nuevo. Para obtener más información sobre cómo personalizar informes integrados, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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
   <td>Informe de proyecto que muestra el coste planificado y el coste real de los proyectos. El informe se agrupa por el nombre del programa, se solicita por el nombre del portafolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costo de portafolio real por proyecto</td> 
   <td>Informe de proyecto que muestra el coste planificado y el coste real de los proyectos. El informe se agrupa por el nombre del proyecto, se solicita por el nombre del portafolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio real por programa</td> 
   <td>Informe de proyecto que muestra los ingresos planificados y los ingresos reales de los proyectos. El informe se agrupa por el nombre del programa, se solicita por el nombre del portafolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio reales por proyecto</td> 
   <td>Informe de proyecto que muestra los ingresos planificados y los ingresos reales de los proyectos. El informe se agrupa por el nombre del proyecto, se solicita por el nombre del portafolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos reales por compañía</td> 
   <td>Informe de proyecto que muestra los ingresos reales y la compañía de los proyectos. El informe se agrupa por el nombre de la empresa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos reales por grupo</td> 
   <td>Informe de proyecto que muestra los ingresos reales y el grupo de los proyectos. El informe se agrupa por el nombre del grupo e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Todas las hojas de horas abiertas</td> 
   <td>Informe de hoja de horas que muestra las hojas de horas abiertas. El informe muestra los siguientes campos: Intervalo de fecha, Nombre del propietario, Total de horas, Horas extra, Nombre del aprobador y Estado de las hojas de horas.</td> 
  </tr> 
  <tr> 
   <td>Hojas de horas de aprobación (solicitado)</td> 
   <td>Informe de hoja de horas que muestra las hojas de horas enviadas o rechazadas con los aprobadores. El informe muestra los siguientes campos: Intervalo de fecha, Propietario, Total de horas, Horas extra, Nombre del aprobador y Estado de las hojas de horas. El informe se solicita por: Fecha de inicio de la hoja de horas, Fecha de finalización de la hoja de horas, Nombre del aprobador de la hoja de horas y Nombre del usuario.</td> 
  </tr> 
  <tr> 
   <td>Proyectos en riesgo</td> 
   <td>Informe de proyecto que muestra los proyectos actuales y planificados que tienen la condición de En riesgo o Con problemas. El informe muestra los siguientes campos: Descripción, Fecha planificada de finalización, Fecha proyectada de finalización, Porcentaje completado, Estado y Prioridad de los proyectos. El informe se agrupa por el nombre del portafolio.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de facturación por compañía</td> 
   <td>Informe de proyecto que muestra la compañía y los ingresos de facturación de los proyectos. El informe se agrupa por el nombre de la empresa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de facturación por grupo</td> 
   <td>Informe de proyecto que muestra los ingresos de facturación y el grupo de los proyectos. El informe se agrupa por el nombre del grupo e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de facturación por mes</td> 
   <td>Informe de registro de facturación que muestra el nombre del proyecto, los ingresos de facturación del proyecto y la fecha de facturación de los registros de facturación. El informe se agrupa por el mes de la fecha de facturación de los registros de facturación e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas completados por semana</td> 
   <td>Informe del problema que muestra la fecha real de finalización de los problemas. El informe se agrupa por la semana de la fecha real de finalización de los problemas e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas completados por semana por usuario</td> 
   <td>Informe del problema que muestra la fecha real de finalización y las asignaciones de los problemas. El informe se agrupa por el usuario asignado principal y por la semana de la fecha real de finalización de los problemas e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos actuales</td> 
   <td>Informe del proyecto que muestra todos los proyectos actuales. El informe muestra los siguientes campos: Descripción, Fecha planificada de finalización, Fecha proyectada de finalización, Porcentaje completado, Estado y Prioridad de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Costes por hora por mes por usuario</td> 
   <td>Informe de hora en matriz que muestra la cantidad de horas registradas y el coste real correspondiente. El informe se agrupa por el nombre del propietario y el mes de la fecha de entrada de las horas.</td> 
  </tr> 
  <tr> 
   <td>Horas por usuario</td> 
   <td>Informe de hora que muestra la cantidad de horas registradas. El informe se agrupa por el nombre del propietario e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Horas por semana por usuario</td> 
   <td>Informe de hora en matriz que muestra la cantidad de horas registradas en las cuatro semanas anteriores y la fecha de entrada de las horas. El informe se solicita por la fecha de entrada de las horas y se agrupa por el nombre del propietario y el mes de la fecha de entrada de las horas.</td> 
  </tr> 
  <tr> 
   <td>Problemas por estado</td> 
   <td>Informe de problema que muestra el estado de los problemas. El informe se agrupa por el estado de los problemas e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas por estado y proyecto</td> 
   <td>Informe de problema en matriz que muestra el estado de los problemas de los proyectos actuales y el nombre del proyecto. El informe se agrupa por el nombre del proyecto y el estado de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Costes de mano de obra contra costes de gastos por portafolio</td> 
   <td>Informe de proyecto que muestra el coste planificado de mano de obra, el coste real de mano de obra, el coste planificado de gastos y el coste real de gastos de los proyectos. El informe se agrupa por el nombre del portafolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costes de mano de obra contra costes de gastos por programa</td> 
   <td>Informe de proyecto que muestra el coste planificado de mano de obra, el coste real de mano de obra, el coste planificado de gastos y el coste real de gastos de los proyectos. El informe se agrupa por el nombre del portafolio y el nombre del programa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Coste planificado mensual de portafolio contra coste real por proyecto</td> 
   <td>Informe de proyecto en matriz (datos financieros) que muestra la fecha de asignación, el coste planificado total, el coste real total y la variación de coste total de los proyectos. El informe se agrupa por el nombre del proyecto, el trimestre y el mes de la fecha de asignación.</td> 
  </tr> 
  <tr> 
   <td>Ingresos planificados de portafolio mensuales contra coste real por proyecto</td> 
   <td>Informe de proyecto en matriz (datos financieros) que muestra la fecha de asignación, los ingresos planificados totales, los ingresos reales totales y la variación de ingresos totales de los proyectos. El informe se agrupa por el nombre del proyecto, el trimestre y el mes de la fecha de asignación.</td> 
  </tr> 
  <tr> 
   <td>Costes planificados de proyecto mensuales contra costes reales</td> 
   <td>Informe de proyecto en matriz (datos financieros) que muestra la fecha de asignación, el coste planificado total, el coste real total y la variación de coste total de los proyectos. El informe se agrupa por el nombre del proyecto, el trimestre y el mes de la fecha de asignación y se solicita por el nombre del proyecto.</td> 
  </tr> 
  <tr> 
   <td>Ingresos planificados de proyecto mensuales vs. costos reales</td> 
   <td>Informe de proyecto en matriz (datos financieros) que muestra la fecha de asignación, los ingresos planificados totales, los ingresos reales totales y la variación de ingresos totales de los proyectos. El informe se agrupa por el nombre del proyecto, el trimestre y el mes de la fecha de asignación y se solicita por el nombre del proyecto.</td> 
  </tr> 
  <tr> 
   <td>Mis documentos</td> 
   <td>Informe de documento que muestra los documentos cargados por el usuario que ha iniciado sesión. El informe muestra los siguientes campos: Nombre del propietario, Fecha de modificación, Tamaño, Recuento de versiones, Fuente y Tipo de los documentos.</td> 
  </tr> 
  <tr> 
   <td>Mis favoritos</td> 
   <td>Informe de favoritos que muestra una lista de objetos marcados como favoritos por el usuario que ha iniciado sesión. El informe muestra los siguientes campos: Tipo de objeto y Nombre de los favoritos.</td> 
  </tr> 
  <tr> 
   <td>Mis problemas</td> 
   <td>Informe de problema que muestra los problemas no completados asignados al usuario que ha iniciado sesión. El informe muestra los siguientes campos: Nombre de fuente, Tipo de problema, Usuario asignado principal, Fecha de entrada, Estado y Prioridad de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Mis portafolios</td> 
   <td>Informe de portafolio que muestra los portafolios activos en los que el usuario que ha iniciado sesión es el administrador de portafolios.</td> 
  </tr> 
  <tr> 
   <td>Mis programas</td> 
   <td>Informe de programa que muestra la descripción de los programas en los que el usuario que ha iniciado sesión es el administrador de programas.</td> 
  </tr> 
  <tr> 
   <td>Mis problemas pendientes del proyecto</td> 
   <td>Informe de problema que muestra los problemas no completados de los proyectos cuyo equipo de proyecto incluye al usuario que ha iniciado sesión. El informe muestra los siguientes campos: Nombre de fuente, Tipo de problema, Usuario asignado principal, Fecha de entrada, Estado y Prioridad de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Mis proyectos</td> 
   <td>Informe de proyecto que muestra los proyectos actuales cuyo equipo de proyectos incluye al usuario que ha iniciado sesión. El informe muestra los siguientes campos: Descripción, Fecha planificada de finalización, Fecha proyectada de finalización, Porcentaje completado, Estado y Prioridad de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Mis problemas enviados</td> 
   <td>Informe de problema que muestra los problemas enviados por el usuario que ha iniciado sesión y que se han cerrado en los tres meses anteriores o que se encuentran abiertos. El informe muestra los siguientes campos: Nombre de fuente, Tipo de problema, Fecha de entrada, Estado y Prioridad de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Mis tareas</td> 
   <td>Informe de tarea que muestra las tareas no completadas de los proyectos actuales asignados al usuario que ha iniciado sesión. El informe muestra los siguientes campos: Duración planificada, Nombre del proyecto, Usuario asignado principal, Inicio planificado, Finalización planificada, Porcentaje completado y Prioridad de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Mis hojas de horas</td> 
   <td>Informe de hoja de horas que muestra todas las hojas de horas del usuario que ha iniciado sesión. El informe muestra los siguientes campos: Intervalo de fecha, Nombre del propietario, Total de horas, Horas extra, Nombre del aprobador y Estado de las hojas de horas.</td> 
  </tr> 
  <tr> 
   <td>Mis problemas sin asignar</td> 
   <td>Informe de problema que muestra los problemas pendientes asignados a cualquiera de las funciones del usuario que ha iniciado sesión y que no están asignadas a ese usuario. El informe muestra los siguientes campos: Nombre de fuente, Tipo de problema, Fecha de entrada, Estado y Prioridad de los problemas.</td> 
  </tr> 
  <tr> 
   <td>Mis tareas sin asignación</td> 
   <td>Informe de tarea que muestra las tareas no completadas asignadas a cualquiera de las funciones del usuario que ha iniciado sesión y que no están asignadas a ese usuario. El informe muestra los siguientes campos: Duración planificada, Nombre del proyecto, Usuario asignado principal, Fecha planificada de inicio, Fecha planificada de finalización, Porcentaje completado y Prioridad de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Mis próximas tareas</td> 
   <td>Informe de tarea que muestra las tareas no completadas que deberían comenzarse en las siguientes dos semanas, que se encuentran en proyectos actuales y que se han asignado al usuario que ha iniciado sesión. El informe muestra los siguientes campos: Nombre del proyecto, Fecha planificada de finalización, Fecha proyectada de finalización, Porcentaje completado y Estado de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Abrir hojas de horas (solicitado)</td> 
   <td>Informe de hoja de horas que muestra las hojas de horas abiertas. El informe muestra los siguientes campos: Intervalo de fecha, Propietario, Total de horas, Horas extra, Nombre del aprobador y Estado de las hojas de horas. El informe se solicita por: Fecha de inicio de la hoja de horas, Fecha de finalización de la hoja de horas, Nombre del aprobador de la hoja de horas y Nombre del usuario.</td> 
  </tr> 
  <tr> 
   <td>Proyecto con presupuesto excedido por portafolio</td> 
   <td>Informe de proyecto que muestra el coste planificado y el coste real de los proyectos. El informe se agrupa por el nombre del portafolio.</td> 
  </tr> 
  <tr> 
   <td>Costo de portafolio planificado por programa</td> 
   <td>Informe de proyecto que muestra el coste planificado y el coste real de los proyectos. El informe se solicita por el nombre del portafolio, se agrupa por el nombre del programa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costo de portafolio planificado por proyecto</td> 
   <td>Informe de proyecto que muestra el coste planificado y el coste real de los proyectos. El informe se solicita por el nombre del portafolio, se agrupa por el nombre del proyecto e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio planificados por programa</td> 
   <td>Informe de proyecto que muestra los ingresos planificados y los ingresos reales de los proyectos. El informe se solicita por el nombre del portafolio, se agrupa por el nombre del programa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio planificados por proyecto</td> 
   <td>Informe de proyecto que muestra los ingresos planificados y los ingresos reales de los proyectos. El informe se solicita por el nombre del portafolio, se agrupa por el nombre del proyecto e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costos planificados contra costos reales por portafolio</td> 
   <td>Informe de proyecto que muestra el coste planificado y el coste real de los proyectos por portafolio. El informe se agrupa por el nombre del portafolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costes planificados contra costes reales por programa</td> 
   <td>Informe de proyecto que muestra el coste planificado y el coste real de los proyectos por programa. El informe se agrupa por el nombre del portafolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos planificados contra ingresos reales por portafolio</td> 
   <td>Informe de proyecto que muestra los ingresos planificados y los ingresos reales de los proyectos. El informe se agrupa por el nombre del portafolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos planificados contra ingresos reales por programa</td> 
   <td>Informe de proyecto que muestra los ingresos planificados y los ingresos reales de los proyectos. El informe se agrupa por el nombre del programa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Costos de portafolio agrupados por programa y por mes</td> 
   <td>Informe de proyecto en matriz que muestra el coste planificado, el coste presupuestado y el coste real de los proyectos. El informe se agrupa por el nombre del portafolio, el nombre del programa y el mes de la fecha planificada de inicio de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Proyectos de portafolio por estado agrupados por programa</td> 
   <td>Informe de proyecto que muestra el estado de progreso de los proyectos. El informe se agrupa por el nombre del programa y el estado de proyecto e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos de portafolio agrupados por estado y portafolio</td> 
   <td>Informe de proyecto que muestra el nombre del proyecto y el estado de los proyectos. El informe se agrupa por el nombre del portafolio y el estado de los proyectos e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio por programa</td> 
   <td>Informe de proyecto que muestra el nombre del portafolio, el nombre del programa, los ingresos planificados y los ingresos reales de los proyectos. El informe se agrupa por el nombre del portafolio y el nombre del programa e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Ingresos de portafolio agrupados por programa y por mes</td> 
   <td>Informe de proyecto en matriz que muestra los ingresos planificados, los ingresos reales, el nombre del portafolio y el nombre del programa. El informe se agrupa por el nombre del portafolio, el nombre del programa y el mes de la fecha planificada de inicio de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Costes e ingresos del proyecto por estado de tarea</td> 
   <td>Informe de tarea en matriz que muestra el coste planificado, el coste real, los ingresos planificados, los ingresos reales y el nombre del proyecto de las tareas. El informe se agrupa por el nombre del proyecto y el estado de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Costes del proyecto contra ingresos por portafolio</td> 
   <td>Informe de proyecto que muestra el nombre del portafolio, el coste real y los ingresos reales de los proyectos. El informe se agrupa por el nombre del portafolio e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Gastos del proyecto por mes y trimestre</td> 
   <td>Informe de gasto en matriz que muestra la fecha de entrada, el importe planificado, el importe real y el proyecto de los gastos. El informe se agrupa por el nombre del proyecto, el trimestre y el mes de la fecha de entrada de los gastos.</td> 
  </tr> 
  <tr> 
   <td>Costes por hora de proyecto por tipo de hora y por mes</td> 
   <td>Informe de hora en matriz que muestra los campos siguientes: Horas, Fecha de entrada, Coste real de los proyectos, Tipo de hora y Nombre del proyecto. El informe se agrupa por el nombre del proyecto, el mes de la fecha de entrada de las horas y el tipo de hora.</td> 
  </tr> 
  <tr> 
   <td>Costes de mano de obra y gastos de proyecto por mes y trimestre</td> 
   <td>Informe de proyecto que muestra el coste planificado de mano de obra, el coste real de mano de obra, el coste planificado de gastos y el coste real de gastos de los proyectos. El informe se agrupa por el nombre del proyecto, el trimestre y el mes de la fecha real de inicio de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Rendimiento del proyecto</td> 
   <td>Informe de proyecto que muestra los siguientes campos de los proyectos actuales: Fecha de vencimiento, IRC, IRCC, ICC, Coste planificado, Presupuesto, CEF y gastos de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Solicitudes de proyectos</td> 
   <td>Informe de proyecto que muestra los proyectos solicitados. El informe muestra los siguientes campos: Descripción, Fecha planificada de finalización, Fecha proyectada de finalización, Porcentaje completado, Estado y Prioridad de los proyectos.</td> 
  </tr> 
  <tr> 
   <td>Proyectos por condición</td> 
   <td>Informe de proyecto que muestra la condición de los proyectos. El informe se agrupa por la condición e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos por condición por grupo</td> 
   <td>Informe de proyecto que muestra el estado de progreso y el grupo de los proyectos. El informe se agrupa por el nombre del grupo y el estado de progreso e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos por prioridad</td> 
   <td>Informe de proyecto que muestra la prioridad de los proyectos. El informe se agrupa por la prioridad e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Proyectos por estado de progreso</td> 
   <td>Informe de proyecto que muestra el estado de progreso de los proyectos. El informe se agrupa por el estado de progreso e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Tareas por estado de progreso</td> 
   <td>Informe de tarea que muestra el estado de progreso de todas las tareas de los proyectos actuales. El informe se agrupa por el estado de progreso e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Tareas por estado</td> 
   <td>Informe de tarea que muestra el estado de todas las tareas. El informe se agrupa por el estado e incluye un gráfico.</td> 
  </tr> 
  <tr> 
   <td>Hojas de horas para revisar</td> 
   <td>Informe de hoja de horas que muestra las hojas de horas enviadas y rechazadas cuyo aprobador sea el usuario que ha iniciado sesión. El informe muestra los campos siguientes: Intervalo de fecha, Propietario, Total de horas, Horas extra, Nombre del aprobador y Estado de las hojas de horas.</td> 
  </tr> 
  <tr> 
   <td>Tarea con problemas</td> 
   <td>Informe de tarea que muestra las tareas no terminadas con un estado de progreso de Retrasado, con una fecha de transferencia anterior a la de mañana y en las cuales el usuario que ha iniciado sesión forma parte del equipo del proyecto donde se encuentran las tareas. El informe muestra los siguientes campos: Duración planificada, Nombre del proyecto, Usuario asignado principal, Inicio planificado, Finalización planificada, Porcentaje completado y Prioridad de las tareas.</td> 
  </tr> 
  <tr> 
   <td>Inicios de sesión del usuario</td> 
   <td>Informe de usuario que muestra los siguientes campos: ID único, Recuento de inicio de sesión (número de veces que el usuario ha iniciado sesión desde que comenzó con Workfront) y Fecha del último inicio de sesión de los usuarios. El informe se agrupa por el nivel de acceso de los usuarios.</td> 
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
1. Expanda el menú desplegable **Filtro** y haga clic en **Nuevo filtro**.

1. Haga clic en **Añadir regla de filtro**.
1. En el campo **Empezar a escribir el nombre del campo**, empiece a escribir **Identidad global**.

1. En el objeto **Informe**, seleccione **Identidad global**.

1. En el menú desplegable del modificador de filtro, seleccione **No está en blanco**.\
   ![Filtro de ID global para informes del sistema](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Haga clic en **Guardar filtro**.\
   La lista de informes únicamente muestra los informes integrados.\
   Para obtener más información sobre los informes integrados disponibles, consulte la sección [Información general sobre los informes integrados](#overview-of-built-in-reports) en este artículo.
