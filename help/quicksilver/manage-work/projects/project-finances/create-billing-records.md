---
navigation-topic: financials
title: Crear registros de facturación
description: Además de configurar los ingresos y llevar el seguimiento de los gastos, puede crear registros de facturación en un proyecto para tener la información de lo que debe facturarse.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '1862'
ht-degree: 98%

---

# Crear registros de facturación

Además de configurar los ingresos y llevar el seguimiento de los gastos, puede crear registros de facturación en un proyecto para tener la información de lo que debe facturarse.

No puede crear registros de facturación para las tareas. Solo puede crear registros de facturación para los proyectos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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

Los registros de facturación se crean como archivos adjuntos a un proyecto y contienen los datos financieros del proyecto, así como información financiera relacionada con las tareas de un proyecto.

Tenga en cuenta lo siguiente cuando planee utilizar registros de facturación:

* Puede crear un registro de facturación cuando desee facturar una cantidad de dinero relacionada con el proyecto a un socio o proveedor externo. Además de facturar una cantidad fija a una fuente externa, hay veces en que necesita facturar la cantidad de trabajo realizado en el proyecto (según las horas registradas) a un contratista externo, así como los gastos incurridos o el importe de ingresos fijos. Puede incluir toda esta información en el mismo registro de facturación.
* Una vez establecido un registro de facturación como Facturado, ya no se puede editar.

  >[!IMPORTANT]
  >
  >Esto es importante cuando las tarifas varían y desea bloquear la información de ingresos y gastos en el proyecto. Añadir esta información a un registro de facturación y marcar ese registro como Facturado impide que se actualice cuando se actualizan las tarifas en el sistema.

* No se pueden eliminar los proyectos con registros de facturación ya marcados como Facturado.

## Crear un registro de facturación

1. Vaya a un proyecto.
1. Haga clic en **Registros de facturación** en el panel izquierdo.
1. Con **Detalles del registro de facturación** seleccionado en el panel izquierdo, haga clic en **Nuevo registro de facturación**.
1. En el cuadro **Nuevo registro de facturación** que aparece, especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Este campo es obligatorio. Especifique una descripción para el registro de facturación que refleje el propósito o la intención de este registro.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estado de facturación</td> 
      <td> <p>Seleccione <strong>No facturado</strong>, si este registro aún no se ha facturado.</p> <p>Seleccione <strong>Facturado</strong> cuando se ha facturado el registro de facturación.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha de facturación</td> 
      <td>Seleccione la fecha de facturación de este registro de facturación, haciendo clic en el icono de calendario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nº de orden de compra</td> 
      <td>Si hay un número de orden de compra asociado a este registro de facturación, especifique esta información en este campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Identificador de factura</td> 
      <td>Si hay una factura asociada a este registro de facturación, especifique esta información en este campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cantidad adicional</td> 
      <td>Introduzca el importe fijo del registro de facturación. Es el importe que desea facturar a un cliente, contratista o socio externo para este proyecto. Este importe no se puede modificar una vez que el estado del registro de facturación se haya cambiado a Facturado.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) En **Formularios personalizados**, seleccione el formulario personalizado de registros de facturación que desee añadir al registro de facturación.

   Usted (u otro usuario con acceso a formularios personalizados) debe crear un formulario personalizado de registros de facturación para poder seleccionarlo aquí. En la lista solo se muestran los formularios personalizados activos. Para obtener información sobre cómo crear formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   Puede repetir este paso para añadir otros formularios personalizados que necesite para el registro de facturación.

1. Haga clic en **Guardar**.

   Se crea el registro de facturación. Para incluir horas facturables, gastos e ingresos fijos en el registro de facturación, siga los pasos que se describen en la siguiente subsección.

## Incluir horas facturables, gastos e ingresos fijos en un registro de facturación

* [Incluir horas facturables en un registro de facturación](#include-billable-hours-in-a-billing-record)
* [Incluir gastos facturables en un registro de facturación](#include-billable-expenses-in-a-billing-record)
* [Incluir ingresos fijos en un registro de facturación](#include-fixed-revenues-in-a-billing-record)

### Incluir horas facturables en un registro de facturación {#include-billable-hours-in-a-billing-record}

Puede incluir horas que se hayan registrado en tareas, problemas o el proyecto en sus registros de facturación.\
Si el usuario que registra las horas o su función principal está asociado a una tarifa de facturación por hora, los ingresos de estas horas se añadirán al registro de facturación.

* [Qué horas se pueden añadir a un registro de facturación](#what-hours-can-be-added-to-a-billing-record)
* [Añadir horas a un registro de facturación](#add-hours-to-a-billing-record)

#### Qué horas se pueden añadir a un registro de facturación {#what-hours-can-be-added-to-a-billing-record}

Puede añadir horas a un registro de facturación cuando se cumplan las siguientes condiciones:

* Las tareas, los problemas o el proyecto tienen horas registradas.
* El tipo de hora de las horas registradas se marca como Contar como ingresos.

  Para obtener más información sobre los tipos de horas, consulte el artículo [Administrar tipos de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Todas las horas registradas para problemas o para el proyecto pueden añadirse a un registro de facturación si el usuario que registra la hora tiene una tarifa de facturación por hora asociada a él o a su función principal.
* Si se registran las horas en una tarea, la tarea debe tener el siguiente tipo de ingresos:

   * El tipo de ingresos no puede establecerse en No facturable.
   * Si el tipo de ingresos se establece en Usuario por hora, el usuario que registre la hora debe tener establecida una tarifa de facturación por hora en su perfil.
   * Si el tipo de ingresos se establece en Función por hora, la función principal del usuario que registra la hora debe tener una tarifa de Facturación por hora.

     >[!NOTE]
     >
     >Puede anular las tarifas de facturación de las funciones a nivel de proyecto.\
     >Para obtener más información sobre cómo anular las tarifas de facturación de funciones, consulte la sección “Anulación de las tarifas de facturación de funciones a nivel de proyecto” en el artículo [Información general sobre cómo anular las tarifas de facturación de funciones y calcular los ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Si **Requerir tiempo para aprobar este proyecto** está marcado en Configuración del proyecto, el propietario del proyecto debe aprobar las horas registradas.\
  Para obtener más información sobre cómo se requiere la aprobación en las horas del proyecto, consulte el artículo [Requerir tiempo de aprobación de un proyecto](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Agregar horas a un registro de facturación {#add-hours-to-a-billing-record}

Para añadir horas facturables a un registro de facturación:

1. Vaya al proyecto con los registros de facturación.
1. Haga clic en **Registros de facturación** en el panel izquierdo.
1. Haga clic en la **Descripción** de un registro de facturación para abrir la pestaña **Detalles del registro de facturación**.
1. Haga clic en **Horas facturables** en el panel de la izquierda.
1. Si hay horas que pudieran incluirse en un registro de facturación, haga clic en **Añadir horas**.\
   Se abre el cuadro **Añadir horas facturables**.

   >[!NOTE]
   >
   >Si no se ha registrado ninguna hora o si las horas registradas no cumplen las condiciones necesarias para añadirse a un registro de facturación, el botón **Añadir horas** no se muestra. Para obtener más información sobre las horas que se pueden registrar en un registro de facturación, consulte la sección [Qué horas se pueden añadir a un registro de facturación](#what-hours-can-be-added-to-a-billing-record) en este artículo.

1. Seleccione las entradas de horas que desea incluir en el registro de facturación y haga clic en **Añadir horas**.\
   El coste real de las horas se añade como la cantidad de **Horas facturables** al **Total del registro de facturación**.

1. (Opcional) Haga clic en **Detalles de registros de facturación** para revisar los importes de **Horas facturables** y **Total del registro de facturación total**. También puede ver el total del registro de facturación en el encabezado del registro de facturación.

### Incluir gastos facturables en un registro de facturación {#include-billable-expenses-in-a-billing-record}

Si va a añadir gastos facturables al registro de facturación, asegúrese de que los gastos de las tareas y el proyecto estén marcados como facturables. Los gastos que no están marcados como Facturable no están disponibles para añadirlos en un registro de facturación. Para obtener más información sobre cómo añadir gastos, consulte el artículo [Administrar gastos dle proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Para añadir gastos facturables a un registro de facturación:

1. Vaya al proyecto con los registros de facturación.
1. Haga clic en **Registros de facturación** en el panel izquierdo.
1. Haga clic en la **Descripción** de un registro de facturación para abrir la pestaña **Detalles del registro de facturación**.
1. Haga clic en **Gastos facturables** en el panel izquierdo.
1. (Condicional) Si ha añadido gastos a las tareas o al proyecto y los ha marcado como Facturable, haga clic en **Añadir gastos**.

   >[!NOTE]
   >
   >Si tiene gastos pero no están marcados como Facturable, el botón **Añadir gastos** no se muestra. Solo los gastos facturables con un importe real mayor que cero pueden incluirse en un registro de facturación.

1. Seleccione los gastos facturables que están disponibles para ser añadidos al registro de facturación y luego haga clic en **Añadir gastos**.\
   El importe real de los gastos se añade como cantidad de **Gastos facturables** al **Total del registro de facturación**.

1. (Opcional) Haga clic en **Detalles del registro de facturación** para revisar las cantidades de **Gastos facturables** y **Total del registro de facturación**. También puede ver el total del registro de facturación en el encabezado del registro de facturación.

### Incluir ingresos fijos en un registro de facturación {#include-fixed-revenues-in-a-billing-record}

Puede añadir Ingresos fijos a los registros de facturación si tiene tareas disponibles con Ingresos fijos. No hay otros tipos de ingresos de tareas o proyectos disponibles para añadir en un registro de facturación. Para obtener más información sobre los tipos de ingresos, consulte la sección [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) en [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Para añadir ingresos fijos a un registro de facturación:

1. Vaya al proyecto con los registros de facturación.
1. Haga clic en **Registros de facturación** en el panel izquierdo.
1. Haga clic en la **Descripción** de un registro de facturación para abrir la pestaña **Detalles del registro de facturación**.
1. Seleccione la pestaña **Ingresos fijos**.
1. Si ha añadido ingresos fijos a sus tareas, haga clic en **Añadir ingresos fijos**.

   >[!NOTE]
   >
   >Si tiene importes de ingresos en tareas pero no están marcados como “Fijo”, el botón **Añadir ingresos fijos** no aparece.

1. Seleccione las tareas cuyos ingresos fijos desee incluir en el registro de facturación y, a continuación, haga clic en **Añadir tareas**.\
   La cantidad de **Ingresos fijos** de las tareas se añade como cantidad de **Ingresos facturables** al **Total del registro de facturación**.

1. (Opcional) Haga clic en **Detalles del registro de facturación** para revisar las cantidades de **Ingresos facturables** y **Total del registro de facturación**. También puede ver el total del registro de facturación en el encabezado del registro de facturación.

## Editar un registro de facturación

Después de crear un registro de facturación e incluir horas, gastos e ingresos en el registro de facturación, puede editar parte de la información del registro existente, antes de que se marque como Facturado.

1. Vaya al registro de facturación.
1. Con **Detalles del registro de facturación** seleccionado en el panel izquierdo, edite la información en cualquier campo disponible

   O

   Haga clic en el **icono Editar** ![Icono Editar](assets/edit-icon.png) en la esquina superior derecha y, a continuación, edite la información en cualquier campo disponible.

   Actualice lo siguiente:

   * **Descripción**
   * **Estado de facturación**

     >[!TIP]
     >
     >Si selecciona **Facturado** como estado de facturación, el registro de facturación no se podrá editar después de guardar los cambios.

   * **Fecha de facturación**
   * **N.º de orden de compra**
   * **Identificador de factura**
   * **Cantidad adicional**

   Los campos siguientes no están disponibles para la edición:

   * **Horas facturables:** el total de los ingresos reales de las horas incluidas en el registro de facturación. Para obtener más información sobre cómo incluir horas en un registro de facturación, consulte la sección [Incluir horas facturables en un registro de facturación](#include-billable-hours-in-a-billing-record) en este artículo.

   * **Gastos facturables**: el total del importe real de los gastos facturables incluidos en el registro de facturación. Para obtener más información sobre cómo incluir los gastos facturables en un registro de facturación, consulte la sección [Incluir gastos facturables en un registro de facturación](#include-billable-expenses-in-a-billing-record) en este artículo.

   * **Ingresos facturables**: el total de los ingresos fijos de las tareas incluidas en el registro de facturación. Para obtener más información acerca de cómo incluir los ingresos fijos en un registro de facturación, consulte la sección [Incluir ingresos fijos en un registro de facturación](#include-fixed-revenues-in-a-billing-record) en este artículo.

   * **Total de registro de facturación**: el total de todas las cantidades facturables. Esto se calcula mediante la fórmula siguiente:

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Haga clic en **Guardar**&#x200B;**cambios**.
