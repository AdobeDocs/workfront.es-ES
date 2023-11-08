---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: variación prevista para Duración y Trabajo planificado en una vista de tareas"
description: Vea un ejemplo de una vista que muestra la información de línea de base de Duración y Trabajo planificado.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2a1eef9c-016c-4a04-acda-6070fcb0e23d
source-git-commit: 324ad45b52dafa96c2854f1fec1172b88643bdc2
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---

# Vista: variación prevista para Duración y Trabajo planificado en una vista de tareas

Esta vista muestra lo siguiente en una vista de tareas:

* Información de la tarea con información de la tarea prevista.
* Diferencia entre Duración y Duración de línea de base predeterminada.
* Diferencia entre el trabajo planificado y el trabajo planificado previsto predeterminado.

>[!NOTE]
>
> Los datos mostrados en la vista siguiente comparan los valores reales de las tareas con los valores asociados con las tareas de Línea de base predeterminada.

 

![baseline_varianza_en_a_vista_tareas.png](assets/baseline-variance-in-a-task-view-350x38.png)

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
   <td> <p>Solicitud para modificar una vista </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Ver variación prevista para Duración y Trabajo planificado en una vista de tareas

1. Ir a una lista de tareas.
1. En el **Ver** menú desplegable, seleccione **Nueva vista**.

1. Quite todas las columnas de la vista, excepto la primera.
1. Con la primera columna seleccionada, haga clic en **Cambiar a modo de texto**.
1. Copie el texto siguiente y péguelo en la primera columna de la vista:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.0.displayname=Nombre de tarea<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=compound<br>column.1.viewalias=duration<br>column.1.width=100<br>column.1.displayname=Duración de la tarea<br>column.2.descriptionkey=view.relatedcolumn<br>column.2.descriptionkeyargkey.0=defaultbaselinetask<br>column.2.descriptionkeyargkey.1=duration<br>column.2.linkedname=defaultBaselineTask<br>column.2.listsort=intAsInt(durationMinutes)<br>column.2.namekey=duration<br>column.2.namekeyargkey.0=defaultbaselinetask.abbr<br>column.2.namekeyargkey.1=duration.abbr<br>column.2.querysort=defaultBaselineTask:durationMinutes<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=defaultBaselineTask:durationFieldLong<br>column.2.valueformat=compound<br>column.2.viewalias=defaultBaselineTask:duration<br>column.2.width=100<br>column.2.displayname=Dflt Baseline Tarea: Dur<br>column.2.durationunitfield=durationUnit.value<br>column.3.description=Duration Variance"column.3.linkedname=direct<br>column.3.listsort=intAsInt(durationMinutes)<br>column.3.name=Variación de duración<br>column.3.querysort=durationMinutes<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valueexpression=CONCAT(SUB(){duration},{defaultBaselineTask}.{duration})/480," Días")<br>column.3.valueformat=HTML<br>column.3.viewalias=duration<br>column.3.width=100<br>column.3.displayname=Variación de duración<br>column.4.descriptionkey=workrequired<br>column.4.linkedname=direct<br>column.4.listsort=doubleAsDouble(workRequired)<br>column.4.namekey=workrequired.abbr<br>column.4.querysort=workRequired<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valuefield=workFieldLong<br>column.4.valueformat=compound<br>column.4.viewalias=workrequired<br>column.4.width=100<br>column.4.displayname=Requisito de trabajo<br>column.5.descriptionkey=view.relatedcolumn<br>column.5.descriptionkeyargkey.0=defaultbaselinetask<br>column.5.descriptionkeyargkey.1=workrequired<br>column.5.linkedname=defaultBaselineTask<br>column.5.listsort=doubleAsDouble(workRequired)<br>column.5.namekey=view.relatedcolumn<br>column.5.namekeyargkey.0=defaultbaselinetask.abbr<br>column.5.namekeyargkey.1=workrequired.abbr<br>column.5.querysort=defaultBaselineTask:workRequired<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valuefield=defaultBaselineTask:workFieldLong<br>column.5.valueformat=compound<br>column.5.viewalias=defaultBaselineTask:workrequired<br>column.5.width=100<br>column.5.displayname=Dflt Baseline Tarea: Req. trabajo<br>column.6.descriptionkey=workrequired<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(workRequired)<br>column.6.name=Variación de esfuerzo<br>column.6.querysort=workRequired<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valueexpression=CONCAT(SUB(){workRequired},{defaultBaselineTask}.{workRequired})/60," Horas")<br>column.6.valueformat=HTML<br>column.6.viewalias=workrequired<br>column.6.width=100<br>column.6.displayname=Variación de esfuerzo</pre>

1. Clic **Guardar vista**.