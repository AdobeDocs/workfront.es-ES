---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 20 de la API
description: Adobe Workfront publicó la versión 20 de la API el 6 de abril de 2022. La versión 20 de la API incorpora los siguientes cambios con respecto a la versión 19.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 6d2aa582a72aad098e397a5e59abdee84165a426
workflow-type: tm+mt
source-wordcount: '1792'
ht-degree: 60%

---

# Novedades de la versión 20 de la API

Adobe Workfront publicó la versión 20 de la API el lunes, 04 de mayo de 2025. La versión 20 de la API incorpora los siguientes cambios con respecto a la versión 19.

## Recursos añadidos

No se han añadido recursos para la versión 20 de la API.

<!--

### AssignmentBillingRole (ASBLRL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>assignmentID</b></li>
          <li><b>customerID</b></li>
          <li><b>endDate</b></li>
          <li><b>ID</b></li>
          <li><b>roleID</b></li>
          <li><b>startDate</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>assignment</b></li>
          <li><b>customer</b></li>
          <li><b>role</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlan (STAFFP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
          <li><b>name</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>name</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COPY</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlanResource (STAFFR)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

## Recursos eliminados

No se han eliminado recursos para la versión 20 de la API

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
                <p><code>REMOVE_CUSTOMFORM</code> (Eliminar de datos personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Agregar subproyectos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--           <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Eliminar de datos personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Agregar subproyectos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Eliminar de datos personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Agregar subproyectos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> (Eliminar de datos personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Agregar subproyectos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> (Eliminar de datos personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Agregar subproyectos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Eliminar de datos personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Agregar subproyectos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Eliminar de datos personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Agregar subproyectos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
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
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>actualValue</li>
              <li>billedRevenue</li>
              <li>presupuesto</li>
              <li>budgetCost</li>
              <li>Horas presupuestadas</li>
              <li>budgetLaborCost</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRiskCost</li>
              <li>plannedValue</li>
              <li>remainingDeCosto</li>
              <li>remainingLocales</li>
              <li>remainingRiesgoCosto</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>Los campos siguientes cambiaron su tipo de <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>plannedDuration</b></p> <p>Se agregaron las marcas <code>DYNAMIC</code>, <code>LAZY_READ</code> y <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Se ha añadido el indicador <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>Se agregó el valor posible <code>URH</code> (usuario y rol por hora) </li>
          <li><p><b>revenueType</b></p> <p>Se agregaron los valores posibles <code>URH</code> (usuario y rol por hora), <code>URC</code> (usuario y rol por hora sin tope) y <code>URF</code> (usuario y rol por hora más fijos)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
          <p>Se han añadido los campos siguientes:</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### Asignación (ASSGN)

Un objeto Assignment representa la conexión entre un elemento de trabajo y el usuario, equipo o grupo asignado para trabajar en él.

El objeto Assignment agregó los indicadores `ATTRIBUTE_ATTACHABLE` y `DOMAIN_EXTENDABLE`.


<!--
<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
             <p>Added the following fields:</p>
             <ul>
              <li><b>assignmentBillingRoles<b></li>
              <li><b>billingRates<b></li>
              <li><b>costRates<b></li>
            </ul>
      </td>
   <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

### Avatar

Un objeto Avatar es una foto de usuario.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p><b>attachmentObjectCode</b>
            </p>
             <p>Agregado</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principales</td>
      <td>
        <ul>
          <li>
            <p><b>attachmentObjectCode</b>
            </p>
             <p>Agregado</p>
           </li>
          </li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operaciones</td>
      <td>
        <ul>
          <li>
            <p><b>COPIAR</b>
            </p>
             <p>Agregado</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
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
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>presupuesto</li>
              <li>eac</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>Los campos siguientes cambiaron su tipo de <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>Se ha añadido el indicador <code>CURRENCY</code></li>
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
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>Los campos siguientes cambiaron su tipo de <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>Se ha añadido el indicador <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### BillingRecord (BILL)

Un objeto BillingRecord registra los ingresos, horas o gastos que se pueden facturar. Esta información puede utilizarse para crear facturas en un sistema contable externo.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>cantidad</li>
              <li>otherAmount</li>
            </ul>
          </li>
          <li><p><b>entryDate</b></p> <p>Agregado</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


<!--### Category (CTGY)

A Category object is a custom form.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>-->

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
            <p><b>configuraciones</b>
            </p>
             <p>Agregado</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Compañía (CMPY)

Un objeto de compañía representa a una organización formada por una colección de personas.

El objeto Company agregó el indicador `SHARABLE`.

<!--

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>billingRates</b>
            </p>
             <p>Added</p>
          </li>
          <li>
            <p><b>costRates</b>
            </p>
             <p>Added</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

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
              <li><p><code>project.mgmt:default.project.singleassignmentschedule</code> (singleassignmentschedule)</p></li>
              <li><p><code>project.mgmt:logged.taskissue.move</code> (config.loggedtaskissue.remove)</p></li>
            </ul>
          </li>
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
      <td>
           <p>Los campos siguientes cambiaron su tipo de <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>clasificar</li>
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
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualExpenseCost</li>
              <li>actualFixedRevenue</li>
              <li>actualLaborCost</li>
              <li>actualLaborCostHours</li>
              <li>actualLaborRevenue</li>
              <li>actualNonBillableExpenseCost</li>
              <li>fixedCost</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedFixedRevenue</li>
              <li>plannedLaborCost</li>
              <li>plannedLaborCostHours</li>
              <li>plannedLaborRevenue</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>totalActualCost</li>
              <li>totalActualRevenue</li>
              <li>totalPlannedCost</li>
              <li>totalPlannedRevenue</li>
              <li>totalVarianceCost</li>
              <li>totalVarianceRevenue</li>
              <li>varianzaCostoGasto</li>
              <li>varianzaCosteLaboral</li>
              <li>varianzaTrabajoCosteHoras</li>
              <li>varianzaIngresosLaborales</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

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
            <p><b>moneda</b>
            </p>
             <p>Agregado</p>
          </li>
         </ul>
      </td>
    </tr>
  </tbody>
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
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
            </ul>
          </li>
          <li>
          <p>Los campos siguientes cambiaron su tipo de <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
          </ul>
          </li>
          <li><p><b>ratesOrigin</b></p> <p>Agregado</p></li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>



### OpTask (OPTASK)

Un objeto OpTask suele conocerse como Problema. Un problema es un elemento de trabajo que normalmente indica que hay un problema que impide la finalización de una tarea o proyecto. Un problema también puede ser una solicitud del servicio de asistencia. Las solicitudes de cambio, las solicitudes y los errores también son problemas.

El objeto OpTask agregó el indicador DOMAIN_EXTENDABLE

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualCost</li>
            </ul>
          </li>
          <li>
          <p>Los campos siguientes cambiaron su tipo de <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
              <li>actualCost</li>
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
            <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>INTRNL</code> (Búsqueda interna)</p>
              </li>
              <li>
                <p><code>MULTINTRNL</code> (Búsqueda interna de selección múltiple)</p>
              </li>
              <li>
                <p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p>
              </li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>



### Portafolio (PORT)

Un objeto Portafolio es una colección de proyectos que compiten por los mismos recursos, generalmente dinero o personas para completarlos.

El objeto Portfolio agregó el marcador `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>alineado</li>
              <li>presupuesto</li>
              <li>currrency</li>
              <li>netValue</li>
              <li>onBudget</li>
              <li>onTime</li>
              <li>portfolioNetValue</li>
              <li>portfolioRoi</li>
              <li>roi</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Programa (PRGM)

Un objeto Program es un subconjunto de proyectos dentro de un portafolio, donde se pueden agrupar proyectos similares.

El objeto Program agregó el marcador `DOMAIN_EXTENDABLE`.

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
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>actualValue</li>
              <li>bcwp</li>
              <li>cptp</li>
              <li>billedRevenue</li>
              <li>presupuesto</li>
              <li>budgetCost</li>
              <li>Horas presupuestadas</li>
              <li>budgetLaborCost</li>
              <li>eac</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
              <li>plannedRiskCost</li>
              <li>plannedValue</li>
              <li>remainingDeCosto</li>
              <li>remainingLocales</li>
              <li>remainingRiesgoCosto</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>Los campos siguientes cambiaron su tipo de <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Se ha añadido el indicador <code>CURRENCY</code></li>
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
                <p><code>REMOVE_CUSTOMFORM</code> (Eliminar de datos personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Agregar subproyectos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Eliminar de datos personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Agregar subproyectos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Tasa (RATE)

Un objeto Rate representa una tarifa de facturación en Workfront.

El objeto Rate agregó el marcador `ATTRIBUTE_ATTACHABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>costPerHour</li>
              <li>localBillingPerHour</li>
              <li>localCostPerHour</li>
              <li>localCurrency</li>
              <li>rateValue</li>
            </ul>
          </li>
          <li>
          <p>Los campos siguientes cambiaron su tipo de <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>costPerHour</li>
          <li>localBillingPerHour</li>
          <li>localCostPerHour</li>
          <li>rateValue</li>
          </ul>
          </li>
         <li>
          <p>Se han añadido los campos siguientes:
          <ul>
          <li>currrency</li>
          <li>bloqueado</li>
          <li>tipo</li>
          <li>value</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Función (ROLE)

Un objeto Role (función) representa una capacidad funcional o un conjunto de aptitudes que un usuario podría completar, como un diseñador o un gestor de productos.

El objeto Role agregó el marcador `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
        <ul>
          <li>
          <p>Se han añadido los campos siguientes:
          <ul>
          <li>billingRates</li>
          <li>costRates</li>
          </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>format</b>
            </p>
             <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Un objeto ScoreCardQuestion representa una pregunta que se ha añadido a un informe de valoración. Estas preguntas suelen ser determinadas por el responsable del portafolio, y sus respuestas le permiten comprender cómo se ajusta un proyecto a las metas del portafolio.

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
             <p>Se añadieron los siguientes valores posibles:</p>
             <ul>
              <li><p><code>INTRNL</code> (Búsqueda interna)</p></li>
              <li><p><code>MULTINTRNL</code> (Búsqueda interna de selección múltiple)</p></li>
              <li><p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tarea (TAREA)

Un objeto Tarea representa un elemento de trabajo que debe realizarse como un paso hacia la meta de un objetivo final (completar un proyecto).

El objeto Task agregó el marcador `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
            </ul>
          </li>
          <li>
          <p>Los campos siguientes cambiaron su tipo de <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>Se añadieron los siguientes valores posibles:<ul><li><code>URH</code> (Usuario y rol por hora)</li></ul></li>
          <li><p><b>revenueType</b></p> <p>Se añadieron los siguientes valores posibles:<ul><li><code>URH</code> (Usuario y rol por hora)</li><li><code>URC</code> (Usuario y rol por hora sin tope)</li><li><code>URF</code> (Usuario y rol por hora más fijos)</li></ul></li>
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
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>presupuesto</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
              <li>plannedRiskCost</li>
              <li>workRequired</li>
            </ul>
          </li>
          <li>
          <p>Los campos siguientes cambiaron su tipo de <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
          <p>Se han añadido los campos siguientes:</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateTask (TTSK)

Un objeto TemplateTask representa un objeto Tarea que forma parte de un objeto Plantilla. Las tareas de plantilla pasan a ser tareas en el proyecto en el que se utiliza la Plantilla.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>billingAmount</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
              <li>revenueType</li>
            </ul>
          </li>
          <li>
          <p>Los campos siguientes cambiaron su tipo de <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>Se añadieron los siguientes valores posibles:<ul><li><code>URH</code> (Usuario y rol por hora)</li></ul></li>
          <li><p><b>revenueType</b></p> <p>Se añadieron los siguientes valores posibles:<ul><li><code>URH</code> (Usuario y rol por hora)</li><li><code>URC</code> (Usuario y rol por hora sin tope)</li><li><code>URF</code> (Usuario y rol por hora más fijos)</li></ul></li>
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
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
             <p>Eliminado</p>
          </li>
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
                <p><code>externalFolderMetadataError</code> (enum.updatetype.externalFolderMetadataError)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Usuario (USER)

Un objeto User representa a una persona con una cuenta en Workfront que puede iniciar sesión e interactuar con el sistema.

El objeto de usuario agregó los campos `ATTRIBUTE_ATTACHABLE` y `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos directos</td>
      <td>
        <ul>
          <li>
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de colección</td>
      <td>
          <p>Se han añadido los campos siguientes:</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
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
            <p>Los campos siguientes agregaron el marcador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
            </ul>
          </li>
          <li>
          <p>Los campos siguientes cambiaron su tipo de <code>double</code> a <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>plannedDuration</b></p> <p>Se agregaron las marcas <code>DYNAMIC</code>, <code>LAZY_READ</code> y <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Se ha añadido el indicador <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>Se agregó el valor posible <code>URH</code> (usuario y rol por hora) </li>
          <li><p><b>revenueType</b></p> <p>Se agregaron los valores posibles <code>URH</code> (usuario y rol por hora), <code>URC</code> (usuario y rol por hora sin tope) y <code>URF</code> (usuario y rol por hora más fijos)</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



