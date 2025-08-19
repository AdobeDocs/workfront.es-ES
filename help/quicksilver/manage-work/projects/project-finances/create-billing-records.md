---
navigation-topic: financials
title: Crear registros de facturación
description: Además de configurar los ingresos y llevar el seguimiento de los gastos, puede crear registros de facturación en un proyecto para tener la información de lo que debe facturarse.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: 4805b93be7ce3dc098c7e160cdb872446f80ecbd
workflow-type: tm+mt
source-wordcount: '1645'
ht-degree: 39%

---

# Crear registros de facturación

<!-- Audited: 6/2025 -->

Además de configurar los ingresos y llevar el seguimiento de los gastos, puede crear registros de facturación en un proyecto para tener la información de lo que debe facturarse.

No puede crear registros de facturación para tareas; sólo puede crear registros de facturación para proyectos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Acceso de edición a proyectos y datos financieros</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Permisos de administración para el proyecto con permisos para administrar finanzas</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Información general de registros de facturación

Los registros de facturación se crean como archivos adjuntos a un proyecto y contienen datos financieros del proyecto, así como información financiera de las tareas del proyecto.

Tenga en cuenta lo siguiente cuando planee utilizar registros de facturación:

* Puede crear un registro de facturación cuando desee facturar una cantidad de dinero relacionada con el proyecto a un socio o proveedor externo. Además de facturar una cantidad fija a una fuente externa, hay veces en que necesita facturar la cantidad de trabajo realizado en el proyecto (según las horas registradas) a un contratista externo, así como los gastos incurridos o el importe de ingresos fijos. Puede incluir toda esta información en el mismo registro de facturación.
* Una vez que un registro de facturación se establece en Facturado, no se puede editar.

  >[!IMPORTANT]
  >
  >Esto es importante cuando las tarifas varían y desea bloquear la información de ingresos y gastos en el proyecto. Añadir esta información a un registro de facturación y marcar ese registro como Facturado impide que se actualice cuando se actualizan las tarifas en el sistema.

* No se puede eliminar un proyecto con registros de facturación que se hayan marcado como Facturado.

## Crear un registro de facturación

{{step1-to-projects}}

1. En la **Página Proyectos** , seleccione un proyecto.
1. Haga clic en **Registros de facturación** en el panel izquierdo.
1. Haga clic en **Nuevo registro** de facturación.
1. En el **cuadro Nuevo facturación registro** que aparece, introduzca la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>(Obligatorio) Introduzca una descripción para el registro de facturación.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estado de facturación</td> 
      <td> <p>Seleccione <strong>No facturado</strong> si aún no se ha facturado este registro.</p> <p>Seleccione <strong>Facturado</strong> si se ha facturado el registro de facturación.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha de facturación</td> 
      <td>Seleccione la fecha en la que se facturó este registro de facturación haciendo clic en el icono de calendario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">N.º de orden de compra</td> 
      <td>Introduzca el número de pedido asociado a este registro de facturación.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Identificador de factura</td> 
      <td>Introduzca la factura asociada a este registro de facturación.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cantidad adicional</td> 
      <td>Introduzca el importe fijo del registro de facturación. Este es el importe que desea facturar a un cliente, contratista o socio externo para este proyecto. Este importe no se puede modificar una vez que el estado del registro de facturación se haya cambiado a Facturado.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) En **Forms personalizado**, seleccione el formulario personalizado de registros de facturación que desee agregar al registro.

   Se debe crear un formulario personalizado de registros de facturación antes de que pueda seleccionarlo aquí. En la lista solo se muestran los formularios personalizados activos. Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Haga clic en **Guardar.**: se ha creado el registro de facturación.

## Incluir horas facturables, gastos e ingresos fijos en un registro de facturación

### Incluir horas facturables en un registro de facturación {#include-billable-hours-in-a-billing-record}

Puede incluir horas que se hayan registrado en tareas, problemas o el proyecto en sus registros de facturación.

Si el usuario que registra las horas o su rol principal está asociado con una tarifa Facturación por hora, los ingresos de estas horas se agregan al registro de facturación.

* [Qué horas se pueden añadir a un registro de facturación](#what-hours-can-be-added-to-a-billing-record)
* [Agregar horas a un registro de facturación](#add-hours-to-a-billing-record)

#### Qué horas se pueden añadir a un registro de facturación {#what-hours-can-be-added-to-a-billing-record}

Puede añadir horas a un registro de facturación cuando se cumplan las siguientes condiciones:

* Se han registrado horas para las tareas, problemas o proyectos.
* El tipo de hora de las horas registradas se marca como Contar como ingresos.

  Para obtener más información, consulte el artículo [Administrar tipos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md) de horas.

* Todas las horas registradas por problemas o el proyecto se pueden agregar a un registro de facturación si el usuario que registra el tiempo tiene una tarifa de facturación por hora asociada con ellos o con su función de trabajo principal.
* Si se registran las horas en una tarea, la tarea debe tener el siguiente tipo de ingresos:

   * El Tipo de ingresos no se puede establecer en No facturable.
   * Si el tipo de ingresos se establece en Usuario por hora, el usuario que registre la hora debe tener establecida una tarifa de facturación por hora en su perfil.
   * Si el Tipo de ingresos se establece en Rol por hora, el función principal del usuario que registra la hora debe tener una tarifa de Facturación por hora.

     >[!NOTE]
     >
     >Puede anular las tarifas de facturación de las funciones a nivel de proyecto.\
     >Para obtener más información, consulte la sección &quot;Anular las tasas de función facturación de trabajo en el nivel de proyecto&quot; en el artículo [Descripción general de anular las tasas de facturación de roles de trabajo y calcular los ingresos de un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Si la opción Requerir tiempo para ser aprobado para este proyecto está seleccionada en Proyecto Configuración, entonces el Propietario del proyecto debe aprobar las horas registradas.\
  Para obtener más información, consulte [Requerir tiempo para ser aprobado para un proyecto](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### añadir horas a un récord facturación {#add-hours-to-a-billing-record}

{{step1-to-projects}}

1. En la página **Proyectos**, seleccione un proyecto.
1. Haga clic en **Registros de facturación** en el panel izquierdo.
1. Haga clic en el registro de facturación **Descripción** para abrir la ficha **Detalles del registro de facturación**.
1. Haga clic en **Horas facturables** en el panel de la izquierda.
1. Si hay horas que podrían incluirse en un registro de facturación, haga clic en **Agregar horas**. Se abre el cuadro **Agregar horas facturables**.

   >[!NOTE]
   >
   >Si no se registran horas o si las horas registradas no cumplen las condiciones necesarias para agregarse a un registro de facturación, el botón **Agregar horas** no se mostrará. Para obtener más información, vea la siguiente sección en este artículo: [Qué horas se pueden agregar a un registro de facturación](#what-hours-can-be-added-to-a-billing-record).

1. Seleccione las entradas de horas que desee incluir en el registro de facturación y luego haga clic en **Agregar horas**. El coste real de las horas se añade como la cantidad de **Horas facturables** al **Total del registro de facturación**.

1. (Opcional) Haga clic en **Detalles de registros de facturación** para revisar los importes de **Horas facturables** y **Registro de facturación total**, y el total del registro de facturación en el encabezado del registro de facturación.

### Incluir gastos facturables en un registro de facturación {#include-billable-expenses-in-a-billing-record}

Si está agregando gastos facturables al registro de facturación, asegúrese de que los gastos de las tareas y el proyecto estén marcados como facturables. Los gastos que no están marcados como Facturable no están disponibles para añadirlos en un registro de facturación. Para obtener más información sobre cómo añadir gastos, consulte el artículo [Administrar gastos dle proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Para añadir gastos facturables a un registro de facturación:

{{step1-to-projects}}

1. En la página **Proyectos**, seleccione un proyecto.
1. Haga clic en **Registros de facturación** en el panel izquierdo.
1. Haga clic en el registro de facturación **Descripción** para abrir la ficha **Detalles del registro de facturación**.
1. Haga clic en **Gastos facturables** en el panel izquierdo.
1. (Condicional) Si has añadido gastos a tus tareas o al proyecto y los has marcado como facturables, haz clic en **añadir gastos**.

   >[!NOTE]
   >
   >Si tiene gastos pero no están marcados como facturables, el botón de gastos **de añadir** no se muestra. Solo los gastos facturables con un importe real mayor que cero pueden incluirse en un registro de facturación.

1. Seleccione los gastos facturables que están disponibles para añadirlos al registro facturación y, a continuación, haga clic en **añadir gastos**.  El importe real de los gastos se añade como cantidad de **Gastos facturables** al **Total del registro de facturación**.

1. (Opcional) Haga clic en **Detalles de registros de facturación** para revisar los importes de **Gastos facturables** y **Registro de facturación total**, y el total del registro de facturación en el encabezado del registro de facturación.

### Incluir ingresos fijos en un registro de facturación {#include-fixed-revenues-in-a-billing-record}

Puede agregar ingresos fijos a los registros de facturación si tiene tareas con ingresos fijos disponibles. No hay disponible ningún otro tipo de ingresos de tarea o proyecto para agregar en un registro de facturación. Para obtener más información acerca de los tipos de ingresos, consulte la sección &quot;Información general sobre facturación e ingresos&quot; en el artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

{{step1-to-projects}}

1. En la página **Proyectos**, seleccione un proyecto.
1. Haga clic en **Registros de facturación** en el panel izquierdo.
1. Haga clic en la **descripción** del registro de facturación para abrir la ficha **Detalles del registro de facturación**.
1. Seleccione la pestaña **Ingresos fijos**.
1. Si ha agregado ingresos fijos a sus tareas, haga clic en **añadir ingresos fijos**.

   >[!NOTE]
   >
   >Si tienes ingresos cantidades en tareas, pero no están marcadas como Fijas, no se mostrarán los **añadir fijos ingresos** botón.

1. Seleccione las tareas cuyos ingresos fijos desee incluir en el registro de facturación y luego haga clic en **Agregar tareas**.  La cantidad de **Ingresos fijos** de las tareas se añade como cantidad de **Ingresos facturables** al **Total del registro de facturación**.

1. (Opcional) Haga clic en **Detalles** de registros de facturación para revisar los importes totales **** de ingresos **facturables y** registro de facturación, así como el total de registro facturación en el encabezado facturación registro.

## Editar un registro de facturación

Después de crear un registro facturación y agregarle horas, gastos e ingresos, puede editar cierta información en el registro existente antes de que se marque como Facturado.

1. Desplácese hasta el registro facturación.
1. Seleccione **Detalles** del registro de facturación en el panel izquierdo.
1. Edite la información en cualquier campo disponible.

   O

   Haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png) en la esquina superior derecha y, a continuación, edite la información en cualquier campo disponible.

   Actualice lo siguiente:

   * **Descripción**
   * **Fecha de facturación**
   * **Estado de facturación**

     >[!TIP]
     >
     >Si seleccionas **Facturado** para el estado de facturación, el registro de facturación no se podrá editar después de guardar los cambios.

   * **Identificador de factura**
   * **N.º de orden de compra**
   * **Cantidad adicional**

   Los campos siguientes no están disponibles para la edición:

   * **Horas facturables:** el total de los ingresos reales de las horas incluidas en el registro de facturación. Para obtener más información, consulte la siguiente sección de este artículo: [Incluir horas facturables en un registro](#include-billable-hours-in-a-billing-record) facturación.

   * **Gastos facturables**: el total del importe real de los gastos facturables incluidos en el registro de facturación. Para obtener más información, vea la siguiente sección de este artículo: [Incluir gastos facturables en un registro de facturación](#include-billable-expenses-in-a-billing-record).

   * **Ingresos facturables**: el total de los ingresos fijos de las tareas incluidas en el registro de facturación. Para obtener más información, consulte la siguiente sección de este artículo: [Incluir ingresos fijos en un registro de facturación](#include-fixed-revenues-in-a-billing-record).

   * **Total de registro de facturación**: el total de todas las cantidades facturables. Esto se calcula mediante la fórmula siguiente:

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Haga clic en **Guardar cambios**.
