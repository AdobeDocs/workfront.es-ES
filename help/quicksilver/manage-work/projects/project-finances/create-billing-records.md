---
navigation-topic: financials
title: Crear registros de facturación
description: Además de configurar los ingresos y rastrear los gastos, puede crear registros de facturación en un proyecto para obtener información que debe facturarse.
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1934'
ht-degree: 1%

---

# Crear registros de facturación

Además de configurar los ingresos y rastrear los gastos, puede crear registros de facturación en un proyecto para obtener información que debe facturarse.

No se pueden crear registros de facturación para tareas. Solo puede crear registros de facturación para proyectos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos y Datos Financieros</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos para el proyecto con permisos para Administrar finanzas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Información general sobre registros de facturación

Los registros de facturación se crean como archivos adjuntos a un proyecto y contienen datos financieros del proyecto, así como información financiera para las tareas de un proyecto.

Tenga en cuenta lo siguiente cuando planifique utilizar registros de facturación:

* Puede crear un registro de facturación si desea facturar una cantidad de dinero relacionada con el proyecto a un proveedor o socio externo. Además de facturar una cantidad fija a un origen externo, hay ocasiones en las que es necesario facturar la cantidad de trabajo en el proyecto (desde horas registradas) a un contratista externo, así como los gastos incurridos o la cantidad de ingresos fijos. Puede incluir toda esta información en el mismo registro de facturación.
* Una vez que un registro de facturación está establecido en Facturado, no se puede editar.

   >[!IMPORTANT]
   >
   >Esto es importante cuando las tasas varían y desea bloquear la información de ingresos y gastos del proyecto. Añadirlo a un registro de facturación y marcarlo como Facturado impide que se actualice cuando las tasas se actualicen en el sistema.

* Un proyecto con registros de facturación marcados como Facturado no se puede eliminar.

## Crear un registro de facturación

1. Vaya a un proyecto.
1. Haga clic en **Registros de facturación** en el panel izquierdo.

   Esta sección puede encontrarse en **Mostrar más**.

1. con **Detalles de registro de facturación** seleccionado en el panel izquierdo, haga clic en **Nuevo registro de facturación**.
1. En el **Nuevo registro de facturación** que se muestra, especifique la siguiente información:

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
      <td> <p>Select <strong>No facturado</strong>, si este registro aún no se ha facturado.</p> <p>Select <strong>Facturado</strong> cuando se factura el registro de facturación.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha de facturación</td> 
      <td>Seleccione la fecha en la que se facturará este registro de facturación haciendo clic en el icono de calendario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nº de orden de compra</td> 
      <td>Si hay un número de orden de compra asociado a este registro de facturación, especifique esta información en este campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Identificador de factura</td> 
      <td>Si hay una Factura asociada a este registro de facturación, especifique esta información en este campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cantidad adicional</td> 
      <td>Introduzca el importe fijo del registro de facturación. Esta es la cantidad que desea facturar a un cliente, contratista o socio externo por este proyecto. Esta cantidad no se puede modificar una vez que el estado del registro de facturación se ha cambiado a Facturado.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) En **Forms personalizado**, seleccione un formulario personalizado de registros de facturación que desee agregar al registro de facturación.

   Usted (u otro usuario con acceso a formularios personalizados) debe crear un formulario personalizado de registros de facturación antes de poder seleccionarlo aquí. En la lista solo aparecen los formularios personalizados activos. Para obtener información sobre la creación de formularios personalizados, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   Puede repetir este paso para agregar otros formularios personalizados que necesite para el registro de facturación.

1. Haga clic en **Guardar.**

   Se crea el registro de facturación. Para incluir Horas facturables, Gastos e Ingresos Fijos en el registro de facturación, siga los pasos descritos en la siguiente subsección.

## Incluir horas facturables, gastos e ingresos fijos en un registro de facturación

* [Incluir horas facturables en un registro de facturación](#include-billable-hours-in-a-billing-record)
* [Incluir gastos facturables en un registro de facturación](#include-billable-expenses-in-a-billing-record)
* [Incluir ingresos fijos en un registro de facturación](#include-fixed-revenues-in-a-billing-record)

### Incluir horas facturables en un registro de facturación {#include-billable-hours-in-a-billing-record}

Puede incluir horas que han iniciado sesión en tareas, problemas o el proyecto en sus registros de facturación.\
Si el usuario que registra las horas o su función de trabajo principal está asociado con una tasa de facturación por hora, los ingresos de estas horas se añaden al registro de facturación.

* [Qué horas se pueden agregar a un registro de facturación](#what-hours-can-be-added-to-a-billing-record)
* [Agregar horas a un registro de facturación](#add-hours-to-a-billing-record)

#### Qué horas se pueden agregar a un registro de facturación {#what-hours-can-be-added-to-a-billing-record}

Puede agregar horas a un registro de facturación cuando se cumplan las siguientes condiciones:

* Las tareas, los problemas o el proyecto tienen horas registradas.
* El tipo de hora de las horas registradas se marca como Recuento como Ingresos.

   Para obtener más información sobre los tipos de hora, consulte el artículo [Administrar tipos de hora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Todas las horas registradas para problemas o para el proyecto se pueden agregar a un registro de facturación si el usuario que registra la hora tiene asociada una tasa de facturación por hora o su función de trabajo principal.
* Si las horas están registradas en una tarea, la tarea debe tener el siguiente tipo de ingresos:

   * El tipo de ingresos no se puede establecer en No facturable.
   * Si el tipo de ingresos se establece en Usuario por hora, el usuario que registre la hora debe tener una tasa de facturación por hora definida en su perfil.
   * Si el tipo de ingresos se establece en Función por hora, la función principal del usuario que registra la hora debe tener una tasa de facturación por hora.

      >[!NOTE]
      >
      >Puede anular las tasas de facturación de las funciones de trabajo en el nivel de proyecto.\
      >Para obtener más información sobre la anulación de las tasas de facturación de funciones de trabajo, consulte la sección &quot;Anulación de las tasas de facturación de funciones de trabajo en el nivel de proyecto&quot; en el artículo [Información general sobre la anulación de la función de trabajo Tasas de facturación y el cálculo de ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* If **Requerir tiempo para ser aprobado para este proyecto** está marcada en Configuración del proyecto, el propietario del proyecto debe aprobar las horas registradas.\
   Para obtener más información sobre la necesidad de aprobar el proyecto en horas, consulte el artículo [Requerir tiempo para ser aprobado para un proyecto](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Agregar horas a un registro de facturación {#add-hours-to-a-billing-record}

Para agregar horas facturables a un registro de facturación:

1. Vaya al proyecto con los registros de facturación.
1. Haga clic en **Registros de facturación** en el panel izquierdo.

   Esta sección puede encontrarse en **Mostrar más**.

1. Haga clic en el **Descripción** de un registro de facturación para abrir el **Detalles de registro de facturación** pestaña .

1. Haga clic en **Horas facturables** en el panel izquierdo.
1. Si hay horas que se podrían incluir en un registro de facturación, haga clic en **Agregar horas**.\
   La variable **Agregar horas facturables** se abre.

   >[!NOTE]
   >
   >Si no hay horas registradas o si las horas registradas no cumplen las condiciones requeridas para ser agregadas a un registro de facturación, la variable **Agregar horas** no se muestra. Para obtener más información sobre las horas que se pueden registrar en un registro de facturación, consulte la sección [Qué horas se pueden agregar a un registro de facturación](#what-hours-can-be-added-to-a-billing-record) en este artículo.

1. Seleccione las entradas de hora que desee incluir en el registro de facturación y haga clic en **Agregar horas**.\
   El costo real de las horas se agrega como la variable **Horas facturables** importe a **Total de registro de facturación**.

1. (Opcional) Haga clic en **Detalles de registros de facturación** para revisar el **Horas facturables** y **Total de registro de facturación** cantidades. También puede ver el total del registro de facturación en el encabezado del registro de facturación.

### Incluir gastos facturables en un registro de facturación {#include-billable-expenses-in-a-billing-record}

Si agrega Gastos Facturables al registro de facturación, asegúrese de que los gastos de las tareas y el proyecto estén marcados como Facturables. Los gastos que no están marcados como Facturables no están disponibles para agregarlos en un registro de facturación. Para obtener más información sobre cómo agregar gastos, consulte el artículo [Administrar los gastos del proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Para agregar gastos facturables a un registro de facturación:

1. Vaya al proyecto con los registros de facturación.
1. Haga clic en **Registros de facturación** en el panel izquierdo.

   Es posible que tenga que hacer clic en **Mostrar más**, luego **Registros de facturación**.

1. Haga clic en el **Descripción** de un registro de facturación para abrir el **Detalles de registro de facturación** pestaña .

1. Haga clic en **Gastos facturables** en el panel izquierdo.
1. (Condicional) Si ha añadido gastos a sus tareas o al proyecto y los ha marcado como Facturables, haga clic en **Agregar gastos**.

   >[!NOTE]
   >
   >Si tiene gastos pero no están marcados como facturables, la variable **Agregar gastos** no se muestra. Solo los gastos facturables con un importe real bueno a cero pueden incluirse en un registro de facturación.

1. Seleccione los gastos facturables disponibles para agregarlos al registro de facturación y haga clic en **Agregar gastos**.\
   La cantidad real de los gastos se agrega como el valor **Gastos facturables** importe a **Total de registro de facturación**.

1. (Opcional) Haga clic en **Detalles de registros de facturación** para revisar el **Gastos facturables** y **Total de registro de facturación** cantidades. También puede ver el total del registro de facturación en el encabezado del registro de facturación.

### Incluir ingresos fijos en un registro de facturación {#include-fixed-revenues-in-a-billing-record}

Puede agregar Ingresos fijos a los registros de facturación si tiene tareas que tengan disponibles Ingresos fijos. No hay otros tipos de ingresos de tareas o proyectos disponibles para agregarlos en un registro de facturación. Para obtener más información sobre los tipos de ingresos, consulte la [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) en [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Para agregar ingresos fijos a un registro de facturación:

1. Vaya al proyecto con los registros de facturación.
1. Haga clic en **Registros de facturación** en el panel izquierdo.

   Es posible que tenga que hacer clic en **Mostrar más**, luego **Registros de facturación**.

1. Haga clic en el **Descripción** de un registro de facturación para abrir el **Detalles de registro de facturación** pestaña .

1. Seleccione el **Ingresos fijos** pestaña .
1. Si ha añadido ingresos fijos a sus tareas, haga clic en **Agregar ingresos fijos**.

   >[!NOTE]
   >
   >Si tiene importes de ingresos en tareas pero no están marcados como &quot;Fijo&quot;, la variable **Agregar ingresos fijos** no se muestra.

1. Seleccione las tareas cuyos ingresos fijos desee incluir en el registro de facturación y haga clic en **Agregar tareas**.\
   La variable **Ingresos fijos** la cantidad de tareas se añade como la variable **Ingresos facturables** importe a **Total de registro de facturación**.

1. (Opcional) Haga clic en **Detalles de registros de facturación** para revisar el **Ingresos facturables** y **Total de registro de facturación** cantidades. También puede ver el total del registro de facturación en el encabezado del registro de facturación.

## Editar un registro de facturación

Después de crear un registro de facturación e incluir horas, gastos e ingresos en el registro de facturación, puede editar información en el registro existente antes de marcarlo como Facturado.

1. Vaya al registro de facturación.
1. con **Detalles de registro de facturación** seleccionado en el panel izquierdo , edite la información en los campos disponibles

   O

   Haga clic en el **Icono Editar** ![](assets/edit-icon.png) en la esquina superior derecha, edite la información en los campos disponibles.

   Actualice lo siguiente:

   * **Descripción**
   * **Estado de facturación**

      >[!TIP]
      >
      >Si selecciona **Facturado** para el estado de facturación, el registro de facturación no se puede editar después de guardar los cambios.

   * **Fecha de facturación**
   * **Nº de orden de compra**
   * **Identificador de factura**
   * **Cantidad adicional**

   Los campos siguientes no están disponibles para la edición:

   * **Horario facturable:** Total de los ingresos reales de las horas incluidas en el registro de facturación. Para obtener más información sobre cómo incluir horas en un registro de facturación, consulte la sección [Incluir horas facturables en un registro de facturación](#include-billable-hours-in-a-billing-record) en este artículo.

   * **Gastos facturables**: El total del importe real de los gastos facturables incluidos en el registro de facturación. Para obtener más información sobre la inclusión de gastos facturables en un registro de facturación, consulte la sección [Incluir gastos facturables en un registro de facturación](#include-billable-expenses-in-a-billing-record) en este artículo.

   * **Ingresos facturables**: Total de los ingresos fijos de las tareas incluidas en el registro de facturación. Para obtener más información sobre la inclusión de ingresos fijos en un registro de facturación, consulte la sección [Incluir ingresos fijos en un registro de facturación](#include-fixed-revenues-in-a-billing-record) en este artículo.

   * **Total de registro de facturación**: Total de las cantidades facturables. Esto se calcula mediante la fórmula siguiente:

      ```
      Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
      ```


1. Haga clic en **Guardar***Cambios**.
