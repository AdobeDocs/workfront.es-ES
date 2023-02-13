---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Resumen de las instrucciones IF
description: Puede utilizar instrucciones "IF" en lenguajes de programación generales. En Adobe Workfront, las instrucciones "IF" permiten comparar, dar formato y agrupar campos de datos para generar informes y datos personalizados. Además, pensar matemáticamente en las instrucciones "IF" conduce a un mejor entendimiento conceptual, ya que las variables para las expresiones se utilizan comúnmente.
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# Resumen de las instrucciones &quot;IF&quot;

Puede utilizar instrucciones &quot;IF&quot; en lenguajes de programación generales. En Adobe Workfront, las instrucciones &quot;IF&quot; permiten comparar, dar formato y agrupar campos de datos para generar informes y datos personalizados. Además, pensar matemáticamente en las instrucciones &quot;IF&quot; conduce a un mejor entendimiento conceptual, ya que las variables para las expresiones se utilizan comúnmente.

## Recommendations para instrucciones &quot;IF&quot;

Considere lo siguiente antes de crear una instrucción &quot;IF&quot;:

* Recomendamos una comprensión básica de cualquier lenguaje de programación general, pero no la necesitamos, para esta guía.
* Se requiere una comprensión avanzada de la sintaxis del modo de texto de Workfront. Esto ayuda a comprender la terminología de la API de Workfront y la sintaxis de los datos personalizados en estos formatos específicos.

   Para obtener información sobre la API de Workfront, consulte [Conceptos básicos de API](../../../wf-api/general/api-basics.md).

   Para obtener información sobre el uso del modo de texto, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* Puede crear instrucciones &quot;IF&quot; para los siguientes elementos de Workfront:

   * Vistas
   * Agrupaciones
   * Campos personalizados calculados

* No se pueden crear instrucciones &quot;IF&quot; para filtros. Esto resulta en un error &quot;Whoops&quot; en Workfront.
* El equipo de asistencia técnica no ayuda a crear datos personalizados. Puede ponerse en contacto con el equipo de asistencia después de crear los campos o columnas personalizados y de no ver los resultados deseados. Para obtener ayuda en la creación de una expresión, póngase en contacto con su ejecutivo de cuentas para solicitar información sobre nuestras opciones de consultoría.
* Se recomienda escribir estas expresiones en primer lugar en un editor de texto, como Sublime o Visual Studio Code, ya que esto le ayuda a ver los datos con más claridad de lo que aparecería en Workfront.

## Componentes de una instrucción &quot;IF&quot;

Puede crear instrucciones &quot;IF&quot; en Workfront con el siguiente formato:
<pre>IF(Condition,True Expression,False Expression)</pre>Los componentes de una instrucción "IF" son:

* **IF**= Esta es la expresión de datos calculados de Workfront para la &quot;función&quot;. Al igual que las expresiones SUM y PROD, esto primero indica al sistema que entienda la función como una instrucción &quot;IF&quot;. Utilice siempre mayúsculas para &quot;IF&quot; en esta instrucción.\
   Para obtener una lista de todas las expresiones de datos calculadas, consulte [Expresiones de datos calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **Condición**= Esta es la condición que debe cumplir la variable de Workfront y es la base de esta ecuación. Todo lo que se puede especificar posteriormente en la ecuación depende de la condición. Puede utilizar una serie de referencias, comparaciones o expresiones matemáticas para iniciar una ecuación. Algunos ejemplos de condiciones son:

   * Una fecha es buena que otra fecha en un objeto especificado.
   * Un estado es igual a uno de los estados disponibles en un objeto especificado.
   * El porcentaje de finalización de una tarea es menor o bueno que un determinado porcentaje.

* **Operador de condiciones** = este es el operador que le ayuda a crear la condición de la instrucción &quot;IF&quot;. Por ejemplo, &quot;es igual a&quot; o &quot;es bueno que&quot; son operadores de condición. Para obtener una lista de los operadores de condición que puede utilizar en las instrucciones, consulte [Operadores de condición en expresiones personalizadas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **True***Expression**= Esta es la variable &quot;True&quot;, que indica a la ecuación qué indicador mostrar una vez que se cumplen los criterios de la condición (indicadores &quot;True&quot;).

* **Expresión falsa**= Esta es la variable &quot;False&quot;, que indica a la ecuación qué indicador mostrar cuando no se cumplen los criterios de la condición (indicadores falsos).

En el siguiente ejemplo, el formato de la sentencia original se utiliza para escribir una expresión de datos simple para una sentencia &quot;IF&quot;. La expresión compara dos campos de fecha diferentes en Workfront seguidos de un resultado True/False como una cadena de datos:

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

En el discurso cotidiano, esta declaración significaría: Si la fecha de finalización prevista de mi objeto es &quot;Buena que&quot; la fecha de finalización prevista de mi mismo objeto, en este campo se mostrarán las palabras &quot;Desactivado&quot;. Si no es así, muestre las palabras &quot;On Track&quot;.

## Generar campos calculados en formularios personalizados o columnas personalizadas utilizando instrucciones &quot;IF&quot;

Puede generar instrucciones &quot;IF&quot; en un campo calculado, ya sea en un formulario personalizado o en una columna personalizada.

Hay una diferencia en la sintaxis que se utiliza en un formulario personalizado calculado frente a una columna personalizada calculada. Consulte los siguientes ejemplos:

* [Instrucciones &quot;IF&quot; únicas](#single-if-statements)
* [Varias instrucciones &quot;IF&quot;](#multiple-if-statements)

### Instrucciones &quot;IF&quot; únicas {#single-if-statements}

Los siguientes son ejemplos de un campo personalizado calculado y su columna correspondiente utilizando una instrucción &quot;IF&quot;:

* Campo personalizado calculado:

Al crear un campo personalizado, utilice la siguiente sintaxis para una instrucción &quot;IF&quot;:

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* Columna personalizada calculada:

Al crear una columna personalizada, debe utilizar la siguiente sintaxis para la sentencia &quot;IF&quot; en la línea de expresión de valor:

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### Varias instrucciones &quot;IF&quot; {#multiple-if-statements}

Puede agrupar varias instrucciones &quot;IF&quot; con la siguiente instrucción para crear una expresión más compleja y dinámica:

<pre>IF(Condition1,True Expression,IF(Condition2,True Expression,False Expression)</pre>Tenga en cuenta que ahora no hay ninguna declaración falsa para el primer "IF". En su lugar, lo reemplazamos con el inicio de un segundo "IF".

Los siguientes son ejemplos de un campo personalizado calculado y su columna personalizada correspondiente utilizando varias instrucciones &quot;IF&quot;:

* Campo personalizado calculado:

   ```
   IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
   ```

* Columna personalizada calculada:

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

En este ejemplo, se ha logrado lo mismo al agrupar dos variables de criterios diferentes.\
Puede explorar aún más estas opciones reconstruyendo estos ejemplos en su propio entorno.

La mejor manera de aprender esto es experimentando con varios campos y escenarios. Además, familiarícese con el Explorador de API, que revela los nombres de campo que se pueden utilizar. Para obtener información sobre el Explorador de API, consulte [Explorador de API](../../../wf-api/general/api-explorer.md).

Para obtener más información sobre la sintaxis de Workfront de las expresiones de datos calculadas, consulte [Expresiones de datos calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
