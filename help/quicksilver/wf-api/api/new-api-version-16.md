---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 16 de la API
description: Adobe Workfront publicó la versión 16 de la API el 6 de abril de 2022. La versión 16 de la API incorpora los siguientes cambios con respecto a la versión 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: acd1fe5500776b8f16c67b05048a88d0c8107079
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 99%

---

# Novedades de la versión 16 de la API

Adobe Workfront publicó la versión 16 de la API el 6 de abril de 2023. La versión 16 de la API incorpora los siguientes cambios con respecto a la versión 15.

## Recursos añadidos

No se han añadido recursos para la versión 16 de la API.

## Recursos eliminados

No se han eliminado recursos para la versión 16 de la API

## Recursos modificados

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [Aprobación (APPROVAL)](#approval-approval)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [Sección externa (EXTSEC)](#externalsection-extsec)
* [Hora (HORA)](#hour-hour)
* [Plantilla de diseño (UITMPL)](#layouttemplate-uitmpl)
* [Nota (NOTA)](#note-note)
* [OpTask / Problema (OPTASK)](#note-note)
* [Proyecto (PROJ)](#project-proj)
* [Tasa (RATE)](#rate-rate)
* [RichTextNote (RHNOTE)](#richtextnote-rhnote)
* [Rol / Función (ROLE)](#role--job-role-role)
* [Tarea (TAREA)](#task-task)
* [Plantilla de horas (TSHET)](#timesheet-tshet)
* [UIFilter / Filter (UIFT)](#uifilter--filter-uift)
* [UIGroupBy / Grouping (UIGB)](#uigroupby--grouping-uigb)
* [UIView / Vista (UIVW)](#uiview--view-uivw)
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

Un elemento de trabajo determinado, como una tarea, un documento o una plantilla de horas, puede requerir que un supervisor u otro usuario firme el elemento de trabajo. Un objeto de aprobación representa la acción de cerrar sesión en un elemento de trabajo.

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
            <p>Este campo se ha añadido y muestra la cantidad de minutos de trabajo por día que debe realizar. Tiene en cuenta el formato <code>YYYY-MM-DD: (number of minutes)</code> y la zona horaria.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Asignación (ASSGN)

Un objeto de asignación representa la conexión entre un elemento de trabajo y el usuario, equipo o grupo que tiene asignado para trabajar en ello.

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
            <p>Este campo se ha añadido y muestra la cantidad de minutos de trabajo por día que debe realizar. Tiene el formato <code>YYYY-MM-DD: (number of minutes)</code> y tiene en cuenta la zona horaria.</p>
          </li>
          <li>
            <p><b>isContoured</b>
            </p>
            <p>Se ha añadido este campo, que es un booleano que refleja si la asignación está contorneada. Si se han editado los minutos diarios de la asignación en el Distribuidor de cargas de trabajo, se ha contorneado la asignación.</p>
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

### CustomerPreferences (CUSTPR)

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
            <p><b>nombre</b>
            </p>
            <p>Se añadieron los siguientes valores posibles:</p>
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
            <p>Esta acción devuelve un booleano que describe si el cliente ha desactivado la opción de actualización automática de los titulares de licencias de colaborador.</p>
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
            <p>Se añadió, y calcula la dirección URL de un iFrame incrustado en un informe.</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>Se añadió, y calcula las direcciones URL de los iFrames incrustados en un informe.</p>
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
            <p>Añadido. Este parámetro se usa para identificar las horas creadas con <code>batchSave</code>. </p>
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

Un objeto de nota es un comentario o una actualización realizada sobre un objeto de Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <ul>
          <li>
            <p><b>attachedDocuments</b>
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
            <p>Este campo se ha añadido y muestra la cantidad de minutos de trabajo por día que debe realizar. Tiene en cuenta el formato <code>YYYY-MM-DD: (number of minutes)</code> y la zona horaria.</p>
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
            <p>Esta acción añadió el campo <code>teamIDs</code> para admitir la funcionalidad de asignar varios equipos a una tarea o problema.</p>
         </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Proyecto (PROJ)

Los proyectos son elementos de trabajo dentro de Workfront y son un componente principal en la forma en que Workfront ayuda a las personas a realizar su trabajo. Un objeto Projecto representa un grupo de tareas con un objetivo común y específico.

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

### Tasa (RATE)

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
          <p>Estos parámetros representan el ID y el código de objeto del objeto al que está asociada la Tasa.
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
           <p>Esta acción se ha añadido y adjunta objetos Rate al objeto dado. Este punto final funciona para todos los objetos que pueden adjuntarse a la tasa.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote (RHNOTE)

Un objeto RichTextNote es un comentario o una actualización realizados en un objeto de Workfront, que incluye texto enriquecido como negrita o cursiva.

El objeto RichTextNote quitó el indicador `REPORTABLE`.

### Rol / Función (ROLE)

Un objeto Role (función) representa una capacidad funcional o un conjunto de aptitudes que un usuario podría completar, como un diseñador o un gestor de productos.

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
            <p>Se ha añadido y representa los objetos Rate adjuntos a esta función.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Tarea (TAREA)

Un objeto Tarea representa un elemento de trabajo que debe realizarse como un paso hacia la meta de un objetivo final (completar un proyecto).

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
            <p>Este campo se ha añadido y muestra la cantidad de minutos de trabajo por día que debe realizar. Tiene en cuenta el formato <code>YYYY-MM-DD: (number of minutes)</code> y la zona horaria.</p>
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
            <p>Esta acción añadió el campo <code>teamIDs</code> para admitir la funcionalidad de asignar varios equipos a una tarea o problema.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### Plantilla de horas (TSHET)

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
            <p>Este parámetro quitó el indicador <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>Este parámetro quitó el indicador <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>Se añadió este parámetro, y guarda la duración de la plantilla de horas en días, independientemente de los cambios a “Horas equivalentes para un día de trabajo completo”.  Por ejemplo, si las horas equivalentes se establecen en 6 y se registra un día, entonces las horas equivalentes se cambian a 8 horas, y <code>totalDays</code> sigue teniendo el valor de 1.</p>
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
            <p>Se ha añadido esta acción, que toma un mapa de consulta de filtro y añade la unión <code>allowingnull</code> para los campos que aceptan valores NULL.</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Estas acciones admiten la capacidad de compartir filtros, vistas y agrupaciones en todo el sistema.</p><p>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs#make-filters-views-or-groupings-available-to-users%22%3E">Hacer que los filtros, las vistas o las agrupaciones estén disponibles para todos los usuarios</a>.</p>
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
            <p>Estas acciones admiten la capacidad de compartir filtros, vistas y agrupaciones en todo el sistema.</p><p>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs#make-filters-views-or-groupings-available-to-users%22%3E">Hacer que los filtros, las vistas o las agrupaciones estén disponibles para todos los usuarios</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView / Vista (UIVW)

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
            <p>Estas acciones admiten la capacidad de compartir filtros, vistas y agrupaciones en todo el sistema.</p><p>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs#make-filters-views-or-groupings-available-to-users%22%3E">Hacer que los filtros, las vistas o las agrupaciones estén disponibles para todos los usuarios</a>.</p>
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
            <p>Se ha añadido, y representa los objetos Rate adjuntos a este usuario.</p>
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

### Work (WORK)

Un objeto de trabajo es una interfaz común que heredan Tarea y OpTask, y que comparte código común entre ambos.

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
            <p>Este campo se ha añadido y muestra la cantidad de minutos de trabajo por día que debe realizar. Tiene en cuenta el formato <code>YYYY-MM-DD: (number of minutes)</code> y la zona horaria.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
