---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 14 de la API
description: Adobe Workfront publicó la versión 14 de la API el viernes, 09 de septiembre de 2021. La versión 14 de la API incorpora los siguientes cambios con respecto a la versión 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
TQID: https://experienceleague.adobe.com/gRCMOHLFlV01R9aOqqFuDzTVjGbxjvU2NVIVmPiTE5E
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 897
ht-degree: 55%

---

# Novedades de la versión 14 de la API

Adobe Workfront publicó la versión 14 de la API el viernes, 09 de septiembre de 2021. La versión 14 de la API incorpora los siguientes cambios con respecto a la versión 14.

## Recursos añadidos

No se han añadido recursos para la versión 14 de la API.

## Recursos eliminados

No se ha eliminado ningún recurso para la versión 14 de la API.

## Recursos modificados

Se han modificado los siguientes recursos para la versión 14 de la API.

* [Registro de facturación (FACTURA)](#billingrecord-bill)
* [Categoría (CTGY)](#category-ctgy)
* [CustomEnum (CSTEM)](#customenum-cstem)
* [Cliente (CUST)](#customer-cust)
* [Preferencias del cliente (CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion (DOCV)](#documentversion-docv)
* [Grupo (GRUPO)](#group-group)
* [EtiquetaNota (NTAG)](#notetag-ntag)
* [Proyecto (PROJ)](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [Asignación de recursos (RSALLO)](#resource-allocation-rsallo)
* [Rol (ROL)](#role-role)
* [Plantilla (TMPL)](#template-tmpl)
* [Plantilla de horas (TSHET)](#timesheet-tshet)

### BillingRecord (BILL) {#billingrecord-bill}

Un objeto BillingRecord registra los ingresos, horas o gastos que se pueden facturar. Esta información puede utilizarse para crear facturas en un sistema contable externo.

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
     <li> <p><b>categoryID</b> </p> <p>Añadido. Una categoría es un formulario personalizado. Este parámetro se agregó para admitir la capacidad de agregar Forms personalizado a objetos BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de referencia</td> 
   <td> 
    <ul> 
     <li> <p><b>categoría</b> </p> <p>Añadido. Una categoría es un formulario personalizado. Este parámetro se agregó para admitir la posibilidad de agregar formularios personalizados a objetos BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de colección</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>Añadido. Representa una colección de categorías (formularios personalizados) asociados al objeto BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>Añadido. Esta acción vuelve a calcular las expresiones de los campos de formulario personalizados.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Categoría (CTGY) {#category-ctgy}

Un objeto de categoría es un formulario personalizado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>Se ha añadido el valor posible:</p> 
      <ul> 
       <li> <p> FACTURA (Registro de facturación)</p> </li> 
      </ul> <p>Este valor se agregó para admitir la posibilidad de agregar formularios personalizados a objetos BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>Esta acción toma los parámetros objID y objCode y devuelve un valor booleano.</p> </li> 
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
     <li> <p><b>getGroupStatus</b> </p> <p>Añadido. Esta consulta admite la capacidad de crear y administrar estados para grupos y subgrupos. </p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">Administrar los estados de un grupo</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Cliente (CUST) {#customer-cust}

Un objeto de cliente representa a una organización que utiliza una instancia de Workfront.

Este es un objeto interno.

### CustomerPreferences (CUSTPR) {#customerpreferences-custpr}

Un objeto CustomerPreferences representa el conjunto de preferencias que un cliente ha establecido para su instancia de Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>Se ha añadido el valor posible:</p> 
      <ul> 
       <li> <p>Permitir que los usuarios agreguen imágenes en las actualizaciones (actualizaciones:images.toggle)</p> </li> 
      </ul> <p>Este parámetro admite la capacidad de agregar imágenes a las actualizaciones de elementos de trabajo. </p> <p>Para obtener más información, consulte <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Trabajo de actualización</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

Un objeto DocumentVersion representa una versión específica de un archivo (como material escrito, imágenes u otras formas de información).

Para obtener más información acerca de las versiones de documentos, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>Añadido. Este campo registra la fecha y la hora de la última llamada de retorno de Workfront Proof, si la versión está asociada a una prueba.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Grupo (GROUP) {#group-group}

Un objeto Group representa un conjunto de usuarios y equipos. Los grupos a menudo representan la estructura departamental.

Para obtener más información sobre los grupos, consulte [Grupos vs. equipos en Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>Añadido. Esta acción toma una matriz de identificadores de grupo y agrega esos grupos como subgrupos al grupo especificado.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Etiqueta de nota (NTAG) {#notetag-ntag}

Un objeto NoteTag representa el acto de etiquetar a un usuario o equipo en una actualización de un elemento de trabajo.

Para obtener más información sobre el etiquetado en las actualizaciones, consulte [Etiquetar a otros en las actualizaciones](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Operaciones</td> 
   <td> <p>Se agregaron las operaciones siguientes al objeto NoteTag:</p> 
    <ul> 
     <li> <p><b>COUNT</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>REPORT</b> </p> </li> 
     <li> <p><b>SEARCH</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Proyecto (PROJ) {#project-proj}

Los proyectos son elementos de trabajo dentro de Workfront y son un componente principal en la forma en que Workfront ayuda a las personas a realizar su trabajo. Un objeto Projecto representa un grupo de tareas con un objetivo común y específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>Añadido.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

Un objeto QueueDef representa una cola, que es un proyecto que se ha publicado en el área del servicio de asistencia para permitir a los usuarios enviarle problemas.

Para obtener más información sobre las colas de solicitudes, consulte [Creación de colas de solicitudes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>Añadido. Esta acción admite la capacidad de buscar solicitudes utilizando la ruta a través de la cola de solicitudes y los grupos de temas.</p> <p>Para obtener más información sobre la búsqueda de colas de solicitudes por ruta, consulte <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Crear solicitudes y generar borradores en la aplicación web de Workfront</a> en <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Crear y enviar solicitudes de Adobe Workfront</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Asignación de recursos (RSALLO) {#resource-allocation-rsallo}

Un objeto Resource Allocation representa la estimación de los recursos necesarios para un proyecto determinado. Este objeto sólo se utiliza en el Planificador de recursos de legado. Para el campo correspondiente en el nuevo Planificador de recursos, utilice Hora presupuestada (BGHR).

El objeto de asignación de recursos quitó el indicador **REPORTABLE**.

### Función (ROLE) {#role-role}

Un objeto Role (función) representa una capacidad funcional o un conjunto de aptitudes que un usuario podría completar, como un diseñador o un gestor de productos.

Para obtener información sobre los roles, consulte [Resumen del rol](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Añadido. Este es un parámetro booleano con un valor de verdadero si un objeto está activo y falso si no lo está. Los objetos que se definen como Activos aparecen en menús desplegables y campos de escritura anticipada y pueden adjuntarse a otros objetos.</p> </li> 
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

### Template (TMPL) {#template-tmpl}

Un objeto de plantilla representa un patrón para un proyecto. Los proyectos se pueden crear a partir de plantillas para ahorrar tiempo. Una plantilla contiene un equipo y tareas, que se copiarán en cualquier proyecto creado a partir de la plantilla.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Añadido. Este campo se ha añadido para permitir asociar grupos con plantillas.</p> <p style="font-weight: normal;">Para obtener más información, consulte <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Editar plantillas de proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupo</p> <p style="font-weight: normal;">Añadido. Este campo se ha añadido para permitir asociar grupos con plantillas.</p> <p style="font-weight: normal;">Para obtener más información, consulte <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Editar plantillas de proyecto</a>.</p> </li> 
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
