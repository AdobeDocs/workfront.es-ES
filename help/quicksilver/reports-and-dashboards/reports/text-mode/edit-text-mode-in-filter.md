---
product-area: reporting
navigation-topic: text-mode-reporting
title: Edición de un filtro mediante el modo de texto
description: Puede editar un filtro en una lista o informe utilizando el modo de texto para acceder a campos que no están disponibles en la interfaz estándar y crear filtros más complejos.
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 12%

---

# Edición de un filtro mediante el modo de texto

<!-- Audited: 1/2025 -->

Puede editar un filtro en una lista o informe utilizando el modo de texto para acceder a campos que no están disponibles en la interfaz estándar y crear filtros más complejos.

Para obtener más ejemplos en modo de texto al crear un filtro, vea también la sección [Ejemplos de filtros personalizados](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md#samples-of-custom-filters) en el artículo [Ejemplos de vista personalizada, filtro y agrupación: índice de artículo](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
      <p>Nuevo:</p>
         <ul>
         <li><p>Estándar</p></li>
         </ul>
      <p>Actual:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a filtros, vistas y agrupaciones</p> <p>Editar el acceso a Informes, Paneles y Calendarios para editar los elementos de un informe</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe para editar filtros en un informe</p> <p>Permisos de administración para un filtro para editarlo</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de empezar a utilizar el modo de texto en un informe o una lista, asegúrese siempre de estar familiarizado con la sintaxis del modo de texto de Workfront.

Para obtener más información, consulte:

* [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Información general sobre la sintaxis del modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Ejemplos de vistas, filtros y agrupaciones personalizados: índice de artículos](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Edición del modo de texto en un filtro

La edición de un filtro mediante el modo de texto es idéntica para informes y listas. El acceso al filtro desde un informe o desde una lista es diferente.

>[!TIP]
>
>Se recomienda crear la mayor cantidad posible de filtro en el modo estándar y, a continuación, convertir el filtro al modo de texto para editarlo.

Para obtener más información acerca de cómo generar filtros, vea [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Para obtener información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Realice una de las siguientes acciones:

   Para acceder al filtro de una lista, ve a la lista y haz clic en el icono **Filtro**, luego pasa el ratón sobre el filtro del panel lateral de **Filtros** que deseas modificar y haz clic en el icono **Editar** ![](assets/edit-icon.png). El panel lateral **Filtros** muestra el filtro seleccionado o se abre el generador de filtros heredados.

   O

   Para acceder al filtro de un informe, ve a él y haz clic en **Acciones de informe** > **Editar** > pestaña **Filtros**.

1. Realice una de las siguientes acciones:

   Si está usando el panel lateral **Filtros** en una lista, haga clic en **Modo de texto**.

   O

   Si está usando el generador de filtros heredado o en un informe, haga clic en **Agregar una regla de filtro** para empezar a agregar las condiciones del filtro. A continuación, haga clic en **Cambiar al modo de texto** y, a continuación, **Editar el modo de texto** en el lado derecho del generador.

1. Agregar instrucciones de filtro mediante el modo de texto. Cada declaración de filtro puede contener las siguientes líneas e información adicional:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>Filtrar línea/información</b></td> 
      <td><b>Ejemplo</b></td> 
     </tr> 
     <tr> 
      <td> <p>Nombre del campo y valor al que es igual que aparecen en la base de datos de Workfront.</p> <p>Esta línea es obligatoria.</p> <p> Para obtener más información sobre cómo aparecen los objetos y campos en la base de datos, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Para filtrar por tareas en un estado de En curso, utilice la siguiente línea:</p> <p><code>status=INP</code> </p> <p><b>Sugerencia</b>

   Al filtrar por estados, debe utilizar el código de tres letras del estado y no el nombre.</p> </td>
   </tr> 
     <tr> 
      <td> <p>Modificador de nombre de campo y equivalente del modificador. Esto indica por qué condiciones debe cumplir el campo por el que está filtrando.</p> <p>Esta línea es obligatoria.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>Para indicar que el estado de las tareas por las que filtra debe ser igual a En curso, utilice la siguiente línea además de la anterior:</p> <p><code>status_Mod=in</code> </p> <p>Si el modificador es un rango, hay dos líneas para indicar el modificador.</p> 
       <div> <span class="autonumber"><span><b>EJEMPLO </b></span></span> 
        <p>Este es un filtro de modo de texto que busca tareas que están en curso, que tienen una fecha planificada de finalización en el mes actual y que están asignadas a un usuario con un GUID específico:</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>Para obtener una lista completa de modificadores de filtro en modo de texto, consulte el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificadores de filtro y condición</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Operador de instrucción. De forma predeterminada, cada instrucción de filtro está conectada por el operador "AND". Esto no se muestra en la interfaz de modo de texto. También puede agregar un operador "OR" entre dos instrucciones para indicar que desea filtrar por objetos que puedan cumplir una o la otra de dos condiciones.</p> <p>Los operadores de filtro solo son necesarios para los filtros que tienen más de una instrucción.</p> <p>Sugerencia:   
        <ul> 
         <li> <p>"OR" distingue entre mayúsculas y minúsculas y siempre debe escribirse con mayúsculas.</p> </li> 
         <li> <p>Al cambiar el operador de AND a OR, el número de elementos de la lista puede aumentar.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>EJEMPLO </b></span></span> 
        <p>Para filtrar por tareas en un estado de En curso o con una Fecha planificada de finalización de Hoy, utilice la siguiente opción: </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Un comodín, que permite generalizar la información en un filtro y hacer referencia a la hora actual del usuario que ha iniciado sesión.</p> <p>Los caracteres comodín son opcionales.</p> <p>Sugerencia:   <p>Se recomienda utilizar caracteres comodín siempre que sea posible para que los filtros sean más dinámicos y no dupliquen los mismos filtros para cada usuario o lapsos de tiempo similares.</p> <p>Para obtener información sobre los comodines de filtro, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Información general sobre las variables de filtro comodín</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>EJEMPLO</b></span></span> 
        <p>Para filtrar por tareas asignadas al usuario que ha iniciado sesión actualmente, utilice el siguiente comando:</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Para agregar una instrucción de filtro conectada por el operador &quot;OR&quot;, haga lo siguiente:

   1. Agregue una nueva línea de código y escriba OR:1: seguido del objeto o atributo por el que desea filtrar y del valor con el que desea compararlo. Para hacer referencia a tareas que están en cualquier estado excepto Nuevo, utilice la línea siguiente:

      `OR:1:status=NEW`

   1. Agregue una segunda línea y escriba OR:1: seguido del objeto, el modificador y el código del modificador. Para definir el modificador de la línea de código que hace referencia a todos los estados de tareas excepto Nuevo, utilice la línea de modificador siguiente:

      `OR:1:status_Mod=notin`

      Cada línea de la nueva instrucción debe ir precedida por &quot;OR:`<number>`:&quot;.

      Para obtener información acerca de cómo crear instrucciones &quot;OR&quot; en un filtro, vea [Crear instrucciones &quot;OR&quot; en los filtros de modo de texto](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

      >[!NOTE]
      >
      >Puede tener varias instrucciones &quot;OR&quot; en el mismo filtro. Cada vez que tiene una nueva instrucción &quot;OR&quot;, aumenta el número después de &quot;OR:&quot;.
      >
      >Para filtrar por tareas que están en estado de En curso o están asignadas al usuario que ha iniciado sesión o que tienen la Fecha planificada de finalización para hoy, utilice la siguiente información:
      >
      >`status=INP`
      >`status_Mod=in`
      >`OR:1:assignedToID=$$USER.ID`
      >`OR:1:assignedToID_Mod=in`
      >`OR:2:plannedCompletionDate=$$TODAY`
      >`OR:2:plannedCompletionDate_Mod=eq`

1. Haga clic en **Aplicar** o **Listo** para guardar los cambios del modo de texto y seguir editando el informe o el filtro.
1. Haga clic en **Guardar + Cerrar** para guardar el informe o en **Guardar filtro** para guardar el filtro en la lista.


