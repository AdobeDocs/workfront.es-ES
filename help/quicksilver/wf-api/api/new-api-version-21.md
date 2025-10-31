---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 21 de la API
description: Adobe Workfront publicó la versión 21 de la API el viernes, 23 de octubre de 2025. La versión 21 de la API incorpora los siguientes cambios con respecto a la versión 20.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 155323314712e020a638619d9bf10d678078645e
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 82%

---

# Novedades de la versión 21 de la API

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>

Adobe Workfront publicó la versión 21 de la API el viernes, 23 de octubre de 2025. La versión 21 de la API incorpora los siguientes cambios con respecto a la versión 20.

## Recursos añadidos

### OriginalRequest (ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>entryDate</li>
          <li>Identificador</li>
          <li>requestID</li>
          <li>requestName</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li>Identificador</li>
          <li>objCode</li>
        </ul>
      </td>
 </tbody>
</table>

<!--

### StaffingPlanTemplate (SPTMPL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li>ADD</li>
          <li>COUNT</li>
          <li>DELETE</li>
          <li>EDIT</li>
          <li>GET</li>
          <li>REPORT</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

## Recursos eliminados

### AssignmentBillingRole (ASBRL)

Se han quitado el objeto AssignmentBillingRole y todos sus campos.

## Recursos modificados

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
            <p><b>coreAction</b>
            </p>
            <p>Se ha añadido el siguiente valor posible:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar información de contacto)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Se ha añadido el siguiente valor posible:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar información de contacto)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Se ha añadido el siguiente valor posible:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar información de contacto)</p>
              </li>
            </ul>
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
            <p><b>action</b>
            </p>
            <p>Se ha añadido el siguiente valor posible:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar información de contacto)</p>
              </li>
            </ul>
         </li>
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
            <p><b>coreAction</b>
            </p>
            <p>Se ha añadido el siguiente valor posible:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar información de contacto)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Se ha añadido el siguiente valor posible:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar información de contacto)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Se ha añadido el siguiente valor posible:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar información de contacto)</p>
              </li>
            </ul>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AnnouncementAttachment (ANMATT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>fileExtension</b>
            </p>
            <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Agregado</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <ul>
          <li>
            <p><b>asignaciones de equipo</b>
            </p>
            <p>Agregado</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Asignación (ASSGN)

Un objeto Assignment representa la conexión entre un elemento de trabajo y el usuario, equipo o grupo asignado para trabajar en él.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <ul>
          <li>
            <p><b>assignmentBillingRoles</b>
            </p>
            <p>Eliminado</p>
              </li>
            </ul>
         </li>
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
            <p><b>catObjCode</b>
            </p>
            <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>TEAMOB</code> (Equipo)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>objTypes</b>
            </p>
            <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>TEAMOB</code> (Equipo)</p>
              </li>
            </ul>
          </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Cliente (CUST)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><code>APDISAB</code> (Deshabilitar el uso de un subprograma Java para cálculos de escala de tiempo)
            </p>
            <p>Agregado</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Document (DOCU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <ul>
          <li>
            <p><b>getTemporaryCloudURL</b>
            </p>
            <p>Agregado</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### CarpetaDocumento

El objeto DocumentFolder añadió el indicador `RESTORABLE`.

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
            <p><b>getTerejectionCommentsCloudURL</b>
            </p>
            <p>Se ha añadido el validador <code>MAX_LENGTH</code></p>
              </li>
            </ul>
         </li>
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
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Agregado</p>
              </li>
            </ul>
         </li>
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
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>Se ha añadido el siguiente valor posible:</p>
             <ul>
              <li>
                <p><code>RICHLX</code> (Texto enriquecido léxico)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Se ha añadido el siguiente valor posible:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Acumulación de una sola línea)</p>
              </li></ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>Agregado</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos predeterminados</td>
      <td>
        <ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>Agregado</p>
           </li>
           </ul>
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
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>overrideCurrency</b>
            </p>
            <p>Agregado</p>
              </li>
            </ul>
         </li>
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
      <td>
        <ul>
          <li>
            <p><b>moneda</b>
            </p>
            <p>Agregado</p>
              </li>
            </ul>
         </li>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Agregado</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Un objeto QueueDef representa una cola, que es un proyecto que se ha publicado en el área del servicio de asistencia para permitir a los usuarios enviarle problemas.

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
            <p>Se ha añadido el siguiente valor posible:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar información de contacto)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Se ha añadido el siguiente valor posible:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar información de contacto)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <ul>
          <li>
            <p><b>helpDeskProjects</b>
            </p>
            <p>Agregado</p>
            </li>
            </ul>
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
            <p><b>localBillingPerHour</b>
            </p>
            <p>Eliminado</p>
              </li>
          <li>
            <p><b>localCostPerHour</b>
            </p>
            <p>Eliminado</p>
              </li>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Función (ROLE)

Un objeto Role (función) representa una capacidad funcional o un conjunto de aptitudes que un usuario podría completar, como un diseñador o un gestor de productos.

<div class="preview">

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>Anular moneda</b>
            </p>
            <p>Eliminado</p>
              </li>
          <li>
            <p><b>Anular tarifa de costo</b>
            </p>
            <p>Eliminado</p>
              </li>
          <li>
            <p><b>Anular tarifa de facturación</b>
            </p>
            <p>Eliminado</p>
              </li>
      </td>
    </tr>
  </tbody>
</table>

</div>

### Informe programado (SCHREP)

Un objeto ScheduledReport representa un informe que se ha configurado para que se programe su envío.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>format</b>
            </p>
            <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>FLV</code></p></li>
              <li><p><code>M4V</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Un objeto ScoreCardQuestion representa una pregunta que se ha añadido a un informe de valoración. Estas preguntas suelen ser determinadas por el responsable del portafolio, y sus respuestas le permiten comprender cómo se ajusta un proyecto a las metas del portafolio.<table>
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
            <p>Se ha añadido el siguiente valor posible:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Acumulación de una sola línea)</p>
              </li></ul>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### StaffingPlan

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

<!--

### StaffingPlanResource

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Agregado</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <ul>
          <li>
            <p><b>asignaciones de equipo</b>
            </p>
            <p>Agregado</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Equipo

El objeto Team agregó los indicadores `DATA_EXTENDIBLE` y `SHARABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Agregado</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td>
        <ul>
          <li>
            <p><b>categoría</b>
            </p>
            <p>Agregado</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
            <p>Agregado</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


### TemplateAssignment

El objeto TemplateAssignment agregó el marcador `ATTRIBUTE_ATTACHABLE`.

### Plantilla de horas (TSHET)

Un objeto Timesheet representa un parte de horas virtual que permite a los usuarios especificar horas trabajadas reales para tareas, proyectos y tipos de horas generales.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos principales</td>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Agregado</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <ul>
          <li>
            <p><b>asignaciones de equipo</b>
            </p>
            <p>Agregado</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


