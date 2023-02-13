---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 15 de la API
description: Adobe Workfront lanzó la versión 14 de la API el 14 de junio de 2022. La versión 15 de la API presenta los siguientes cambios con respecto a la versión 14.
author: John
feature: Workfront API
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '2349'
ht-degree: 3%

---

# Novedades de la versión 15 de la API

Adobe Workfront lanzó la versión 15 de la API el 14 de junio de 2022. La versión 15 de la API presenta los siguientes cambios con respecto a la versión 14.

## Recursos añadidos

* [Iniciativa (INITIV)](#Initiati)

* [IssueDef (ISSDEF)](#IssueDef)

* [ObjectIntegration (OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [TaskDef (TSKDEF)](#TaskDef)

* [UserApproval (USRAPV)](#UserAppr)

### Iniciativa (INITIV)

El objeto Initiative crea estimaciones en Workfront Scenario Planner para el tipo y el número de funciones, los costes fijos y las prestaciones planificadas.

Para obtener más información sobre las iniciativas, consulte [Información general sobre las iniciativas en el planificador de escenarios](../../scenario-planner/initiatives-overview.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>Se trata de un objeto interno.</p>
          </li>
          <li>
            <p><b>duración</b>
            </p>
            <p>Cantidad de tiempo entre endDate y startDate.</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>Fecha de finalización prevista de la Iniciativa.</p>
          </li>
          <li>
            <p><b>enteredByID</b>
            </p>
            <p>El ID asociado al usuario que envió la solicitud.</p>
          </li>
          <li>
            <p><b>Identificador</b>
            </p>
            <p>ID asociado a la acción</p>
          </li>
          <li>
            <p><b>InitiativeID</b>
            </p>
            <p>ID asociado a la Iniciativa.</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>La fecha en que se publicó la iniciativa por última vez en Workfront Scenario Planner.</p>
          </li>
          <li>
            <p><b>name</b>
            </p>
            <p>Nombre de la Iniciativa</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>La identificación del Plan asociado a la Iniciativa.</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>Nombre del Plan asociado a la Iniciativa.</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>ID del proyecto asociado a la iniciativa.</p>
          </li>
          <li>
            <p><b>scenarioID</b>
            </p>
            <p>ID del escenario en el planificador de escenario de Workfront asociado con la iniciativa.</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>Fecha de inicio prevista de la Iniciativa.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td >
        <ul>
          <li>
            <p><b>cliente</b>
            </p>
          </li>
          <li>
            <p><b>enteredBy</b>
            </p>
          </li>
          <li>
            <p><b>proyecto</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li>
            <p><b>Identificador</b>
            </p>
          </li>
          <li>
            <p><b>name</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operaciones</td>
      <td>
        <ul>
          <li>
            <p><b>RECUENTO</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>INFORME </b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### IssueDef (ISSDEF)

El objeto IssueDef representa un conjunto de datos relativos al formato de los problemas. Este objeto se puede adjuntar a Proyectos o Plantillas y afecta a los problemas agregados a ese proyecto o plantilla.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>Identificador</b>
            </p>
          </li>
          <li>
            <p><b>isInlineAddEnabled</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li>
            <p><b>Identificador</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ObjectIntegration (OBJINT)

En algunos casos, es posible vincular elementos de trabajo de Workfront directamente a objetos de un producto de software externo. El objeto ObjectIntegration representa este vínculo.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>Se trata de un objeto interno.</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>Fecha y hora en que se introdujo ObjectIntegration en el sistema Workfront.</p>
          </li>
          <li>
            <p><b>Identificador</b>
            </p>
            <p>ID de Workfront único del objeto ObjectIntegration específico.</p>
          </li>
          <li>
            <p><b>integrationType</b>
            </p>
            <p>Software externo con el que el objeto ObjectIntegration crea un vínculo. Los valores posibles son:</p>
            <ul>
              <li>
                <p>JIRA</p>
              </li>
              <li>
                <p>SALESFORCE</p>
              </li>
              <li>
                <p>ANAPLAN</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>linkedObjectID</b>
            </p>
          </li>
          <li>
            <p><b>objID</b>
            </p>
            <p>El objeto de Workfront al que está asociado ObjectIntegration.</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>Código de objeto del objeto en Workfront al que está asociado ObjectIntegration.</p>
          </li>
          <li>
            <p><b>param1</b>
            </p>
          </li>
          <li>
            <p><b>param2</b>
            </p>
          </li>
          <li>
            <p style="font-weight: bold;">param3</p>
          </li>
          <li>
            <p><b>Dirección URL</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td >
        <ul>
          <li>
            <p><b>cliente</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li>
            <p><b>Identificador</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TaskDef (TSKDEF)

El objeto TaskDef representa un conjunto de datos sobre el formato de las tareas. Este objeto se puede adjuntar a Proyectos o Plantillas y afecta a las tareas agregadas a ese proyecto o plantilla.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcPlannedHours </b>
            </p>
          </li>
          <li>
            <p><b>Identificador</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td >
        <ul>
          <li>
            <p><b>defaultApprovalProcess </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de recopilación</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories
</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li>
            <p><b>Identificador</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserApproval (USRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos </td>
      <td>
        <ul>
          <li>
            <p><b>aprobadorID</b>
            </p>
          </li>
          <li>
            <p><b>customerID</b>
            </p>
          </li>
          <li>
            <p><b>Identificador</b>
            </p>
          </li>
          <li>
            <p><b>requestedDate</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td >
        <ul>
          <li>
            <p><b>aprobador</b>
            </p>
          </li>
          <li>
            <p><b>cliente</b>
            </p>
          </li>
          <li>
            <p><b>requestor</b>
            </p>
          </li>
          <li>
            <p><b>usuario</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li>
            <p><b>Identificador</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos predeterminados</td>
      <td >
        <ul>
          <li>
            <p><b>aprobadorID</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <ul>
          <li>
            <p><b>approve</b>
            </p>
          </li>
          <li>
            <p><b>rechazar</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operaciones</td>
      <td>
        <ul>
          <li>
            <p><b>AGREGAR</b>
            </p>
          </li>
          <li>
            <p><b>RECUENTO</b>
            </p>
          </li>
          <li>
            <p><b>DELETE</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>INFORME</b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Recursos eliminados

No se eliminaron recursos para la versión 15 de la API.

## Recursos modificados

* [AccessLevel (ACSLVL)](#AccessLe)

* [AccessLevelPermissions (ALVPER)](#AccessLe2)

* [AccessRequest (ACSREQ)](#AccessRe)

* [AccessRule (ACSRUL)](#AccessRu)

* [Aprobación (APROBACIÓN)](#Approval)

* [Categoría (CTGY)](#Category)

* [CategoryParameter (CTGYPA)](#Category2)

* [Preferencias de cliente (CUSTPR)](#Customer)

* [DocumentFolder (DOCFDR)](#Document)

* [DocumentVersion (DOCV)](#Document2)

* [Grupo (GRUPO)](#Group)

* [Entrada de diario (JRNLE)](#JournalE)

* [LinkedFolder (LNKFDR)](#LinkedFo)

* [OpTask / Problema (OPTASK)](#OpTask)

* [Parámetro (PARAM)](#Paramete)

* [Portfolio (PUERTO)](#Portfoli)

* [Programa (PRGM)](#Program)

* [Proyecto (PROJ)](#Project)

* [QueueDef (QUED)](#QueueDef)

* [ScoreCardQuestion (SCOREQ)](#ScoreCar)

* [Tarea (TAREA)](#Task)

* [Plantilla (TMPL)](#Template)

* [Hoja de horas (HOJA)](#Timeshee)

* [Ver (UIVIEW)](#View)

* [Actualizar (ACTUALIZAR)](#Update)

* [Usuario (USUARIO)](#User)

* [UserNote (USRNOT)](#UserNote)

* [Trabajo (TRABAJO)](#Work)

### AccessLevel (ACSLVL)

Un objeto AccessLevel está asociado a los usuarios y describe el conjunto de AccessLevelPermissions que determinan a qué puede acceder el usuario.

Para obtener más información sobre los niveles de acceso, consulte [Niveles de acceso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b> (cadena[])</p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>VTMAWMG (Ver equipos asociados con mis grupos)</p>
              </li>
              <li>
                <p>VALLTM (Ver todos los equipos)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessLevelPermissions (ALVPER)

Un objeto AccessLevelPermissions representa un permiso específico para acceder, crear o modificar un objeto de Workfront. Estos permisos se pueden asociar a un nivel de acceso.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (cadena[])</p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipos en grupos que administro (solo administradores de grupo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>prohibidaActions</b> (cadena[])</p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipos en grupos que administro (solo administradores de grupo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secundarioActions</b> (cadena[])</p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipos en grupos que administro (solo administradores de grupo))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

Si un usuario no tiene acceso a un objeto de Workfront que necesite, puede solicitar acceso a ese objeto. El objeto AccessRequest representa esta solicitud.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>acción</b> (cadena)</p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipos en grupos que administro (solo administradores de grupo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b> (cadena)</p>
            <p>Se ha añadido el siguiente valor posible:</p>
            <ul>
              <li>
                <p>WDL</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule (ACSRUL)

Un objeto AccessRule representa un conjunto de reglas en niveles de acceso personalizados que determina cómo pueden compartir los usuarios los proyectos que crean.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (cadena[])</p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipos en grupos que administro (solo administradores de grupo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>prohibidaActions</b> (cadena[])</p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipos en grupos que administro (solo administradores de grupo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secundarioActions</b> (cadena[])</p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipos en grupos que administro (solo administradores de grupo))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Aprobación (APROBACIÓN)

Un elemento de trabajo determinado, como una tarea, un documento o un parte de horas, puede requerir que un supervisor u otro usuario cierre la sesión en el elemento de trabajo. Un objeto Approval representa la acción de cerrar sesión en un elemento de trabajo.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td >
        <ul>
          <li>
            <p><b>iniciativa</b>
            </p>
            <p>Agregado.</p>
            <p>El objeto Initiative crea estimaciones en Workfront Scenario Planner para el tipo y el número de funciones, los costes fijos y las prestaciones planificadas. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>Agregado.</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>Agregado.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de recopilación</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegrations
</b>
            </p>
            <p style="font-weight: normal;">Agregado.</p>
            <p>En algunos casos, es posible vincular elementos de trabajo de Workfront directamente a objetos de un producto de software externo. El objeto ObjectIntegration representa este vínculo.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Categoría (CTGY)

Un objeto Category es un formulario personalizado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b> (cadena)</p>
            <p>Se ha añadido el siguiente valor posible:</p>
            <ul>
              <li>
                <p>GRUPO (Grupo)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (cadena[])</p>
            <p>Agregado.</p>
            <p style="font-weight: normal;">Este parámetro es una matriz de posibles objetos a los que se puede adjuntar el formulario personalizado. Se agregó para admitir la capacidad de adjuntar un formulario personalizado a varios tipos de objetos.</p>
            <p>Valores posibles: </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USUARIO, DOCU, EXPNS, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de recopilación</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (cadena[])</p>
            <p>Agregado.</p>
            <p style="font-weight: normal;">Este parámetro es una matriz de posibles objetos a los que se puede adjuntar el formulario personalizado. Se agregó para admitir la capacidad de adjuntar un formulario personalizado a varios tipos de objetos.</p>
            <p>Valores posibles: </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USUARIO, DOCU, EXPNS, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategoryParameter (CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>hideFormulaFromDescription</b>
            </p>
            <p>Agregado.</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>Agregado.</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>Agregado.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Preferencias de cliente (CUSTPR)

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
            <p>Se agregaron los siguientes valores:</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (Integración de SharePoint (API de gráficos) activada)</p>
                <p>Este valor admite la integración actualizada de Sharepoint.</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (Permitir a los usuarios crear proyectos sin usar una plantilla)</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> (config.taskissue.delegate)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder (DOCFDR)

Los documentos se pueden organizar en carpetas. Puede crear carpetas personales en su área de documentos personales. El objeto DocumentFolder representa una de estas carpetas.

El objeto DocumentFolder agregó el indicador `SHARABLE`.

### DocumentVersion (DOCV)

Un objeto DocumentVersion representa una versión específica de un archivo (como material escrito, imágenes u otras formas de información).

Para obtener más información sobre las versiones de documentos, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Se ha añadido el siguiente valor: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (API de gráficos))</p>
                <p>Este valor admite la integración actualizada de Sharepoint.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Grupo (GRUPO)

Un objeto Group representa un conjunto de usuarios y equipos. Los grupos suelen representar la estructura departamental.

Para obtener más información sobre los grupos, consulte Grupos vs. equipos.

El objeto Group agregó el indicador `DATA_EXTENDIBLE`

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <p>Se agregaron los campos siguientes:</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Una categoría es un formulario personalizado. Este parámetro se agregó para admitir la capacidad de agregar Forms personalizado a los objetos de grupo. </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Se trata de un parámetro booleano que tiene el valor "True" si un objeto es Activo y "False" si no lo es. Los objetos que se establecen como Activo aparecen en los menús desplegables y en los campos de avance de tipo y se pueden adjuntar a otros objetos.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td >
        <p>Se agregaron los campos siguientes:</p>
        <ul>
          <li>
            <p><b>aprobador</b>
            </p>
          </li>
          <li>
            <p><b>cliente</b>
            </p>
          </li>
          <li>
            <p><b>requestor</b>
            </p>
          </li>
          <li>
            <p><b>usuario</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de recopilación</td>
      <td>
        <p>Se agregaron los campos siguientes:</p>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>En algunos casos, es posible vincular elementos de trabajo de Workfront directamente a objetos de un producto de software externo. El objeto ObjectIntegration representa este vínculo.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos predeterminados</td>
      <td >
        <p>Se ha añadido el siguiente campo:</p>
        <ul>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Se trata de un parámetro booleano que tiene el valor "True" si un objeto es Activo y "False" si no lo es. Los objetos que se establecen como Activo aparecen en los menús desplegables y en los campos de avance de tipo y se pueden adjuntar a otros objetos.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <p>Se agregaron los campos siguientes:</p>
        <ul>
          <li>
            <p><b>calculateDataExtension</b>
            </p>
            <p>Esta acción vuelve a calcular las expresiones de los campos de formulario personalizados.</p>
          </li>
          <li>
            <p><b>completeGroupInfo</b>
            </p>
          </li>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Entrada de diario (JRNLE)

El objeto JournalEntry se puede configurar para registrar información sobre campos de objeto específicos cada vez que se modifiquen dichos campos. Cuando un campo está configurado para registrarse como parte del objeto Entrada de diario, se crea una Entrada de diario correspondiente cada vez que se modifica ese campo.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <p><b>changeType</b>
        </p>
        <p>Se ha añadido el siguiente valor: </p>
        <ul>
          <li>
            <p>DW (descarga)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder (LNKFDR)

Un objeto LinkedFolder representa una carpeta vinculada desde un proveedor de documentos externo, como Google Drive o Dropbox.

Para obtener más información sobre carpetas vinculadas, consulte Vincular documentos de aplicaciones externas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Se ha añadido el siguiente valor: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (API de gráficos))</p>
                <p>Este valor admite la integración actualizada de Sharepoint.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask / Problema (OPTASK)

Un objeto OpTask se conoce comúnmente como Problema. Un problema es un elemento de trabajo que normalmente indica que hay un problema que impide la finalización de una tarea o proyecto. Un problema también puede ser una solicitud de asistencia técnica. Los cambios de pedidos, solicitudes y errores también son problemas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <p>Se agregaron las siguientes acciones:</p>
        <ul>
          <li>
            <p><b>bulkMoveWithOptions</b>
            </p>
          </li>
          <li>
            <p><b>getRequestPath</b>
            </p>
          </li>
        </ul>
        <p>Se modificó la siguiente acción:</p>
        <ul>
          <li>
            <p><b>copyIssue</b>
            </p>
            <p>Campo añadido <code>parentID</code></p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Parámetro (PARAM)

Un objeto Parameter es un campo personalizado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <p>Se ha añadido el siguiente campo:</p>
        <ul>
          <li>
            <p><b>fieldDefinition</b>
            </p>
          </li>
        </ul>
        <p>Se modificaron los campos siguientes:</p>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>Se ha añadido el valor posible <code>WIDGET </code>(Utilidad) </p>
            <p>Este valor admite el uso de imágenes en formularios personalizados.</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Se ha añadido el valor posible <code>WIDGET </code>(Utilidad)</p>
            <p>Este valor admite el uso de imágenes en formularios personalizados.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio (PUERTO)

Un objeto Portfolio es una colección de proyectos que compiten por los mismos recursos, normalmente dinero o personas para completarlos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de recopilación</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Programa (PRGM)

Un objeto Program es un subconjunto de proyectos dentro de un portafolio, donde proyectos similares se pueden agrupar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de recopilación</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Proyecto (PROJ)

Los proyectos son elementos de trabajo dentro de Workfront y son un componente principal de la forma en que Workfront ayuda a las personas a hacer su trabajo. Un objeto Project representa un grupo de tareas con un objetivo específico común.

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
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td >
        <ul>
          <li>
            <p><b>iniciativa</b>
            </p>
            <p>El objeto Initiative crea estimaciones en Workfront Scenario Planner para el tipo y el número de funciones, los costes fijos y las prestaciones planificadas. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de recopilación</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>En algunos casos, es posible vincular elementos de trabajo de Workfront directamente a objetos de un producto de software externo. El objeto ObjectIntegration representa este vínculo.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Un objeto QueueDef representa una cola, que es un proyecto que se ha publicado en el área de asistencia técnica para permitir a los usuarios enviar problemas.

Para obtener más información sobre las colas de solicitud, consulte [Crear una cola de solicitud](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>requestorCoreAction</b>
            </p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipos en grupos que administro (solo administradores de grupo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbioredActions</b>
            </p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipos en grupos que administro (solo administradores de grupo))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Un objeto ScoreCardQuestion representa una pregunta que se ha agregado a un informe de valoración. Estas preguntas suelen ser determinadas por el administrador de Portfolio y sus respuestas permiten al administrador comprender cómo se alinea un proyecto con los objetivos del portafolio.

Para obtener más información sobre las preguntas del informe de valoración, consulte [Crear un informe de valoración](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Se ha añadido el valor posible <code>WIDGET </code>(Utilidad)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tarea (TAREA)

Un objeto Task representa un elemento de trabajo que debe realizarse como paso hacia el logro de un objetivo final (completar un proyecto).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de recopilación</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>En algunos casos, es posible vincular elementos de trabajo de Workfront directamente a objetos de un producto de software externo. El objeto ObjectIntegration representa este vínculo.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Plantilla (TMPL)

Un objeto Template representa un patrón para un proyecto. Los proyectos se pueden crear a partir de plantillas para ahorrar tiempo. Una plantilla contiene un equipo y tareas que se copiarán en cualquier proyecto creado a partir de la plantilla.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td>
        <ul>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Hoja de horas (HOJA)

Un objeto de parte de horas representa un panel de tiempo virtual que permite a los usuarios introducir horas reales trabajadas para tareas, proyectos y tipos de horas generales.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <p>Se ha eliminado el siguiente campo:</p>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Ver (UIVIEW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>uiviewType</b>
            </p>
            <p>Se eliminaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>FOUR_COL</code> (Diseño de cuatro columnas)</p>
              </li>
              <li>
                <p><code>UPDATES</code> (Actualizaciones)</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> (Actualizaciones)</p>
              </li>
              <li>
                <p><code>WORKINGON</code> (Trabajando en)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> (Datos personalizados)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> (Actualizar datos personalizados)</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> (Actualización de estado)</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> (Actualización de estado)</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> (Actualización de estado)</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> (Actualización de estado)</p>
              </li>
              <li>
                <p><code>DLIST</code> (Lista de detalles)</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> (Sección de lista de detalles)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Actualizar (ACTUALIZAR)

Los elementos de trabajo de Workfront se pueden actualizar para mantener a los usuarios informados del estado actual. Un objeto Update representa una de estas actualizaciones. Los usuarios pueden introducir actualizaciones o crearlas en el sistema Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>updateType</b>
            </p>
            <p>Se ha añadido el valor posible <code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Usuario (USUARIO)

Un objeto User representa a una persona con una cuenta en Workfront que puede iniciar sesión e interactuar con el sistema.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td>
        <ul>
          <li>
            <p><b>userApproval</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <ul>
          <li>
            <p><b>getUsersAvailableTime</b>
            </p>
          </li>
          <li>
            <p><b>resetRopgPassword</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserNote (USRNOT)

Un objeto UserNote es una notificación.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>eventType</b>
            </p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>DUP </code>(Solicitado que pruebe un documento)</p>
              </li>
              <li>
                <p><code>DUV </code>(Permiten ver un documento)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Trabajo (TRABAJO)

Un objeto Work es una interfaz común que heredan Task y OpTask, y comparte código común entre ambos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de recopilación</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>En algunos casos, es posible vincular elementos de trabajo de Workfront directamente a objetos de un producto de software externo. El objeto ObjectIntegration representa este vínculo.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
