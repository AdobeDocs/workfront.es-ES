---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Información general sobre instrucciones IF
description: Puede utilizar instrucciones "IF" en lenguajes de programación generales. En Adobe Workfront, las instrucciones "IF" permiten comparar, dar formato y agrupar campos de datos para fines de creación de informes y datos personalizados. Además, pensar matemáticamente en las frases "IF" conduce a una mejor comprensión conceptual, ya que las variables para expresiones se utilizan comúnmente.
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 23b5ba9564b514e11c1ca9d5cca276238ef11066
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Información general sobre las instrucciones &quot;IF&quot;

<!-- Audited: 1/2024 -->

Puede utilizar instrucciones &quot;IF&quot; en lenguajes de programación generales. En Adobe Workfront, las instrucciones &quot;IF&quot; permiten comparar, dar formato y agrupar campos de datos para fines de creación de informes y datos personalizados. Además, pensar matemáticamente en las frases &quot;IF&quot; conduce a una mejor comprensión conceptual, ya que las variables para expresiones se utilizan comúnmente.

## Recommendations para instrucciones &quot;IF&quot;

Tenga en cuenta lo siguiente antes de crear una instrucción &quot;IF&quot;:

* Recomendamos una comprensión básica de cualquier lenguaje de programación general, pero no la necesitamos, para esta guía.
* Necesitamos una comprensión avanzada de la sintaxis del modo de texto de Workfront. Esto ayuda a comprender la terminología de la API de Workfront y la sintaxis de los datos personalizados en estos formatos específicos.

  Para obtener información acerca de la API de Workfront, consulte [Conceptos básicos de la API](../../../wf-api/general/api-basics.md).

  Para obtener información acerca del uso del modo de texto, vea [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* Puede crear instrucciones &quot;IF&quot; para los siguientes elementos de Workfront:

   * Vistas
   * Agrupaciones
   * Campos personalizados calculados

* No puede generar instrucciones &quot;IF&quot; para los filtros. Esto resulta en un error &quot;¡Uy!&quot; en Workfront.
* El equipo de asistencia no ayuda a crear datos personalizados. Puede ponerse en contacto con el equipo de asistencia después de crear los campos o columnas personalizados y de no ver los resultados deseados. Para obtener ayuda para crear una expresión, póngase en contacto con su administrador de cuentas para consultar sobre nuestras opciones de consultoría.
* Se recomienda escribir primero estas expresiones en un editor de texto, como Sublime o Visual Studio Code, ya que esto le ayuda a ver los datos con mayor claridad de lo que aparecería en Workfront.

## Componentes de una instrucción &quot;IF&quot;

Puede crear instrucciones &quot;IF&quot; en Workfront con el siguiente formato:
<pre>IF(Condición,Expresión verdadera,Expresión falsa)</pre>Los componentes de una instrucción "IF" son:

* **IF** = Es la expresión de datos calculados de Workfront para &quot;función&quot;. Similar a las expresiones SUMA y PROD, esto primero indica al sistema que comprenda la función como una sentencia &quot;IF&quot;. Utilice siempre mayúsculas para &quot;IF&quot; en esta instrucción.\
  Para obtener una lista de todas las expresiones de datos calculados, vea [Información general sobre expresiones de datos calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **Condición** = Esta es la condición que debe cumplir la variable Workfront y es la base de esta ecuación. Todo lo que se puede especificar posteriormente en la ecuación depende de la condición. Puede utilizar varias referencias, comparaciones o expresiones matemáticas para iniciar una ecuación. Algunos ejemplos de condiciones son los siguientes:

   * Una fecha es posterior a otra fecha en un objeto especificado.
   * Un estado es igual a uno de los estados disponibles en un objeto especificado.
   * El porcentaje completado de una tarea es menor o mayor que un determinado porcentaje.

* **Operador de condición** = este es el operador que le ayuda a generar la condición de su instrucción &quot;IF&quot;. Por ejemplo, &quot;es igual a&quot; o &quot;es mayor que&quot; son operadores de condición. Para obtener una lista de los operadores de condición que se pueden usar en las instrucciones, vea [Operadores de condición en expresiones personalizadas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **True**&#x200B;**Expression** = Es la variable &quot;True&quot;, que indica a la ecuación qué indicador mostrar una vez que se cumplen los criterios de la condición (indicadores true).

* **Expresión falsa** = Es la variable &quot;False&quot;, que indica a la ecuación qué indicador mostrar cuando no se cumplen los criterios de la condición (indicadores falsos).

En el ejemplo siguiente, se utiliza el formato de instrucción original para escribir una expresión de datos simple para una instrucción &quot;IF&quot;. La expresión compara dos campos de fecha diferentes en Workfront seguidos de un resultado Verdadero/Falso como cadena de datos:

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

En el discurso diario, esta afirmación significaría: Si la fecha proyectada de finalización de mi objeto es &quot;mayor que&quot; la fecha planificada de finalización de mi mismo objeto, entonces mostrar las palabras &quot;Fuera de pista&quot; en este campo. Si no es así, muestre las palabras &quot;En seguimiento&quot;.

## Generar campos calculados en formularios personalizados o columnas personalizadas con instrucciones &quot;IF&quot;

Puede crear instrucciones &quot;IF&quot; en un campo calculado, ya sea en un formulario personalizado o en una columna personalizada.

Hay una diferencia en la sintaxis que utiliza en un formulario personalizado calculado frente a una columna personalizada calculada. Consulte los siguientes ejemplos:

* [Instrucciones &quot;IF&quot; únicas](#single-if-statements)
* [Varias instrucciones &quot;IF&quot;](#multiple-if-statements)

### Instrucciones &quot;IF&quot; únicas {#single-if-statements}

A continuación se muestran ejemplos de un campo personalizado calculado y su columna correspondiente con una instrucción &quot;IF&quot;:

* Campo personalizado calculado:

Al crear un campo personalizado, utilice la siguiente sintaxis para una instrucción &quot;IF&quot;:

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* Columna personalizada calculada:

Al crear una columna personalizada, debe utilizar la siguiente sintaxis para la instrucción &quot;IF&quot; en la línea de expresión de valor:

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### Varias instrucciones &quot;IF&quot; {#multiple-if-statements}

Puede juntar varias instrucciones &quot;IF&quot; con la siguiente instrucción para generar una expresión más compleja y dinámica:

<pre>IF(Condición1,Expresión verdadera,IF(Condición2,Expresión verdadera,Expresión falsa)</pre>Tenga en cuenta que ahora no hay ninguna instrucción falsa para el primer "IF". En su lugar, lo reemplazamos con el inicio de un segundo "IF".

A continuación se muestran ejemplos de un campo personalizado calculado y su columna personalizada correspondiente que utiliza varias instrucciones &quot;IF&quot;:

* Campo personalizado calculado:

  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* Columna personalizada calculada:

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

En este ejemplo, se ha logrado lo mismo juntando dos variables de criterios diferentes.\
Puede explorar estas opciones reconstruyendo estos ejemplos en su propio entorno.

La mejor manera de aprender esto es experimentando con varios campos y escenarios. Además, familiarícese con el Explorador de API, que muestra los nombres de campo que se pueden usar. Para obtener información sobre el Explorador de API, consulte [Explorador de API](../../../wf-api/general/api-explorer.md).

Para obtener más información acerca de la sintaxis de Workfront de las expresiones de datos calculados, vea [Información general sobre las expresiones de datos calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
