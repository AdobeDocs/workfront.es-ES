---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 15 de la API
description: Adobe Workfront lanzó la versión 14 de la API el 14 de junio de 2022. La versión 15 de la API incorpora los siguientes cambios con respecto a la versión 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
TQID: https://experienceleague.adobe.com/8aay3Ew3jFaxu2L-uvvlW-aqGo7ZT5Jj5TvrTCg96gM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: d3382524-5489-431b-bde9-271ab257bc37id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 2294
ht-degree: 100%

---

# Novedades de la versión 15 de la API

Adobe Workfront lanzó la versión 15 de la API el 14 de junio de 2022. La versión 15 de la API incorpora los siguientes cambios con respecto a la versión 14.

## Recursos añadidos

* [Iniciativa (INITIV)](#Initiati)

* [IssueDef (ISSDEF)](#IssueDef)

* [ObjectIntegration (OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [TaskDef (TSKDEF)](#TaskDef)

* [UserApproval (USRAPV)](#UserAppr)

### Iniciativa (INITIV)

El objeto Iniciativa crea estimaciones en el Planificador de escenarios de Workfront para el tipo y el número de funciones, los costes fijos y el beneficio estimado.

Para obtener más información sobre iniciativas, consulte [Información general sobre iniciativas en el Planificador de escenarios](../../scenario-planner/initiatives-overview.md).

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
            <p>Este es un objeto interno.</p>
          </li>
          <li>
            <p><b>duración</b>
            </p>
            <p>Cantidad de tiempo entre endDate y startDate.</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>Fecha planificada de finalización de la iniciativa.</p>
          </li>
          <li>
            <p><b>enteredByID</b>
            </p>
            <p>El ID asociado con el usuario que envió la solicitud.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>Cualquier identificador asociado con la acción</p>
          </li>
          <li>
            <p><b>initiativeID</b>
            </p>
            <p>El ID asociado a la iniciativa.</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>La fecha en la que se publicó por última vez la Iniciativa en el Planificador de escenarios de Workfront.</p>
          </li>
          <li>
            <p><b>nombre</b>
            </p>
            <p>El nombre de la Iniciativa</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>El identificador del plan asociado a la iniciativa.</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>El nombre del plan asociado a la iniciativa.</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>El ID del proyecto asociado a la iniciativa.</p>
          </li>
          <li>
            <p><b>scenarioID</b>
            </p>
            <p>El ID del escenario en el Planificador de escenarios de Workfront asociado a la iniciativa.</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>La fecha de inicio planificada de la iniciativa.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td >
        <ul>
          <li>
            <p><b>Cliente</b>
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
            <p><b>ID</b>
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
            <p><b>COUNT</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>REPORT </b>
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

El objeto IssueDef representa un conjunto de datos relativos al formato de los problemas. Este objeto se puede adjuntar a Proyectos o Plantillas y afecta a los problemas añadidos a ese Proyecto o Plantilla.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
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
            <p><b>ID</b>
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
            <p>Este es un objeto interno.</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>La fecha y hora en que se ingresó ObjectIntegration en el sistema de Workfront.</p>
          </li>
          <li>
            <p><b>ID</b>
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
            <p>El objeto en Workfront con el que está asociado ObjectIntegration.</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>El código de objeto del objeto en Workfront con el que está asociado ObjectIntegration.</p>
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
            <p><b>URL</b>
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
            <p><b>customer</b>
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
            <p><b>ID</b>
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

El objeto TaskDef representa un conjunto de datos relativos al formato de las tareas. Este objeto se puede adjuntar a Proyectos o Plantillas y afecta a las tareas añadidas a ese Proyecto o Plantilla.

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
            <p><b>ID</b>
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
      <td role="rowheader">Campos de colección</td>
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
            <p><b>ID</b>
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
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>customerID</b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
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
            <p><b>approver</b>
            </p>
          </li>
          <li>
            <p><b>Cliente</b>
            </p>
          </li>
          <li>
            <p><b>requestor</b>
            </p>
          </li>
          <li>
            <p><b>user</b>
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
            <p><b>ID</b>
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
            <p><b>approverID</b>
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
            <p><b>reject</b>
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
            <p><b>ADD</b>
            </p>
          </li>
          <li>
            <p><b>COUNT</b>
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
            <p><b>REPORT</b>
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

No se ha eliminado ningún recurso para la versión 15 de la API.

## Recursos modificados

* [AccessLevel (ACSLVL)](#AccessLe)

* [AccessLevelPermissions (ALVPER)](#AccessLe2)

* [AccessRequest (ACSREQ)](#AccessRe)

* [AccessRule (ACSRUL)](#AccessRu)

* [Aprobación (APPROVAL)](#Approval)

* [Categoría (CTGY)](#Category)

* [CategoryParameter (CTGYPA)](#Category2)

* [CustomerPreferences (CUSTPR)](#Customer)

* [DocumentFolder (DOCFDR)](#Document)

* [DocumentVersion (DOCV)](#Document2)

* [Grupo (GROUP)](#Group)

* [JournalEntry (JRNLE)](#JournalE)

* [LinkedFolder (LNKFDR)](#LinkedFo)

* [OpTask / Problema (OPTASK)](#OpTask)

* [Parámetro (PARAM)](#Paramete)

* [Portafolio (PORT)](#Portfoli)

* [Programa (PRGM)](#Program)

* [Proyecto (PROJ)](#Project)

* [QueueDef (QUED)](#QueueDef)

* [ScoreCardQuestion (SCOREQ)](#ScoreCar)

* [Tarea (TAREA)](#Task)

* [Template (TMPL)](#Template)

* [Plantilla de horas (TSHET)](#Timeshee)

* [View (UIVIEW)](#View)

* [Actualizar (UPDATE)](#Update)

* [Usuario (USER)](#User)

* [UserNote (USRNOT)](#UserNote)

* [Work (WORK)](#Work)

### AccessLevel (ACSLVL)

Un objeto AccessLevel está asociado a los usuarios y describe el conjunto de AccessLevelPermissions que determinan a qué puede tener acceso el usuario.

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
            <p><b>fieldAccessPrivileges</b> (string[])</p>
            <p>Se añadieron los siguientes valores posibles:</p>
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

Un objeto AccessLevelPermissions representa un permiso específico para tener acceso, crear o modificar un objeto de Workfront. Estos permisos se pueden asociar a un nivel de acceso.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar los equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN [Editar los equipos de los grupos que administro (solo para Administradores de grupos)]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar los equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN [Editar los equipos de los grupos que administro (solo para Administradores de grupos)]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar los equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN [Editar los equipos de los grupos que administro (solo para Administradores de grupos)]</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

Si un usuario no tiene acceso a un objeto en Workfront que necesita, puede solicitar acceso a ese objeto. El objeto AccessRequest representa esta solicitud.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>action</b> (string)</p>
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar los equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN [Editar los equipos de los grupos que administro (solo para Administradores de grupos)]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b> (string)</p>
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

Un objeto AccessRule representa un conjunto de reglas en los niveles de acceso personalizados que determina cómo los usuarios pueden compartir los proyectos que crean.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar los equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN [Editar los equipos de los grupos que administro (solo para Administradores de grupos)]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar los equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN [Editar los equipos de los grupos que administro (solo para Administradores de grupos)]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar los equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN [Editar los equipos de los grupos que administro (solo para Administradores de grupos)]</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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
            <p>Añadido.</p>
            <p>El objeto Iniciativa crea estimaciones en el Planificador de escenarios de Workfront para el tipo y el número de funciones, los costes fijos y el beneficio estimado. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>Añadido.</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>Añadido.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegrations
</b>
            </p>
            <p style="font-weight: normal;">Añadido.</p>
            <p>En algunos casos, es posible vincular elementos de trabajo de Workfront directamente a objetos de un producto de software externo. El objeto ObjectIntegration representa este vínculo.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Categoría (CTGY)

Un objeto de categoría es un formulario personalizado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b> (string)</p>
            <p>Se ha añadido el siguiente valor posible:</p>
            <ul>
              <li>
                <p>GROUP (grupo)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>Añadido.</p>
            <p style="font-weight: normal;">Este parámetro es una matriz de objetos posibles a los que se puede adjuntar el formulario personalizado. Se ha añadido para incorporar la capacidad de adjuntar un formulario personalizado a varios tipos de objetos.</p>
            <p>Valores posibles: </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>Añadido.</p>
            <p style="font-weight: normal;">Este parámetro es una matriz de objetos posibles a los que se puede adjuntar el formulario personalizado. Se ha añadido para incorporar la capacidad de adjuntar un formulario personalizado a varios tipos de objetos.</p>
            <p>Valores posibles: </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
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
            <p>Añadido.</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>Añadido.</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>Añadido.</p>
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
            <p>Se han añadido los siguientes valores:</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (Integración de SharePoint [API de gráficos] habilitada)</p>
                <p>Este valor admite la integración actualizada con Sharepoint.</p>
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

Los documentos se pueden organizar en carpetas. Puede crear carpetas personales en el área de documentos personales. El objeto DocumentFolder representa una de estas carpetas.

El objeto DocumentFolder añadió el indicador `SHARABLE`.

### DocumentVersion (DOCV)

Un objeto DocumentVersion representa una versión específica de un archivo (como material escrito, imágenes u otras formas de información).

Para obtener más información acerca de las versiones de documentos, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md).

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
                <p><code>SHAREPOINT_V2</code> (SharePoint [API de gráficos])</p>
                <p>Este valor admite la integración actualizada con SharePoint.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Grupo (GROUP)

Un objeto Group representa un conjunto de usuarios y equipos. Los grupos a menudo representan la estructura departamental.

Para obtener más información sobre los grupos, consulte Grupos frente a equipos.

El objeto Group añadió el indicador `DATA_EXTENDIBLE`

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <p>Se han añadido los campos siguientes:</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Una categoría es un formulario personalizado. Este parámetro se ha añadido para habilitar la posibilidad de añadir formularios personalizados a objetos de grupo. </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Este es un parámetro booleano con un valor de verdadero si un objeto está activo y falso si no lo está. Los objetos que se definen como Activos aparecen en menús desplegables y campos de escritura anticipada y pueden adjuntarse a otros objetos.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td >
        <p>Se han añadido los campos siguientes:</p>
        <ul>
          <li>
            <p><b>approver</b>
            </p>
          </li>
          <li>
            <p><b>Cliente</b>
            </p>
          </li>
          <li>
            <p><b>requestor</b>
            </p>
          </li>
          <li>
            <p><b>user</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <p>Se han añadido los campos siguientes:</p>
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
            <p>Este es un parámetro booleano con un valor de verdadero si un objeto está activo y falso si no lo está. Los objetos que se definen como Activos aparecen en menús desplegables y campos de escritura anticipada y pueden adjuntarse a otros objetos.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <p>Se han añadido los campos siguientes:</p>
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

### JournalEntry (JRNLE)

El objeto JournalEntry se puede configurar para que registre información sobre campos de objeto específicos cada vez que se modifiquen dichos campos. Cuando un campo está configurado para registrarse como parte del objeto Entrada de cuaderno, se creará una entrada de cuaderno correspondiente cada vez que se modifique ese campo.

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

Para obtener más información sobre las carpetas vinculadas, consulte Vincular documentos desde aplicaciones externas.

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
                <p><code>SHAREPOINT_V2</code> (SharePoint [API de gráficos])</p>
                <p>Este valor admite la integración actualizada con SharePoint.</p>
              </li>
            </ul>
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
      <td role="rowheader">Acciones</td>
      <td>
        <p>Se añadieron las siguientes acciones:</p>
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
        <p>Se han modificado los campos siguientes:</p>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>Se añadió el valor posible <code>WIDGET </code>(Widget) </p>
            <p>Este valor admite el uso de imágenes en formularios personalizados.</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Se añadió el valor posible <code>WIDGET </code>(Widget)</p>
            <p>Este valor admite el uso de imágenes en formularios personalizados.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portafolio (PORT)

Un objeto Portafolio es una colección de proyectos que compiten por los mismos recursos, generalmente dinero o personas para completarlos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de colección</td>
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

Un objeto Program es un subconjunto de proyectos dentro de un portafolio, donde se pueden agrupar proyectos similares.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de colección</td>
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
            <p>El objeto Iniciativa crea estimaciones en el Planificador de escenarios de Workfront para el tipo y el número de funciones, los costes fijos y el beneficio estimado. </p>
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
      <td role="rowheader">Campos de colección</td>
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

Un objeto QueueDef representa una cola, que es un proyecto que se ha publicado en el área del servicio de asistencia para permitir a los usuarios enviarle problemas.

Para obtener más información sobre las colas de solicitudes, consulte [Creación de colas de solicitudes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

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
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar los equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN [Editar los equipos de los grupos que administro (solo para Administradores de grupos)]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar los equipos en los que estoy)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN [Editar los equipos de los grupos que administro (solo para Administradores de grupos)]</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Un objeto ScoreCardQuestion representa una pregunta que se ha añadido a un informe de valoración. Estas preguntas suelen ser determinadas por el responsable del portafolio, y sus respuestas le permiten comprender cómo se ajusta un proyecto a las metas del portafolio.

Para obtener más información sobre las preguntas del cuadro de resultados, consulte [Crear un informe de valoración](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

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
            <p>Se añadió el valor posible <code>WIDGET </code>(Widget)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tarea (TAREA)

Un objeto Tarea representa un elemento de trabajo que debe realizarse como un paso hacia la meta de un objetivo final (completar un proyecto).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de colección</td>
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

### Template (TMPL)

Un objeto de plantilla representa un patrón para un proyecto. Los proyectos se pueden crear a partir de plantillas para ahorrar tiempo. Una plantilla contiene un equipo y tareas, que se copiarán en cualquier proyecto creado a partir de la plantilla.

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

### Plantilla de horas (TSHET)

Un objeto Timesheet representa un parte de horas virtual que permite a los usuarios especificar horas trabajadas reales para tareas, proyectos y tipos de horas generales.

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

### View (UIVIEW)

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

### Actualizar (UPDATE)

Los elementos de trabajo de Workfront se pueden actualizar para mantener a los usuarios informados del estado actual. Un objeto de actualización representa una de estas actualizaciones. Los usuarios pueden introducir actualizaciones o el sistema de Workfront puede crearlas.

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
            <p>Se añadió el valor posible <code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Usuario (USER)

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
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>DUP </code>(Solicitó que usted revise un documento)</p>
              </li>
              <li>
                <p><code>DUV </code>(Permite que usted vea un documento)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Work (WORK)

Un objeto de trabajo es una interfaz común que heredan Tarea y OpTask, y que comparte código común entre ambos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de colección</td>
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
