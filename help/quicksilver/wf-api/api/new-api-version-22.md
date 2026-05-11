---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 22 de la API
description: Adobe Workfront lanzó la versión 22 de la API el 11 de mayo de 2026. La versión 22 de la API incorpora los siguientes cambios con respecto a la versión 21.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 682cf24c4c7932afeb66a2e5434fe3cec887e889
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 54%

---

# Novedades de la versión 22 de la API

Adobe Workfront lanzó la versión 22 de la API el 8 de mayo de 2026. La versión 22 de la API incorpora los siguientes cambios con respecto a la versión 21.

## Recursos añadidos

Se agregaron los siguientes recursos para la versión 22 de la API.

### ReportShareableFolder (RPSHFD)

Puede utilizar carpetas de informes que se pueden compartir para organizar informes y compartir esas carpetas con otros usuarios. Esta función está diseñada para equipos que administran grandes volúmenes de informes y necesitan un control de acceso escalable y coherente.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Campos predeterminados</td>
      <td>
        <ul>
          <li>name</li>
        </ul>
      </td>
    </tr>
   <tr>
      <td role="rowheader">Operaciones</td>
      <td>
        <ul>
          <li>ADD</li>
          <li>COUNT</li>
          <li>ELIMINAR</li>
          <li>EDITAR</li>
          <li>GET</li>
          <li>REPORT</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

## Recursos eliminados

Se eliminaron los siguientes recursos de la versión 22 de la API.

### UserLocation (USRLOC)

Este objeto se ha eliminado.

## Recursos modificados

Se modificaron los siguientes recursos para la versión 22 de la API.

### AccessLevel (ACSLVL)

Un objeto AccessLevel está asociado a los usuarios y describe el conjunto de AccessLevelPermissions que determinan a qué puede tener acceso el usuario.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>El siguiente campo se ha modificado con cambios en posibles valores. Para obtener más información, consulte la documentación para desarrolladores.
        <ul>
          <li><b>fieldAccessPrivileges</b></li>
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
      <td>Los campos siguientes se han modificado con cambios en posibles valores. Para obtener más información, consulte la documentación para desarrolladores.
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
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
      <td>El siguiente campo se ha modificado con cambios en posibles valores. Para obtener más información, consulte la documentación para desarrolladores.
        <ul>
          <li><b>acción</b></li>
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
      <td>Los campos siguientes se han modificado con cambios en posibles valores. Para obtener más información, consulte la documentación para desarrolladores.
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
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
      <td>Se agregaron los campos siguientes para admitir la administración de almacenamiento empresarial.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
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
      <td>Se ha añadido el siguiente campo.
        <ul>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### Compañía (CMPY)

Un objeto de compañía representa a una organización formada por una colección de personas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>Se agregaron los campos siguientes para admitir la administración de almacenamiento empresarial.
        <ul>
          <li><b>esmProjectID</b></li>
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
      <td>Agregado
        <ul>
          <li><p><b>getDefaultAssignmentStatusEnum</b></p></li>
          <li><p><b>getDefaultBookingStatusEnum</b></p></li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">Consultas</td>
      <td>Agregado
        <ul>
          <li><p><b>assignmentStatus</b></p></li>
          <li><p><b>bookingStatus</b></p></li>
        </ul>
      </td>
    </tr>
</tbody>
</table>

### Cliente (CUST)

Un objeto de cliente representa a una organización que utiliza una instancia de Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>Se ha modificado el siguiente campo.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>Se agregaron los siguientes valores posibles.</p>
             <ul>
              <li>
                <p><code>STATUS_BOOKING</code> (Estados de reserva)</p>
              </li>
              <li>
                <p><code>STATUS_ASSIGNMENT</code> (Estados de asignación)</p>
              </li>
            </ul>
         </li>
         </ul>
         <p>Se agregaron los campos siguientes para admitir la administración de almacenamiento empresarial.
         <ul>
         <li><b>isLegacyCustomerEsmStorageEnabled</b></li>
         <li><b>isLegacyCustomerSystemFileMigrationEnabled</b></li>
         <li><b>legacyCustomerEsmStorageMigrationDate</b></li>
         <li><b>legacyCustomerSystemFileMigrationDate</b></li>
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
      <td>Se ha modificado el siguiente campo.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>Se agregaron los siguientes valores posibles para admitir la administración de almacenamiento empresarial:</p>
             <ul>
              <li>
                <p><code>customer:config.defaultStorageModeAllowOverride</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageMode</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageGroupRollout</code> </p>
              </li>
               <li>
                <p><code>customer:config.defaultStorageGroupOptions</code> </p>
              </li>
             </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>


### Document (DOCU)

Un objeto de documento representa un archivo (como material escrito, imágenes u otras formas de información).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>Se agregaron los campos siguientes para admitir la administración de almacenamiento empresarial.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmAsset</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>Se ha modificado la siguiente acción.
        <ul>
          <li><p><b>createLargeDocument
          </b></p><p>Se agregaron los campos siguientes para admitir la administración de almacenamiento empresarial.
         <ul>
         <li><b>docObjCode</b></li>
         <li><b>objID</b></li>
         </ul>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### DocumentFolder (DOCFDR)

Los documentos se pueden organizar en carpetas. Puede crear carpetas personales en el área de documentos personales. El objeto DocumentFolder representa una de estas carpetas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>Se agregaron los campos siguientes para admitir la administración de almacenamiento empresarial.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmFolder</b></li>
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
      <td>Se ha agregado el siguiente campo para admitir la administración de almacenamiento empresarial.
        <ul>
          <li><b>esmVersionID</b></li>
        </ul>
      Se ha modificado el siguiente campo.
        <ul>
          <li><b>version</b><p>Se ha eliminado el validador "REQUERIDO".</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>Se ha añadido la siguiente acción.
        <ul>
          <li><p><b>sendToAEMDetails</b></p>
         </li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">Operaciones</td>
      <td>Se ha añadido la siguiente operación.
        <ul>
          <li><p><b>EDITAR</b></p>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### ExchangeRate (EXRATE)

Un objeto ExchangeRate representa un tipo de cambio de divisa configurado en Workfront. Los objetos ExchangeRate no son dinámicos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>Se agregaron los campos siguientes.
        <ul>
          <li><b>portfolioID</b></li>
          <li><b>programID
          </b></li>
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
      <td>Se han modificado los campos siguientes.
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Se agregaron los siguientes valores posibles.</p>
             <ul>
              <li>
                <p><code>PFM</code>(Mover carpeta)</p>
              </li>
              </ul>
         </li>
          <li>
            <p><b>indicadores</b>
            </p>
            <p>Se agregaron los siguientes valores posibles.</p>
             <ul>
              <li>
                <p><code>CI</code>(enum.Journalentryflagenum.iscontactinfoentry)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalField (JRNLF)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>Se han modificado los campos siguientes.
        <ul>
          <li>
            <p><b>action</b>
            </p>
            <p>Se agregaron los siguientes valores posibles.</p>
             <ul>
              <li>
                <p><code>PFM</code>(Mover carpeta)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask (OPTASK)

Un objeto OpTask suele conocerse como Problema. Un problema es un elemento de trabajo que normalmente indica que hay un problema que impide la finalización de una tarea o proyecto. Un problema también puede ser una solicitud del servicio de asistencia. Las solicitudes de cambio, las solicitudes y los errores también son problemas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li><b>actualWorkRequired</b><p>Se han añadido los siguientes indicadores:
           <ul>
           <li><code>AUTO_LOAD</code></li>
           <li><code>DYNAMIC</code></li>
           </ul>
           </p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Buscar campos</td>
      <td>
        <ul>
          <li><b>actualWork</b><p>El tipo cambió de <code>null</code> a <code>double</code>.</p></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OriginalRequest(ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Operaciones</td>
      <td>Se han añadido las siguientes operaciones.
        <ul>
          <li><p><b>COUNT</b></p>
          <li><p><b>GET</b></p>
          <li><p><b>REPORT</b></p>
          <li><p><b>SEARCH</b></p>
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
      <td>Se agregaron los campos siguientes.
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### Grupo de parámetros (PGRP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>Se agregaron los campos siguientes.
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### SecciónPortal (PTLSEC)

Un objeto PortalSection es un informe.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>Se ha añadido el siguiente campo.
        <ul>
          <li><b>reportShareableFolderID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td>Se ha añadido el siguiente campo.
        <ul>
          <li><b>reportShareableFolder</b></li>
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
      <td role="rowheader">Campos directos</td>
      <td>Se agregaron los campos siguientes para admitir la administración de almacenamiento empresarial.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
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
      <td role="rowheader">Campos directos</td>
      <td>Se agregaron los campos siguientes para admitir la administración de almacenamiento empresarial.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      Se ha modificado el siguiente campo.
        <ul>
          <li><b>portfolioID</b><p>Se ha agregado el validador "REQUERIDO".</li>
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
      <td>Se agregaron los campos siguientes para admitir la administración de almacenamiento empresarial.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### QueueDef (QUED)

Un objeto QueueDef representa una definición de cola de solicitud en Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>Los campos siguientes se han modificado con cambios en posibles valores. Para obtener más información, consulte la documentación para desarrolladores.
        <ul>
          <li><b>requestorCoreAction</b></li>
          <li><b>requestorForbiddenActions</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Informe programado (SCHREP)

Un objeto ScheduledReport representa un informe que se ha configurado para que se programe su envío.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>El siguiente campo se ha modificado con grandes cambios en los posibles valores. Para obtener más información, consulte la documentación para desarrolladores.
        <ul>
          <li><b>formato</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Tarea (TAREA)

Un objeto Task representa un elemento de trabajo que debe completarse como parte del objetivo final (completar un proyecto).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li><p><b>convertedOpTaskID</b><p>
              <p>Agregado</p></li>
          <li><p><b>actualWorkRequired</b></p><p>Se agregaron las marcas <code>AUTO_LOAD</code> y <code>DYNAMIC</code>.</p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td>
        <ul>
          <li>
            <p><b>convertedOpTask</b>
            </p>
            <p>Agregado</p>
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
      <td role="rowheader">Campos directos</td>
      <td>Se agregaron los campos siguientes para admitir la administración de almacenamiento empresarial.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
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
      <td>Se ha modificado el siguiente campo.
        <ul>
          <li>
            <p><b>action</b>
            </p>
            <p>Se ha agregado el siguiente valor posible.</p>
             <ul>
              <li>
                <p><code>primaryFolderMoved</code></p>
              </li>
              </ul>
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
      <td role="rowheader">Campos directos</td>
      <td>Se ha añadido el siguiente campo.
        <ul>
          <li><b>eauthUserID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>Se ha eliminado el siguiente campo.
        <ul>
          <li><b>userLocations</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>





