---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Expresiones de datos calculadas
description: Puede utilizar expresiones de datos para definir campos de datos personalizados calculados en Adobe Workfront. Conectan campos Workfront existentes en instrucciones que generan un nuevo campo.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 22438c38727f5cc36b07b3530818f5bda2b0bacf
workflow-type: tm+mt
source-wordcount: '2270'
ht-degree: 7%

---

# Expresiones de datos calculadas

Puede utilizar expresiones de datos para definir campos de datos personalizados calculados en Adobe Workfront. Conectan campos Workfront existentes en instrucciones que generan un nuevo campo.

Puede utilizar expresiones de datos calculados en:

* Un formulario personalizado

   Para obtener más información sobre la creación de campos de datos personalizados calculados en formularios personalizados en Workfront, consulte [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Columna personalizada calculada en un informe o lista, cuando se usa el modo de texto

   Para obtener más información sobre el uso del modo de texto en los informes y las vistas, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Sintaxis de campos personalizados calculados frente a columnas personalizadas calculadas

Aunque las funciones que utiliza son las mismas, la sintaxis para crear una expresión en un campo personalizado calculado puede ser diferente que para crear una columna personalizada calculada.

Por ejemplo:

* En un campo personalizado, en un formulario personalizado para tareas, se utilizaría lo siguiente para generar el nombre del proyecto principal de la tarea donde está adjunto el formulario personalizado:

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
   >La misma sintaxis se aplica a todos los elementos de informes en modo de texto donde se utilizan expresiones calculadas: vistas, filtros, agrupaciones, mensajes.

Las diferencias entre las dos sintaxis son:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Campo personalizado calculado</strong></td> 
   <td><strong>Elemento de informe personalizado calculado</strong></td> 
  </tr> 
   <td>Escriba los nombres de los campos entre llaves.</td> 
   <td>No escriba nombres de campo entre corchetes o paréntesis al utilizarlos en una <code>valuefield </code>línea. <p>Rellene los nombres de campo entre llaves al utilizarlos en una <code>valueexpression</code> línea.</p> </td> 
  </tr> 
  <tr> 
   <td>Separe los campos por puntos.</td> 
   <td> <p>Separe los campos por dos puntos al utilizarlos en una <code>valuefield </code>line</p> <p>Separe los campos por puntos al utilizarlos en un <code>valueexpression </code>línea. </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre la sintaxis que debe utilizar en una columna personalizada calculada, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Expresiones de datos que puede utilizar

Las listas siguientes definen las expresiones disponibles que puede utilizar al crear uno de los 3 tipos diferentes de campos personalizados calculados en Workfront:

* [Campos personalizados calculados por fecha y hora](#date-time-calculated-custom-fields)
* [Campos personalizados calculados matemáticos](#mathematical-calculated-custom-fields)
* [Campos personalizados y calculados de texto](#text-calculated-custom-fields)

### Campos personalizados calculados por fecha y hora {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Si crea un cálculo de fecha y hora que no incluye una parte de tiempo, o que utiliza los comodines de fecha $$TODAY o $$Now, el sistema utiliza la fecha según la zona de Hora Universal Coordinada (UTC), no según la zona horaria local. Esto puede provocar un resultado de fecha inesperado.

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
   <td> <p>Esta expresión agrega el número de días a la fecha y tiene el formato siguiente:</p><pre>ADDDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Esta expresión agrega el número de días de la semana a la fecha y tiene el formato siguiente:</p><pre>ADDWEEKDAYS(fecha, cantidad)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Esta expresión agrega el número de meses a la fecha y tiene el siguiente formato:</p><pre>ADDMONTHS(fecha, número)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Esta expresión agrega el número de años a la fecha y tiene el formato siguiente:</p><pre>ADDYEARS(fecha, número)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Esta expresión borra la parte de tiempo de una fecha y tiene el formato siguiente. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>Esta expresión convierte una cadena en una fecha y tiene el formato siguiente:</p><pre>DATE(cadena)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Esta expresión devuelve el número de días entre las dos fechas, teniendo en cuenta los días de inicio y fin del periodo seleccionado, así como las marcas de hora de esos días. Por ejemplo, si la hora de inicio de la fecha de inicio es 3 p. m., el día de inicio no se contará como un día completo.</p> <p>La expresión tiene el formato siguiente:</p><pre>DATEDIFF(fecha1, fecha2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Esta expresión devuelve el día del mes de la fecha como un número, entre 1 y 31.</p> <p>La expresión tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Esta expresión devuelve el día de la semana de la fecha como un número, entre 1 (domingo) y 7 (sábado).</p> <p>La expresión tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Esta expresión devuelve el total de días del mes de la fecha como un número y tiene el formato siguiente. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Esta expresión devuelve el total de días laborables entre la fecha y el final de la semana, o el final del mes, lo que suceda primero. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p> <p>La expresión tiene el formato siguiente:</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Esta expresión devuelve el total de días del año de la fecha como un número y tiene el formato siguiente. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Esta expresión devuelve la fecha más reciente de la lista y tiene el siguiente formato:</p><pre>DMAX(fecha1, fecha2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Esta expresión devuelve la fecha más temprana de la lista y tiene el siguiente formato:</p><pre>DMIN(fecha1, fecha2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>Esta expresión devuelve la hora de la fecha como un número entre 0 y 23.</p> <p>La expresión tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>Esta expresión devuelve el minuto de la fecha como un número entre 0 y 60, con el formato siguiente. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MONTH</strong> </td> 
   <td> <p>Esta expresión devuelve el mes de la fecha como un número entre 1 y 12, con el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>Esta expresión devuelve el segundo de la fecha como un número entre 0 y 60, con el formato siguiente. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Esta expresión devuelve el número de días laborables entre dos fechas, teniendo en cuenta los días de inicio y fin del periodo seleccionado, así como las marcas de hora de esos días. Por ejemplo, si la hora de inicio de la fecha de inicio es 3 p. m., el día de inicio no se contará como un día completo.</p> <p>La expresión tiene el formato siguiente:</p><pre>WEEKDAYDIFF(fecha2, fecha1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Esta expresión devuelve el número de minutos programados entre las fechas según la programación predeterminada.</p> <p>La expresión tiene el formato siguiente:</p><pre>WORKMINUTESDIFF(fecha1, fecha2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>AÑO</strong> </td> 
   <td> <p>Esta expresión devuelve el año de la fecha como un número de 4 dígitos, con el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p><pre>YEAR({entryDate})</pre> </td> 
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
   <td>Esta expresión devuelve el valor absoluto del número y tiene el siguiente formato. En este ejemplo se utiliza el número de objetos situados debajo del objeto al que se adjunta el formulario personalizado.<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>Esta expresión devuelve el promedio de números y tiene el formato siguiente:<pre>AVERAGE(número1, número2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Esta expresión redondea un número al entero más cercano y tiene el siguiente formato. En este ejemplo se utiliza el número de objetos situados debajo del objeto al que se adjunta el formulario personalizado.<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Esta expresión divide todos los números en el orden proporcionado y tiene el formato siguiente:<pre>DIV(número1, número2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Esta expresión redondea un número al entero más cercano y tiene el formato siguiente. En este ejemplo se utiliza el número de objetos situados debajo del objeto al que se adjunta el formulario personalizado.<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Esta expresión devuelve el valor logaritmo natural del número y tiene el formato siguiente:<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Esta expresión devuelve el valor logarítmico de number2 al número base1 y tiene el siguiente formato:<pre>LOG(número1, número2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Esta expresión devuelve el elemento más grande de la lista y tiene el formato siguiente:<pre>MAX(elemento1, elemento2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Esta expresión devuelve el elemento más pequeño de la lista y tiene el siguiente formato:<pre>MIN(elemento1, elemento2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>NÚMERO</strong> </td> 
   <td>Esta expresión convierte una cadena en un número y tiene el formato siguiente:<pre>NUMBER(cadena)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Esta expresión devuelve un número elevado a una potencia y tiene el formato siguiente:<pre>POWER(número, potencia)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Esta expresión multiplica todos los números y tiene el formato siguiente:<pre>PROD(número1, número2, ....)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>Esta expresión redondea el número a decimales especificados de precisión y tiene el formato siguiente:<p>ROUND(número, precisión)</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Esta expresión ordena los números en orden ascendente y tiene el formato siguiente:</p><pre>SORTASCNUM(número1, número2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Esta expresión ordena los números en orden descendente y tiene el formato siguiente:<pre>SORTDESCNUM(número1, número2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Esta expresión devuelve una raíz cuadrada de un número y tiene el siguiente formato. En este ejemplo se utiliza el número de objetos situados debajo del objeto al que se adjunta el formulario personalizado.</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Esta expresión resta todos los números en el orden proporcionado y tiene el formato siguiente:<pre>SUB(número1, número2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Esta expresión agrega todos los números y tiene el formato siguiente:<pre>SUM(número1, número2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### Campos personalizados y calculados de texto {#text-calculated-custom-fields}

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
   <td> <p>Esta expresión se utiliza con otras expresiones para elegir un valor de una lista, basado en un número de índice. Un número de índice es un campo o función que devuelve un valor numérico (normalmente en un intervalo conocido).</p> <p>La expresión tiene el formato siguiente:</p><pre>CASE(indexNumber, value1, value2, ...)</pre> <p>Por ejemplo, la siguiente expresión devuelve el nombre del día de la semana, donde 1=domingo, 2=lunes, etc., en una columna calculada:</p><pre>CASE(DAYOFWEEK({entryDate}),"Sunday","Lunes","Martes", "Miércoles", "Jueves", "Viernes", "Sábado")</pre> <p>Esta expresión funciona mejor con otras expresiones que devuelven un número, como DAYOFWEEK, DAYOFMONTH y MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Esta expresión concatena la cadena y tiene el formato siguiente:</p><pre>CONCAT(string1,"separator", string2)</pre> <p>Los siguientes son ejemplos de separadores que puede incluir:</p> 
    <ul> 
     <li>un espacio: "</li> 
     <li>un guión: "-"</li> 
     <li>una barra oblicua: "/"</li> 
     <li>una coma: ","</li> 
     <li>una palabra: "o", "y"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTAINS</strong> </td> 
   <td>Esta expresión devuelve el valor "True" si la cadena findText se encuentra dentro de la cadena WithinText y tiene el formato siguiente:<pre>CONTAINS(texto, enTexto)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Esta expresión omite cualquier carácter especial de la cadena para que se pueda incluir en un argumento de URL.<p>La expresión tiene el formato siguiente:</p><pre>ENCODEURL(cadena)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Esta expresión evalúa una condición que especifica y devuelve el valor de trueExpression si es true o el valor de falseExpression si es false.</p> <p>La expresión tiene el formato siguiente:</p><pre>IF(condición, Expresión verdadera, Expresión falsa)</pre> <p>Por ejemplo, puede comparar dos campos de fecha diferentes seguidos de un resultado Verdadero/Falso como una cadena de datos:</p><pre>IF({estimatedCompletionDate}&gt;{scheduledCompletionDate},"Off Track","On Track")</pre> <p>En el discurso cotidiano, esta declaración significa: "SI la fecha de finalización prevista de mi objeto es "Buena que" la fecha de finalización prevista de mi mismo objeto, en este campo se mostrarán las palabras "Fuera de pista"; de lo contrario, muestre las palabras 'On Track'".</p> <p>Si no desea etiquetar las expresiones true o false, debe insertar una etiqueta en blanco en la instrucción, como:</p><pre>IF({estimatedCompletionDate}&gt;{scheduledCompletionDate},"","On Track")</pre> <p>O</p><pre>IF({estimatedCompletionDate}&gt;{scheduledCompletionDate},"Off Track",")</pre> <p>Para obtener más información sobre la creación de instrucciones "IF", consulte <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">Resumen de las instrucciones "IF"</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Esta expresión le permite buscar un valor específico en una cadena de valores posibles. Si el valor que busca es igual a uno de los valores proporcionados, la expresión devuelve trueExpression; de lo contrario, devuelve falseExpression.</p> <p>La expresión tiene el formato siguiente:</p><pre>IFIN(value, value1, value2,..., trueExpression, falseExpression)</pre> <p>Por ejemplo, puede encontrar un propietario de proyecto específico y marcar esos proyectos con una etiqueta especificada en una vista de proyecto: <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> En el discurso cotidiano, esta declaración significa: "Si el propietario del proyecto es Jennifer Campbell o Rick Kuvec, marque este proyecto con 'Marketing Team'; de lo contrario, marque con "Otros equipos"."</p> <p> Si no desea etiquetar las expresiones true o false, debe insertar una etiqueta en blanco en la instrucción, como: </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>O </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>EN</strong> </td> 
   <td> <p>Esta expresión devuelve el valor "True" si el valor es igual a uno de los valores proporcionados; en caso contrario, la expresión devuelve false.</p> <p>La expresión tiene el formato siguiente:</p><pre>IN(valor, valor1[, valor2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Esta expresión devuelve el valor "True" si el valor es nulo o está vacío; en caso contrario, la expresión devuelve false.</p> <p>La expresión tiene el formato siguiente:</p><pre>ISBLANK(valor)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>Esta expresión devuelve un número especificado de caracteres de la parte izquierda de una cadena y tiene el formato siguiente:</p><pre>LEFT(cadena, longitud)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Esta expresión devuelve la longitud de una cadena y tiene el formato siguiente:</p><pre>LEN(cadena)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>Esta expresión devuelve la cadena en minúsculas y tiene el formato siguiente:<pre>LOWER(cadena)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>REEMPLAZAR</strong> </td> 
   <td> <p>Esta expresión reemplaza todas las ocurrencias de string2 con string3 en string1.</p> <p>La expresión tiene el formato siguiente:</p><pre>REPLACE(cadena1, cadena2, cadena3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>Esta expresión devuelve un número especificado de caracteres desde la derecha de una cadena y tiene el formato siguiente:</p><pre>RIGHT(cadena, longitud)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>Esta expresión devuelve el índice de la primera incidencia de findText en la cadena enText, empezando en la posición inicial determinada o -1 si no se encuentra el texto.</p> <p>La expresión tiene el formato siguiente:</p><pre>SEARCH(findText, WithinText, start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CADENA</strong> </td> 
   <td> <p>Esta expresión convierte un número en una cadena y tiene el formato siguiente:</p><pre>CADENA(número)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Esta expresión ordena una lista de cadenas en orden ascendente y tiene el formato siguiente:</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Esta expresión ordena una lista de cadenas en orden descendente y tiene el formato siguiente:</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Esta expresión devuelve caracteres de una cadena en función del índice inicial y final especificado y tiene el formato siguiente:</p><pre>SUBSTR({string}, número de posición inicial, número de posición final)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Esta expresión elimina los espacios en blanco del principio y del final de una cadena y tiene el formato siguiente:</p><pre>TRIM(cadena)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>Esta expresión devuelve una cadena en mayúsculas y tiene el formato siguiente:</p><pre>UPPER(cadena)</pre> </td> 
  </tr> 
 </tbody> 
</table>
