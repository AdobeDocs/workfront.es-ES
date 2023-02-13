---
product-area: reporting
navigation-topic: text-mode-reporting
title: Crear instrucciones "OR" en filtros de modo de texto
description: Puede incluir varias instrucciones al crear un filtro en listas e informes.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Crear instrucciones &quot;OR&quot; en filtros de modo de texto

Puede incluir varias instrucciones al crear un filtro en listas e informes.

Para obtener información sobre la creación de filtros, consulte los siguientes artículos:

* [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Edición de un filtro mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Operadores de filtro de modo de texto

Para obtener información sobre los operadores de filtro de Adobe Workfront en la interfaz de filtro estándar, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront tiene 2 operadores de filtro que conectan cada instrucción de filtro:

* **Y**: Cuando se une a la instrucción de filtro 2 mediante el operador AND , indica que desea que ambas instrucciones de filtro se cumplan al mismo tiempo.

   De forma predeterminada, las instrucciones de un filtro se unen mediante el operador AND.

   Al crear un filtro AND en la interfaz de modo de texto, no es necesario utilizar el operador AND. Se supone.

   **Ejemplo:** Para filtrar tareas que tengan una fecha de finalización planificada de Hoy y un porcentaje de finalización inferior al 100 %, utilice el siguiente código de modo de texto:

   <pre>scheduledCompletionDate=$$TODAY</pre><pre>scheduledCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **O**: Cuando se unen 2 instrucciones de filtro por el operador OR, se indica que se desea que se cumpla cualquiera de estas instrucciones.

   >[!TIP]
   >
   >Al cambiar las instrucciones AND a OR , el número de elementos del informe debe aumentar.

   Al crear un filtro OR mediante la interfaz de modo de texto, debe utilizar el operador OR.

   **Ejemplo:** Para filtrar tareas que tengan una fecha de finalización planificada de Hoy o un porcentaje de finalización inferior al 100 %, utilice el siguiente código de modo de texto:

   <pre>scheduledCompletionDate=$$TODAY</pre><pre>scheduledCompletionDate_Mod=eq</pre><pre>O:1:percentComplete=100</pre><pre>O:1:percentComplete_Mod=lt</pre>

## Sintaxis del modo de texto para filtros OR

La sintaxis del modo de texto de un filtro OR debe contener lo siguiente:

* El operador OR seguido de dos puntos, un número y otros dos puntos al principio de cada línea de filtro que hace referencia al objeto en la instrucción OR. Esto incluye la línea que hace referencia al campo o atributo de filtro y la línea que hace referencia al modificador de filtro.

   Siga este patrón al crear un filtro OR:

   <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>O:1:<field name in camel case>=<value></pre><pre>O:1:<field name in camel case>_Mod=<modifier value></pre>

   >[!TIP]
   >
   >El operador OR distingue entre mayúsculas y minúsculas y siempre está en mayúsculas.

   Puede tener varias instrucciones OR en un filtro. En este caso, cada instrucción OR recibe un número, en el orden en que desea que se apliquen las instrucciones.

   **Ejemplo:**  Para filtrar tareas que tengan una fecha de finalización planificada de hoy o un porcentaje de finalización inferior al 100 % o un estado de nuevo, utilice el siguiente código de modo de texto:

   <pre>scheduledCompletionDate=$$TODAY</pre><pre>scheduledCompletionDate_Mod=eq</pre><pre>O:1:status=NEW</pre><pre>O:1:status_Mod=in</pre><pre>O:2:percentComplete=100</pre><pre>O:2:percentComplete_Mod=lt</pre>

* El nombre de los campos o los atributos a los que se hace referencia en un filtro deben escribirse en mayúsculas. Para obtener información sobre el caso de camello, consulte [Información general sobre la sintaxis del modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* Al hacer referencia a campos personalizados en un filtro OR, debe insertar DE: entre la sintaxis del modificador OR y el nombre del campo personalizado. Debe escribir el nombre del campo personalizado tal como aparece en la interfaz de Workfront.

   **Ejemplo:** Para filtrar tareas que tengan un Estado Nuevo o un Porcentaje completado inferior al 100 % O un campo personalizado llamado &quot;Tipo de cuenta&quot; con el valor &quot;Igual&quot;, utilice el siguiente código de modo de texto:

   <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>O:1:percentComplete=100</pre><pre>O:1:percentComplete_Mod=lt</pre><pre>O:2:DE:Account Type=Capital</pre><pre>O:2:DE:Account Type_Mod=in</pre>
