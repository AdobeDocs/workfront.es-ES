---
product-area: reporting
navigation-topic: text-mode-reporting
title: Crear instrucciones "OR" en los filtros del modo de texto
description: Puede incluir varias instrucciones al crear un filtro en listas e informes.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

# Crear instrucciones &quot;OR&quot; en los filtros del modo de texto

Puede incluir varias instrucciones al crear un filtro en listas e informes.

Para obtener información sobre la creación de filtros, consulte los siguientes artículos:

* [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Edición de un filtro mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Operadores de filtro de modo de texto

Para obtener información acerca de los operadores de filtros de Adobe Workfront en la interfaz de filtros estándar, vea [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront tiene dos operadores de filtro que conectan cada instrucción de filtro:

* **AND**: cuando se une a 2 instrucciones de filtro del operador AND, se indica que se desea que ambas instrucciones de filtro se cumplan al mismo tiempo.

  De forma predeterminada, las instrucciones de un filtro se unen mediante el operador AND.

  Al crear un filtro AND en la interfaz de modo de texto, no es necesario utilizar el operador AND. Se supone.

  **Ejemplo:** Para filtrar por tareas que tengan una Fecha planificada de finalización de hoy y un porcentaje completado inferior al 100%, use el siguiente código de modo de texto:

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **OR**: Cuando se unen 2 instrucciones de filtro del operador OR, se indica que se desea cumplir cualquiera de las instrucciones.

  >[!TIP]
  >
  >Al cambiar las instrucciones AND a las instrucciones OR, el número de elementos del informe debería aumentar.

  Al crear un filtro OR mediante la interfaz de modo de texto, debe utilizar el operador OR.

  **Ejemplo:** Para filtrar por tareas que tengan una Fecha planificada de finalización de hoy o un porcentaje completado inferior al 100%, use el siguiente código de modo de texto:

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>O:1:percentComplete=100</pre><pre>OR:1:percentComplete_Mod=lt</pre>

## Sintaxis del modo de texto para filtros OR

La sintaxis del modo de texto para un filtro OR debe contener lo siguiente:

* El operador OR seguido de dos puntos, un número y otro signo de dos puntos al principio de cada línea de filtro que hace referencia al objeto en la instrucción OR. Esto incluye la línea que hace referencia al campo o atributo de filtro y la línea que hace referencia al modificador de filtro.

  Siga este patrón al crear un filtro OR:

  <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>O:1:<field name in camel case>=<value></pre><pre>O:1:<field name in camel case>_Mod=<modifier value></pre>

  >[!TIP]
  >
  >El operador OR distingue entre mayúsculas y minúsculas y siempre está en mayúsculas.

  Puede tener varias instrucciones OR en un filtro. En este caso, cada instrucción OR recibe un número, en el orden en que desea que se apliquen las instrucciones.

  **Ejemplo:** Para filtrar por tareas que tengan una fecha planificada de finalización de hoy O un porcentaje completado inferior al 100% O un estado de nuevo, use el siguiente código de modo de texto:

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>OR:1:status=NUEVO</pre><pre>OR:1:status_Mod=in</pre><pre>O:2:percentComplete=100</pre><pre>OR:2:percentComplete_Mod=lt</pre>

* El nombre de los campos o los atributos a los que hace referencia en un filtro deben escribirse en minúscula. Para obtener información acerca de camel case, vea [Introducción a la sintaxis del modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* Cuando haga referencia a campos personalizados en un filtro OR, debe insertar DE: entre la sintaxis del modificador OR y el nombre del campo personalizado. Debe deletrear el nombre del campo personalizado tal como aparece en la interfaz de Workfront.

  **Ejemplo:** Para filtrar por tareas que tengan un estado de Nuevo o un porcentaje completado inferior al 100%, o bien, para un campo personalizado denominado &quot;Tipo de cuenta&quot; con un valor de &quot;Igual que&quot;, use el siguiente código de modo de texto:

  <pre>status=NUEVO</pre><pre>status_Mod=in</pre><pre>O:1:percentComplete=100</pre><pre>OR:1:percentComplete_Mod=lt</pre><pre>OR:2:DE:Tipo de cuenta=Capital</pre><pre>OR:2:DE:Tipo de cuenta_Mod=in</pre>
