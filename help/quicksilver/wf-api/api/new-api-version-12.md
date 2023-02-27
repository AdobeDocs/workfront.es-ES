---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 12 de la API
description: Workfront lanzó la versión 12 de la API el 12 de noviembre de 2020. La versión 12 de la API presenta los siguientes cambios con respecto a la versión 11
author: Becky
feature: Workfront API
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '2516'
ht-degree: 2%

---

# Novedades de la versión 12 de la API

Workfront lanzó la versión 12 de la API el 12 de noviembre de 2020. La versión 12 de la API presenta los siguientes cambios con respecto a la versión 11

## Recursos añadidos

Los siguientes recursos son nuevos en la versión 12 de la API de Workfront.

* [BreadCrumb](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

Un objeto BreadCrumb representa un elemento en la jerarquía principal/secundaria de un elemento de trabajo de Adobe Workfront. Las rutas de exploración indican cómo encaja un elemento de trabajo en la buena estructura de Portfolio, Proyectos, Proyectos y Tareas.

Para obtener más información sobre rutas de exploración en Workfront, consulte [Información general sobre rutas de exploración en la nueva experiencia de Adobe Workfront](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

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

No se eliminaron recursos para la versión 12 de la API.

## Recursos modificados

Se modificaron los siguientes recursos para la versión 12 de la API de Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">AccessRule</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">ActivityLog</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">AnuncioAdjunto</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">Ruta de aprobación</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">SecciónCalendario</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">Compañía</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">Cliente</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">Preferencias de cliente</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">Documento</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Grupo </a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">Parámetro</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">Portafolio</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">Programar</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">Informe programado</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Tarea</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Equipo</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">TemplateTask</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Hoja de horas</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">Usuario</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Trabajo </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevel {#accesslevel}

Un objeto AccessLevel está asociado a los usuarios y describe el conjunto de AccessLevelPermissions que determinan a qué puede acceder el usuario.

Para obtener más información sobre los niveles de acceso, consulte [Funcionamiento de los niveles de acceso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

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

Un objeto AccessLevelPermissions representa un permiso específico para acceder, crear o modificar un objeto de Workfront. Estos permisos se pueden asociar a un nivel de acceso.

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
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede actualizar las horas programadas en el equilibrador de carga de trabajo.</p> <p>Para obtener más información, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Actualizar las horas planificadas de la tarea al administrar las asignaciones de usuario</a> en <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Administrar asignaciones de usuario en el equilibrador de carga de trabajo</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede agregar campos a formularios personalizados.</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> en <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede compartir un campo personalizado de todo el sistema con acceso de eliminación.</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configuración del uso compartido para campos personalizados y widgets</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>prohibidaActions</strong> </p> <p>Se agregaron los siguientes valores posibles:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secundarioActions</strong> </p> <p>Se agregaron los siguientes valores posibles:</p> 
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
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede actualizar las horas programadas en el equilibrador de carga de trabajo.</p> <p>Para obtener más información, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Actualizar las horas planificadas de la tarea al administrar las asignaciones de usuario</a> en <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Administrar asignaciones de usuario en el equilibrador de carga de trabajo</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede agregar campos a formularios personalizados.</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> en <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede compartir un campo personalizado de todo el sistema con acceso de eliminación.</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configuración del uso compartido para campos personalizados y widgets</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

Un objeto AccessRule representa un conjunto de reglas en niveles de acceso personalizados que determina cómo pueden compartir los usuarios los proyectos que crean.

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
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede actualizar las horas programadas en el equilibrador de carga de trabajo.</p> <p>Para obtener más información, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Actualizar las horas planificadas de la tarea al administrar las asignaciones de usuario</a> en <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Administrar asignaciones de usuario en el equilibrador de carga de trabajo</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede agregar campos a formularios personalizados.</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> en <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede compartir un campo personalizado de todo el sistema con acceso de eliminación.</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configuración del uso compartido para campos personalizados y widgets</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>prohibidaActions</strong> </p> <p>Se agregaron los siguientes valores posibles:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secundarioActions</strong> </p> <p>Se agregaron los siguientes valores posibles:</p> 
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

Un objeto ActivityLog es una lista completa de toda la actividad que se ha realizado en una cuenta de prueba de Workfront determinada.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Operaciones</p> </td> 
   <td> <p>Se eliminó la siguiente operación del objeto ActivityLog:</p> 
    <ul> 
     <li> <p><strong>AGREGAR</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AnuncioAdjunto {#announcementattachment}

Un objeto AnnouncementoAttachment representa un archivo que se ha adjuntado a un anuncio de Workfront.

Para obtener más información sobre los archivos adjuntos a los anuncios, consulte [Enviar anuncios](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos directos</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>Se han añadido valores posibles:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qSlide (enum.fileextension.qSlide)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Ruta de aprobación {#approval}

Un elemento de trabajo determinado, como una tarea, un documento o un parte de horas, puede requerir que un supervisor u otro usuario cierre la sesión en el elemento de trabajo. Un objeto Approval representa la acción de cerrar sesión en un elemento de trabajo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Se han eliminado los siguientes indicadores:</p> 
      <ul> 
       <li> <p>DINÁMICO,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Se agregaron los siguientes indicadores</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DINÁMICO,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>Este campo se ha añadido y representa si se requiere un esfuerzo diario pequeño, medio o grande para completar una tarea. Los valores posibles son:</p> 
      <ul> 
       <li> <p>1 (pequeño)</p> </li> 
       <li> <p>2 (Medio)</p> </li> 
       <li> <p>3 (Grande)</p> </li> 
      </ul> <p>Para obtener más información sobre el esfuerzo de trabajo en Workfront, consulte <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Información general sobre el esfuerzo de trabajo</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### SecciónCalendario {#calendarsection}

Una sección del calendario es un informe del calendario.

Para obtener más información sobre los informes de calendario, consulte [Información general sobre los informes del calendario](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p style="font-weight: normal;">Se agregaron los siguientes campos al objeto CalendarSection para admitir la nueva funcionalidad de usar fechas personalizadas en informes de calendario. </p> <p style="font-weight: normal;">Para obtener más información, consulte <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">Usar campos de fecha personalizados en un informe de calendario</a>.</p> 
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

Un objeto Company representa una organización que consta de una colección de personas.

Para obtener más información sobre las empresas, consulte [Crear y editar empresas](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">El ID del grupo al que está asociada la empresa.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupo</p> <p style="font-weight: normal;">Grupo al que está asociada la empresa. La asociación de una empresa con un grupo permite que el administrador del grupo amplíe el acceso y los permisos del grupo a la empresa.</p> </li> 
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

### Preferencias de cliente {#customerpreferences}

Un objeto CustomerPreferences representa el conjunto de preferencias que un cliente ha establecido para su instancia de Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Se han añadido valores posibles:</p> 
      <ul> 
       <li style="font-weight: normal;">password:zoomIntegrationEnabled (habilitar la integración de zoom en el flujo de actualizaciones)</li> 
       <li style="font-weight: normal;"> password:quipIntegrationEnabled (config.general.quip.enabled)  </li> 
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

Para obtener más información sobre las versiones de documentos, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Se ha eliminado el posible valor:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>proofdecisions</strong> </p> <p>Agregado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Acciones</td> 
   <td> <p>Se agregaron las siguientes acciones al objeto Document .</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerdecisions</p> <p style="font-weight: normal;">Esta acción toma el argumento documentVersonID (cadena) y devuelve un mapa que indica la decisión del revisor.</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerdecisions</p> <p style="font-weight: normal;">Esta acción toma los siguientes argumentos:</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID (cadena)</p> </li> 
       <li> <p>reviewerdecisions (cadena)</p> </li> 
       <li> <p>comment (cadena)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Grupo  {#group}

Un objeto Group representa un conjunto de usuarios y equipos. Los grupos suelen representar la estructura departamental.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">ID del líder empresarial asignado al grupo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeader</p> <p style="font-weight: normal;">Líder empresarial asignado al grupo. Un líder empresarial es alguien que toma decisiones comerciales para el grupo.</p> <p style="font-weight: normal;">Para obtener más información sobre los líderes empresariales, consulte <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Información general de Business Leader</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Acciones</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>Esta acción toma los siguientes argumentos:</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (string[])</p> </li> 
       <li> <p>teamID (cadena)</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>Esta acción toma los siguientes argumentos:</p> 
      <ul> 
       <li> <p>newMemberIDs (string[])</p> </li> 
       <li> <p>removeMemberDs (string[])</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

Un objeto LinkedFolder representa una carpeta vinculada desde un proveedor de documentos externo, como Google Drive o Dropbox.

Para obtener más información sobre las carpetas vinculadas, consulte [Vincular documentos de aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos directos</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Se ha eliminado el posible valor:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Un objeto OpTask se conoce comúnmente como Problema. Un problema es un elemento de trabajo que normalmente indica que hay un problema que impide la finalización de una tarea o proyecto. Un problema también puede ser una solicitud de asistencia técnica. Los cambios de pedidos, solicitudes y errores también son problemas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Campos directos</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>El orden indica una tarea o la posición de un artículo en el registro acumulado Agile.</p> <p>Este campo ha eliminado los siguientes indicadores:
       <ul>
        <li>DINÁMICO,</li>
        <li>LAZY_READ,</li>
        <li>NOT_GROUPABLE:</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> <p>Estas acciones agregaron el estado del argumento para admitir la nueva funcionalidad del botón Inicio , que cambia el estado de un elemento de trabajo cuando un usuario hace clic en el botón para indicar que ha empezado a trabajar en el elemento.</p> <p>Para obtener más información, consulte <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Reemplazar el botón Trabajar en él con un botón Inicio</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parámetro {#parameter}

Un objeto Parameter es un campo personalizado.

El recurso Parámetro ha añadido el indicador SHARABLE.

Para obtener más información sobre los campos personalizados, consulte [Crear o editar un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) en [Crear o editar un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>Se ha añadido un valor posible:</p> 
      <ul> 
       <li> <p>RICH (texto enriquecido)</p> <p>Para obtener más información, consulte <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Campos de texto enriquecido en la API de Adobe Workfront</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>Se ha añadido un valor posible:</p> 
      <ul> 
       <li> <p>RICH (Campo de texto con formato)</p> <p>Para obtener más información, consulte <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Campos de texto enriquecido en la API de Adobe Workfront</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>label</strong> </p> <p>Agregado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de colección</td> 
   <td> 
    <ul> 
     <li> <p><strong>accessRules</strong> </p> <p>Agregado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos predeterminados</td> 
   <td> 
    <ul> 
     <li> <p class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><strong>label</strong> </p> <p>Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portafolio {#portfolio}

Un objeto Portfolio es una colección de proyectos que compiten por los mismos recursos, normalmente dinero o personas para completarlos.

Para obtener más información sobre portafolios, consulte [Información general del Portfolio en Adobe Workfront](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

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
     <li style="font-weight: bold;"> <p>grupo</p> <p style="font-weight: normal;">Grupo al que está asociada la cartera. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programar {#program}

Un objeto Program es un subconjunto de proyectos dentro de un portafolio, donde proyectos similares se pueden agrupar.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">ID del grupo al que está asociado el programa.</p> </li> 
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

Un objeto QueueDef representa una cola, que es un proyecto que se ha publicado en el área de asistencia técnica para permitir a los usuarios enviarle problemas.

Para obtener más información sobre las colas de solicitud, consulte [Crear una cola de solicitud](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

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
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede actualizar las horas programadas en el equilibrador de carga de trabajo.</p> <p>Para obtener más información, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Actualizar las horas planificadas de la tarea al administrar las asignaciones de usuario</a> en <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Administrar asignaciones de usuario en el equilibrador de carga de trabajo</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede agregar campos a formularios personalizados.</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> en <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Un usuario con un nivel de acceso que incluya este permiso puede compartir un campo personalizado de todo el sistema con acceso de eliminación.</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configuración del uso compartido para campos personalizados y widgets</a></p> </li> 
      </ul> <li> <p><strong>requestorForbioredActions</strong> </p> <p>Se agregaron los siguientes valores posibles:</p> 
       <ul> 
        <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
        <li> <p>EDIT_SYSTEMWIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Informe programado {#scheduledreport}

Un objeto ScheduledReport representa un informe que se ha configurado para su envío programado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><strong>format</strong> </p> <p>Se han añadido valores posibles:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qSlide (enum.fileextension.qSlide)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Un objeto ScoreCardQuestion representa una pregunta que se ha agregado a un informe de valoración. Estas preguntas suelen ser determinadas por el administrador de Portfolio y sus respuestas permiten al administrador comprender cómo se alinea un proyecto con los objetivos del portafolio.

Para obtener más información sobre las preguntas del informe de valoración, consulte [Crear un informe de valoración](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Se ha añadido un posible valor RICH (campo de texto con formato) </p> <p style="font-weight: normal;">Para obtener más información, consulte <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Campos de texto enriquecido en la API de Adobe Workfront</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tarea {#task}

Un objeto Task representa un elemento de trabajo que debe realizarse como paso hacia el logro de un objetivo final (completar un proyecto).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>Este campo se ha añadido y representa si se requiere un esfuerzo diario pequeño, medio o grande para completar una tarea. Los valores posibles son:</p> 
      <ul> 
       <li> <p>1 (pequeño)</p> </li> 
       <li> <p>2 (Medio)</p> </li> 
       <li> <p>3 (Grande)</p> </li> 
      </ul> <p>Para obtener más información sobre el esfuerzo de trabajo en Workfront, consulte <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Información general sobre el esfuerzo de trabajo</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> <p>Estas acciones agregaron el estado del argumento para admitir la nueva funcionalidad del botón Inicio , que cambia el estado de un elemento de trabajo cuando un usuario hace clic en el botón para indicar que ha empezado a trabajar en el elemento.</p> <p>Para obtener más información, consulte <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Reemplazar el botón Trabajar en él con un botón Inicio</a>.</p> 
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
   <td> <p>Se agregaron los siguientes campos al recurso Equipo :</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>Este campo representa el número de días que una tarjeta completada permanece en el tablero Kanban.</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Este campo asocia un equipo con un grupo. Esto identifica al equipo como parte del grupo y permite que el administrador del grupo administre los equipos.</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>Este es un parámetro booleano que indica si el botón Trabajar en él del equipo se ha configurado como botón de Inicio. Cuando un miembro del equipo hace clic en un botón Inicio para comenzar a trabajar en un elemento de trabajo, el estado del elemento cambia de Nuevo a un estado configurado en la configuración del equipo.</p> </li> 
     <li> <p>Los siguientes campos le permiten especificar estados personalizados para el botón Inicio de los elementos de trabajo individuales.</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatus</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatus</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatus</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatus</strong> </p> <p><strong>workOnItTaskStatus</strong> </p> </li> 
      </ul> <p>Para obtener más información sobre el botón Inicio, consulte <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Reemplazar el botón Trabajar en él con un botón Inicio</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de referencia</td> 
   <td> <p>Se ha añadido el siguiente campo al recurso Equipo :</p> 
    <ul> 
     <li> <p><strong>grupo</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

Un objeto TemplateTask representa una tarea que forma parte de una plantilla. Las tareas de plantilla se convierten en tareas del proyecto en el que se utiliza la plantilla.

Para obtener más información sobre las tareas de plantilla, consulte [Editar una tarea de plantilla](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>Este campo se ha añadido y representa si se requiere un esfuerzo diario pequeño, medio o grande para completar una tarea. Los valores posibles son:</p> 
      <ul> 
       <li> <p>1 (pequeño)</p> </li> 
       <li> <p>2 (Medio)</p> </li> 
       <li> <p>3 (Grande)</p> </li> 
      </ul> <p>Para obtener más información sobre el esfuerzo de trabajo en Workfront, consulte <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Información general sobre el esfuerzo de trabajo</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Hoja de horas {#timesheet}

Un objeto de parte de horas representa un panel de tiempo virtual que permite a los usuarios introducir horas reales trabajadas para tareas, proyectos y tipos de horas generales.

Para obtener más información sobre las hojas de tiempo, consulte [Información general sobre las hojas de tiempo](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos principales</td> 
   <td> <p>Se ha eliminado el siguiente campo del recurso de parte de horas:</p> 
    <ul> 
     <li> <p><strong>objcode</strong> </p> </li> 
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
       <li> <p>InitiativeAdd (enum.updatetypeenum.initiativeadd)</p> </li> 
       <li> <p>InitiativeEdit (enum.updatetypeenum.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Para obtener más información sobre las iniciativas, consulte <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">Información general sobre las iniciativas en el planificador de escenarios</a>.</p> </li> 
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
   <td> <p>Se agregaron los siguientes campos al recurso Usuario :</p> 
    <ul> 
     <li> <p><strong>realDeactivationDate</strong> </p> <p>Representa la fecha y hora en que se desactivó un usuario.</p> <p>Para obtener más información sobre los usuarios desactivados, consulte <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>Este campo muestra el acceso del usuario a los objetivos de Workfront. Los valores posibles son:</p> 
      <ul> 
       <li> <p>Sin acceso</p> </li> 
       <li> <p>Vista</p> </li> 
       <li> <p>Editar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> <p>Se ha añadido la siguiente acción al recurso Usuario :</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>Esta acción toma los siguientes argumentos</p> 
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
     <li> <p><strong>backlogOrder</strong> </p> <p>El orden indica una tarea o la posición de un artículo en el registro acumulado Agile.</p> <p>Este campo ha eliminado los siguientes indicadores:</p> 
      <ul> 
       <li> <p>DINÁMICO,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Este campo agregó los siguientes indicadores:</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DINÁMICO,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>Este campo se ha añadido y representa si se requiere un esfuerzo diario pequeño, medio o grande para completar una tarea. Los valores posibles son:</p> 
      <ul> 
       <li> <p>1 (pequeño)</p> </li> 
       <li> <p>2 (Medio)</p> </li> 
       <li> <p>3 (Grande)</p> </li> 
      </ul> <p>Para obtener más información sobre el esfuerzo de trabajo en Workfront, consulte <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Información general sobre el esfuerzo de trabajo</a>.</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
