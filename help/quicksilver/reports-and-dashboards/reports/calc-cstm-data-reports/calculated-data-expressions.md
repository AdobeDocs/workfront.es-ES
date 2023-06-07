---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Expresiones de datos calculadas
description: Puede utilizar expresiones de datos para definir campos de datos personalizados calculados en Adobe Workfront. Conectan los campos de Workfront existentes en las instrucciones que generan un nuevo campo.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '2368'
ht-degree: 7%

---

# Expresiones de datos calculadas

Puede utilizar expresiones de datos para definir campos de datos personalizados calculados en Adobe Workfront. Conectan los campos de Workfront existentes en las instrucciones que generan un nuevo campo.

Puede utilizar expresiones de datos calculados en:

* Un formulario personalizado

   Para obtener más información sobre la creación de campos de datos personalizados calculados en formularios personalizados en Workfront, consulte [Añadir datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Columna personalizada calculada en un informe o una lista, cuando se utiliza el modo de texto

   Para obtener más información sobre el uso del modo de texto en informes y vistas, consulte [Introducción al modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Sintaxis de campos personalizados calculados frente a columnas personalizadas calculadas

Aunque las funciones que utiliza son las mismas, la sintaxis para crear una expresión en un campo personalizado calculado puede ser diferente de la que se utiliza para crear una columna personalizada calculada.

Por ejemplo:

* En un campo personalizado, en un formulario personalizado para tareas, debe utilizar lo siguiente para generar el nombre del proyecto principal de la tarea donde se adjunta el formulario personalizado:

   ```
   {project}.{name}
   ```

* En una columna personalizada de un informe, utilizaría lo siguiente para agregar una columna personalizada Nombre del proyecto en un informe de tareas:

   ```
   valuefield=project:name
   ```

   O

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >La misma sintaxis se aplica a todos los elementos de creación de informes en modo de texto donde se utilizan expresiones calculadas: vistas, filtros, agrupaciones, indicadores.

Las diferencias entre las dos sintaxis son las siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Campo personalizado calculado</strong></td> 
   <td><strong>Elemento de informe personalizado calculado</strong></td> 
  </tr> 
   <td>Escriba los nombres de los campos entre llaves.</td> 
   <td>No escriba los nombres de los campos entre corchetes o paréntesis cuando los utilice en una <code>valuefield </code>línea. <p>Incluya los nombres de los campos entre llaves cuando los utilice en una <code>valueexpression</code> línea.</p> </td> 
  </tr> 
  <tr> 
   <td>Separe los campos por puntos.</td> 
   <td> <p>Separe los campos por dos puntos al usarlos en una <code>valuefield </code>línea</p> <p>Separe los campos por puntos al usarlos en una <code>valueexpression </code>línea. </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre la sintaxis que debe utilizar en una columna personalizada calculada, consulte [Introducción al modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Expresiones de datos que puede utilizar

Las siguientes listas definen las expresiones disponibles que puede utilizar al crear uno de los tres tipos diferentes de campos personalizados calculados en Workfront:

* [Campos personalizados calculados por fecha y hora](#date-time-calculated-custom-fields)
* [Campos personalizados calculados matemáticos](#mathematical-calculated-custom-fields)
* [Campos personalizados calculados de texto](#text-calculated-custom-fields)

### Campos personalizados calculados por fecha y hora {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Si crea un cálculo de fecha y hora que no incluye una parte de hora o que utiliza los caracteres comodín de fecha $$TODAY o $$NOW, el sistema utilizará la fecha según la zona horaria universal coordinada (UTC), no según la zona horaria local. Esto puede provocar un resultado de fecha inesperado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expresión</th> 
   <th>Explicación y ejemplo</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>Esta expresión agrega el número de días a la fecha. El valor numérico puede incluir días parciales (por ejemplo, 1,5 añadirá un día y medio a la fecha).</p> <p>La expresión tiene el siguiente formato:</p><pre>ADDDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Esta expresión agrega el número de días de la semana a la fecha. Esta expresión solo agrega valores enteros a la fecha, redondeando hacia abajo. </p> <p>La expresión tiene el siguiente formato:</p><pre>ADDWEEKDAYS(fecha, cantidad)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Esta expresión agrega el número de meses a la fecha y tiene el siguiente formato:</p><pre>ADDMONTHS(fecha, número)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Esta expresión agrega el número de años a la fecha y tiene el siguiente formato:</p><pre>ADDYEARS(fecha, número)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Esta expresión borra la parte de hora de una fecha y tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>Esta expresión convierte una cadena en una fecha y tiene el siguiente formato:</p><pre>DATE(cadena)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Esta expresión devuelve el número de días entre las dos fechas, teniendo en cuenta los días de inicio y finalización del periodo seleccionado, así como las marcas de tiempo de esos días. Por ejemplo, si la hora de inicio de la fecha de inicio es 15:00, el día de inicio no se contará como un día completo.</p> <p>La expresión tiene el siguiente formato:</p><pre>DATEDIFF(fecha1, fecha2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Esta expresión devuelve el día del mes de la fecha en forma de número, entre 1 y 31.</p> <p>La expresión tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Esta expresión devuelve el día de la semana de la fecha en forma de número, entre 1 (domingo) y 7 (sábado).</p> <p>La expresión tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Esta expresión devuelve el total de días del mes de la fecha en forma de número y tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Esta expresión devuelve el total de días de la semana entre la fecha y el final de la semana o el final del mes, lo que ocurra primero. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p> <p>La expresión tiene el siguiente formato:</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Esta expresión devuelve el total de días del año de la fecha en forma de número y tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Esta expresión devuelve la última fecha de la lista y tiene el siguiente formato:</p><pre>DMAX(fecha1, fecha2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Esta expresión devuelve la fecha más temprana de la lista y tiene el siguiente formato:</p><pre>DMIN(fecha1, fecha2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>Esta expresión devuelve la hora de la fecha en forma de número entre 0 y 23.</p> <p>La expresión tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>Esta expresión devuelve el minuto de la fecha en forma de número entre 0 y 60, con el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MONTH</strong> </td> 
   <td> <p>Esta expresión devuelve el mes de la fecha en forma de número entre 1 y 12, con el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>Esta expresión devuelve el segundo de la fecha como un número entre 0 y 60, con el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Esta expresión devuelve el número de días de la semana entre dos fechas, teniendo en cuenta los días de inicio y finalización del periodo seleccionado, así como las marcas de tiempo de esos días. Por ejemplo, si la hora de inicio de la fecha de inicio es 15:00, el día de inicio no se contará como un día completo.</p> <p>La expresión tiene el siguiente formato:</p><pre>WEEKDAYDIFF(fecha2, fecha1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Esta expresión devuelve el número de minutos programados entre las fechas según el horario predeterminado.</p> <p>La expresión tiene el siguiente formato:</p><pre>WORKMINUTESDIFF(fecha1, fecha2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>AÑO</strong> </td> 
   <td> <p>Esta expresión devuelve el año de la fecha como un número de 4 dígitos, con el formato siguiente. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>YEAR({entryDate})</pre> </td> 
  </tr> 
 </tbody> 
</table>

### Campos personalizados calculados matemáticos {#mathematical-calculated-custom-fields}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expresión</th> 
   <th>Explicación</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ABS</strong> </td> 
   <td>Esta expresión devuelve el valor absoluto del número y tiene el siguiente formato. En este ejemplo se utiliza el número de objetos situados debajo del objeto donde está adjunto el formulario personalizado.<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>Esta expresión devuelve el promedio de números y tiene el siguiente formato:<pre>AVERAGE(número1, número2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Esta expresión redondea un número hacia arriba hasta el entero más próximo y tiene el siguiente formato. En este ejemplo se utiliza el número de objetos situados debajo del objeto donde está adjunto el formulario personalizado.<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Esta expresión divide todos los números en el orden proporcionado y tiene el siguiente formato:<pre>DIV(número1, número2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Esta expresión redondea un número hacia abajo hasta el entero más próximo y tiene el siguiente formato. En este ejemplo se utiliza el número de objetos situados debajo del objeto donde está adjunto el formulario personalizado.<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Esta expresión devuelve el valor de logaritmo natural del número y tiene el siguiente formato:<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Esta expresión devuelve el valor de logaritmo del número2 en base el número1 y tiene el siguiente formato:<pre>LOG(número1, número2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Esta expresión devuelve el elemento más grande de la lista y tiene el siguiente formato:<pre>MAX(elemento1, elemento2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Esta expresión devuelve el elemento más pequeño de la lista y tiene el siguiente formato:<pre>MIN(elemento1, elemento2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>NÚMERO</strong> </td> 
   <td>Esta expresión convierte una cadena en un número y tiene el siguiente formato:<pre>NUMBER(cadena)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Esta expresión devuelve un número elevado a una potencia y tiene el siguiente formato:<pre>POWER(número, potencia)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Esta expresión multiplica todos los números y tiene el siguiente formato:<pre>PROD(número1, número2, ....)</pre>
   <b>NOTA</b>

Al multiplicar los campos que contienen horas, asegúrese de comprender si las horas de los campos seleccionados se guardan en minutos, horas o segundos en la base de datos. Si las horas se guardan en minutos o segundos pero se muestran en horas en la interfaz de Workfront, es posible que tenga que tener en cuenta la conversión de minutos o segundos a horas al escribir una expresión con este cálculo.
</td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>Esta expresión redondea el número hacia arriba hasta los decimales de precisión especificados y tiene el siguiente formato:<p>ROUND(número, precisión)</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Esta expresión ordena los números en orden ascendente y tiene el siguiente formato:</p><pre>SORTASCNUM(número1, número2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Esta expresión ordena los números en orden descendente y tiene el siguiente formato:<pre>SORTDESCNUM(número1, número2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Esta expresión devuelve una raíz cuadrada de un número y tiene el siguiente formato. En este ejemplo se utiliza el número de objetos situados debajo del objeto donde está adjunto el formulario personalizado.</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Esta expresión resta todos los números en el orden proporcionado y tiene el siguiente formato:<pre>SUB(número1, número2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Esta expresión suma todos los números y tiene el siguiente formato:<pre>SUM(número1, número2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### Campos personalizados calculados de texto {#text-calculated-custom-fields}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expresión</th> 
   <th>Explicación</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>CASE</strong> </td> 
   <td> <p>Esta expresión se utiliza con otras expresiones para elegir un valor de una lista, basado en un número de índice. Un número de índice es un campo o una función que devuelve un valor numérico (normalmente en un intervalo conocido).</p> <p>La expresión tiene el siguiente formato:</p><pre>CASE(númeroDeÍndice, valor1, valor2, ...)</pre> <p>Por ejemplo, la siguiente expresión devuelve el nombre del día de la semana, donde 1=domingo, 2=lunes, etc., en una columna calculada:</p><pre>CASE(DAYOFWEEK({entryDate}),"Domingo","Lunes","Martes","Miércoles","Jueves","Viernes","Sábado")</pre> <p>Esta expresión funciona mejor con otras expresiones que devuelven un número, como DAYOFWEEK, DAYOFMONTH y MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Esta expresión concatena la cadena y tiene el siguiente formato:</p><pre>CONCAT(cadena1,"separador", cadena2)</pre> <p>Los siguientes son ejemplos de separadores que puede incluir:</p> 
    <ul> 
     <li>un espacio: " "</li> 
     <li>un guión: "-"</li> 
     <li>una barra diagonal: "/"</li> 
     <li>una coma: ","</li> 
     <li>una palabra: "o", "y"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTAINS</strong> </td> 
   <td>Esta expresión devuelve true si la cadena texto se encuentra dentro de la cadena enTexto y tiene el siguiente formato:<pre>CONTAINS(texto, enTexto)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Esta expresión omite cualquier carácter especial de la cadena para que se pueda incluir en un argumento URL.<p>La expresión tiene el siguiente formato:</p><pre>ENCODEURL(cadena)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Esta expresión evalúa una condición especificada y devuelve el valor de la expresión verdadera si es verdadera o el valor de la expresión falsa si es falsa.</p> <p>La expresión tiene el siguiente formato:</p><pre>IF(condición, Expresión verdadera, Expresión falsa)</pre> <p>Por ejemplo, puede comparar dos campos de fecha diferentes seguidos de un resultado Verdadero/Falso como cadena de datos:</p><pre>IF({projectCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</pre> <p>En el discurso diario, esta afirmación significa: "SI la fecha proyectada de finalización de mi objeto es 'Buena que' la fecha planificada de finalización de mi mismo objeto, entonces muestre las palabras 'Desfasado' en este campo; de lo contrario, muestre las palabras 'En seguimiento'".</p> <p>Si no desea etiquetar las expresiones true o false, debe insertar una etiqueta en blanco en la instrucción, como:</p><pre>IF({projectCompletionDate}&gt;{plannedCompletionDate},"","On Track")</pre> <p>O</p><pre>IF({projectCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</pre> <p>Para obtener más información sobre la creación de instrucciones "IF", consulte <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">Información general sobre las instrucciones "IF"</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Esta expresión le permite buscar un valor específico en una cadena de valores posibles. Si el valor que busca es igual a uno de los valores proporcionados, la expresión devuelve la expresión verdadera; de lo contrario, devuelve la expresión falsa.</p> <p>La expresión tiene el siguiente formato:</p><pre>IFIN(valor, valor1, valor2,..., expresión_verdadero, expresión_falso)</pre> <p>Por ejemplo, puede encontrar un Propietario del proyecto específico y marcar esos proyectos con una etiqueta especificada en una vista de proyecto: <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> En el discurso diario, esta declaración significa: "Si el propietario del proyecto es Jennifer Campbell o Rick Kuvec, marque este proyecto con 'Equipo de marketing'; de lo contrario, márquelo con 'Otros equipos'".</p> <p> Si no desea etiquetar las expresiones true o false, debe insertar una etiqueta en blanco en la instrucción, como: </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>O </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>EN</strong> </td> 
   <td> <p>Esta expresión devuelve true si el valor es igual a uno de los valores proporcionados; de lo contrario, la expresión devuelve false.</p> <p>La expresión tiene el siguiente formato:</p><pre>IN(valor, valor1[, valor2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Esta expresión devuelve true si el valor es nulo o está vacío; de lo contrario, la expresión devuelve false.</p> <p>La expresión tiene el siguiente formato:</p><pre>ISBLANK(valor)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>Esta expresión devuelve un número especificado de caracteres desde el lado izquierdo de una cadena y tiene el siguiente formato:</p><pre>LEFT(cadena, longitud)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Esta expresión devuelve la longitud de una cadena y tiene el siguiente formato:</p><pre>LEN(cadena)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>Esta expresión devuelve la cadena en minúsculas y tiene el siguiente formato:<pre>LOWER(cadena)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>REEMPLAZAR</strong> </td> 
   <td> <p>Esta expresión reemplaza todas las apariciones de cadena2 por cadena3 en cadena1.</p> <p>La expresión tiene el siguiente formato:</p><pre>REPLACE(cadena1, cadena2, cadena3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>Esta expresión devuelve un número especificado de caracteres desde el lado derecho de una cadena y tiene el siguiente formato:</p><pre>RIGHT(cadena, longitud)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>Esta expresión devuelve el índice de la primera aparición de texto en la cadena enTexto, comenzando en la posición de inicio dada o -1 si no se encuentra el texto.</p> <p>La expresión tiene el siguiente formato:</p><pre>SEARCH(texto, enTexto, inicio)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CADENA</strong> </td> 
   <td> <p>Esta expresión convierte un número en una cadena y tiene el siguiente formato:</p><pre>STRING(número)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Esta expresión ordena una lista de cadenas en orden ascendente y tiene el siguiente formato:</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Esta expresión ordena una lista de cadenas en orden descendente y tiene el siguiente formato:</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Esta expresión devuelve los caracteres de una cadena basándose en el índice inicial y final especificado y tiene el siguiente formato:</p><pre>SUBSTR({string}, número de posición inicial, número de posición final)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Esta expresión elimina el espacio en blanco del principio y del final de una cadena y tiene el siguiente formato:</p><pre>TRIM(cadena)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>Esta expresión devuelve una cadena en mayúsculas y tiene el siguiente formato:</p><pre>UPPER(cadena)</pre> </td> 
  </tr> 
 </tbody> 
</table>
