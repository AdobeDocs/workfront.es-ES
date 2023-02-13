---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 14 de la API
description: Adobe Workfront lanzó la versión 14 de la API el 9 de septiembre de 2021. La versión 14 de la API presenta los siguientes cambios con respecto a la versión 14.
author: John
feature: Workfront API
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 2%

---

# Novedades de la versión 14 de la API

Adobe Workfront lanzó la versión 14 de la API el 9 de septiembre de 2021. La versión 14 de la API presenta los siguientes cambios con respecto a la versión 14.

## Recursos añadidos

No se agregaron recursos para la versión 14 de la API.

## Recursos eliminados

No se eliminaron recursos para la versión 14 de la API.

## Recursos modificados

Se modificaron los siguientes recursos para la versión 14 de la API.

* [Registro de facturación (BILL)](#billingrecord-bill)
* [Categoría (CTGY)](#category-ctgy)
* [CustomEnum (CSTEM)](#customenum-cstem)
* [Cliente (CUST)](#customer-cust)
* [Preferencias de cliente (CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion (DOCV)](#documentversion-docv)
* [Grupo (GRUPO)](#group-group)
* [NoteTag (NTAG)](#notetag-ntag)
* [Proyecto (PROJ)](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [Asignación de recursos (RSALLO)](#resource-allocation-rsallo)
* [Función (FUNCIÓN)](#role-role)
* [Plantilla (TMPL)](#template-tmpl)
* [Hoja de horas (HOJA)](#timesheet-tshet)

### Registro de facturación (BILL) {#billingrecord-bill}

Un objeto BillingRecord registra los ingresos, horas o gastos que se pueden facturar. Esta información se puede utilizar para crear facturas en un sistema de contabilidad externo.

Para obtener más información sobre los registros de facturación, consulte [Crear registros de facturación](../../manage-work/projects/project-finances/create-billing-records.md).

El objeto BillingRecord agregó el indicador **DATA_EXTENDIBLE**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Campos directos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>Agregado. Una categoría es un formulario personalizado. Este parámetro se agregó para admitir la capacidad de agregar Forms personalizado a los objetos BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de referencia</td> 
   <td> 
    <ul> 
     <li> <p><b>categoría</b> </p> <p>Agregado. Una categoría es un formulario personalizado. Este parámetro se agregó para admitir la capacidad de agregar formularios personalizados a objetos BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de colección</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>Agregado. Representa una colección de Categorías (formularios personalizados) asociadas al objeto Registro de facturación.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>Agregado. Esta acción vuelve a calcular las expresiones de los campos de formulario personalizados.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Categoría (CTGY) {#category-ctgy}

Un objeto Category es un formulario personalizado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>Se ha añadido un valor posible:</p> 
      <ul> 
       <li> <p> BILL (BillingRecord)</p> </li> 
      </ul> <p>Este valor se agregó para admitir la capacidad de agregar formularios personalizados a los objetos BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>Esta acción toma los parámetros objID y objCode, y devuelve un valor booleano.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum (CSTEM) {#customenum-cstem}

El objeto CustomEnum ayuda a convertir los códigos de estado en texto legible en lenguaje natural.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Consultas</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatus</b> </p> <p>Agregado. Esta consulta admite la capacidad de crear y administrar estados para grupos y subgrupos. </p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">Administrar estados de grupo</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Cliente (CUST) {#customer-cust}

Un objeto Customer representa una organización que utiliza una instancia de Workfront.

Se trata de un objeto interno.

### Preferencias de cliente (CUSTPR) {#customerpreferences-custpr}

Un objeto CustomerPreferences representa el conjunto de preferencias que un cliente ha establecido para su instancia de Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>Se ha añadido un valor posible:</p> 
      <ul> 
       <li> <p>Permitir que los usuarios agreguen imágenes en actualizaciones (actualizaciones:imágenes.alternar)</p> </li> 
      </ul> <p>Este parámetro admite la capacidad de agregar imágenes a las actualizaciones de elementos de trabajo. </p> <p>Para obtener más información, consulte <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Actualizar trabajo</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

Un objeto DocumentVersion representa una versión específica de un archivo (como material escrito, imágenes u otras formas de información).

Para obtener más información sobre las versiones de documentos, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>Agregado. Este campo registra la fecha y la hora de la última llamada de retorno de Workfront Proof, si la versión está asociada a una prueba.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Grupo (GRUPO) {#group-group}

Un objeto Group representa un conjunto de usuarios y equipos. Los grupos suelen representar la estructura departamental.

Para obtener más información sobre los grupos, consulte [Grupos frente a equipos en Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>Agregado. Esta acción toma una matriz de groupIDs y agrega esos grupos como subgrupos al grupo especificado.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NoteTag (NTAG) {#notetag-ntag}

Un objeto NoteTag representa el acto de etiquetar a un usuario o equipo en una actualización de un elemento de trabajo.

Para obtener más información sobre el etiquetado de actualizaciones, consulte [Etiquetar otros en actualizaciones](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Operaciones</td> 
   <td> <p>Se agregaron las siguientes operaciones al objeto NoteTag :</p> 
    <ul> 
     <li> <p><b>RECUENTO</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>INFORME</b> </p> </li> 
     <li> <p><b>SEARCH</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Proyecto (PROJ) {#project-proj}

Los proyectos son elementos de trabajo dentro de Workfront y son un componente principal de la forma en que Workfront ayuda a las personas a hacer su trabajo. Un objeto Project representa un grupo de tareas con un objetivo específico común.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>Agregado.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

Un objeto QueueDef representa una cola, que es un proyecto que se ha publicado en el área de asistencia técnica para permitir a los usuarios enviar problemas.

Para obtener más información sobre las colas de solicitud, consulte [Crear una cola de solicitud](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>Agregado. Esta acción admite la capacidad de encontrar solicitudes utilizando la ruta a través de la cola de solicitudes y los grupos de temas.</p> <p>Para obtener más información sobre la búsqueda de colas de solicitud por ruta, consulte <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Crear solicitudes y generar borradores en la aplicación web de Workfront</a> en <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Crear y enviar solicitudes de Adobe Workfront</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Asignación de recursos (RSALLO) {#resource-allocation-rsallo}

Un objeto Asignación de recursos representa la estimación de los recursos necesarios para un proyecto determinado. Este objeto solo se utiliza en el planificador de recursos heredado. Para el campo correspondiente en el nuevo planificador de recursos, utilice la hora presupuestada (BGHR).

El objeto Asignación de recursos quitó el indicador **REPORTABLE**.

### Función (FUNCIÓN) {#role-role}

Un objeto Rol (función de trabajo) representa una capacidad funcional o un conjunto de habilidades que un usuario podría rellenar, como Designer o Product Manager.

Para obtener información sobre las funciones de trabajo, consulte [Información general sobre la función de trabajo](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Agregado. Se trata de un parámetro booleano que tiene el valor "True" si un objeto es Activo y "False" si no lo es. Los objetos que se establecen como Activo aparecen en los menús desplegables y en los campos de avance de tipo y se pueden adjuntar a otros objetos.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos predeterminados</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Plantilla (TMPL) {#template-tmpl}

Un objeto Template representa un patrón para un proyecto. Los proyectos se pueden crear a partir de plantillas para ahorrar tiempo. Una plantilla contiene un equipo y tareas que se copiarán en cualquier proyecto creado a partir de la plantilla.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Agregado. Este campo se agregó para admitir la capacidad de asociar grupos con plantillas.</p> <p style="font-weight: normal;">Para obtener más información, consulte <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Editar plantillas de proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupo</p> <p style="font-weight: normal;">Agregado. Este campo se agregó para admitir la capacidad de asociar grupos con plantillas.</p> <p style="font-weight: normal;">Para obtener más información, consulte <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Editar plantillas de proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Timesheet (TSHET)</strong></p>
<p>A&nbsp;Timesheet object represents a virtual timecard that allows users to enter actual hours worked for tasks, projects, and overhead hour types.</p>
<p>For more information, see <a href="../../timesheets/timesheets/timesheets-overview.md" class="MCXref xref">Timesheets overview</a>.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Core Fields</td>
<td>
<ul>
<li> <p><b>objCode</b> </p> <p>Removed.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
</div>
-->
