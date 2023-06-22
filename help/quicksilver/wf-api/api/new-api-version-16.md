---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 16 de la API
description: Adobe Workfront publicó la versión 16 de la API el 6 de abril de 2022. La versión 16 de la API incorpora los siguientes cambios con respecto a la versión 15.
author: Becky
feature: Workfront API
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: 3e6f4b8c8bfb9cb6106dbb9522d77f5133a886e3
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Novedades de la versión 16 de la API

Adobe Workfront publicó la versión 16 de la API el 6 de abril de 2022. La versión 16 de la API incorpora los siguientes cambios con respecto a la versión 15.

## Recursos añadidos

No se han añadido recursos para la versión 16 de la API.

## Recursos eliminados

No se han eliminado recursos para la versión 16 de la API

## Recursos modificados

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [Aprobación (APPROVAL)](#approval-approval)
* [Preferencias del cliente (CUSTPR)](#customerpreferences-custpr)
* [Sección externa (EXTSEC)](#externalsection-extsec)
* [Hora (HORA)](#hour-hour)
* [Plantilla de diseño (UITMPL)](#layouttemplate-uitmpl)
* [Nota (NOTA)](#note-note)
* [OpTask / Problema (OPTASK)](#note-note)
* [Proyecto (PROJ)](#project-proj)
* [Tasa (TASA)](#rate-rate)
* [RichTextNote (RHNOTE)](#richtextnote-rhnote)
* [Rol / Rol (ROLE)](#role--job-role-role)
* [Tarea (TAREA)](#task-task)
* [Hoja de horas (TSHET)](#timesheet-tshet)
* [UIFilter / Filter (UIFT)](#uifilter--filter-uift)
* [UIGroupBy / Grouping (UIGB)](#uigroupby--grouping-uigb)
* [Vista/vista de IU (UIVW)](#uiview--view-uivw)
* [Usuario (USER)](#user-user)
* [UserNote (USRNOT)](#usernote-usrnot)

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

-->

### Aprobación (APPROVAL)

Un elemento de trabajo determinado, como una tarea, un documento o una plantilla de horas, puede requerir que un supervisor u otro usuario firme el elemento de trabajo. Un objeto Approval representa la acción de cerrar sesión en un elemento de trabajo.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Este campo se ha añadido y muestra la cantidad de minutos de trabajo por día que debe realizar. Tiene el formato <code>YYYY-MM-DD: (number of minutes)</code>y tiene en cuenta la zona horaria.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Asignación (ASIGNAR)

Un objeto de asignación representa la conexión entre un elemento de trabajo y el usuario, equipo o grupo asignado para trabajar en él.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Este campo se ha añadido y muestra la cantidad de minutos de trabajo por día que debe realizar. Tiene el formato <code>YYYY-MM-DD: (number of minutes)</code>y tiene en cuenta la zona horaria.</p>
          </li>
          <li>
            <p><b>isContour</b>
            </p>
            <p>Se ha añadido este campo, que es un booleano que refleja si la asignación está contorneada. Si se han editado los minutos diarios de la asignación en el Distribuidor de cargas de trabajo, se ha perfilado la asignación.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum (CSTEM)

El objeto CustomEnum ayuda a convertir los códigos de estado en texto legible en lenguaje natural.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <ul>
          <li>
            <p><b>getDefaultProjectStatusEnumForGroup
</b>
            </p>
            <p></p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Preferencias del cliente (CUSTPR)

Un objeto CustomerPreferences representa el conjunto de preferencias que un cliente ha establecido para su instancia de Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>name</b>
            </p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>customer:config.general.autoupgradedisabled</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">acciones</td>
      <td>
        <ul>
          <li>
            <p><b>getIsAutoUpgradeDisabled</b>
            </p>
            <p>Esta acción devuelve un valor booleano que describe si el cliente ha deshabilitado la opción para actualizar automáticamente los titulares de licencias de colaborador.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Sección externa (EXTSEC)

Un objeto ExternalSection es una página web externa incrustada en un informe de Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">acciones</td>
      <td>
        <ul>
           <li>
            <p><b>calculateIframeURL</b>
            </p>
            <p>Se agregó y calcula la dirección URL de un iFrame incrustado en un informe.</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>Se agregó y calcula las direcciones URL de los iFrames incrustados en un informe.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Hora (HORA)

Un objeto Hour representa una hora registrada por un usuario en una plantilla de horas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>timesheetHourIdentifier</b>
            </p>
            <p>Agregado. Este parámetro se utiliza para identificar las horas creadas con <code>batchSave</code>. </p>
           </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### LayoutTemplate (UITMPL)

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. A LayoutTemplate object represents one of these templates.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
-->

### Nota (NOTA)

Un objeto Note es un comentario o una actualización realizada sobre un objeto Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <ul>
          <li>
            <p><b>attachmentDocuments</b>
            </p>
            <p>Este campo se ha añadido y representa una lista de documentos adjuntos al comentario.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask / Problema (OPTASK)

Un objeto OpTask suele conocerse como Problema. Un problema es un elemento de trabajo que normalmente indica que hay un problema que impide la finalización de una tarea o proyecto. Un problema también puede ser una solicitud del servicio de asistencia. Las solicitudes de cambio, las solicitudes y los errores también son problemas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Este campo se ha añadido y muestra la cantidad de minutos de trabajo por día que debe realizar. Tiene el formato <code>YYYY-MM-DD: (number of minutes)</code>y tiene en cuenta la zona horaria.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">acciones</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>Esta acción añadió el campo <code>teamIDs</code> para admitir la funcionalidad de asignar varios equipos a una tarea o un problema.</p>
         </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Proyecto (PROJ)

Los proyectos son elementos de trabajo dentro de Workfront y son un bloque de creación principal en la forma en que Workfront ayuda a las personas a realizar su trabajo. Un objeto Project representa un grupo de tareas con un objetivo común y específico.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours</b>
            </p>
            <p>Este campo se ha añadido y representa la suma de todas las horas presupuestadas del proyecto.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Tasa (TASA)

Un objeto Rate representa una tarifa de facturación en Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
             <p><b>costPerHour</b></p>
            <p><b>LocalBillingPerHour</b></p>
            <p><b>localCostPerHour</b></p>
            <p><b>localCurrency</b></p>
           <p>Estos parámetros se han movido al objeto Rate desde el objeto Role, de modo que los objetos Role y User pueden tener varios valores (para intervalos de fechas independientes).</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>Estos parámetros representan el ID. y el código de objeto del objeto al que está asociada la Tasa.
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <ul>
          <li>
             <p><b>setRateForObject</b></p>
           <p>Esta acción se ha añadido y adjunta objetos Rate al objeto dado. Este punto de conexión funciona para todos los objetos de tasa de conexión.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote (RHNOTE)

Un objeto RichTextNote es un comentario o una actualización realizados en un objeto de Workfront, que incluye texto enriquecido como negrita o cursiva.

El objeto RichTextNote quitó el indicador `REPORTABLE`.

### Rol / Rol (ROLE)

Un objeto Role (función del puesto) representa una capacidad funcional o un conjunto de aptitudes que un usuario podría rellenar, como Designer o Product Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <ul>
           <li>
            <p><b>tarifas</b>
            </p>
            <p>Se ha agregado y representa los objetos Rate adjuntos a este rol.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Tarea (TAREA)

Un objeto Task representa un elemento de trabajo que debe realizarse como un paso hacia el logro de un objetivo final (completar un proyecto).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Este campo se ha añadido y muestra la cantidad de minutos de trabajo por día que debe realizar. Tiene el formato <code>YYYY-MM-DD: (number of minutes)</code>y tiene en cuenta la zona horaria.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">acciones</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>Esta acción añadió el campo <code>teamIDs</code> para admitir la funcionalidad de asignar varios equipos a una tarea o un problema.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### Hoja de horas (TSHET)

Un objeto Timesheet representa un parte de horas virtual que permite a los usuarios especificar horas trabajadas reales para tareas, proyectos y tipos de horas generales.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
           <li>
            <p><b>availableActions</b>
            </p>
            <p>Este parámetro ha eliminado el indicador <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>Este parámetro ha eliminado el indicador <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>Se agregó este parámetro, y almacena la duración de la hoja de horas en días independientemente de los cambios a "Horas equivalentes para Workday completo".  Por ejemplo, si Horas equivalentes se establece en 6 y se registra un día, entonces Horas equivalentes se cambia a 8 horas, <code>totalDays</code> aún tiene un valor de 1.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter / Filter (UIFT)



<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">acciones</td>
      <td>
        <ul>
          <li>
            <p><b>addJoinForNullableFields</b>
            </p>
            <p>Esta acción se añadió y toma un mapa de consulta de filtro y añade el <code>allowingnull</code> unir para campos que admiten valores NULL.</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Estas acciones admiten la capacidad de compartir filtros, vistas y agrupaciones en todo el sistema.</p><p>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Hacer que los filtros, vistas o agrupaciones estén disponibles para todos los usuarios</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy / Grouping (UIGB)


<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">acciones</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Estas acciones admiten la capacidad de compartir filtros, vistas y agrupaciones en todo el sistema.</p><p>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Hacer que los filtros, vistas o agrupaciones estén disponibles para todos los usuarios</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### Vista/vista de IU (UIVW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>layoutType</b>
            </p>
            <p>Se ha añadido el siguiente valor posible:</p>
            <ul>
              <li>
                <p><code>WLIST</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">acciones</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Estas acciones admiten la capacidad de compartir filtros, vistas y agrupaciones en todo el sistema.</p><p>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Hacer que los filtros, vistas o agrupaciones estén disponibles para todos los usuarios</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Usuario (USER)

Un objeto User representa a una persona con una cuenta en Workfront que puede iniciar sesión e interactuar con el sistema.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <ul>
           <li>
            <p><b>tarifas</b>
            </p>
            <p>Se ha agregado, y representa los objetos Rate adjuntos a este usuario.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote (USRNOT)

Un objeto UserNote es una notificación.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Consultas</td>
      <td>
        <ul>
          <li>
            <p><b>myAllObjectTypesUnreadNotifications</b>
            </p>
            <p>Se ha añadido el siguiente valor posible:
            <ul>
            <li>
            includeAll
            </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Trabajo (TRABAJO)

Un objeto Work es una interfaz común que heredan Task y OpTask, y comparte código común entre ambos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Este campo se ha añadido y muestra la cantidad de minutos de trabajo por día que debe realizar. Tiene el formato <code>YYYY-MM-DD: (number of minutes)</code>y tiene en cuenta la zona horaria.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
