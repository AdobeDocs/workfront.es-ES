---
product-area: reports and dashboards
navigation-topic: data-connect
title: Usar la vista Supervisión de actualizaciones de datos en Data Connect
description: Con Data Connect, los administradores de Workfront pueden acceder a registros detallados de las actualizaciones recientes que se realizaron en la fecha del lago de datos durante la actualización más reciente.
author: Courtney
feature: Reports and Dashboards
exl-id: 230d1a30-2af9-4d2c-9ec1-34c3d4c080d4
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 6%

---

# Usar la vista Supervisión de actualizaciones de datos en Data Connect

La vista Monitorización de actualizaciones de datos muestra las actualizaciones recientes realizadas en la fecha del lago de datos durante la actualización más reciente. Los datos de esta vista se actualizan después de cada finalización correcta de una carga de datos.

Debido al gran volumen de datos y a la complejidad de las agregaciones, la vista Actualización de datos sólo muestra las vistas de objetos que se han actualizado en las últimas 2 semanas. Si un tipo de registro específico no existe en esta vista, es probable que se deba a una falta de actividad dentro de ese intervalo de tiempo.

>[!NOTE]
>
>Esta vista muestra una recopilación detallada de los datos proporcionados por la aplicación y las actividades de actualización, en lugar de una vista del historial diario o de eventos que muestra el historial de actividades de actualización. Para obtener detalles históricos de la actividad de actualización, puede utilizar <code>DL_LOAD_TIMESTAMP</code> objeto de fecha.

## Columnas de vista de actualizaciones de datos de supervisión

Las columnas de la vista Actualizaciones de Datos de Control contienen la siguiente información:

<table>
    <tr>
        <td><b>Nombre de columna</b></td>
        <td><b>Tipo</b></td>
        <td><b>Descripción</b></td>
    </tr>
    <tr>
        <td>OBJ_TYPE</td>
        <td>Varchar
        </td>
        <td> 
      Tipo de objeto asociado a los registros de Workfront enviados al lago de datos. 
        </ul></td>
    </tr>
    <tr>
        <td>CALENDAR_DATE </td>
        <td>Fecha</td>
        <td>
   Fecha de la última actualización correcta de datos para el tipo de objeto mostrado en la columna OBJ_TYPE. </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ</td>
        <td>
 Fecha y hora de la actualización de datos más reciente para el tipo de objeto mostrado en la columna OBJ_TYPE.  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ </td>
        <td>
       Fecha y hora de la segunda actualización de datos más reciente para el tipo de objeto mostrado en la columna OBJ_TYPE. </td>
    </tr>
        <tr>
        <td>MINUTES_SINCE_PREVIOUS_LOAD </td>
        <td>Número</td>
        <td>
     Tiempo en minutos transcurrido desde la última actualización de datos para el tipo de objeto. </td>
    </tr>
            <tr>
        <td>CREADO </td>
        <td>Número </td>
        <td>Recuento de los eventos CREATE record capturados entre la actualización de datos anterior y la más reciente para el tipo de objeto.  </td>
    </tr>
                <tr>
        <td>ACTUALIZADO</td>
        <td>Número </td>
        <td>Recuento de los eventos de registro UPDATE capturados entre la actualización de datos anterior y la más reciente para el tipo de objeto.</td>
    </tr>
                <tr>
        <td>ELIMINADO</td>
        <td>Número </td>
        <td>Recuento de los eventos de registro de DELETE capturados entre las actualizaciones de datos anteriores y las más recientes para el tipo de objeto. </td>
    </tr>
                <tr>
        <td>TOTAL</td>
        <td>Número </td>
        <td>Recuento del número total de eventos entre la actualización de datos anterior y la más reciente para el tipo de objeto. 
        <br> 
        <br><b>Nota</b>: No es el mismo que el número total de registros afectados por los eventos CREATE, UPDATE o DELETE, ya que el mismo registro se puede CREAR y ACTUALIZAR varias veces en el intervalo entre actualizaciones.  </td>
    </tr>
   </table>
