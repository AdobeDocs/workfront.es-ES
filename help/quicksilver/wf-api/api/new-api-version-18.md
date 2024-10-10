---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 18 de la API
description: Adobe Workfront publicó la versión 18 de la API el 6 de abril de 2022. La versión 18 de la API incorpora los siguientes cambios con respecto a la versión 17.
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
source-git-commit: 842b26177a11225049ef42f779ca77dd81926b74
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 0%

---

# Novedades de la versión 18 de la API

Adobe Workfront publicó la versión 18 de la API el 8 de abril de 2024. La versión 18 de la API incorpora los siguientes cambios con respecto a la versión 17.

## Recursos añadidos

No se han añadido recursos para la versión 18 de la API.

## Recursos eliminados

No se han eliminado recursos para la versión 18 de la API

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
            <p>Se agregaron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tasas de costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar tarifas de facturación)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar finanzas generales)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>acciones prohibidas</b>
            </p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tasas de costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar tarifas de facturación)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar finanzas generales)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tasas de costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar tarifas de facturación)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar finanzas generales)</p>
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
            <p><b>acción</b>
            </p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tasas de costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar tarifas de facturación)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar finanzas generales)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule (ACSRUL)

Un objeto AccessRule representa un conjunto de reglas en niveles de acceso personalizados que determina cómo los usuarios pueden compartir los proyectos que crean.

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
            <p>Se agregaron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tasas de costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar tarifas de facturación)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar finanzas generales)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>acciones prohibidas</b>
            </p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tasas de costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar tarifas de facturación)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar finanzas generales)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tasas de costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar tarifas de facturación)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar finanzas generales)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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
            <p>Se agregaron los campos siguientes:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Esperando aprobación (AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Operaciones</td>
      <td>
        <ul>
          <li>
            <p>Se agregaron las siguientes operaciones:
            </p>
            <ul>
              <li>
                <p><b>AGREGAR</b>
                </p>
              </li>
              <li>
                <p><b>DELETE</b>
                </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Línea base (BLIN)

Las líneas de base son instantáneas del aspecto que tuvo el rendimiento de un proyecto en un momento determinado. Almacenan información clave sobre el proyecto, como fechas clave, progreso, valores de costes e ingresos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Se agregaron los campos siguientes:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tarea de línea base (BSTSK)

Las líneas de base son instantáneas del aspecto que tuvo el rendimiento de un proyecto en un momento determinado. Almacenan información clave sobre el proyecto, como fechas clave, progreso, valores de costes e ingresos. Cuando se crea una línea de base, la información de la tarea también se captura en las tareas de línea de base de esa línea de base.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Se agregaron los campos siguientes:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
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
            <p><b>catObjCode</b>:
            </p>
            <p>Se agregaron los siguientes valores posibles:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Categoría de recursos no laborales)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (hora)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Tarjeta de tarifa)
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>objTypes</b>:
            </p>
            <p>Se agregaron los siguientes valores posibles:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Categoría de recursos no laborales)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (hora)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Tarjeta de tarifa)
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Documento (DOCU)

Un objeto Document representa un archivo (como material escrito, imágenes u otras formas de información).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Acciones</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b>:
            </p>
            <p>Se ha añadido el siguiente parámetro:
            <ul>
              <li>
                <p><code>documentID</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>moveToFolder</b>:
            </p>
            <p>Añadido. Esta nueva acción emplea los parámetros siguientes:
            <ul>
              <li>
                <p><code>documentIDs</code>
                </p>
              </li>
              <li>
                <p><code>folderID</code> 
                </p>
              </li>
              <li>
                <p><code>moveToFolder</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Datos financieros (FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Se agregaron los campos siguientes:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p>Se agregaron los campos siguientes:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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
              <li>
                <p><code>AAO</code> (enum.actiontypeenum.assetapproval.opened)</p>
              </li>
              <li>
                <p><code>ADM</code> (enum.actiontypeenum.assetapproval.locked.all.decisions.made)</p>
              </li>
              <li>
                <p><code>AUL</code> (enum.actiontypeenum.assetapproval.unlocked.manual)</p>
              </li>
              <li>
                <p><code>ALM</code> (enum.actiontypeenum.assetapproval.locked.manual)</p>
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
      <td role="rowheader">Acciones</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>:
            </p>
            <p>Se agregaron los campos siguientes:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>convertToTask</b>:
            </p>
            <p>Se agregaron los campos siguientes:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
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
            <p>Se agregaron los campos siguientes:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p><b>createProjectWithOverride</b>
            </p>
             <p>Añadido.
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### FunciónUsuarioProyecto (PTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Se ha añadido el siguiente campo:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li>
            <p>Se ha añadido el siguiente campo:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Un objeto QueueDef representa una cola, que es un proyecto que se ha publicado en el área del servicio de asistencia para permitir a los usuarios enviar problemas al mismo.

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
                <p><code>VIEW_COST_RATES</code> (Ver tasas de costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar tarifas de facturación)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar finanzas generales)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Se agregaron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tasas de costo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de costo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar tarifas de facturación)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar finanzas generales)</p>
              </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tasa (TASA)

Un objeto Rate representa una tarifa de facturación en Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>companyID</b></p><p>Se agregaron los siguientes indicadores:
            </p>
            <ul>
              <li>
                <p>AUTO_LOAD
                </p>
              </li>
              <li>
                <p>DINÁMICO
                </p>
              </li>
             </ul>
          </li>
          <li>
          <p><b>displayName</b></p><p>Añadido.</p>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li>
            <p><b>displayName</b>
            </p><p>Añadido.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
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
            <p>Se agregaron los campos siguientes:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p><b>convertToProject</b>
            </p>
             <p>Se ha añadido el siguiente campo:
             <ul><li><code>copyCategories</code></li></ul>
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Plantilla (TMPL)

Un objeto Template representa un patrón para un proyecto. Los proyectos se pueden crear a partir de plantillas para ahorrar tiempo. Una plantilla contiene un equipo y tareas, que se copiarán en cualquier proyecto creado a partir de la plantilla.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Se agregaron los campos siguientes:
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### TemplateTask (TTSK)

Un objeto TemplateTask representa un objeto Task que forma parte de un objeto Template. Las Tareas de plantilla pasan a ser Tareas en el Proyecto en el que se utiliza la Plantilla.<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Se agregaron los campos siguientes:
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateUserRole (TEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Se ha añadido el siguiente campo:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li>
            <p>Se ha añadido el siguiente campo:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
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
            <p>Se ha eliminado el siguiente campo:
            </p>
            <ul>
              <li>
                <p><b>objCode</b>
                </p>
              </li>
             </ul>
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
            <p><b>updateType</b>
            </p>
            <p>Se agregaron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>assetapprovalsLockedAllDecisionsMade</code></p>
              </li>
              <li>
                <p><code>assetapprovalsUnlockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalsLockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalOpened</code> </p>
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
            <p><b>recentUpdatesObjID</b>
            </p>
            <p>Añadido.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserPrefValue (USERPF)

Un objeto UserPrefValue representa una preferencia de usuario.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>valor</b>
            </p>
            <p>Se ha añadido el validador <code>MAX_LENGTH</code></p>
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
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Se agregaron los campos siguientes:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

