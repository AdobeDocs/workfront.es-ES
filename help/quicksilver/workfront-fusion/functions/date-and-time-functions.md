---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funciones de fecha y hora en Adobe Workfront Fusion
description: Las siguientes funciones de fecha y hora están disponibles en el panel de asignación de Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 76c63afc-4bb6-4895-9bba-6b3913ecbcf6
source-git-commit: 7de4016e489c5194aee674f4ea090e7bcbb1ce79
workflow-type: tm+mt
source-wordcount: '1992'
ht-degree: 1%

---

# Funciones de fecha y hora en [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL formatDate (fecha; formato; [timezone])]

Utilice esta función cuando tenga un valor Date como, por ejemplo, `12-10-2021 20:30`, que desea formatear como un valor de texto, como `Dec 10, 2021 8:30 PM`.

Esto resulta útil, por ejemplo, cuando necesita cambiar el formato de fecha de una aplicación o servicio web al de una aplicación o servicio web conectado en el mismo escenario.

Para obtener más información, consulte [Fecha](../../workfront-fusion/mapping/item-data-types.md#date) y [Texto](../../workfront-fusion/mapping/item-data-types.md#text) en el artículo [Tipos de datos de elementos en Adobe Workfront Fusion](../../workfront-fusion/mapping/item-data-types.md).

### Parámetros

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Parámetro</th> 
   <th>Tipo de datos esperado* </th> 
   <th>Qué hace</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL fecha] </td> 
   <td>Fecha </td> 
   <td> <p>Convierte un valor Date en un valor Text. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL formato] </td> 
   <td>Texto </td> 
   <td> <p>Permite especificar un formato mediante tokens de formato de fecha y hora. Para obtener más información, consulte <a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">Tokens para el formato de fecha y hora en [!DNL Adobe Workfront Fusion]</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL huso horario] </td> 
   <td>Texto </td> 
   <td> <p>(Opcional) Permite especificar la zona horaria utilizada para la conversión. </p> <p>Para ver la lista de husos horarios reconocidos, consulte la columna "Nombre de la base de datos TZ" en Wikipedia <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">Lista de zonas horarias de base de datos tz</a>. La función solo reconoce los valores enumerados en esta columna como una zona horaria válida. Se ignora cualquier otro valor y se utiliza la zona horaria de escenarios especificada en su perfil. Para obtener más información, consulte en el artículo <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Cambio de la configuración de perfil en [!DNL Adobe Workfront Fusion]</a>.</p> <p>Si omite este parámetro, se aplica la zona horaria de escenarios especificada en la configuración del perfil. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>Europe/Prague</code>, <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

Si se proporciona un tipo diferente, se aplica coerción de tipo. Para obtener más información, consulte [Coerción de tipos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

### Valor devuelto y tipo

El `formatDate` función devuelve una representación de texto del valor Date dado según el formato y la zona horaria especificados. El tipo de datos es Texto.

>[!INFO]
>
>**Ejemplos:** Tanto el escenario como la zona horaria web se establecieron en `Europe/Prague` en estos ejemplos.
>
>![](assets/date&time-functions-examples-350x61.png)
>
>* `formatDate(1. Date created;MM/DD/YYYY)`
>
>    Devuelve 10/01/2018
>
>* `formatDate(1. Date created; YYYY-MM-DD hh:mm A)`
>
>   Devuelve 2018-10-01 09:32 AM
>
>* `formatDate(1. Date created;DD.MM.YYYY HH:mm;UTC)`
>
>    Devuelve 01.10.2018 07:32
>
>* `formatDate(now;DD.MM.YYYY HH:mm)`
>
>    Devuelve 19.03.2019 15:30

## [!UICONTROL parseDate (texto; formato; [timezone])]

Utilice esta función cuando tenga un valor de texto que represente una fecha (como `12-10-2019 20:30` o `Aug 18, 2019 10:00 AM`) y desea convertirlo (analizarlo) en un valor Date (una representación binaria legible por máquina). Para obtener más información, consulte [Fecha](../../workfront-fusion/mapping/item-data-types.md#date) y [Texto](../../workfront-fusion/mapping/item-data-types.md#text) en el artículo [Tipos de datos de elementos en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

### Parámetros

La segunda columna indica el tipo esperado. Si se proporciona un tipo diferente, se aplica coerción de tipo. Para obtener más información, consulte [Coerción de tipos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Parámetro</th> 
   <th>Tipo de datos esperado* </th> 
   <th>Qué hace</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL texto] </td> 
   <td>Texto </td> 
   <td> <p>Convierte un valor Date en un valor Text. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL formato] </td> 
   <td>Texto </td> 
   <td> <p>Permite especificar un formato mediante tokens de formato de fecha y hora. Para obtener más información, consulte <a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">Tokens para el formato de fecha y hora en Adobe Workfront Fusion</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL huso horario] </td> 
   <td>Texto </td> 
   <td> <p>(Opcional) Permite especificar la zona horaria utilizada para la conversión. </p> <p>Para ver la lista de husos horarios reconocidos, consulte la columna "Nombre de la base de datos TZ" en Wikipedia <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">Lista de zonas horarias de base de datos tz</a>. La función solo reconoce los valores enumerados en esta columna como una zona horaria válida. Se ignora cualquier otro valor y se utiliza la zona horaria de escenarios especificada en su perfil. Para obtener más información, consulte en el artículo <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Cambio de la configuración de perfil en Adobe Workfront Fusion</a>.</p> <p>Si omite este parámetro, se aplica la zona horaria de escenarios especificada en la configuración del perfil.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>Europe/Prague</code>, <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

Si se proporciona un tipo diferente, se aplica coerción de tipo. Para obtener más información, consulte [Coerción de tipos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

### Valor devuelto y tipo

Esta función convierte una cadena de texto en una fecha, según el formato y la zona horaria que especifique. El tipo de datos del valor es Fecha.

>[!INFO]
>
>**Ejemplos:** En los ejemplos siguientes, el valor Date devuelto se expresa según la norma ISO 8601, pero el tipo de datos del resultado es Date.
>
>* `parseDate(2016-12-28;YYYY-MM-DD)`
>
>    Devuelve 2016-12-28T00:00:00,000Z
>
>* `parseDate(2016-12-28 16:03;YYYY-MM-DD HH:mm)`
>
>    Devuelve 2016-12-28T16:03:00,000Z
>
>* `parseDate(2016-12-28 04:03 pm; YYYY-MM-DD hh:mm a)`
>
>    Devuelve 2016-12-28T16:03:06,000Z
>
>* `parseDate(1482940986;X)`
>
>   Devuelve 2016-12-28T16:03:06,000Z

## [!UICONTROL addDays (fecha; número)] {#adddays-date-number}

Devuelve una nueva fecha como resultado de agregar un número determinado de días a una fecha. Para restar días, introduzca un número negativo.

>[!INFO]
>
>**Ejemplos:**
>
>* `addDays(2016-12-08T15:55:57.536Z;2)`
>
>    Devuelve 2016-12-10T15:55:57,536Z
>
>* `addDays(2016-12-08T15:55:57.536Z;-2)`
>
>    Devuelve 2016-12-6T15:55:57,536Z

## [!UICONTROL addHours (fecha; número)] {#addhours-date-number}

Devuelve una nueva fecha como resultado de agregar un número determinado de horas a una fecha. Para restar horas, introduzca un número negativo.

>[!INFO]
>
>**Ejemplos:**
>
>* `addHours(2016-12-08T15:55:57.536Z; 2)`
>
>    Devuelve 2016-12-08T17:55:57,536Z
>
>* `addHours(2016-12-08T15:55:57.536Z;-2)`
>
>    Devuelve 2016-12-08T13:55:57,536Z

## [!UICONTROL addMinutes (fecha; número)] {#addminutes-date-number}

Devuelve una nueva fecha como resultado de agregar un número determinado de minutos a una fecha. Para restar minutos, introduzca un número negativo.

>[!INFO]
>
>**Ejemplos:**
>
>* `addMinutes(2016-12-08T15:55:57.536Z;2)`
>
>    Devuelve 2016-12-08T15:57:57,536Z
>
>* `addMinutes(2016-12-08T15:55:57.536Z;-2)`
>
>    Devuelve 2016-12-08T15:53:57,536Z

## [!UICONTROL addMonths (fecha; número)] {#addseconds-date-number}

Devuelve una nueva fecha como resultado de agregar un número determinado de meses a una fecha. Para restar meses, introduzca un número negativo.

>[!INFO]
>
>**Ejemplos:**
>
>* `addMonths(2016-08-08T15:55:57.536Z;2)`
>
>    Devuelve 2016-10-08T15:55:57,536Z
>
>* `addMonths(2016-08-08T15:55:57.536Z;-2)`
>
>    Devuelve 2016-06-08T15:55:57,536Z

## [!UICONTROL addSeconds (fecha; número)]

Devuelve una nueva fecha como resultado de agregar un número determinado de segundos a una fecha. Para restar segundos, introduzca un número negativo.

>[!INFO]
>
>**Ejemplos:**
>
>* `addSeconds(2016-12-08T15:55:57.536Z;2)`
>
>   Devuelve 2016-12-08T15:55:59,536Z
>
>* `addSeconds(2016-12-08T15:55:57.536Z;-2)`
>
>   Devuelve 2016-12-08T15:55:55,536Z

## [!UICONTROL addYears (fecha; número)]

Devuelve una nueva fecha como resultado de agregar un número determinado de años a una fecha. Para restar años, introduzca un número negativo.

>[!INFO]
>
>**Ejemplos:**
>
>* `addYears(2016-08-08T15:55:57.536Z;2)`
>
>    Devuelve 2018-08-08T15:55:57,536Z
>
>* `addYears(2016-12-08T15:55:57.536Z; -2)`
>
>    Devuelve 2014-08-08T15:55:57,536Z

## [!UICONTROL setSecond (fecha; número)]

Esta función devuelve una nueva fecha con los segundos especificados en parámetros.

Especifique un número del 0 al 59. Si el número está fuera de ese intervalo, la función devuelve un segundo desde el minuto anterior (para un número negativo) o un minuto posterior (para un número positivo).

Si necesita especificar un número fuera del intervalo, le recomendamos que utilice[!UICONTROL  addSeconds], tal como se describe más arriba en la sección [addSeconds (fecha; número)](#addseconds-date-number).

>[!INFO]
>
>**Ejemplos:**
>
>* `setSecond(2015-10-07T11:36:39.138Z;10)`
>
>    Devuelve 2015-10-07T11:36:10,138Z
>
>* `setSecond(2015-10-07T11:36:39.138Z; 6)`
>
>    Devuelve 2015-10-07T11:37:01,138Z

## [!UICONTROL setMinute (fecha; número)]

Esta función devuelve una nueva fecha con los minutos especificados en los parámetros.

Especifique un número del 0 al 59. Si el número está fuera de ese intervalo, la función devuelve un minuto desde la hora anterior (para un número negativo) o una hora posterior (para un número positivo).

Si necesita especificar un número fuera del intervalo, le recomendamos que utilice addMinutes, tal como se describe anteriormente en [addMinutes (fecha; número)](#addminutes-date-number).

>[!INFO]
>
>**Ejemplos:**
>
>* `setMinute(2015-10-07T11:36:39.138Z;10)`
>
>    Devuelve 2015-10-07T11:10:39,138Z
>
>* `setMinute(2015-10-07T11:36:39.138Z;61)`
>
>    Devuelve 2015-10-07T12:01:39,138Z

## [!UICONTROL setHour (date; number)]

Esta función devuelve una nueva fecha con la hora especificada en parámetros.

Especifique un número del 0 al 23. Si el número está fuera de este intervalo, la función devuelve una hora desde el día anterior (para un número negativo) o un día posterior (para un número positivo).

Si necesita especificar un número fuera del intervalo, le recomendamos que utilice addHours, tal como se describe anteriormente en [addHours (fecha; número)](#addhours-date-number).

>[!INFO]
>
>**Ejemplos:**
>
>* `setHour(2015-08-07T11:36:39.138Z;6)`
>
>   Devuelve 2015-08-07T06:36:39,138Z
>
>* `setHour(2015-08-07T11:36:39.138;-6)`
>
>    Devuelve 2015-08-06T18:36:39,138Z

## [!UICONTROL setDay (fecha; número/nombre del día en inglés)]

Esta función devuelve una nueva fecha con el día especificado en parámetros.

Puede utilizar esta función para establecer el día de la semana, con domingo como 1 y sábado como 7. Si especifica un número del 1 al 7, la fecha resultante se encuentra dentro de la semana actual (de domingo a sábado). Si el número está fuera de ese intervalo, la función devuelve un día de la semana anterior (para un número negativo) o de la semana siguiente (para un número positivo).

Si necesita especificar un número fuera del intervalo, le recomendamos que utilice addDays, tal como se describe anteriormente en [addDays (fecha; número)](#adddays-date-number).

>[!INFO]
>
>**Ejemplos:**
>
>* `setDay(2018-06-27T11:36:39.138Z;Monday)`
>
>   Devuelve 2018-06-25T11:36:39,138Z
>
>* `setDay(2018-06-27T11:36:39.138Z;1)`
>
>   Devuelve 2018-06-24T11:36:39,138Z
>
>* `setDay(2018-06-27T11:36:39.138Z;7)`
>
>   Devuelve 2018-06-30T11:36:39,138Z

## [!UICONTROL setDate (fecha; número)]

Esta función devuelve una nueva fecha con el día del mes especificado en parámetros.

Especifique un número del 1 al 31. Si el número está fuera de este intervalo, la función devuelve un día del mes anterior (para un número negativo) o del mes siguiente (para un número positivo).

>[!INFO]
>
>**Ejemplos:**
>
>* `setDate(2015-08-07T11:36:39.138Z;5)`
>
>   Devuelve 2015-08-05T11:36:39,138Z
>
>* `setDate(2015-08-07T11:36:39.138Z;32)`
>
>   Devuelve 2015-09-01T11:36:39,138Z

## [!UICONTROL setMonth (fecha; número/nombre del mes en inglés)]

Esta función devuelve una nueva fecha con el mes especificado en parámetros.

Especifique un número del 1 al 12. Si el número está fuera de este intervalo, la función devuelve el mes del año anterior (para un número negativo) o del año siguiente (para un número positivo).

>[!INFO]
>
>**Ejemplos:**
>
>* `setMonth(2015-08-07T11:36:39.138Z;5)`
>
>   Devuelve 2015-05-07T11:36:39,138Z
>
>* `setMonth(2015-08-07T11:36:39.138Z;17)`
>
>   Devuelve 2016-05-07T11:36:39,138Z
>
>* `setMonth(2015-08-07T11:36:39.138Z;january)`
>
>   Devuelve 2015-01-07T12:36:39,138Z

## [!UICONTROL setYear (fecha; número)]

Devuelve una nueva fecha con el año especificado en parámetros.

>[!INFO]
>
>**Ejemplo:**
>
>* `setYear(2015-08-07T11:36:39.138Z;2017)`
>
>   Devuelve 2017-08-07T11:36:39,138Z

## [!UICONTROL dateDifference (Date1; Date2; Unit)]

Devuelve un número que representa la diferencia entre las dos fechas, expresada en la unidad especificada.

Fecha2 se resta de Fecha1.

Utilice uno de los siguientes valores de tiempo para `unit` parámetro:

* milisegundos
* segundos
* minutos
* horas
* días
* semanas
* meses

Si no se especifica ninguna unidad, la función devuelve la diferencia en milisegundos.

>[!INFO]
>
>**Ejemplos:**
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z)`
>
>    Devuelve `600,000`
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;hours)`
>
>    Devuelve `4`
>
>* `dateDifference2021-06-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;months)`
>
>    Devuelve `1`

## Ejemplos adicionales

### Cómo calcular el n-º día de la semana del mes

Esta sección está adaptada para [!DNL Workfront Fusion] desde el [!DNL Exceljet] página web que explica cómo obtener el enésimo día de la semana de un mes.

Si necesita calcular una fecha correspondiente al n-º día de la semana del mes (por ejemplo, primer martes, tercer viernes, etc.), puede utilizar la siguiente fórmula:

![](assets/date&time-functions-calc-nth-day-350x31.png)

```
{{addDays(setDate(1.date; 1); 1.n * 7 - formatDate(addDays(setDate(1.date; 1); "-" + 1.dow); "E"))}}
```

La fórmula contiene los siguientes elementos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>1.n</code> </td> 
   <td> <p> Día n:</p> 
    <ul> 
     <li><code>1</code> para el primer martes</li> 
     <li><code>2</code> para el 2.º martes</li> 
     <li><code>3</code> para el tercer martes, etc</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>2.dow</code> </td> 
   <td> <p> día de la semana:</p> 
    <ul> 
     <li><code>1</code> para el lunes</li> 
     <li><code>2</code> para el martes</li> 
     <li><code>3</code> para el miércoles</li> 
     <li><code>4</code> para el jueves</li> 
     <li><code>5</code> para el viernes</li> 
     <li><code>6</code> para el sábado</li> 
     <li><code>7</code> para el domingo</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>1.date</code> </td> 
   <td> <p> La fecha determina el mes. Para calcular el n-º día de la semana del mes actual utilice la variable <code>now</code> variable.</p> </td> 
  </tr> 
 </tbody> 
</table>

Si desea calcular solo un caso específico, por ejemplo, cada segundo miércoles, puede reemplazar los elementos `1.n` y `2.dow` en la fórmula con los números correspondientes. Para el segundo miércoles del mes actual, se utilizarían los siguientes valores:

* `1.n` = `2`
* `1.dow` = `3`
* `1.date` = `now`

![](assets/nth-day-variable-value-350x33.png)

### Explicación:

* `setDate(now;1)` devuelve el primero del mes actual
* `formatDate(....;E)` devuelve el día de la semana (1, 2, ... 6)

## Cálculo de días entre fechas

Una posibilidad es utilizar la siguiente expresión:

![](assets/calculate-days-between-dates-350x68.png)

```
{{round((2.value - 1.value) / 1000 / 60 / 60 / 24)}}
```

>[!NOTE]
>
>* Valores de `D1`y `D2` deben ser valores de tipo Fecha. Si son valores de tipo cadena (por ejemplo, 20.10.2018), utilice el `parseDate()` para convertirlos en valores de tipo Fecha.
>
>* El `round()` se utiliza para casos en los que una de las fechas se encuentra dentro del período de horario de verano y la otra no. En estos casos, la diferencia de horas es de una hora menos o más. Puede dividirlo entre 24 para obtener un resultado que no sea entero. Pierdes una hora de horario de verano. El redondeo lo aplana para que no tenga ningún porcentaje

### Cómo calcular el último día/milisegundo del mes

Cuando se especifica un intervalo de fechas, por ejemplo, en un módulo de búsqueda, si el intervalo abarca todo el mes anterior como un intervalo cerrado (el intervalo que incluye ambos puntos límite), se debe calcular el último día del mes.

01-09-2019 ≤ D ≤ 30-09-2019

La fórmula siguiente muestra una forma de calcular el último día del mes anterior:

![](assets/last-day-prev-month.png)

```
{{addDays(setDate(now; 1); -1)}}
```

En algunos casos, debe calcular no solo el último día del mes, sino literalmente su último milisegundo:

01-09-2019 T00:00:00.000Z ≤ D ≤ 2019-09-30T23:59:59,999Z

Esta fórmula muestra una forma de calcular el último milisegundo del mes anterior:

![](assets/last-millisecond-prev-month-350x45.png)

```
{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD"; "UTC") - 1; "x")}}
```

Si necesita que el resultado utilice la configuración de zona horaria, omita el argumento UTC:

![](assets/omit-utc-argument-350x45.png)

`{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD") - 1; "x")}}`

Sin embargo, es preferible utilizar el intervalo de semiapertura en su lugar (el intervalo que excluye uno de sus puntos límite), especificando el primer día del mes siguiente en su lugar y sustituyendo el operador &quot;menor o igual que&quot; por &quot;menor que&quot; de la siguiente manera:

`2019-09-01 ≤ D < 2019-10-01`

`2019-09-01T00:00:00.000Z ≤ D < 2019-10-01T00:00:00.000Z`
