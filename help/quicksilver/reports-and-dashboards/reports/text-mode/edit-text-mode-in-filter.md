---
product-area: reporting
navigation-topic: text-mode-reporting
title: Edición de un filtro mediante el modo de texto
description: "NOTA: añada una sección en este artículo: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Además, redacte esta área en el artículo Información general sobre el modo de texto"
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1035'
ht-degree: 0%

---

# Edición de un filtro mediante el modo de texto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

Puede editar un filtro en una lista o informe utilizando el modo de texto para acceder a campos que no están disponibles en la interfaz estándar y crear filtros más complejos.

Para ver más ejemplos en modo texto al crear un filtro, consulte también la sección Ejemplos de filtros personalizados en el artículo [Ejemplos de vistas, filtros y agrupaciones personalizadas: índice de artículos](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Editar el acceso a los informes, paneles y calendarios para editar los elementos de un informe</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe para editar filtros en un informe</p> <p>Administración de permisos de un filtro para editarlo</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Requisitos previos

Antes de empezar a utilizar el modo de texto en un informe o una lista, asegúrese siempre de estar familiarizado con la sintaxis del modo de texto de Workfront.

Para obtener más información, consulte:

* [Introducción al modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Resumen de sintaxis de modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Ejemplos de vistas, filtros y agrupaciones personalizadas: índice de artículos](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Edición del modo de texto en un filtro

La edición de un filtro mediante el modo de texto es idéntica para informes y listas. El acceso al filtro desde un informe o desde una lista es diferente.

>[!TIP]
>
>Se recomienda crear la mayor cantidad posible de filtro en el modo estándar y, a continuación, convertir el filtro al modo de texto para editarlo.

Para obtener más información sobre la creación de filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Para obtener información sobre cómo crear un informe, consulte [Creación de un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Realice una de las siguientes acciones:

   1. Para acceder al filtro desde un informe, vaya al informe y, a continuación, haga clic en **Acciones de informe** > **Editar** > **Filtros** pestaña.
   1. Para acceder al filtro desde una lista, vaya a la lista y desde el **Filtrar** , pase el ratón sobre el filtro que desea modificar y haga clic en el botón **Editar** icono ![](assets/edit-icon.png).

      Se abre el generador de filtros.

1. Clic **Agregar una regla de filtro** para empezar a añadir las condiciones del filtro, haga clic en **Cambiar a modo de texto** en la esquina superior derecha del generador.
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
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Para filtrar por tareas en un estado de En curso, utilice la siguiente línea:</p> <p><code>status=INP</code> </p> <p><b>SUGERENCIA</b>

   Al filtrar por estados, debe utilizar el código de tres letras del estado y no el nombre.</p> </td>
   </tr> 
     <tr> 
      <td> <p>Modificador de nombre de campo y a qué equivale el modificador. Esto indica qué condiciones debe cumplir el campo por el que está filtrando.</p> <p>Esta línea es obligatoria.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>Para indicar que el estado de las tareas por las que filtra debe ser igual a En curso, utilice la siguiente línea además de la anterior:</p> <p><code>status_Mod=in</code> </p> <p>Si el modificador es un rango, hay dos líneas para indicar el modificador.</p> 
       <div> <span class="autonumber"><span><b>EJEMPLO </b></span></span> 
        <p>Este es un filtro de modo de texto que busca tareas que están en curso, que tienen una fecha planificada de finalización en el mes actual y que están asignadas a un usuario con un GUID específico:</p> 
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
      <td> <p>Operador de instrucción. De forma predeterminada, cada instrucción de filtro está conectada por el operador "AND". Esto no se muestra en la interfaz de modo de texto. También puede agregar un operador "OR" entre dos instrucciones para indicar que desea filtrar por objetos que puedan cumplir una o la otra de dos condiciones.</p> <p>Los operadores de filtro solo son necesarios para los filtros que tienen más de una instrucción.</p> <p>Sugerencia:   
        <ul> 
         <li> <p>"OR" distingue entre mayúsculas y minúsculas y siempre debe escribirse con mayúsculas.</p> </li> 
         <li> <p>Al cambiar el operador de AND a OR, el número de elementos de la lista puede aumentar.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>EJEMPLO </b></span></span> 
        <p>Para filtrar por tareas en un estado de En curso o con una Fecha planificada de finalización de Hoy, utilice la siguiente opción: </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Un comodín que permite generalizar la información en un filtro y hacer referencia a la hora actual del usuario que ha iniciado sesión.</p> <p>Los caracteres comodín son opcionales.</p> <p>Sugerencia:   <p>Se recomienda utilizar caracteres comodín siempre que sea posible para que los filtros sean más dinámicos y no dupliquen los mismos filtros para cada usuario o lapsos de tiempo similares.</p> <p>Para obtener información sobre los caracteres comodín de filtro, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Variables de filtro comodín</a>.</p> </p> </td> 
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

      ```
      OR:1:status=NEW
      ```

   1. Agregue una segunda línea y escriba OR:1: seguido del objeto, el modificador y el código del modificador. Para definir el modificador de la línea de código que hace referencia a todos los estados de tareas excepto Nuevo, utilice la línea de modificador siguiente:

      ```
      OR:1:status_Mod=notin
      ```

      Cada línea de la nueva instrucción debe ir precedida por &quot;OR:`<number>`:&quot;.

      Para obtener información sobre la creación de instrucciones &quot;OR&quot; en un filtro, consulte [Crear instrucciones &quot;OR&quot; en los filtros del modo de texto](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

<!--WRITER - reformat note below -->

>[!NOTE]
>
>Puede tener varias instrucciones &quot;OR&quot; en el mismo filtro. Cada vez que tiene una nueva instrucción &quot;OR&quot;, aumenta el número después de &quot;OR:&quot;.
>
Para filtrar por tareas que están en estado de En curso o están asignadas al usuario que ha iniciado sesión o que tienen la Fecha planificada de finalización para hoy, utilice la siguiente información:
>
`status=INP`
>
`status_Mod=in`
>
`OR:1:assignedToID=$$USER.ID`
>
`OR:1:assignedToID_Mod=in`
>
`OR:2:plannedCompletionDate=$$TODAY`
>
`OR:2:plannedCompletionDate_Mod=eq`

1. Clic **Listo** si desea guardar los cambios y seguir editando el informe o el filtro.
1. Clic **Guardar + Cerrar** para guardar el informe o **Guardar filtro** para guardar el filtro en la lista.


