---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Información general sobre las instrucciones IF
description: Las instrucciones “IF” se pueden utilizar en lenguajes de programación generales. En Adobe Workfront, las instrucciones “IF” le permiten comparar, dar formato y agrupar campos de datos para fines de creación de informes y datos personalizados. Además, el pensamiento matemático en las instrucciones “IF” conduce a una mejor comprensión conceptual, ya que las variables para expresiones se utilizan con frecuencia.
author: Jenny
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 100%

---

# Información general sobre las instrucciones “IF”

<!-- Audited: 1/2024 -->

Las instrucciones “IF” se pueden utilizar en lenguajes de programación generales. En Adobe Workfront, las instrucciones “IF” le permiten comparar, dar formato y agrupar campos de datos para fines de creación de informes y datos personalizados. Además, el pensamiento matemático en las instrucciones “IF” conduce a una mejor comprensión conceptual, ya que las variables para expresiones se utilizan con frecuencia.

## Recomendaciones para las instrucciones “IF”

Tenga en cuenta lo siguiente antes de crear una instrucción “IF”:

* Aunque no es un requisito, se recomienda una comprensión básica de cualquier lenguaje de programación general para esta guía.
* Se requiere una comprensión avanzada de la sintaxis del modo de texto de Workfront. Esto ayuda a comprender la terminología de la API de Workfront y la sintaxis de los datos personalizados en estos formatos específicos.

  Para obtener más información sobre la API de Workfront, consulte [Conceptos básicos de la API](../../../wf-api/general/api-basics.md).

  Para obtener más información sobre el uso del modo de texto, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* Puede crear instrucciones &quot;IF&quot; para los siguientes elementos de Workfront:

   * Vistas
   * Agrupaciones
   * Campos personalizados calculados

* No es posible generar instrucciones “IF” para los filtros. Esto resulta en un error “¡Uy!” en Workfront.
* El equipo de soporte no interviene en la generación de datos personalizados. Puede ponerse en contacto con el equipo de soporte cuando genere los campos o columnas personalizados y no vea los resultados deseados. Para obtener ayuda con la generación de una expresión, póngase en contacto con su administrador de cuentas para informarse sobre nuestras opciones de consultoría.
* En primer lugar, se recomienda escribir estas expresiones en un editor de texto como Sublime o Visual Studio Code, ya que esto ayuda a ver los datos de forma más clara que en Workfront.

## Componentes de una instrucción “IF”

En Workfront, se pueden generar instrucciones “IF” con el siguiente formato:
<pre>IF(Condición, Expresión verdadera, Expresión falsa)</pre>Los componentes de una instrucción “IF” son los siguientes:

* **IF** = Es la expresión de datos calculados de Workfront para “función”. Como sucede de forma similar con las expresiones SUM y PROD, esto indica al sistema que entienda la función como una instrucción “IF”. En esta instrucción, escriba “IF” siempre en mayúsculas.\
  Para obtener una lista de todas las expresiones de datos calculados, consulte [Información general sobre expresiones de datos calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **Condición** = Es la condición que debe cumplir la variable Workfront y constituye la base de esta ecuación. Todo lo que se puede especificar posteriormente en la ecuación depende de la condición. Para iniciar una ecuación, se pueden utilizar varias referencias, comparaciones o expresiones matemáticas. A continuación, se muestran algunos ejemplos de condiciones:

   * Una fecha es posterior a otra en un objeto especificado.
   * Un estado es igual a uno de los disponibles en un objeto especificado.
   * El porcentaje completado de una tarea es menor o mayor que un determinado porcentaje.

* **Operador de condición** = es el operador que le ayuda a generar la condición de la instrucción “IF”. Por ejemplo, “es igual a” o “es mayor que” son operadores de condición. Para obtener una lista de los operadores de condición que se pueden usar en las instrucciones, consulte [Operadores de condición en expresiones personalizadas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **Expresión****verdadera** = Es la variable “Verdadero”, que indica a la ecuación qué indicador mostrar cuando se cumplen los criterios de la condición (indicadores verdaderos).

* **Expresión falsa** = Es la variable “Falso”, que ordena a la ecuación qué indicador mostrar cuando no se cumplen los criterios de la condición (indicadores falsos).

En el siguiente ejemplo, se utiliza el formato de instrucción original para escribir una expresión de datos simple para una instrucción “IF”. La expresión compara dos campos de fecha diferentes en Workfront seguidos de un resultado Verdadero/Falso como cadena de datos:

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

En el lenguaje cotidiano, esta instrucción significaría: si la fecha proyectada de finalización de mi objeto es “mayor que” la fecha planificada de finalización, mostrar “Fuera de pista” en este campo. Si no lo es, mostrar “En seguimiento”.

## Generar campos calculados en formularios personalizados o columnas personalizadas con instrucciones “IF”

Puede crear instrucciones “IF” en un campo calculado, ya sea en un formulario personalizado o en una columna personalizada.

Hay una diferencia en la sintaxis que utiliza en un formulario personalizado calculado frente a una columna personalizada calculada. Consulte los siguientes ejemplos:

* [Instrucciones “IF” únicas](#single-if-statements)
* [Varias instrucciones “IF”](#multiple-if-statements)

### Instrucciones “IF” únicas {#single-if-statements}

A continuación se muestran ejemplos de un campo personalizado calculado y su columna correspondiente con una instrucción “IF”:

* Campo personalizado calculado:

Al crear un campo personalizado, utilice la siguiente sintaxis para una instrucción “IF”:

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* Columna personalizada calculada:

Al crear una columna personalizada, debe utilizar la siguiente sintaxis para la instrucción “IF” en la línea de expresión de valor:

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### Varias instrucciones “IF” {#multiple-if-statements}

Puede juntar varias instrucciones “IF” con la siguiente instrucción para generar una expresión más compleja y dinámica:

<pre>IF(Condition1,True Expression,IF(Condition2,True Expression,False Expression))</pre>Tenga en cuenta que ahora no hay ninguna instrucción falsa para el primer “IF”. En su lugar, lo reemplazamos con el inicio de un segundo “IF".

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

La mejor manera de aprender esto es experimentando con varios campos y escenarios. Además, puede familiarizarse con el Explorador de API, que muestra los nombres de campo que se pueden usar. Para obtener información sobre el Explorador de API, consulte [Explorador de API](../../../wf-api/general/api-explorer.md).

Para obtener más información acerca de la sintaxis de Workfront de las expresiones de datos calculados, consulte [Información general sobre las expresiones de datos calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
