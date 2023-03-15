---
product-area: reporting
navigation-topic: text-mode-reporting
title: Edición de un filtro mediante el modo de texto
description: '''NOTA: agregue una sección en este artículo: /Contenido/Informes y tableros/Informes/Informes Elements/create-customize-fitlers.html; *** También, redactar esta área en el artículo de información general del modo de texto)"'
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 0%

---

# Edición de un filtro mediante el modo de texto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

Puede editar un filtro en una lista o informe utilizando el modo de texto para acceder a los campos que no están disponibles en la interfaz estándar y crear filtros más complejos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a filtros, vistas y grupos</p> <p>Editar acceso a informes, tableros y calendarios para editar elementos de informes en un informe</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe para editar filtros en un informe</p> <p>Administrar permisos en un filtro para editarlo</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de empezar a utilizar el modo de texto en un informe o lista, asegúrese siempre de que está familiarizado con la sintaxis del modo de texto de Workfront.

Para obtener más información, consulte:

* [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Información general sobre la sintaxis del modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Ejemplos de vista, filtro y agrupamiento personalizados](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Editar el modo de texto en un filtro

La edición de un filtro mediante el modo de texto es idéntica para los informes y las listas. El acceso a la vista desde un informe o desde una lista es distinto.

>[!TIP]
>
>Se recomienda generar el filtro mayor número posible en el modo estándar y, a continuación, convertir el filtro al modo de texto para editarlo.

Para obtener más información sobre la creación de filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Para obtener información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Realice una de las siguientes acciones:

   1. Para acceder al filtro de un informe, vaya al informe y haga clic en **Acciones de informe** > **Editar** > **Filtros** pestaña .
   1. Para acceder al filtro de una lista, vaya a la lista y desde el **Filtro** menú desplegable, pase el ratón sobre el filtro que desea modificar y haga clic en el **Editar** icono ![](assets/edit-icon.png).

      Se abre el generador de filtros.

1. Haga clic en **Agregar una regla de filtro** para empezar a añadir las condiciones del filtro, haga clic en **Cambiar al modo de texto** en la esquina superior derecha del generador.
1. Añada instrucciones de filtro mediante el modo de texto. Cada instrucción de filtro puede contener las siguientes líneas e información adicional:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Filtrar línea/información</td> 
      <td>Ejemplo</td> 
     </tr> 
     <tr> 
      <td> <p>Nombre del campo y el valor igual a como aparecen en la base de datos de Workfront.</p> <p>Esta línea es obligatoria.</p> <p> Para obtener más información sobre cómo aparecen los objetos y los campos en la base de datos, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Para filtrar tareas en estado In Progress, utilice la siguiente línea:</p> <p><code>status=INP</code> </p> <p>Sugerencia: Al filtrar por estados, debe utilizar el código de tres letras del estado y no el nombre.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Modificador de nombre de campo y al que es igual el modificador. Esto indica las condiciones que debe cumplir el campo por el que está filtrando.</p> <p>Esta línea es obligatoria.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>Para indicar que el estado de las tareas para las que filtre debe ser igual a En curso, utilice la línea siguiente además de la anterior:</p> <p><code>status_Mod=in</code> </p> <p>Si el modificador es un rango, hay dos líneas que indican el modificador.</p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Ejemplo: </b></span></span> 
        <p>Este es un filtro de modo de texto que busca tareas que estén en curso, que tengan una fecha de finalización planeada dentro del mes actual y que estén asignadas a un usuario con un GUID específico:</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>Para obtener una lista completa de los modificadores de filtro en el modo de texto, consulte el artículo <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificadores de filtro y condición</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Operador de instrucción. De forma predeterminada, cada instrucción de filtro está conectada por el operador "AND". Esto no se muestra en la interfaz del modo de texto. También puede agregar un operador "O" entre dos instrucciones para indicar que desea filtrar por objetos que puedan cumplir una o las otras dos condiciones.</p> <p>Los operadores de filtro solo son necesarios para filtros que tienen más de una instrucción.</p> <p>Sugerencia:   
        <ul> 
         <li> <p>"O" distingue entre mayúsculas y minúsculas y siempre debe escribirse en mayúsculas.</p> </li> 
         <li> <p>Cuando cambia el operador de AND a OR, el número de elementos de lista puede aumentar.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Ejemplo: </b></span></span> 
        <p>Para filtrar tareas en un estado en curso o con una fecha de finalización prevista de hoy, utilice lo siguiente: </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Comodín que permite generalizar la información en un filtro y hacer referencia a la hora actual o al usuario que ha iniciado sesión.</p> <p>Los comodines son opcionales.</p> <p>Sugerencia:   <p>Se recomienda utilizar caracteres comodín siempre que sea posible para que los filtros sean más dinámicos y no se dupliquen en los mismos filtros para cada usuario o marcos de tiempo similares.</p> <p>Para obtener información sobre los comodines de filtro, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Variables de filtro comodín</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Ejemplo: </b></span></span> 
        <p>Para filtrar tareas asignadas al usuario que ha iniciado sesión en ese momento, utilice el siguiente:</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Para añadir una instrucción de filtro conectada por el operador &quot;O&quot;, haga lo siguiente:

   1. Añada una nueva línea de código y escriba O:1: seguido del objeto o atributo por el que desea filtrar y del valor con el que desea compararlo. Para hacer referencia a tareas que están en cualquier estado excepto New, utilice la siguiente línea:

      ```
      OR:1:status=NEW
      ```

   1. Añada una segunda línea y escriba O:1: seguido del objeto , el modificador y el código del modificador . Para definir el modificador de la línea de código que hace referencia a todos los estados de tarea excepto New, utilice la siguiente línea de modificador:

      ```
      OR:1:status_Mod=notin
      ```

      Cada línea de la nueva instrucción debe ir precedida por &quot;O:`<number>`:&quot;.

      Para obtener información sobre la creación de instrucciones &quot;O&quot; en un filtro, consulte [Crear instrucciones &quot;OR&quot; en filtros de modo de texto](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

<!--WRITER - reformat note below -->

>[!NOTE]
>
>Puede tener varias instrucciones &quot;O&quot; en el mismo filtro. Cada vez que tiene una nueva instrucción &quot;O&quot;, aumenta el número después de &quot;O:&quot;.
Para filtrar tareas que estén en estado In Progress o que estén asignadas al usuario que ha iniciado sesión, o que tengan la Fecha de finalización planeada hoy, utilice lo siguiente:
`status=INP`
`status_Mod=in`
`OR:1:assignedToID=$$USER.ID`
`OR:1:assignedToID_Mod=in`
`OR:2:plannedCompletionDate=$$TODAY`
`OR:2:plannedCompletionDate_Mod=eq`

1. Haga clic en **Listo** si desea guardar los cambios y continuar editando el informe o el filtro.
1. Haga clic en **Guardar + Cerrar** para guardar el informe o **Guardar filtro** para guardar el filtro en la lista.
