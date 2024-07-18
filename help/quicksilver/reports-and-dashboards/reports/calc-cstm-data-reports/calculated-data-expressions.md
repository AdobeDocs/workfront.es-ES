---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Resumen de las expresiones de datos calculados
description: Puede utilizar expresiones de datos para definir campos de datos personalizados calculados en Adobe Workfront. Las expresiones calculadas conectan los campos de Workfront existentes en las instrucciones que generan un nuevo campo.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '2165'
ht-degree: 0%

---

# Resumen de las expresiones de datos calculados

<!--Audited: 12/2023-->

Puede utilizar expresiones de datos para definir campos personalizados calculados en Adobe Workfront. Las expresiones calculadas conectan los campos de Workfront existentes en las instrucciones que generan un nuevo campo.

Puede utilizar expresiones de datos calculados en:

* Un campo personalizado calculado en un formulario personalizado

  Para obtener más información sobre la creación de campos personalizados calculados en formularios personalizados en Workfront, consulte [Agregar campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Columna personalizada calculada en un informe o una lista, cuando se utiliza el modo de texto

  Para obtener más información acerca del uso del modo de texto en informes y vistas, vea [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Sintaxis de campos personalizados calculados frente a columnas personalizadas calculadas

Aunque las funciones que utiliza son las mismas, la sintaxis para crear una expresión en un campo personalizado calculado puede ser diferente de la que utiliza para crear una columna personalizada calculada.

Las diferencias entre las dos sintaxis son las siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Campo personalizado calculado</strong></td> 
   <td><strong>Elemento de informe personalizado calculado</strong></td> 
  </tr> 
   <td>Incluir los nombres de los campos entre llaves</td> 
   <td>No escriba los nombres de los campos entre corchetes o paréntesis cuando los utilice en una <p><code>valuefield </code></p>línea. <p>Incluya los nombres de los campos entre llaves cuando los utilice en una <p><code>valueexpression</code></p> línea.</p> </td> 
  </tr> 
  <tr> 
   <td>Separar los campos por puntos</td> 
   <td> <p>Separe los campos por dos puntos al usarlos en una <p><code>valuefield </code></p>línea</p> <p>Separe los campos por puntos al usarlos en una <p><code>valueexpression </code></p>línea. </p> </td> 
  </tr> 
 </tbody> 
</table>

Por ejemplo:

* En un campo personalizado, en un formulario personalizado para tareas, debe utilizar lo siguiente para generar el nombre del proyecto principal de la tarea donde se adjunta el formulario personalizado:


  ` {project}.{name}`


* En una columna personalizada de un informe, utilizaría lo siguiente para agregar una columna personalizada Nombre del proyecto en un informe de tareas:


  `valuefield=project:name`


  O

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >La misma sintaxis se aplica a todos los elementos de creación de informes en modo de texto donde se utilizan expresiones calculadas: vistas, filtros, agrupaciones, indicadores.

Para obtener más información acerca de la sintaxis que debe usar en una columna personalizada calculada, vea [Introducción al modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Expresiones de datos que puede utilizar

Las siguientes listas definen las expresiones disponibles que puede utilizar al crear uno de los tres tipos diferentes de campos personalizados calculados en Workfront:

* [Campos personalizados calculados por fecha y hora](#date-time-calculated-custom-fields)
* [Campos personalizados calculados matemáticos](#mathematical-calculated-custom-fields)
* [Campos personalizados calculados de texto](#text-calculated-custom-fields)

Puede utilizar las expresiones enumeradas a continuación para crear columnas personalizadas calculadas. Sin embargo, debe utilizar la sintaxis correcta para una columna personalizada calculada, tal como se describe en la sección [Sintaxis de los campos personalizados calculados frente a columnas personalizadas calculadas](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) de este artículo.

### Campos personalizados calculados por fecha y hora {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Si crea un cálculo de fecha y hora que no incluye una parte de hora o que utiliza los caracteres comodín de fecha $$TODAY o $$NOW, el sistema utilizará la fecha según la zona horaria universal coordinada (UTC), no según la zona horaria local. Esto puede provocar un resultado de fecha inesperado.

Puede crear un campo personalizado calculado de fecha y hora con las siguientes expresiones:

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
   <td> <p>Añade el número de días a la fecha. El valor numérico puede incluir días parciales. Por ejemplo, 1,5 añade un día y medio a la fecha.</p> <p>La expresión tiene el siguiente formato:</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Agrega el número de días de la semana a la fecha. Esta expresión solo agrega valores enteros a la fecha, redondeando hacia abajo. </p> <p>La expresión tiene el siguiente formato:</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Añade el número de meses a la fecha y tiene el siguiente formato:

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Añade el número de años a la fecha y tiene el siguiente formato:</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Borra la parte de hora de una fecha y tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>FECHA</strong> </td> 
   <td> <p>Convierte una cadena en una fecha y tiene el siguiente formato:</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Devuelve el número de días entre las dos fechas, teniendo en cuenta los días de inicio y finalización del periodo seleccionado, así como las marcas de tiempo de esos días. Por ejemplo, si la hora de inicio de la fecha de inicio es 15:00, el día de inicio no se cuenta como un día completo.</p> <p>La expresión tiene el siguiente formato:</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Devuelve el día del mes de la fecha en forma de número, entre 1 y 31.</p> <p>La expresión tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Devuelve el día de la semana de la fecha en forma de número, entre 1 (domingo) y 7 (sábado).</p> <p>La expresión tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Devuelve el total de días del mes de la fecha en forma de número y tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Devuelve el total de días de la semana entre la fecha y el final de la semana o el final del mes, el que sea primero. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p> <p>La expresión tiene el siguiente formato:</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Devuelve el total de días del año de la fecha en forma de número y tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Devuelve la fecha más reciente en la lista y tiene el siguiente formato:</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADMINISTRADOR</strong> </td> 
   <td> <p>Devuelve la fecha más temprana de la lista y tiene el siguiente formato:</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>HORA</strong> </td> 
   <td> <p>Devuelve la hora de la fecha en forma de número entre 0 y 23.</p> <p>La expresión tiene el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTO</strong> </td> 
   <td> <p>Devuelve el minuto de la fecha en forma de número entre 0 y 60, con el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MES</strong> </td> 
   <td> <p>Devuelve el mes de la fecha en forma de número entre 1 y 12, con el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SEGUNDO</strong> </td> 
   <td> <p>Devuelve el segundo de la fecha en forma de número entre 0 y 60, con el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Devuelve el número de días de la semana entre dos fechas, teniendo en cuenta los días de inicio y finalización del periodo seleccionado, así como las marcas de tiempo de esos días. Por ejemplo, si la hora de inicio de la fecha de inicio es 15:00, el día de inicio no se contará como un día completo.</p> <p>La expresión tiene el siguiente formato:</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Devuelve la cantidad de minutos programados entre las fechas según el horario predeterminado.</p> <p>La expresión tiene el siguiente formato:</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>AÑO</strong> </td> 
   <td> <p>Devuelve el año de la fecha en un número de 4 dígitos con el siguiente formato. En este ejemplo, la fecha es la fecha de entrada de un objeto de trabajo.</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### Campos personalizados calculados matemáticos {#mathematical-calculated-custom-fields}

Puede crear un campo personalizado calculado que utilice algunas de las siguientes expresiones matemáticas:

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
   <td>Devuelve el valor absoluto del número y tiene el siguiente formato. En este ejemplo se utiliza el número de objetos situados debajo del objeto donde está adjunto el formulario personalizado.

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROMEDIO</strong> </td> 
   <td>Devuelve el promedio de números y tiene el siguiente formato:

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Redondea un número hacia arriba hasta el entero más próximo y tiene el siguiente formato. En este ejemplo se utiliza el número de objetos situados debajo del objeto donde está adjunto el formulario personalizado.

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Divide todos los números en el orden proporcionado y tiene el siguiente formato:

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PISO</strong> </td> 
   <td>Redondea un número hacia abajo hasta el entero más próximo y tiene el siguiente formato. En este ejemplo se utiliza el número de objetos situados debajo del objeto donde está adjunto el formulario personalizado.

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Devuelve el valor de logaritmo natural del número y tiene el siguiente formato:

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>REGISTRO</strong> </td> 
   <td>Devuelve el valor de logaritmo del número2 en base el número1 y tiene el siguiente formato:

<p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Devuelve el elemento más grande de la lista y tiene el siguiente formato:

<p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Devuelve el elemento más pequeño de la lista y tiene el siguiente formato:

<p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>NÚMERO</strong> </td> 
   <td>Convierte una cadena en un número y tiene el siguiente formato:<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>POTENCIA</strong> </td> 
   <td>Devuelve un número elevado a una potencia y tiene el siguiente formato:

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Multiplica todos los números y tiene el siguiente formato:

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>NOTA</b></p>

<p>Al multiplicar los campos que contienen horas, asegúrese de comprender si la base de datos guarda las horas de los campos seleccionados en minutos, horas o segundos. Si las horas se guardan en minutos o segundos pero se muestran en horas en la interfaz de Workfront, es posible que tenga que tener en cuenta la conversión de minutos o segundos a horas al escribir una expresión con este cálculo. </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>RONDA</strong> </td> 
   <td>Redondea el número hacia arriba para especificar los decimales de precisión y tiene el siguiente formato:

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Ordena los números en orden ascendente y tiene el siguiente formato:</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Ordena los números en orden descendente y tiene el siguiente formato:

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Devuelve la raíz cuadrada de un número y tiene el siguiente formato. En este ejemplo se utiliza el número de objetos situados debajo del objeto donde está adjunto el formulario personalizado.</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Resta todos los números en el orden proporcionado y tiene el siguiente formato:

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SUMA</strong> </td> 
   <td>Suma todos los números y tiene el siguiente formato:

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### Campos personalizados calculados de texto {#text-calculated-custom-fields}

Puede crear un campo personalizado calculado que muestre un valor con formato de texto mediante las siguientes expresiones:

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
   <td><strong>CASO</strong> </td> 
   <td> <p>Se utiliza con otras expresiones para elegir un valor de una lista, según un número de índice. </p>
   <p>Un número de índice es un campo o una función que devuelve un valor numérico (normalmente en un intervalo conocido).</p> 
   <p>La expresión tiene el siguiente formato:</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>Por ejemplo, la siguiente expresión devuelve el nombre del día de la semana, donde 1=domingo, 2=lunes, etc., en una columna calculada:</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>Funciona mejor con otras expresiones que devuelven un número, como DAYOFWEEK, DAYOFMONTH y MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Concatena la cadena y tiene el siguiente formato:</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>Los siguientes son ejemplos de separadores que puede incluir:</p> 
    <ul> 
     <li>un espacio: " "</li> 
     <li>un guión: "-"</li> 
     <li>una barra diagonal: "/"</li> 
     <li>una coma: ","</li> 
     <li>una palabra: "o", "y"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTIENE</strong> </td> 
   <td>Devuelve true si la cadena texto se encuentra dentro de la cadena enTexto y tiene el siguiente formato:

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Omite cualquier carácter especial de la cadena para que se pueda incluir en un argumento URL.<p>La expresión tiene el siguiente formato:</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SI</strong> </td> 
   <td> <p>Evalúa una condición especificada y devuelve el valor de la expresión verdadera si es verdadera o el valor de la expresión falsa si es falsa.</p>

<p>La expresión tiene el siguiente formato:</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>Por ejemplo, puede comparar dos campos de fecha diferentes seguidos de un resultado Verdadero/Falso como cadena de datos:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>En el discurso diario, esta afirmación significa: "SI la fecha proyectada de finalización de mi objeto es 'mayor que' que la fecha planificada de finalización de mi mismo objeto, entonces muestre las palabras 'Fuera de pista' en este campo; de lo contrario, muestre las palabras 'En pista'".</p>

<p>Si no desea etiquetar las expresiones true o false, debe insertar una etiqueta en blanco en la instrucción, como:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>O</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>Para obtener más información acerca de la creación de instrucciones "IF", vea <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref"> información general sobre instrucciones "IF"</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Permite buscar un valor específico en una cadena de valores posibles. Si el valor que busca es igual a uno de los valores proporcionados, la expresión devuelve la expresión verdadera; de lo contrario, devuelve la expresión falsa.</p> 
   <p>La expresión tiene el siguiente formato:</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>Por ejemplo, puede encontrar un Propietario del proyecto específico y marcar esos proyectos con una etiqueta especificada en una vista de proyecto: <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> En el discurso diario, esta declaración significa: "Si el propietario del proyecto es Jennifer Campbell o Rick Kuvec, marque este proyecto con 'Equipo de marketing'; de lo contrario, márquelo con 'Otros equipos'".</p> 
    <p> Si no desea etiquetar las expresiones true o false, debe insertar una etiqueta en blanco en la instrucción, como: </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>O </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>EN</strong> </td> 
   <td> <p>Devuelve verdadero si el valor equivale a uno de los valores proporcionados; de lo contrario, la expresión devuelve falso.</p> <p>La expresión tiene el siguiente formato:

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ESBLANCO</strong> </td> 
   <td> <p>Devuelve verdadero si el valor es nulo o está vacío; de lo contrario, la expresión devuelve falso.</p> <p>La expresión tiene el siguiente formato:

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>IZQUIERDA</strong> </td> 
   <td> <p>Devuelve un número especificado de caracteres desde el lado izquierdo de una cadena y tiene el siguiente formato:</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Devuelve la longitud de una cadena y tiene el siguiente formato:</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>INFERIOR</strong> </td> 
   <td>Devuelve la cadena en minúsculas y tiene el siguiente formato:

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>REEMPLAZAR</strong> </td> 
   <td> <p>Reemplaza todas las apariciones de cadena2 por cadena3 en cadena1.</p> <p>La expresión tiene el siguiente formato:</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DERECHO</strong> </td> 
   <td> <p>Devuelve el número de caracteres especificado del lado derecho de una cadena y tiene el siguiente formato:</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>BUSCAR</strong> </td> 
   <td> <p>Devuelve el índice de la primera aparición de texto en la cadena enTexto, comenzando en la posición de inicio dada o -1 si no se encuentra el texto.</p> <p>La expresión tiene el siguiente formato:</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>CADENA</strong> </td> 
   <td> <p>Convierte un número en una cadena y tiene el siguiente formato:</p>

<p><code>STRING(number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Ordena una lista de cadenas en orden ascendente y tiene el siguiente formato:</p>

<p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Ordena una lista de cadenas en orden descendente y tiene el siguiente formato:</p>

<p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Devuelve los caracteres de una cadena en función del índice inicial y final especificado y tiene el siguiente formato:</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>RECORTAR</strong> </td> 
   <td> <p>Elimina los espacios en blanco del principio y del final de una cadena y tiene el siguiente formato:</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUPERIOR</strong> </td> 
   <td> <p>Devuelve una cadena en mayúsculas con el siguiente formato:</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>
