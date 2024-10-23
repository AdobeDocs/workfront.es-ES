---
navigation-topic: financials
title: Crear registros de facturación
description: Además de configurar los ingresos y los gastos de seguimiento, puede crear registros de facturación en un proyecto para la información que debe facturarse.
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1931'
ht-degree: 0%

---

# Crear registros de facturación

Además de configurar los ingresos y los gastos de seguimiento, puede crear registros de facturación en un proyecto para la información que debe facturarse.

No se pueden crear registros de facturación para las tareas. Solo puede crear registros de facturación para proyectos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos y datos financieros</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el proyecto con permisos para Administrar finanzas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Resumen de registros de facturación

Los registros de facturación se crean como archivos adjuntos a un proyecto y contienen datos financieros del proyecto, así como información financiera para las tareas de un proyecto.

Tenga en cuenta lo siguiente cuando planee utilizar registros de facturación:

* Puede crear un registro de facturación cuando desee facturar una cantidad de dinero relacionada con el proyecto a un proveedor o socio externo. Además de facturar una cantidad fija a una fuente externa, hay veces en que necesita facturar la cantidad de trabajo en el proyecto (de horas registradas) a un contratista externo, así como los gastos incurridos o la cantidad de ingresos fijos. Puede incluir toda esta información en el mismo registro de facturación.
* Una vez establecido un registro de facturación como Facturado, no se puede editar.

  >[!IMPORTANT]
  >
  >Esto es importante cuando las tarifas varían y desea bloquear la información de ingresos y gastos en el proyecto. Añadirlo a un registro de facturación y marcarlo como Facturado impide que se actualice cuando se actualizan las tarifas en su sistema.

* No se puede eliminar un proyecto con registros de facturación que se hayan marcado como Facturado.

## Crear un registro de facturación

1. Vaya a un proyecto.
1. Haga clic en **Registros de facturación** en el panel izquierdo.

   Esta sección podría encontrarse en **Mostrar más**.

1. Con **Detalles del registro de facturación** seleccionado en el panel izquierdo, haga clic en **Nuevo registro de facturación**.
1. En el cuadro **Nuevo registro de facturación** que aparece, especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Este campo es obligatorio. Especifique una descripción para el registro de facturación para reflejar el propósito o la intención de este registro.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estado de facturación</td> 
      <td> <p>Seleccione <strong>No facturado</strong>, si este registro aún no se ha facturado.</p> <p>Seleccione <strong>Facturado</strong> cuando se factura el registro de facturación.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha de facturación</td> 
      <td>Seleccione la fecha de facturación de este registro de facturación, haciendo clic en el icono de calendario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nº de orden de compra</td> 
      <td>Si hay un número de pedido asociado a este registro de facturación, especifique esta información en este campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Identificador de factura</td> 
      <td>Si hay una factura asociada a este registro de facturación, especifique esta información en este campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cantidad adicional</td> 
      <td>Introduzca el importe fijo del registro de facturación. Este es el importe que desea facturar a un cliente, contratista o socio externo para este proyecto. Este importe no se puede modificar una vez que el estado del registro de facturación se haya cambiado a Facturado.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) En **Forms personalizado**, seleccione el formulario personalizado de registros de facturación que desee agregar al registro de facturación.

   Usted (u otro usuario con acceso a formularios personalizados) debe crear un formulario personalizado de registros de facturación para poder seleccionarlo aquí. En la lista solo se muestran los formularios personalizados activos. Para obtener información sobre cómo crear formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   Puede repetir este paso para agregar otros formularios personalizados que necesite para el registro de facturación.

1. Haga clic en **Guardar.**

   Se crea el registro de facturación. Para incluir horas facturables, gastos e ingresos fijos en el registro de facturación, siga los pasos descritos en la siguiente subsección.

## Incluir horas facturables, gastos e ingresos fijos en un registro de facturación

* [Incluir horas facturables en un registro de facturación](#include-billable-hours-in-a-billing-record)
* [Incluir gastos facturables en un registro de facturación](#include-billable-expenses-in-a-billing-record)
* [Incluir ingresos fijos en un registro de facturación](#include-fixed-revenues-in-a-billing-record)

### Incluir horas facturables en un registro de facturación {#include-billable-hours-in-a-billing-record}

Puede incluir horas que se han registrado en tareas, problemas o el proyecto en sus registros de facturación.\
Si el usuario que registra las horas o su rol principal está asociado con una tarifa de facturación por hora, los ingresos de estas horas se agregan al registro de facturación.

* [Qué horas se pueden agregar a un registro de facturación](#what-hours-can-be-added-to-a-billing-record)
* [Agregar horas a un registro de facturación](#add-hours-to-a-billing-record)

#### Qué horas se pueden agregar a un registro de facturación {#what-hours-can-be-added-to-a-billing-record}

Puede añadir horas a un registro de facturación cuando se cumplan las siguientes condiciones:

* Las tareas, los problemas o el proyecto tienen horas registradas.
* El tipo de hora de las horas registradas se marca como Contar como Ingresos.

  Para obtener más información acerca de los tipos de horas, vea el artículo [Administrar tipos de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Todas las horas registradas para problemas o para el proyecto pueden agregarse a un registro de facturación si el usuario que registra la hora tiene una tarifa de facturación por hora asociada a él o a su rol principal.
* Si se registran las horas en una tarea, la tarea debe tener el siguiente tipo de ingresos:

   * El tipo de ingresos no puede establecerse en No facturable.
   * Si el Tipo de ingresos se establece en Usuario por hora, el usuario que registre la hora debe tener establecida una tarifa de Facturación por hora en su perfil.
   * Si el Tipo de ingresos se establece en Rol por hora, el Rol principal del usuario que registra la hora debe tener una tarifa de Facturación por hora.

     >[!NOTE]
     >
     >Puede anular las tarifas de facturación de los roles de trabajo en el nivel de proyecto.\
     >Para obtener más información sobre la anulación de tarifas de facturación de rol, consulte la sección &quot;Anulación de tarifas de facturación de rol en el nivel de proyecto&quot; en el artículo [Información general sobre la anulación de tarifas de facturación de rol y el cálculo de ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Si **Requerir tiempo para aprobar este proyecto** está marcado en Configuración del proyecto, el propietario del proyecto debe aprobar las horas registradas.\
  Para obtener más información acerca de cómo se requiere aprobación en las horas del proyecto, vea el artículo [Requerir tiempo para aprobar un proyecto](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Agregar horas a un registro de facturación {#add-hours-to-a-billing-record}

Para agregar horas facturables a un registro de facturación:

1. Vaya al proyecto con los registros de facturación.
1. Haga clic en **Registros de facturación** en el panel izquierdo.

   Esta sección podría encontrarse en **Mostrar más**.

1. Haga clic en la **descripción** de un registro de facturación para abrir la pestaña **Detalles del registro de facturación**.

1. Haga clic en **Horas facturables** en el panel izquierdo.
1. Si hay horas que podrían incluirse en un registro de facturación, haga clic en **Agregar horas**.\
   Se abre el cuadro **Agregar horas facturables**.

   >[!NOTE]
   >
   >Si no se ha registrado ninguna hora o si las horas registradas no cumplen las condiciones necesarias para agregarse a un registro de facturación, el botón **Agregar horas** no se muestra. Para obtener más información sobre las horas que se pueden registrar en un registro de facturación, consulte la sección [Qué horas se pueden agregar a un registro de facturación](#what-hours-can-be-added-to-a-billing-record) en este artículo.

1. Seleccione las entradas de horas que desee incluir en el registro de facturación y haga clic en **Agregar horas**.\
   El costo real de las horas se agrega como la cantidad de **horas facturables** al **Total del registro de facturación**.

1. (Opcional) Haga clic en **Detalles de registros de facturación** para revisar los importes de **Horas facturables** y **Registro de facturación total**. También puede ver el total del registro de facturación en el encabezado del registro de facturación.

### Incluir gastos facturables en un registro de facturación {#include-billable-expenses-in-a-billing-record}

Si está agregando gastos facturables al registro de facturación, asegúrese de que los gastos de las tareas y el proyecto estén marcados como facturables. Los gastos que no están marcados como facturables no están disponibles para agregar en un registro de facturación. Para obtener más información sobre cómo agregar gastos, consulte el artículo [Administrar gastos de proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Para agregar gastos facturables a un registro de facturación:

1. Vaya al proyecto con los registros de facturación.
1. Haga clic en **Registros de facturación** en el panel izquierdo.

   Es posible que tenga que hacer clic en **Mostrar más** y luego en **Registros de facturación**.

1. Haga clic en la **descripción** de un registro de facturación para abrir la pestaña **Detalles del registro de facturación**.

1. Haga clic en **Gastos facturables** en el panel izquierdo.
1. (Condicional) Si ha agregado gastos a las tareas o al proyecto y los ha marcado como facturables, haga clic en **Agregar gastos**.

   >[!NOTE]
   >
   >Si tiene gastos pero no se han marcado como facturables, el botón **Agregar gastos** no se muestra. Solo los gastos facturables con un importe real mayor que cero pueden incluirse en un registro de facturación.

1. Seleccione los gastos facturables que están disponibles para ser agregados al registro de facturación, luego haga clic en **Agregar gastos**.\
   El monto real de los gastos se agrega como la cantidad de **gastos facturables** al **Total de registro de facturación**.

1. (Opcional) Haga clic en **Detalles de registros de facturación** para revisar las cantidades de **Gastos facturables** y **Registro de facturación total**. También puede ver el total del registro de facturación en el encabezado del registro de facturación.

### Incluir ingresos fijos en un registro de facturación {#include-fixed-revenues-in-a-billing-record}

Puede agregar Ingresos fijos a los registros de facturación si tiene tareas disponibles con Ingresos fijos. No hay otros tipos de ingresos de tareas o proyectos disponibles para agregarse en un registro de facturación. Para obtener más información sobre los tipos de ingresos, consulte la sección [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) en [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Para agregar ingresos fijos a un registro de facturación:

1. Vaya al proyecto con los registros de facturación.
1. Haga clic en **Registros de facturación** en el panel izquierdo.

   Es posible que tenga que hacer clic en **Mostrar más** y luego en **Registros de facturación**.

1. Haga clic en la **descripción** de un registro de facturación para abrir la pestaña **Detalles del registro de facturación**.

1. Seleccione la ficha **Ingresos fijos**.
1. Si ha agregado ingresos fijos a sus tareas, haga clic en **Agregar ingresos fijos**.

   >[!NOTE]
   >
   >Si tiene importes de ingresos en tareas pero no están marcados como &quot;Fijo&quot;, no aparece el botón **Agregar ingresos fijos**.

1. Seleccione las tareas cuyos ingresos fijos desee incluir en el registro de facturación y luego haga clic en **Agregar tareas**.\
   La cantidad de **Ingresos fijos** de las tareas se agrega como la cantidad de **Ingresos facturables** al **Total de registro de facturación**.

1. (Opcional) Haga clic en **Detalles de registros de facturación** para revisar los **ingresos facturables** y los **importes totales de registros de facturación**. También puede ver el total del registro de facturación en el encabezado del registro de facturación.

## Editar un registro de facturación

Después de crear un registro de facturación e incluir horas, gastos e ingresos en el registro de facturación, puede editar parte de la información del registro existente, antes de que se marque como Facturado.

1. Vaya al registro de facturación.
1. Con **Detalles del registro de facturación** seleccionado en el panel izquierdo, edite la información en cualquier campo disponible

   O

   Haga clic en el **icono Editar** ![](assets/edit-icon.png) en la esquina superior derecha y, a continuación, edite la información en cualquier campo disponible.

   Actualice lo siguiente:

   * **Descripción**
   * **Estado de facturación**

     >[!TIP]
     >
     >Si selecciona **Facturado** para el estado de facturación, el registro de facturación no se podrá editar después de guardar los cambios.

   * **Fecha de facturación**
   * **Número de PC**
   * **Id. de factura**
   * **Importe adicional**

   Los campos siguientes no están disponibles para la edición:

   * **Horas facturables:** El total de los ingresos reales de las horas incluidas en el registro de facturación. Para obtener más información acerca de cómo incluir horas en un registro de facturación, consulte la sección [Incluir horas facturables en un registro de facturación](#include-billable-hours-in-a-billing-record) en este artículo.

   * **Gastos facturables**: El total del importe real de los gastos facturables incluidos en el registro de facturación. Para obtener más información acerca de cómo incluir los gastos facturables en un registro de facturación, consulte la sección [Incluir gastos facturables en un registro de facturación](#include-billable-expenses-in-a-billing-record) en este artículo.

   * **Ingresos facturables**: El total de los ingresos fijos de las tareas incluidas en el registro de facturación. Para obtener más información acerca de cómo incluir los ingresos fijos en un registro de facturación, vea la sección [Incluir ingresos fijos en un registro de facturación](#include-fixed-revenues-in-a-billing-record) en este artículo.

   * **Total de registro de facturación**: El total de todos los importes facturables. Esto se calcula mediante la fórmula siguiente:

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Haga clic en **Guardar****Cambios**.
