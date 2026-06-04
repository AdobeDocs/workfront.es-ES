---
product-area: reports and dashboards
navigation-topic: data-connect
title: Usar la vista Supervisión de actualizaciones de datos en Data Connect
description: Con Data Connect, los administradores de Workfront pueden acceder a los registros detallados de las actualizaciones recientes realizadas en la fecha del lago de datos durante la actualización más reciente.
author: Courtney
feature: Reports and Dashboards
exl-id: 230d1a30-2af9-4d2c-9ec1-34c3d4c080d4
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/i-F8ebsLAFO-0mP-bXzzEyFDsfvuWH-qswPc7C5cyMg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 362
ht-degree: 7%

---

# Usar la vista Supervisión de actualizaciones de datos en Data Connect

La vista Monitorización de actualizaciones de datos muestra las actualizaciones recientes realizadas en la fecha del lago de datos durante la actualización más reciente. Los datos de esta vista se actualizan después de cada finalización correcta de una carga de datos.

Debido al gran volumen de datos y a la complejidad de las agregaciones, la vista Supervisión de actualizaciones de datos solo muestra las vistas de objetos que se han actualizado en las últimas 2 semanas. Si un tipo de registro específico está ausente en esta vista, es probable que se deba a una falta de actividad dentro de ese periodo de tiempo.

>[!NOTE]
>
>Esta vista muestra una recopilación detallada de los datos proporcionados por la aplicación y las actividades de actualización, a diferencia de un historial diario o una vista de evento que muestra el historial de actividades de actualización. Para obtener los detalles de la actividad de actualización histórica, puede utilizar <code>DL_LOAD_TIMESTAMP</code> objeto de fecha.

## Monitorización de columnas de vista de actualizaciones de datos

Las columnas de la vista Actualizaciones de datos de supervisión contienen la siguiente información:

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
      El tipo de objeto asociado con los registros de Workfront enviados al lago de datos. 
        </ul></td>
    </tr>
    <tr>
        <td>CALENDAR_DATE </td>
        <td>Fecha</td>
        <td>
   Fecha de la última actualización de datos correcta para el tipo de objeto mostrado en la columna OBJ_TYPE. </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ</td>
        <td>
 Fecha y hora de la última actualización de datos para el tipo de objeto mostrado en la columna OBJ_TYPE.  </td>
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
     Cantidad de tiempo en minutos que ha transcurrido desde la última actualización de datos para el tipo de objeto. </td>
    </tr>
            <tr>
        <td>CREADO </td>
        <td>Número </td>
        <td>Recuento de los eventos de registro CREATE capturados entre las actualizaciones de datos anteriores y más recientes para el tipo de objeto.  </td>
    </tr>
                <tr>
        <td>ACTUALIZADO</td>
        <td>Número </td>
        <td>Recuento de los eventos de registro UPDATE capturados entre las actualizaciones de datos anteriores y las más recientes para el tipo de objeto.</td>
    </tr>
                <tr>
        <td>ELIMINADO</td>
        <td>Número </td>
        <td>Recuento de los eventos de registro de DELETE capturados entre las actualizaciones de datos anteriores y las más recientes para el tipo de objeto. </td>
    </tr>
                <tr>
        <td>TOTAL</td>
        <td>Número </td>
        <td>Recuento del número total de eventos entre las actualizaciones de datos anteriores y las más recientes para el tipo de objeto. 
        <br> 
        <br><b>Nota</b>: No es lo mismo que el número total de registros afectados por los eventos CREATE, UPDATE o DELETE, ya que el mismo registro se puede CREAR y ACTUALIZAR varias veces en el intervalo entre actualizaciones.  </td>
    </tr>
   </table>
