---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Ver: tareas afectadas por excepciones de programación'
description: Esta vista de tareas identifica las tareas que deberán completarse tarde debido a los fines de semana, a la desactivación del tiempo personal u otras excepciones de programación.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Ver: tareas afectadas por las excepciones de programación

Esta vista de tareas identifica las tareas que deberán completarse tarde debido a los fines de semana, a la desactivación del tiempo personal u otras excepciones de programación.

Esta vista muestra lo siguiente:

* Duración de las tareas
* Fechas de inicio y finalización previstas de las tareas
* Duración de las tareas según el número de días entre las fechas de inicio planeado y de finalización planeada de las tareas (Duración del calendario)
* Número del día de la programación del proyecto cuando se inicia la tarea (Fecha de inicio del calendario)
* La semana Duración de las tareas según el número de días laborables entre las fechas de inicio planeado y de finalización planeada de las tareas (Duración del día de la semana)
* Si la Duración del día de la semana es buena que la duración de las tareas, lo que sugiere que hay días de excepción en la duración de las tareas, las tareas se marcan como una &quot;Excepción&quot;.\
   ![tasks_with_calendar_exception.png](assets/tasks-with-calendar-exceptions-350x51.png)

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
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ver tareas afectadas por las excepciones de programación

1. Vaya a una lista de tareas.
1. En el **Ver** menú desplegable, seleccione **Nueva vista**.

1. En el **Vista previa de columna** , elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y, a continuación, haga clic en **Cambiar al modo de texto**.
1. Pase el cursor sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Elimine el texto que encuentra en la sección **Modo de texto** y sustitúyalo por el siguiente código:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.value.format=int<br>column.0.link.lookup=link.view<br>column.0.link.value.field=objCode<br>column.0.link.value.format=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.name=name.abbr<br>column.0.querysort=name<br>column.0.abreviview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.abreviview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=complex<br>column.1.viewalias=duration<br>column.1.width=80<br>column.2.descriptionkey=plannedstartdate<br>column.2.linkedname=direct<br>column.2.listsort=atDateAsAtDate(scheduledStartDate)<br>column.2.namekey=plannedstartdate.abbr<br>column.2.querysort=scheduledStartDate<br>column.2.abreviview=false<br>column.2.stretch=0<br>column.2.valuefield=scheduledStartDate<br>column.2.value eformat=atDate<br>column.2.width=80<br>column.3.descriptionkey=plannedcompletiondate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(scheduledCompletionDate)<br>column.3.namekey=plannedcompletiondate.abbr<br>column.3.querysort=scheduledCompletionDate<br>column.3.abreviview=false<br>column.3.stretch=0<br>column.3.valuefield=scheduledCompletionDate<br>column.3.valueformat=atDate<br>column.3.width=80<br>column.4.agregator.displayformat=int<br>column.4.agregator.function=SUM<br>column.4.gregator.namekey=id<br>column.4.agregator.valueexpression=DATEDIFF({scheduledCompletionDate},<br>{scheduledStartDate})+1<br>column.4.agregator.valueformat=intAsInt<br>column.4.descriptionkey=id<br>column.4.linkedname=direct<br>column.4.listsort=intAsInt(ID)<br>column.4.name=Duración del calendario<br>column.4.querysort=ID<br>column.4.shorview=false<br>column.4.stretch=0<br>column.4.valueexpression=DATEDIFF({scheduledCompletionDate},{scheduledStartDate})+1<br>column.4.valueformat=int<br>column.4.width=80<br>column.5.agregator.displayformat=int<br>column.5.agregator.function=SUM<br>column.5.agregator.namekey=id<br>column.5.agregator.valueexpression=DATEDIFF({scheduledStartDate},{project}.<br>{scheduledStartDate})+0<br>column.5.agregator.valueformat=intAsInt<br>column.5.descriptionkey=id<br>column.5.linkedname=direct<br>column.5.listsort=intAsInt(ID)<br>column.5.name=Calendar Start Date<br>column.5.querysort=ID<br>column.5.abreviview=false<br>column.5.stretch=0<br>column.5.valueexpression=DATEDIFF({scheduledStartDate},{project}.{scheduledStartDate})+0<br>column.5.valueformat=int<br>column.5.width=80<br>column.6.agregator.displayformat=int<br>column.6.agregator.function=SUM<br>column.6.agregator.namekey=id<br>column.6.agregator.valueexpression=WEEKDAYDIFF({scheduledStartDate},<br>{scheduledCompletionDate})+0<br>column.6.agregator.value.format=HTML<br>column.6.descriptionkey=id<br>column.6.linkedname=direct<br>column.6.listsort=intAsInt(ID)<br>column.6.name=Week Day Duration<br>column.6.querysort=ID<br>column.6.abreviview=false<br>column.6.stretch=0<br>column.6.valueexpression=WEEKDAYDIFF({scheduledStartDate},{scheduledCompletionDate})+0<br>column.6.valueformat=int<br>column.6.width=80<br>column.7.agregator.displayformat=int<br>column.7.agregator.expression=IF((WEEKDAYDIFF({scheduledStartDate},{scheduledCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.agregator.function=SUM<br>column.7.agregator.namekey=id<br>column.7.agregator.value.format=HTML<br>column.7.linkedname=direct<br>column.7.listsort=intAsInt(ID)<br>column.7.name=Schedule<br>column.7.querysort=ID<br>column.7.abreviview=false<br>column.7.stretch=0<br>column.7.valueexpression=IF((WEEKDAYDIFF({scheduledStartDate},{scheduledCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.valueformat=HTML<br>column.7.width=80</pre>

1. Haga clic en **Guardar vista**.
