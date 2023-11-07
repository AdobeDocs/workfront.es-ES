---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 17 de la API
description: Adobe Workfront publicó la versión 17 de la API el 6 de abril de 2022. La versión 17 de la API incorpora los siguientes cambios con respecto a la versión 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: 08e90754-5505-424c-ae67-015cc987b5df
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 4%

---

# Novedades de la versión 17 de la API

Adobe Workfront lanzó la versión 17 de la API el 12 de octubre de 2023. La versión 17 de la API incorpora los siguientes cambios con respecto a la versión 16.

## Recursos añadidos

<!--

### Booking (BOOKNG)

-->

### Documento externo (EXTDOC)

Un objeto ExternalDocument es un documento u otro recurso digital que se encuentra en un proveedor de almacenamiento de documentos externo a Workfront. Estos recursos se pueden vincular desde y hacia Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>description</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>ext.</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>Identificador</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>ruta</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>talla</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>description</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>ext.</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>Identificador</b></p></li>
          <li><p><b>isGoogleRootItem</b></p></li>
          <li><p><b>isTeamDriveItem</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
          <li><p><b>ruta</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>talla</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
          <li><p><b>valor</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos predeterminados</td>
      <td>
        <ul>
          <li><p><b>Identificador</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <ul>
          <li><p><b>browseListWithLinkAction</b></p></li>
          <li><p><b>getDocumentDownloadUrl</b></p></li>
          <li><p><b>getRootFolderID</b></p></li>
          <li><p><b>getRootFolderIDFromDB</b></p></li>
          <li><p><b>linkExternalDocumentObjects</b></p></li>
          <li><p><b>setLinkedFolderMetadata</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Consultas</td>
      <td>
        <ul>
          <li><p><b>browseList</b></p></li>
          <li><p><b>getFolderMetaData</b></p></li>
          <li><p><b>searchExternalDocuments</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operaciones</td>
      <td>
        <ul>
          <li><p><b>SEARCH</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### NlbrGroups (NLBRGP)

### NonLaborResource (NLBR)

### NonLaborResourceParameterValue (NLBRPV)

### RichTextNonLaborResourceParameterValue (NLRRPV)

-->

### UserLocation (USRLOC)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li><p><b>classifierID</b></p></li>
          <li><p><b>customerID</b></p></li>
          <li><p><b>endDate</b></p></li>
          <li><p><b>Identificador</b></p></li>
          <li><p><b>isCurrent</b></p></li>
          <li><p><b>startDate</b></p></li>
          <li><p><b>userID</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td>
        <ul>
          <li><p><b>cliente</b></p></li>
          <li><p><b>usuario</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li><p><b>Identificador</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

## Recursos eliminados

No se han eliminado recursos para la versión 17 de la API

## Recursos modificados

Se modificaron los siguientes recursos para la versión 17 de la API.

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### Línea base (BLIN)

Las líneas de base son instantáneas del aspecto que tuvo el rendimiento de un proyecto en un momento determinado. Almacenan información clave sobre el proyecto, como fechas clave, progreso, valores de costes e ingresos.

El objeto Baseline quitó el indicador **INLINE_EDITABLE**.

### Registro de facturación (FACTURA)

Un objeto BillingRecord registra los ingresos, horas o gastos que se pueden facturar. Esta información se puede utilizar para crear facturas en un sistema de contabilidad externo.

El objeto BillingRecord quitó el indicador **INLINE_EDITABLE**.

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### Empresa (CMPY)

Un objeto Company representa una organización formada por una colección de personas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Eliminado</p>
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
            <p>Se ha agregado el posible valor "config.defaultToNewHomeDescription" (customer:config.defaultToNewHome)&gt;/p?<p>Esto permite a una organización hacer que la nueva experiencia de Inicio sea la predeterminada para sus usuarios.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

Un objeto DocumentVersion representa una versión específica de un archivo (como material escrito, imágenes u otras formas de información).

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
            <p>Se ha añadido el valor posible "Frame.io" (FRAMEIO)</p>
          </li>
          <li>
            <p><b>fileType</b>
            </p>
            <p>Se ha agregado el posible valor "enum.filetype.site" (site)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Tipo de cambio (EXRATE)

Un objeto ExchangeRate representa un tipo de cambio de divisa configurado en Workfront. Los objetos ExchangeRate no son dinámicos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>Se agregaron los campos siguientes:
        <ul>
          <li><p><b>endDate</b></p></li>
          <li><p><b>startDate</b></p></li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <ul>
          <li><p><b>getCustomerCurrencies</b></p></li>
          <p>Agregado.</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### Gasto (EXPNS)

Los gastos representan los costos no laborales en los que se podría incurrir durante la duración de un proyecto.

El objeto Expense ha eliminado el indicador **INLINE_EDITABLE**.

### Grupo (GROUP)

Un objeto Group representa un conjunto de usuarios y equipos. Los grupos a menudo representan la estructura departamental.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Eliminado</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Hora (HORA)

Un objeto Hour representa una hora registrada por un usuario en una plantilla de horas.

El objeto Hour quitó el indicador **INLINE_EDITABLE**.

### Iteración (ITRN)

Un objeto Iteration representa una sola iteración Agile. Las iteraciones son períodos de tiempo discretos que se utilizan para planificar y completar historias de Agile.

El objeto Iteration quitó el indicador **INLINE_EDITABLE**.


### Entrada de diario (JRNLE)

El objeto JournalEntry se puede configurar para que registre información sobre campos de objeto específicos cada vez que se modifiquen dichos campos. Cuando un campo está configurado para registrarse como parte del objeto Entrada de cuaderno, se creará una Entrada de cuaderno correspondiente cada vez que se modifique ese campo.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>Aprobador agregado (AAA)</li>
              <li>Se ha agregado un revisor (AAR)</li>
              <li>Revisor eliminado (ARR)</li>
              <li>Aprobador eliminado (ARA)</li>
              <li>Decisión aprobada (ADA)</li>
              <li>Decisión aprobada con cambios (ADC)</li>
              <li>La decisión necesita trabajo (ADN)</li>
              <li>Decisión revocada (ADR)</li>
              <li>Aprobador cambiado (AAC)</li>
              <li>Revisor cambiado (ARC)</li>
              <li>Revisión finalizada (RDC)</li>
              <li>Revisión revocada (RDR)</li>
              <li>Publicar (PUB)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Panel Kanban (KNBNBD)

Se utiliza un panel Kanban para realizar el seguimiento de tareas en un entorno Agile.

El objeto Panel Kanban ha eliminado el indicador **INLINE_EDITABLE**.


### LinkedFolder (LNKFDR)

Un objeto LinkedFolder representa una carpeta vinculada desde un proveedor de documentos externo, como Google Drive o Dropbox.

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
            <p>Se ha agregado el valor posible "Frame.io (FRAMEIO)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask / Problema (OPTASK)

Un objeto OpTask suele conocerse como Problema. Un problema es un elemento de trabajo que normalmente indica que hay un problema que impide la finalización de una tarea o proyecto. Un problema también puede ser una solicitud del servicio de asistencia. Las solicitudes de cambio, las solicitudes y los errores también son problemas.

El objeto Problema eliminó el indicador **INLINE_EDITABLE**.

### Proyecto (PROJ)

Los proyectos son elementos de trabajo dentro de Workfront y son un bloque de creación principal en la forma en que Workfront ayuda a las personas a realizar su trabajo. Un objeto Project representa un grupo de tareas con un objetivo común y específico.

El objeto Project quitó el indicador **INLINE_EDITABLE**.

### Usuario de proyecto (PRTU)

Un objeto ProjectUser representa un usuario asociado a un proyecto específico.

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
            <p>Agregado.</p>
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
            <p>Agregado.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

-->

### Tasa (TASA)

Un objeto Rate representa una tarifa de facturación en Workfront.

El objeto Rate ha eliminado el indicador **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>Se han agregado las siguientes acciones para admitir la funcionalidad Tarjeta de tarifa:
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p>El <b>setRatesForRole</b> se ha modificado la acción para añadir los campos siguientes:
        <ul>
        <li>classifierID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Riesgo (RIESGO)

Un objeto Risk representa un posible evento que puede impedir que un proyecto finalice a tiempo o dentro del presupuesto. Se añaden riesgos a los proyectos en la fase de planificación para identificar posibles obstáculos antes de la aprobación de cualquier trabajo.

El objeto Riesgo quitó el indicador **INLINE_EDITABLE**.

### Rol / Rol (ROLE)

Un objeto Role (función del puesto) representa una capacidad funcional o un conjunto de aptitudes que un usuario podría rellenar, como Designer o Product Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Eliminado</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Tarea (TAREA)

Un objeto Task representa un elemento de trabajo que debe realizarse como un paso hacia el logro de un objetivo final (completar un proyecto).

El objeto Task quitó el indicador **INLINE_EDITABLE**.

### Equipo (TEAMOB)

Un objeto Team es una colección de usuarios que se pueden asignar a un elemento de trabajo.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Eliminado</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Miembro del equipo (TEAMMB)

Un objeto TeamMember es un usuario asociado a un equipo específico.

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
            <p>Agregado.</p>
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
            <p>Agregado.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Usuario de plantilla (TMTU)

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
            <p>Agregado.</p>
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
            <p>Agregado.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
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
            <p><b>objCode</b>
            </p>
            <p>Eliminado</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Actualizar (UPDATE)

Los elementos de trabajo de Workfront se pueden actualizar para mantener a los usuarios informados del estado actual. Un objeto Update representa una de estas actualizaciones. Los usuarios pueden introducir actualizaciones o el sistema de Workfront puede crearlas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Se agregaron los siguientes valores:</p>
            <ul>
              <li>Aprobador agregado (assetapprovalAddApprover)</li>
              <li>Se ha agregado un revisor (assetapprovalAddReviewer)</li>
              <li>Aprobador eliminado (assetapprovalRemoveApprover)</li>
              <li>Revisor eliminado (assetapprovalRemoveReviewer)</li>
              <li>Decisión aprobada (assetapprovalDecisionApproved)</li>
              <li>La decisión necesita trabajo (assetapprovalDecisionNeedsWork)</li>
              <li>Decisión aprobada con cambios (assetapprovalDecisionApprovedChanges)</li>
              <li>Decisión revocada (assetapprovalDecisionRevked)</li>
              <li>Aprobador modificado (assetapprovalApproverChanged)</li>
              <li>Revisor modificado (assetapprovalReviewerChanged)</li>
              <li>Revisión completa (assetapprovalReviewerDecisionComplete)</li>
              <li>Revisión revocada (assetapprovalReviewerDecisionRevked)</li>
              <li>Error de envío de documento externo (externalDocumentSendError)</li>
              <li>Versión de documento publicada (documentVersionPublish)</li>
              <li>Flujo de trabajo de carpeta vinculada (linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### Usuario (USER)

Un objeto User representa a una persona con una cuenta en Workfront que puede iniciar sesión e interactuar con el sistema.

El objeto User eliminó el indicador **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>workTime</b>
            </p>
            <p>Este campo se ha agregado y es un número entre 0 y 1 que representa el porcentaje de tiempo que un usuario puede dedicar al trabajo del proyecto (trabajo no general) cada día. El valor 1 significa que el usuario puede dedicar el 100% de su tiempo al trabajo del proyecto.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <ul>
          <li>
            <p><b>userLocations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Grupos de usuarios (USRGPS)

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
            <p>Agregado.</p>
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
            <p>Agregado.</p>
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
            <p><b>changeType</b>
            </p>
            <p>Se agregaron los siguientes valores:</p>
            <ul>
              <li>El documento necesita su aprobación (AAA)</li>
              <li>El documento necesita su revisión (AAR)</li>
              <li>El documento ya no necesita su aprobación (ARA)</li>
              <li>El documento ya no necesita su revisión (ARR)</li>
              <li>El documento necesita la aprobación (ATA) del usuario</li>
              <li>Documento necesita revisión (ATR) del usuario</li>
              <li>El documento ya no necesita la aprobación de (usuario) (RTA)</li>
              <li>El documento ya no necesita revisión (RTR) del usuario</li>
              <li>Documento aprobado (ADA)</li>
              <li>Documento aprobado con cambios (ADC)</li>
              <li>El documento necesita trabajo (AND)</li>
              <li>(Usuario) ha marcado (documento) como aprobado. Su aprobación ya no es necesaria. (AAN)</li>
              <li>(Usuario) ha marcado (documento) como aprobado con cambios. Su aprobación ya no es necesaria. (ACN)</li>
              <li>(Usuario) ha marcado (documento) como necesita trabajar. Su aprobación ya no es necesaria. (AWN)</li>
              <li>El documento necesita su revisión ahora, no su aprobación (AAC)</li>
              <li>El documento necesita su aprobación ahora, en lugar de una revisión (Y)</li>
              <li>Documento revisado (RDC)</li>
              <li>Documento revisado (TRC)</li>
              <li>(Usuario) ha revisado (documento) como completado. Su revisión ya no es necesaria. (TRN)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserRole (USROL)

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
            <p>Agregado.</p>
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
            <p>Agregado.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
