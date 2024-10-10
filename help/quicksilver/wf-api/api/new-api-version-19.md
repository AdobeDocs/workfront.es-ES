---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 19 de la API
description: Adobe Workfront publicó la versión 19 de la API el 6 de abril de 2022. La versión 19 de la API incorpora los siguientes cambios con respecto a la versión 18.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 13910328903744aa9bf619e8b4c376520c21b89e
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# Novedades de la versión 19 de la API

Adobe Workfront publicó la versión 19 de la API el 8 de abril de 2024. La versión 19 de la API incorpora los siguientes cambios con respecto a la versión 18.

## Recursos añadidos

No se han añadido recursos para la versión 19 de la API.

## Recursos eliminados

No se han eliminado recursos para la versión 19 de la API

## Recursos modificados

### AccessLevel (ACSLVL)

Un objeto AccessLevel está asociado a los usuarios y describe el conjunto de AccessLevelPermissions que determinan a qué puede tener acceso el usuario.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>accessRestrictions</b><p>Se agregaron los siguientes valores posibles:
            </p>
            <ul>
              <li>
                <p>Desactivar el asistente de Workfront AI (AIOFF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Asignación (ASIGNAR)

Un objeto Assignment representa la conexión entre un elemento de trabajo y el usuario, equipo o grupo asignado para trabajar en él.

El objeto Assignment agregó el indicador **DATA_EXTENDIBLE**.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>Se agregaron los siguientes campos directos:
        <ul>
          <li>
            <p><b>categoryID</b><p>Una categoría es un formulario personalizado. Este campo admite la capacidad de agregar un formulario personalizado a una asignación.
            </p>
          </li>
          <li>
            <p><b>prioridad</b><p>Este campo permite los siguientes valores:
            <ul>
              <li>0 (Ninguno)</li>
              <li>1 (bajo)</li>
              <li>2 (Normal)</li>
              <li>3 (Alta)</li>
              <li>4 (Urgente)</li>
             </ul>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td>Se agregaron los siguientes campos de referencia:
        <ul>
          <li>
            <p><b>categoría</b><p>Una categoría es un formulario personalizado. Este campo admite la capacidad de agregar un formulario personalizado a una asignación.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>Se agregaron los siguientes campos de colección:
        <ul>
          <li>
            <p><b>objectCategories</b><p>Una categoría es un formulario personalizado. Este campo admite la capacidad de agregar un formulario personalizado a una asignación.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### Categoría (CTGY)

Un objeto Category es un formulario personalizado.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>Se han agregado los siguientes campos para admitir la capacidad de agregar un formulario personalizado a una asignación.
        <ul>
          <li>
            <p><b>catObjCode</b><p>Se agregaron los siguientes valores posibles:
            </p>
            <ul>
              <li>
                <p>Asignación (ASIGNAR)
                </p>
              </li>
             </ul>
          </li>
          <li>
            <p><b>objTypes</b><p>Se agregaron los siguientes valores posibles:
            </p>
            <ul>
              <li>
                <p>Asignación (ASIGNAR)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Clasificador (CLSF)

Un clasificador es una ubicación.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>Se agregaron las siguientes acciones:
        <ul>
          <li>
            <b>activateClassifiers</b>
          </li>
          <li>
            <b>desactivarClasificadores</b>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Cliente

Un objeto Customer representa una organización que utiliza una instancia de Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>customEnumTypes</b><p>Se agregaron los siguientes valores posibles:
            </p>
            <ul>
              <li>
                <p>Prioridades de asignación (PRIORITY_ASSIGNMENT)
                </p>
              </li>
             </ul>
          </li>
              <p>El objeto CustomEnum ayuda a convertir los códigos de estado en texto legible en lenguaje natural.</p>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Preferencias del cliente (CUSTPR)

Un objeto CustomerPreferences representa el conjunto de preferencias que un cliente ha establecido para su instancia de Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>name</b><p>Se han eliminado los siguientes valores posibles:
            </p>
            <ul>
              <li>
                <p>Habilitar integración de Zoom en el flujo de actualizaciones (contraseña:zoomIntegrationEnabled)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Documento (DOCU)

Un objeto Document representa un archivo (como material escrito, imágenes u otras formas de información).

<table>
  <tbody>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b><p>Se agregó el campo <code>folderID</code>.</p>
          </li>
          <li>
            <p><b>sendDocumentsToExternalProvider</b><p>Añadido.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### Tipo de cambio (EXRATE)

Un objeto ExchangeRate representa un tipo de cambio de divisa configurado en Workfront. Los objetos ExchangeRate no son dinámicos.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
      <ul>
      <li>Los siguientes campos han agregado el validador <code>REQUIRED</code>:
        <ul>
          <li><p><b>moneda</b></li>
          <li><p><b>clasificar</b></li></ul>
      <li>Se han añadido los campos siguientes:
        <ul>
          <li><p><b>enteredByID</b></li>
          <li><p><b>entryDate</b></li>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td>
      <ul>
        <li>Se han añadido los campos siguientes:
        <ul>
          <li><p><b>enteredBy</b></li>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Grupo (GROUP)

Un objeto Group representa un conjunto de usuarios y equipos. Los grupos a menudo representan la estructura departamental.

El objeto Group agregó el marcador **SHARABLE**.

### Hora (HORA)

Un objeto Hour representa una hora registrada por un usuario en una plantilla de horas.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
      Se han añadido los campos siguientes:
        <ul>
          <li><p><b>assignedApproverID</b></li>
          <li><p><b>isBillable</b></li>
          <li><p><b>isBilled</b></li>
          <li><p><b>rejectByID</b></li>
          <li><p><b>rejectOnDate</b></li>
          <li><p><b>rejectionComment</b></li>
          <li><p><b>submittedByID</b></li>
          </ul>
          <p>Se realizaron los siguientes cambios en el campo <b>hours</b>.</p>
          <ul> 
          <li> Se eliminó el validador <b>GREATER_THAN</b></li>
          <li> Se agregó el validador <b>NOT_EQUAL</b></li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
      Se han añadido las siguientes acciones:
        <ul>
          <li><p><b>aprobar</b></li>
          <li><p><b>desaprobar</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### Entrada de diario (JRNLE)

El objeto JournalEntry se puede configurar para que registre información sobre campos de objeto específicos cada vez que se modifiquen dichos campos. Cuando un campo está configurado para registrarse como parte del objeto Entrada de cuaderno, se creará una Entrada de cuaderno correspondiente cada vez que se modifique ese campo.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>banderas</b><p>Se agregaron los siguientes valores posibles:
            </p>
            <ul>
              <li>
                <p>Es la tasa de coste (CR)
                </p>
              </li>
              <li>
                <p>Es la tasa de facturación (BR)
                </p>
              </li>
              <li>
                <p>Es finanzas generales (GF)
                </p>
              </li>
              <li>
                <p>Es una financiación combinada (FC)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Parámetro (PARAM)

Un objeto Parameter es un campo personalizado.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>dataType</b></p><p>Se ha añadido el siguiente valor posible:
            <ul>
            <li>Duración (DRTN)</li>
            </ul>
          </li>
          <li>
            <p><b>displayType</b></p><p>Para crear un sistema más flexible y fácil de usar, el tipo de campo <b>Widget (WIDGET)</b> se ha quedado obsoleto y se ha dividido en los siguientes tipos de campo:
            <ul>
            <li>Adobe XD (ADOBE EXD)</li>
            <li>Imagen (IMAGEN)</li>
            <li>PDF (PDF)</li>
            <li>Vídeo (VÍDEO)</li>
            <li>Búsqueda externa (EXTRNL)</li>
            <li>Búsqueda externa de selección múltiple (MULTEXTRNL)</li>
            <li>Campo nativo (WFNATIVE)</li>
            <li>Campo de planificación (WFPLANNING)</li>
            <li>KPI de fase temporal (FASE TEMPORAL)</li>
            <li>Acumulación (RESUMEN)</li>
            <li>Documentos (DOCUMENTO)</li>
           </ul>
          </li>
          <li>
            <p><b>configuraciones</b><p>Añadido.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Rol (ROLE)

Un objeto Role (función del puesto) representa una capacidad funcional o un conjunto de aptitudes que un usuario podría completar, como Designer o Product Manager.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
    Se han añadido los campos siguientes:
        <ul>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td>
        Se han añadido los campos siguientes:
        <ul>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion {#scorecardquestion}

Un objeto ScoreCardQuestion representa una pregunta que se ha agregado a un informe de valoración. Estas preguntas suelen ser determinadas por el gestor del Portfolio, y sus respuestas le permiten comprender cómo se ajusta un proyecto a los objetivos del portafolio.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
            <p><b>displayType</b></p><p>Para crear un sistema más flexible y fácil de usar, el tipo de campo <b>Widget (WIDGET)</b> se ha quedado obsoleto y se ha dividido en los siguientes tipos de campo:
            <ul>
            <li>Adobe XD (ADOBE EXD)</li>
            <li>Imagen (IMAGEN)</li>
            <li>PDF (PDF)</li>
            <li>Vídeo (VÍDEO)</li>
            <li>Búsqueda externa (EXTRNL)</li>
            <li>Búsqueda externa de selección múltiple (MULTEXTRNL)</li>
            <li>Campo nativo (WFNATIVE)</li>
            <li>Campo de planificación (WFPLANNING)</li>
            <li>KPI de fase temporal (FASE TEMPORAL)</li>
            <li>Acumulación (RESUMEN)</li>
            <li>Documentos (DOCUMENTO)</li>
           </ul>
      </td>
  </tbody>
</table>

### TemplateAssignment (TASSGN)

Un objeto TemplateAssignment representa la conexión entre una tarea de plantilla y el usuario, equipo o grupo asignado para trabajar en ella. Cuando se utiliza la plantilla para un proyecto, ese usuario, equipo o grupo se asigna a la tarea.

El objeto TemplateAssignment agregó el indicador **DATA_EXTENDIBLE**.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>Se agregaron los siguientes campos directos:
        <ul>
          <li>
            <p><b>categoryID</b><p>Una categoría es un formulario personalizado. Este campo admite la capacidad de agregar un formulario personalizado a una asignación.
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Campos de referencia</td>
      <td>Se agregaron los siguientes campos de referencia:
        <ul>
          <li>
            <p><b>categoría</b><p>Una categoría es un formulario personalizado. Este campo admite la capacidad de agregar un formulario personalizado a una asignación.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>Se agregaron los siguientes campos de colección:
        <ul>
          <li>
            <p><b>objectCategories</b><p>Una categoría es un formulario personalizado. Este campo admite la capacidad de agregar un formulario personalizado a una asignación.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Hoja de horas (TSHET)

Un objeto Timesheet representa un parte de horas virtual que permite a los usuarios especificar horas trabajadas reales para tareas, proyectos y tipos de horas generales.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b></p><p>Eliminado.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


