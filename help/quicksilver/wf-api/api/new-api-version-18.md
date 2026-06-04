---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 18 de la API
description: Adobe Workfront publicó la versión 18 de la API el 6 de abril de 2022. La versión 18 de la API incorpora los siguientes cambios con respecto a la versión 17.
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
TQID: https://experienceleague.adobe.com/FEwGBTsppCVzahbxXInxmIc9nSJ0WjGekoDzZP6YovY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1140
ht-degree: 99%

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
            <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tarifas de coste)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de coste)</p>
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
            <p><b>forbiddenActions</b>
            </p>
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tarifas de coste)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de coste)</p>
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
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tarifas de coste)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de coste)</p>
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
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tarifas de coste)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de coste)</p>
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
            <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tarifas de coste)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de coste)</p>
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
            <p><b>forbiddenActions</b>
            </p>
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tarifas de coste)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de coste)</p>
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
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tarifas de coste)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de coste)</p>
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
            <p>Se han añadido los campos siguientes:
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

### AwaitingApproval (AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Operaciones</td>
      <td>
        <ul>
          <li>
            <p>Se han añadido las siguientes operaciones:
            </p>
            <ul>
              <li>
                <p><b>ADD</b>
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

### Baseline (BLIN)

Las líneas de base son instantáneas del aspecto que ha tenido el rendimiento de un proyecto en un momento determinado. Almacenan información clave sobre el proyecto, como fechas clave, progreso, valores de costes e ingresos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Se han añadido los campos siguientes:
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

### BaselineTask (BSTSK)

Las líneas de base son instantáneas del aspecto que ha tenido el rendimiento de un proyecto en un momento determinado. Almacenan información clave sobre el proyecto, como fechas clave, progreso, valores de costes e ingresos. Cuando se crea una línea de base, la información de la tarea también se captura en las tareas de línea de base de esa línea de base.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Se han añadido los campos siguientes:
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
            <p><b>catObjCode</b>:
            </p>
            <p>Se añadieron los siguientes valores posibles:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Categoría de recurso no laboral)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Hora)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Tarjeta de tarifas)
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>objTypes</b>:
            </p>
            <p>Se añadieron los siguientes valores posibles:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Categoría de recurso no laboral)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Hora)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Tarjeta de tarifas)
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

### Document (DOCU)

Un objeto de documento representa un archivo (como material escrito, imágenes u otras formas de información).

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

### FinancialData (FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Se han añadido los campos siguientes:
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
            <p>Se han añadido los campos siguientes:
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

### JournalEntry (JRNLE)

El objeto JournalEntry se puede configurar para que registre información sobre campos de objeto específicos cada vez que se modifiquen dichos campos. Cuando un campo está configurado para registrarse como parte del objeto Entrada de cuaderno, se creará una entrada de cuaderno correspondiente cada vez que se modifique ese campo.

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
            <p>Se añadieron los siguientes valores posibles:</p>
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
            <p>Se han añadido los campos siguientes:
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
            <p>Se han añadido los campos siguientes:
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
            <p>Se han añadido los campos siguientes:
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


### ProjectUserRole (PTEAM)

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
            <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tarifas de coste)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de coste)</p>
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
            <p>Se añadieron los siguientes valores posibles:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Ver tarifas de coste)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver tarifas de facturación)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Ver finanzas generales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar tarifas de coste)</p>
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

### Rate (RATE)

Un objeto Rate representa una tarifa de facturación en Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>companyID</b></p><p>Se han añadido los siguientes indicadores:
            </p>
            <ul>
              <li>
                <p>AUTO_LOAD
                </p>
              </li>
              <li>
                <p>DYNAMIC
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


### Task (TASK)

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
            <p>Se han añadido los campos siguientes:
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

### Template (TMPL)

Un objeto de plantilla representa un patrón para un proyecto. Los proyectos se pueden crear a partir de plantillas para ahorrar tiempo. Una plantilla contiene un equipo y tareas, que se copiarán en cualquier proyecto creado a partir de la plantilla.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Se han añadido los campos siguientes:
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

Un objeto TemplateTask representa un objeto Tarea que forma parte de un objeto Plantilla. Las tareas de plantilla pasan a ser tareas en el proyecto en el que se utiliza la Plantilla.<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Se han añadido los campos siguientes:
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

### TemplateUserRole (TTEAM)

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

### Plantilla de horas (TSHET)

Un objeto Timesheet representa un parte de horas virtual que permite a los usuarios especificar horas trabajadas reales para tareas, proyectos y tipos de horas generales.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li>
            <p>Se ha eliminado el campo siguiente:
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
            <p>Se añadieron los siguientes valores posibles:</p>
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

Un objeto UserPrefValue representa una preferencia del usuario.

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
            <p>Se han añadido los campos siguientes:
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

