---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 12 de la API
description: Workfront lanzó la versión 12 de la API el 12 de noviembre de 2020. La versión 12 de la API incorpora los siguientes cambios con respecto a la versión 11
author: Becky
feature: Workfront API
role: Developer
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '2422'
ht-degree: 1%

---

# Novedades de la versión 12 de la API

Workfront lanzó la versión 12 de la API el 12 de noviembre de 2020. La versión 12 de la API incorpora los siguientes cambios con respecto a la versión 11

## Recursos añadidos

Los siguientes recursos son nuevos en la versión 12 de la API de Workfront.

* [RutaPan](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### RutaPan {#breadcrumb}

Un objeto BreadCrumb representa un elemento en la jerarquía principal/secundario de un elemento de trabajo de Adobe Workfront. Las rutas de exploración indican cómo encaja un elemento de trabajo en la mayor estructura de Portfolio, Proyectos, Proyectos y Tareas.

Para obtener más información sobre las rutas de exploración en Workfront, consulte [Información general sobre las rutas de exploración en la nueva experiencia de Adobe Workfront](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Acción</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">getObjectHierarchy</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RichTextParameterValue {#richtextparametervalue}

Los campos de texto enriquecido ahora están disponibles en más objetos. El objeto RichTextParameterValue se agregó a Workfront para admitir esta disponibilidad.

Para obtener más información, consulte [Campos de texto enriquecido en la API de Adobe Workfront](../../wf-api/general/rich-text-field-api.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">Identificador</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos principales</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">Identificador</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Recursos eliminados

No se ha eliminado ningún recurso para la versión 12 de la API.

## Recursos modificados

Se han modificado los siguientes recursos para la versión 12 de la API de Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">NivelDeAcceso</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">PermisosDeNivelDeAcceso</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">Solicitud de acceso</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">Regla de acceso</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">Registro de actividad</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">AnuncioAdjunto</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">Aprobación</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">SecciónCalendario</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">Empresa</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">Cliente</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">PreferenciasDelCliente</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">Documento</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">VersiónDocumento</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Grupo </a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">CarpetaVinculada</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">TareaOperación</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">Parámetro</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">Portfolio</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">Programa</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">Informe programado</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">PreguntaDeTarjetaDePuntuación</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Tarea</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Equipo</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">TareaPlantilla</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Hoja de horas</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">Usuario</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Trabajo </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevel {#accesslevel}

Un objeto AccessLevel está asociado a los usuarios y describe el conjunto de AccessLevelPermissions que determinan a qué puede tener acceso el usuario.

Para obtener más información sobre los niveles de acceso, vea [Funcionamiento de los niveles de acceso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Direct Fields</td>
   --> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">fieldAccessPrivileges</p>
      --> <!--
       <p style="font-weight: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Added the possible value CPJ (Copy). This allows Users with Planner Access Level to copy Projects.</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevelPermissions {#accesslevelpermissions}

Un objeto AccessLevelPermissions representa un permiso específico para tener acceso, crear o modificar un objeto de Workfront. Estos permisos se pueden asociar a un nivel de acceso.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>Se agregaron los siguientes valores posibles:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede actualizar las horas planificadas en el Distribuidor de cargas de trabajo.</p> <p>Para obtener más información, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Actualizar horas planificadas para la tarea al administrar asignaciones de usuarios</a> en <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede agregar campos a los formularios personalizados.</p> <p>Para obtener más información, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede compartir un campo personalizado en todo el sistema con acceso de eliminación.</p> </li> 
      </ul> </li> 
     <li> <p><strong>acciones prohibidas</strong> </p> <p>Se agregaron los siguientes valores posibles:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>Se agregaron los siguientes valores posibles:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">OR</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value PLANNED_HOURS_CONTOURING, which allows a user to update planned hours in the Workload Balancer</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value ADD_TO_CUSTOM_FORMS, which allows a user to add fields to custom forms.</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value EDIT_SYSTEMWIDE, which allows a user to share a custom field system-wide with Delete access. </p>
    --> <!--
     <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <li> <p>coreAction</p> </li> 
      <li> <p>forbiddenActions</p> </li> 
      <li> <p>secondaryActions</p> </li> 
     </ul>
    --> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

Si un usuario no tiene acceso a un objeto de Workfront que necesite, puede solicitar acceso a ese objeto. El objeto AccessRequest representa esta solicitud.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">acción</p> <p>Se agregaron los siguientes valores posibles:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede actualizar las horas planificadas en el Distribuidor de cargas de trabajo.</p> <p>Para obtener más información, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Actualizar horas planificadas para la tarea al administrar asignaciones de usuarios</a> en <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede agregar campos a los formularios personalizados.</p> <p>Para obtener más información, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede compartir un campo personalizado en todo el sistema con acceso de eliminación.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

Un objeto AccessRule representa un conjunto de reglas en niveles de acceso personalizados que determina cómo los usuarios pueden compartir los proyectos que crean.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>Se agregaron los siguientes valores posibles:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede actualizar las horas planificadas en el Distribuidor de cargas de trabajo.</p> <p>Para obtener más información, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Actualizar horas planificadas para la tarea al administrar asignaciones de usuarios</a> en <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede agregar campos a los formularios personalizados.</p> <p>Para obtener más información, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede compartir un campo personalizado en todo el sistema con acceso de eliminación.</p> </li> 
      </ul> </li> 
     <li> <p><strong>acciones prohibidas</strong> </p> <p>Se agregaron los siguientes valores posibles:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>Se agregaron los siguientes valores posibles:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ActivityLog {#activitylog}

Un objeto ActivityLog es una lista completa de todas las actividades que se han realizado en una cuenta de Workfront Proof determinada.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Operaciones</p> </td> 
   <td> <p>Se quitó la siguiente operación del objeto ActivityLog:</p> 
    <ul> 
     <li> <p><strong>AGREGAR</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AnuncioAdjunto {#announcementattachment}

Un objeto AnnouncementAttachment representa un archivo que se ha adjuntado a un anuncio de Workfront.

Para obtener más información acerca de los archivos adjuntos de los anuncios, vea [Enviar anuncios](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos directos</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>Se agregaron valores posibles:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslide (enum.fileextension.qslide)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aprobación {#approval}

Un elemento de trabajo determinado, como una tarea, un documento o una plantilla de horas, puede requerir que un supervisor u otro usuario firme el elemento de trabajo. Un objeto Approval representa la acción de cerrar sesión en un elemento de trabajo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><strong>pedidoRegistroAtrasado</strong> </p> <p>Se han eliminado los siguientes indicadores:</p> 
      <ul> 
       <li> <p>DINÁMICO,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>Id. de grupo</strong> </p> <p>Se agregaron los siguientes indicadores</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DINÁMICO,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>esfuerzoDeTrabajo</strong> </p> <p>Este campo se ha añadido y representa si un usuario necesita un esfuerzo diario pequeño, medio o grande para completar una tarea. Los valores posibles son:</p> 
      <ul> 
       <li> <p>1 (Pequeño)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Grande)</p> </li> 
      </ul> <p>Para obtener más información sobre el esfuerzo de trabajo en Workfront, consulte <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Resumen del esfuerzo de trabajo</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### SecciónCalendario {#calendarsection}

Una sección de calendario es un informe de calendario.

Para obtener más información sobre los informes de calendario, consulte [Resumen de informes de calendario](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p style="font-weight: normal;">Se agregaron los campos siguientes al objeto CalendarSection para admitir la nueva funcionalidad de usar fechas personalizadas en los informes de calendario. </p> <p style="font-weight: normal;">Para obtener más información, consulte <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">Usar campos de fecha personalizados en un informe de calendario</a>.</p> 
    <ul> 
     <li> <p style="font-weight: normal;">customDate</p> </li> 
     <li> <p style="font-weight: normal;">customEndDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">customStartDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">ignoreActualDates</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Compañía {#company}

Un objeto Company representa una organización formada por una colección de personas.

Para obtener más información sobre las compañías, consulte [Crear y editar compañías](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">El ID del grupo con el que está asociada la compañía.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupo</p> <p style="font-weight: normal;">El grupo con el que está asociada la compañía. La asociación de una empresa con un grupo permite al administrador del grupo ampliar el acceso y los permisos del grupo a la empresa.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Cliente {#customer}

Un objeto Customer representa una organización que utiliza una instancia de Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Acciones</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">Esta acción toma un argumento CustomerProductTypeEnum y devuelve un valor booleano que indica si el cliente tiene una cuenta para ese producto. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Preferencias del cliente {#customerpreferences}

Un objeto CustomerPreferences representa el conjunto de preferencias que un cliente ha establecido para su instancia de Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Se agregaron valores posibles:</p> 
      <ul> 
       <li style="font-weight: normal;">contraseña:zoomIntegrationEnabled (habilitar la integración de Zoom en el flujo de actualizaciones)</li> 
       <li style="font-weight: normal;"> contraseña:quipIntegrationEnabled (config.general.quip.enabled)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Documento {#document}

Un objeto Document representa un archivo (como material escrito, imágenes u otras formas de información).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Acciones</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

Un objeto DocumentVersion representa una versión específica de un archivo (como material escrito, imágenes u otras formas de información).

Para obtener más información acerca de las versiones de documentos, vea [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Se ha eliminado el valor posible:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>decisiónDeRevisión</strong> </p> <p>Agregado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Acciones</td> 
   <td> <p>Se agregaron las siguientes acciones al objeto Document.</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">Esta acción toma el argumento documentVersionID (cadena) y devuelve un mapa que indica la decisión del revisor.</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">Esta acción emplea los argumentos siguientes:</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID (cadena)</p> </li> 
       <li> <p>reviewerDecision (cadena)</p> </li> 
       <li> <p>comentario (cadena)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Grupo  {#group}

Un objeto Group representa un conjunto de usuarios y equipos. Los grupos a menudo representan la estructura departamental.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">El ID del coordinador empresarial asignado al grupo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeader</p> <p style="font-weight: normal;">El coordinador empresarial asignado al grupo. Un líder empresarial es alguien que toma decisiones comerciales para el grupo.</p> <p style="font-weight: normal;">Para obtener más información sobre los líderes empresariales, consulte <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Resumen del líder empresarial</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Acciones</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>Esta acción emplea los argumentos siguientes:</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (cadena[])</p> </li> 
       <li> <p>teamID (cadena)</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>Esta acción emplea los argumentos siguientes:</p> 
      <ul> 
       <li> <p>newMemberIDs (string[])</p> </li> 
       <li> <p>removeMemberDs (cadena[])</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

Un objeto LinkedFolder representa una carpeta vinculada desde un proveedor de documentos externo, como Google Drive o Dropbox.

Para obtener más información sobre las carpetas vinculadas, consulte [Enlazar documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos directos</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Se ha eliminado el valor posible:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Un objeto OpTask suele conocerse como Problema. Un problema es un elemento de trabajo que normalmente indica que hay un problema que impide la finalización de una tarea o proyecto. Un problema también puede ser una solicitud del servicio de asistencia. Las solicitudes de cambio, las solicitudes y los errores también son problemas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Campos directos</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>pedidoRegistroAtrasado</strong> </p> <p>El orden indica la posición de una tarea o historia en el registro de asuntos pendientes de Agile.</p> <p>Este campo ha eliminado los siguientes indicadores:
       <ul>
        <li>DINÁMICO,</li>
        <li>LAZY_READ,</li>
        <li>NOT_GROUPABLE:</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> <p>Estas acciones agregaron el estado del argumento para admitir la nueva funcionalidad del botón Inicio, que cambia el estado de un elemento de trabajo cuando un usuario hace clic en el botón para indicar que ha comenzado a trabajar en el elemento.</p> <p>Para obtener más información, vea <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Reemplazar el botón Trabajar en ello por un botón Iniciar</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parámetro {#parameter}

Un objeto Parameter es un campo personalizado.

El recurso Parámetro agregó el indicador SHARABLE.

Para obtener más información sobre los campos personalizados, consulte [Crear o editar un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md) en [Crear o editar un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>Se ha agregado el valor posible:</p> 
      <ul> 
       <li> <p>ENRIQUECIDO (texto enriquecido)</p> <p>Para obtener más información, consulte <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Campos de texto enriquecido en la API de Adobe Workfront</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>Se ha agregado el valor posible:</p> 
      <ul> 
       <li> <p>RICH (Campo de texto con formato)</p> <p>Para obtener más información, consulte <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Campos de texto enriquecido en la API de Adobe Workfront</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>etiqueta</strong> </p> <p>Agregado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de colección</td> 
   <td> 
    <ul> 
     <li> <p><strong>reglas de acceso</strong> </p> <p>Agregado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos predeterminados</td> 
   <td> 
    <ul> 
     <li> <p class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><strong>etiqueta</strong> </p> <p>Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portafolio {#portfolio}

Un objeto Portfolio es una colección de proyectos que compiten por los mismos recursos, normalmente dinero o personas para completarlos.

Para obtener más información sobre portafolios, consulte [descripción general del Portfolio en Adobe Workfront](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">El ID del grupo al que está asociado el portafolio.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupo</p> <p style="font-weight: normal;">El grupo al que está asociado el portafolio. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programar {#program}

Un objeto Program es un subconjunto de proyectos dentro de un portafolio, donde se pueden agrupar proyectos similares.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">El ID del grupo al que está asociado el programa.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupo</p> <p style="font-weight: normal;">Grupo al que está asociado el programa. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Un objeto QueueDef representa una cola, que es un proyecto que se ha publicado en el área del servicio de asistencia para permitir a los usuarios enviar problemas al mismo.

Para obtener más información sobre las colas de solicitudes, vea [Crear una cola de solicitudes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li><strong>requestorCoreAction</strong> <p>Se agregaron los siguientes valores posibles:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede actualizar las horas planificadas en el Distribuidor de cargas de trabajo.</p> <p>Para obtener más información, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Actualizar horas planificadas para la tarea al administrar asignaciones de usuarios</a> en <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede agregar campos a los formularios personalizados.</p> <p>Para obtener más información, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede compartir un campo personalizado en todo el sistema con acceso de eliminación.</p> </li>
       <ul> 
        <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
        <li> <p>EDIT_SYSTEMWIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### InformeProgramado {#scheduledreport}

Un objeto ScheduledReport representa un informe que se ha configurado para que se programe su envío.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><strong>formato</strong> </p> <p>Se agregaron valores posibles:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslide (enum.fileextension.qslide)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Un objeto ScoreCardQuestion representa una pregunta que se ha agregado a un informe de valoración. Estas preguntas suelen ser determinadas por el gestor del Portfolio, y sus respuestas le permiten comprender cómo se ajusta un proyecto a los objetivos del portafolio.

Para obtener más información sobre las preguntas del informe de valoración, consulte [Crear un informe de valoración](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Se ha agregado un posible valor ENRIQUECIDO (Campo de texto con formato) </p> <p style="font-weight: normal;">Para obtener más información, consulte <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Campos de texto enriquecido en la API de Adobe Workfront</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tarea {#task}

Un objeto Task representa un elemento de trabajo que debe realizarse como un paso hacia el logro de un objetivo final (completar un proyecto).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><strong>esfuerzoDeTrabajo</strong> </p> <p>Este campo se ha añadido y representa si un usuario necesita un esfuerzo diario pequeño, medio o grande para completar una tarea. Los valores posibles son:</p> 
      <ul> 
       <li> <p>1 (Pequeño)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Grande)</p> </li> 
      </ul> <p>Para obtener más información sobre el esfuerzo de trabajo en Workfront, consulte <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Resumen del esfuerzo de trabajo</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> <p>Estas acciones agregaron el estado del argumento para admitir la nueva funcionalidad del botón Inicio, que cambia el estado de un elemento de trabajo cuando un usuario hace clic en el botón para indicar que ha comenzado a trabajar en el elemento.</p> <p>Para obtener más información, vea <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Reemplazar el botón Trabajar en ello por un botón Iniciar</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Equipo {#team}

Un objeto Team es una colección de usuarios que se pueden asignar a un elemento de trabajo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> <p>Se agregaron los campos siguientes al recurso de equipo:</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>Este campo representa el número de días que una tarjeta completada permanece en el Panel Kanban.</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>Id. de grupo</strong> </p> <p>Este campo asocia un equipo con un grupo. Esto identifica al equipo como parte del grupo y permite al administrador del grupo administrar los equipos.</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>Es un parámetro booleano que indica si el botón Trabajar en ello del equipo se ha configurado como botón Inicio. Cuando un miembro del equipo hace clic en un botón Iniciar para comenzar a trabajar en un elemento de trabajo, el estado del elemento cambia de Nuevo a un estado configurado en la configuración del equipo.</p> </li> 
     <li> <p>Los campos siguientes permiten especificar estados personalizados para el botón Inicio en los elementos de trabajo individuales.</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatus</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuses</strong> </p> <p><strong>workOnItTaskStatus</strong> </p> </li> 
      </ul> <p>Para obtener más información sobre el botón Inicio, vea <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Reemplazar el botón Trabajar en ello por un botón Iniciar</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de referencia</td> 
   <td> <p>Se agregó el campo siguiente al recurso de equipo:</p> 
    <ul> 
     <li> <p><strong>grupo</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

Un objeto TemplateTask representa un objeto Task que forma parte de un objeto Template. Las Tareas de plantilla pasan a ser Tareas en el Proyecto en el que se utiliza la Plantilla.

Para obtener más información sobre las tareas de plantilla, consulte [Editar una tarea de plantilla](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><strong>esfuerzoDeTrabajo</strong> </p> <p>Este campo se ha añadido y representa si un usuario necesita un esfuerzo diario pequeño, medio o grande para completar una tarea. Los valores posibles son:</p> 
      <ul> 
       <li> <p>1 (Pequeño)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Grande)</p> </li> 
      </ul> <p>Para obtener más información sobre el esfuerzo de trabajo en Workfront, consulte <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Resumen del esfuerzo de trabajo</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Hoja de horas {#timesheet}

Un objeto Timesheet representa un parte de horas virtual que permite a los usuarios especificar horas trabajadas reales para tareas, proyectos y tipos de horas generales.

Para obtener más información sobre las hojas de horas, consulte [Información general sobre hojas de horas](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos principales</td> 
   <td> <p>El campo siguiente se ha eliminado del recurso de plantilla de horas:</p> 
    <ul> 
     <li> <p><strong>código de objeto</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Actualizar

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><strong>updateType</strong> </p> <p>Se agregaron los siguientes valores posibles:</p> 
      <ul> 
       <li> <p>initiativeAdd (enum.updatetype.initiativeadd)</p> </li> 
       <li> <p>initiativeEdit (enum.updatetype.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Para obtener más información sobre las iniciativas, consulte <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">Información general sobre iniciativas en el Scenario Planner</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Usuario {#user}

Un objeto User representa a una persona con una cuenta en Workfront que puede iniciar sesión e interactuar con el sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> <p>Se agregaron los campos siguientes al recurso de usuario:</p> 
    <ul> 
     <li> <p><strong>actualDeactivationDate</strong> </p> <p>Representa la fecha y la hora en que se desactivó un usuario.</p> <p>Para obtener más información sobre los usuarios desactivados, consulte <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>Este campo muestra el acceso del usuario a las Metas de Workfront. Los valores posibles son:</p> 
      <ul> 
       <li> <p>Sin acceso</p> </li> 
       <li> <p>Ver</p> </li> 
       <li> <p>Editar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> <p>Se ha añadido la siguiente acción al recurso de usuario:</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>Esta acción emplea los argumentos siguientes</p> 
      <ul> 
       <li> <p>ids (cadena)</p> </li> 
       <li> <p>objCode (cadena)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Trabajo  {#work}

Un objeto Work es una interfaz común que heredan Task y OpTask, y comparte código común entre ambos.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><strong>pedidoRegistroAtrasado</strong> </p> <p>El orden indica la posición de una tarea o historia en el registro de asuntos pendientes de Agile.</p> <p>Este campo ha eliminado los siguientes indicadores:</p> 
      <ul> 
       <li> <p>DINÁMICO,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>Id. de grupo</strong> </p> <p>Este campo añadió los siguientes indicadores:</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DINÁMICO,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>esfuerzoDeTrabajo</strong> </p> <p>Este campo se ha añadido y representa si un usuario necesita un esfuerzo diario pequeño, medio o grande para completar una tarea. Los valores posibles son:</p> 
      <ul> 
       <li> <p>1 (Pequeño)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Grande)</p> </li> 
      </ul> <p>Para obtener más información sobre el esfuerzo de trabajo en Workfront, consulte <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Resumen del esfuerzo de trabajo</a>.</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
