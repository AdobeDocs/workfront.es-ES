---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Tokens para el formato de fecha y hora en [!DNL Adobe Workfront Fusion]
description: Los siguientes tokens para el formato de fecha y hora están disponibles en la [!DNL Adobe Workfront Fusion mapping] panel.
author: Becky
feature: Workfront Fusion
exl-id: 19d0608e-7902-4d09-b71d-e6ae8ed7a6fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 6%

---

# Tokens para el formato de fecha y hora en [!DNL Adobe Workfront Fusion]

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Tokens de año, mes y día

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Token </th> 
   <th>Output </th> 
   <th> <p>Descripción</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>YY </code> </td> 
   <td><code>70 71 ... 29 30</code> </td> 
   <td> <p> El año expresado con 2 dígitos</p> </td> 
  </tr> 
  <tr> 
   <td><code>YYYY </code> </td> 
   <td><code>1970 1971 ... 2029 2030 </code> </td> 
   <td> <p>El año expresado con 4 dígitos</p> </td> 
  </tr> 
  <tr> 
   <td><code>Y</code> </td> 
   <td><code>1970 1971 ... 9999 +10000 +10001</code> </td> 
   <td> <p>[!UICONTROL Year con cualquier número de dígitos y signo]</p> </td> 
  </tr> 
  <tr> 
   <td><code>Q</code> </td> 
   <td><code>1 2 3 4 </code> </td> 
   <td> <p> Trimestre del año</p> </td> 
  </tr> 
  <tr> 
   <td><code>Qo</code> </td> 
   <td><code>1st 2nd 3rd 4th </code></td> 
   <td> <p>Trimestre del año con ordinal</p> </td> 
  </tr> 
  <tr> 
   <td><code>M</code> </td> 
   <td><code>1 2 ... 11 12</code></td> 
   <td> <p>Número de mes</p> </td> 
  </tr> 
  <tr> 
   <td><code>Mo </code> </td> 
   <td><code>1st 2nd ... 11th 12th</code> </td> 
   <td> <p>[!UICONTROL Mes] con ordinal</p> </td> 
  </tr> 
  <tr> 
   <td><code>MM</code> </td> 
   <td><code>01 02 ... 11 12 </code> </td> 
   <td> <p> Número de mes con cero a la izquierda</p> </td> 
  </tr> 
  <tr> 
   <td><code>MMM</code> </td> 
   <td><code>Jan Feb ... Nov Dec</code></td> 
   <td> <p> Abreviatura del mes</p> </td> 
  </tr> 
  <tr> 
   <td><code>MMMM</code> </td> 
   <td><code> January February ... November December</code> </td> 
   <td> <p> Nombre del mes</p> </td> 
  </tr> 
  <tr> 
   <td><code>D</code> </td> 
   <td><code>1 2 ... 30 31 </code></td> 
   <td> <p>Día del mes</p> </td> 
  </tr> 
  <tr> 
   <td><code>Do</code> </td> 
   <td><code>1st 2nd ... 30th 31st</code></td> 
   <td> <p> Día del mes con ordinal</p> </td> 
  </tr> 
  <tr> 
   <td><code>DD</code> </td> 
   <td><code>01 02 ... 30 31</code></td> 
   <td> <p> Día del mes con cero a la izquierda</p> </td> 
  </tr> 
  <tr> 
   <td><code>DDD</code> </td> 
   <td><code>1 2 ... 364 365 </code></td> 
   <td> <p>Día del año</p> </td> 
  </tr> 
  <tr> 
   <td><code>DDDo</code> </td> 
   <td><code>1st 2nd ... 364th 365th</code> </td> 
   <td> <p>[!UICONTROL Día del año] con ordinal</p> </td> 
  </tr> 
  <tr> 
   <td><code>DDDD </code> </td> 
   <td><code>001 002 ... 364 365</code> </td> 
   <td> <p> Día del año con cero a la izquierda</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tokens de semana, año, semana y día de la semana

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Token </th> 
   <th>Output </th> 
   <th> <p>Descripción</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>d</code> </td> 
   <td><code>0 1 ... 5 6 </code> </td> 
   <td> <p> Día de la semana</p> </td> 
  </tr> 
  <tr> 
   <td><code>do</code> </td> 
   <td><code>0th 1st ... 5th 6th </code> </td> 
   <td> <p>[!UICONTROL Día de la semana con ordinal]</p> </td> 
  </tr> 
  <tr> 
   <td><code>dd </code> </td> 
   <td><code>Su Mo ... Fr Sa </code> </td> 
   <td> <p>Abreviatura de día</p> </td> 
  </tr> 
  <tr> 
   <td><code>ddd</code> </td> 
   <td><code>Sun Mon ... Fri Sat </code> </td> 
   <td> <p> Abreviatura de día</p> </td> 
  </tr> 
  <tr> 
   <td><code>dddd </code> </td> 
   <td><code>Sunday Monday ... Friday Saturday</code> </td> 
   <td> <p> Nombre del día</p> </td> 
  </tr> 
  <tr> 
   <td><code>E</code> </td> 
   <td><code>1 2 ... 6 7 </code> </td> 
   <td> <p> Día de la semana (ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>w </code> </td> 
   <td><code>1 2 ... 52 53 </code> </td> 
   <td> <p>Semana del año</p> </td> 
  </tr> 
  <tr> 
   <td><code>wo </code> </td> 
   <td><code>1st 2nd ... 52nd 53rd</code> </td> 
   <td> <p>[!UICONTROL Semana del año con ordinal]</p> </td> 
  </tr> 
  <tr> 
   <td><code>ww </code> </td> 
   <td><code>01 02 ... 52 53 </code> </td> 
   <td> <p>Semana del año con cero a la izquierda</p> </td> 
  </tr> 
  <tr> 
   <td><code>W</code></td> 
   <td><code>1 2 ... 52 53 </code> </td> 
   <td> <p>Semana del año (ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>Wo</code> </td> 
   <td><code>1st 2nd ... 52nd 53rd </code> </td> 
   <td> <p> Semana del año con ordinal (ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>WW</code> </td> 
   <td><code>01 02 ... 52 53 </code> </td> 
   <td> <p> Semana del año con cero a la izquierda (ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>gg</code></td> 
   <td><code>70 71 ... 29 30 </code> </td> 
   <td> <p>Semana del año</p> </td> 
  </tr> 
  <tr> 
   <td><code>gggg </code> </td> 
   <td><code>1970 1971 ... 2029 2030</code> </td> 
   <td> <p> Semana del año</p> </td> 
  </tr> 
  <tr> 
   <td><code>GG </code> </td> 
   <td><code>70 71 ... 29 30 </code> </td> 
   <td> <p>Año de la semana (ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>GGGG </code> </td> 
   <td><code>1970 1971 ... 2029 2030</code> </td> 
   <td> <p> Año de la semana (ISO)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tokens de hora, minuto, segundo, milisegundo y desplazamiento

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Token </p> </th> 
   <th>Output </th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>H</code> </td> 
   <td><code>0 1 ... 22 23</code></td> 
   <td> <p>24 horas</p> </td> 
  </tr> 
  <tr> 
   <td><code>HH</code> </td> 
   <td><code>00 01 ... 22 23</code></td> 
   <td> <p> Tiempo de 24 horas con cero a la izquierda</p> </td> 
  </tr> 
  <tr> 
   <td><code>h</code> </td> 
   <td><code>1 2 ... 11 12</code></td> 
   <td> <p> 12 horas</p> </td> 
  </tr> 
  <tr> 
   <td><code>hh </code> </td> 
   <td><code>01 02 ... 11 12</code> </td> 
   <td> <p> Tiempo de 12 horas con cero a la izquierda</p> </td> 
  </tr> 
  <tr> 
   <td><code>k</code> </td> 
   <td><code>1 2 ... 23 24</code></td> 
   <td> <p> 24 horas</p> </td> 
  </tr> 
  <tr> 
   <td><code>kk</code></td> 
   <td><code>01 02 ... 23 24</code> </td> 
   <td> <p> Tiempo de 24 horas con cero a la izquierda</p> </td> 
  </tr> 
  <tr> 
   <td><code>A</code></td> 
   <td><code>AM PM </code> </td> 
   <td> <p>Post o ante meridiem (mayúsculas)</p> </td> 
  </tr> 
  <tr> 
   <td><code>a</code> </td> 
   <td><code>am pm </code> </td> 
   <td> <p> Méridiem post o ante (minúscula)</p> </td> 
  </tr> 
  <tr> 
   <td><code>m</code> </td> 
   <td><code> 0 1 ... 58 59</code> </td> 
   <td> <p> minutos</p> </td> 
  </tr> 
  <tr> 
   <td><code>mm</code> </td> 
   <td><code>00 01 ... 58 59</code> </td> 
   <td> <p>[!UICONTROL Minutos con] cero a la izquierda</p> </td> 
  </tr> 
  <tr> 
   <td><code>s</code> </td> 
   <td><code>0 1 ... 58 59</code> </td> 
   <td> <p> Seconds</p> </td> 
  </tr> 
  <tr> 
   <td><code>ss</code> </td> 
   <td><code>00 01 ... 58 59</code></td> 
   <td> <p>Segundos con cero a la izquierda</p> </td> 
  </tr> 
  <tr> 
   <td><code>S</code> </td> 
   <td><code>0 1 ... 8 9 </code> </td> 
   <td> <p> Segundos fraccionarios</p> </td> 
  </tr> 
  <tr> 
   <td><code>SS</code> </td> 
   <td><code>00 01 ... 98 99</code> </td> 
   <td> <p> Segundos fraccionarios con cero a la izquierda</p> </td> 
  </tr> 
  <tr> 
   <td><code>SSS</code> </td> 
   <td><code>000 001 ... 998 999</code> </td> 
   <td> <p> Segundos fraccionarios con dos ceros a la izquierda</p> </td> 
  </tr> 
  <tr> 
   <td><code>SSSS ... SSSSSSSSS</code> </td> 
   <td><code>000[0..] 001[0..] ... 998[0..] 999[0..] </code> </td> 
   <td> <p> Segundos fraccionarios</p> </td> 
  </tr> 
  <tr> 
   <td><code>Z</code> </td> 
   <td><code>-07:00 -06:00 ... +06:00 +07:00 </code></td> 
   <td> <p>Zona horaria</p> </td> 
  </tr> 
  <tr> 
   <td><code>ZZ</code> </td> 
   <td><code>-0700 -0600 ... +0600 +0700 </code></td> 
   <td> <p>Zona horaria</p> </td> 
  </tr> 
  <tr> 
   <td><code>X</code> </td> 
   <td><code>1360013296</code> </td> 
   <td> <p> Unix Timestamp</p> </td> 
  </tr> 
  <tr> 
   <td><code>x</code> </td> 
   <td><code>1360013296123</code></td> 
   <td> <p> Marca de tiempo Unix en milisegundos</p> </td> 
  </tr> 
 </tbody> 
</table>
