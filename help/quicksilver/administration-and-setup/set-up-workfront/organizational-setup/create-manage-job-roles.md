---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Crear y administrar roles
description: Como [!DNL Adobe Workfront] administrador o usuario con acceso administrativo a las funciones, puede crear funciones que se pueden asignar a usuarios y eliminar funciones predeterminadas que no sean relevantes para su organización.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: d342df9949eb1434acbb53c29b7e329dd91c9b28
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 39%

---

# Crear y administrar funciones de trabajo

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>Con la versión 25.11, la moneda de anulación para los roles de trabajo quedará obsoleta en Producción. (La obsolescencia se producirá el 30 de octubre en el entorno de vista previa). En lugar de tener una divisa base y divisas de sustitución, habrá una divisa disponible para los roles de trabajo y las tarifas de coste y facturación se definirán en esa divisa.

Como administrador de [!DNL Adobe Workfront] o usuario con acceso administrativo a las funciones, puede crear funciones que se puedan asignar a los usuarios y eliminar las funciones predeterminadas que no sean relevantes para su organización. Para obtener información acerca del acceso administrativo en [!DNL Workfront], consulte [Conceder acceso administrativo a los usuarios a ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Acceso administrativo a los roles</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de una función

Para crear una función:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Funciones].**
1. Haga clic en **[!UICONTROL Nueva función].**
1. Configure los campos siguientes:

   * **Nombre**: indique un nombre para el rol. Este es el nombre que se muestra en todas las partes de Workfront donde aparece el campo Rol.

     >[!TIP]
     >
     >El nombre de un rol puede contener hasta 255 caracteres. Sin embargo, los nombres más largos pueden truncarse en determinadas áreas de Workfront.

   * **Descripción**: escriba una descripción para el rol que indique lo que tiene de único.
   * **Está activo**: seleccione **Sí** si desea que el rol esté activo y disponible en cualquier lugar de Workfront para asociarlo a usuarios, elementos de trabajo, etc. Seleccione **No** si desea que el rol se desactive y no esté disponible para asignarlo a usuarios, elementos de trabajo, etc.

     Para obtener información sobre cómo desactivar roles, consulte [Desactivación de funciones](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

   * **Moneda base**: Esta es la Moneda base, tal como la estableció el administrador de Workfront en el área de Configuración. Para obtener más información, consulte [Configuración de tipos de cambio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     >[!TIP]
     >
     >No puede editar la divisa base en el nivel de rol. Este campo aparece atenuado y sirve como recordatorio de cuál es la divisa base del sistema.

   * **Tasa de costo**: Es la tasa de costo por hora del rol. Este valor calcula los costes planificados y reales de las tareas y problemas asociados con la función y, en última instancia, los costes planificados y reales de los proyectos. Introduzca el tipo de cambio utilizando la divisa base.

     Para ver las tarifas de coste efectivas por fecha, haga clic en **Añadir tarifa**. Introduzca el valor del coste/hora para el período de tiempo y asigne una fecha de inicio y una fecha de finalización según sea necesario. La primera tarifa de coste no tendrá una fecha de inicio y la última tarifa de coste no tendrá una fecha de finalización.

     Algunas fechas se añaden automáticamente. Por ejemplo, si la primera tarifa de coste no tiene una fecha de finalización y añade una segunda tarifa de coste con una fecha de inicio del viernes, 01 de mayo de 2025, se añade una fecha de finalización del jueves, 30 de abril de 2025 a la primera tarifa de coste para que no haya huecos.

     >[!TIP]
     >
     >Al editar un rol existente, puede seleccionar **Ordenar por fecha de inicio** para ver la fecha de inicio más reciente en la parte superior de la lista de tarifas.

   * **Tarifa de facturación**: Es la tarifa de facturación por hora del rol. Este valor calcula los ingresos planificados y reales de las tareas y los problemas asociados a la función, y, en última instancia, los ingresos planificados y reales de los proyectos. Introduzca el tipo de cambio utilizando la divisa base.

     Para ver las tarifas de facturación vigentes por fecha, haga clic en **Añadir tarifa**. Introduzca el valor de la facturación/hora para el período de tiempo y asigne una Fecha de inicio y una Fecha de finalización según sea necesario. La primera tarifa de facturación no tendrá fecha de inicio y la última tarifa de facturación no tendrá fecha de finalización.

     Algunas fechas se añaden automáticamente. Por ejemplo, si la primera tarifa de facturación no tiene una fecha de finalización y añade una segunda con una fecha de inicio del viernes, 01 de mayo de 2025, se añade una fecha de finalización del jueves, 30 de abril de 2025 a la primera tarifa de facturación para que no existan huecos.

     >[!TIP]
     >
     >Al editar un rol existente, puede seleccionar **Ordenar por fecha de inicio** para ver la fecha de inicio más reciente en la parte superior de la lista de tarifas.

   * **Anular moneda**: seleccione una moneda asociada con este rol. Esta es la divisa que utiliza Workfront para calcular los costes y los ingresos asociados con este rol.

     Es diferente a la Moneda base configurada por el administrador de Workfront en el área de Configuración y puede ser diferente a la moneda asociada a un proyecto.

     >[!TIP]
     >
     >En este campo sólo están disponibles las divisas disponibles en el área Tasas de cambio del sistema. Si solo tiene una divisa configurada, este campo no aparece.

     Para obtener información sobre cómo configurar la divisa base en Workfront, consulte [Configurar tasas de cambio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     Para obtener información acerca de cómo cambiar la moneda de un proyecto, vea [Cambiar la moneda del proyecto](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

   * **Anular tarifa de costo de moneda**: tarifa de costo por hora del rol que usa la moneda de anulación seleccionada. Workfront utiliza este valor para calcular los costos planificados y reales de las tareas y los problemas asociados con el rol.

     Introduzca el tipo de cambio en la divisa de anulación especificada arriba. Esto también actualiza la tasa de coste para este rol cuando se utiliza la divisa base.

     Para obtener información acerca de cómo Workfront calcula los costos, vea [Rastrear costos](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >Al actualizar un rol existente que ya tiene una tasa de coste asociada, Workfront calcula la tasa de anulación de moneda en función de la tasa de conversión del sistema. Si actualiza el Ratio de Coste de Divisa de Sustitución, el ratio de coste del rol también se actualiza automáticamente.

   * **Anular tarifa de facturación de moneda**: Esta es la tarifa de facturación por hora del rol que usa la moneda de anulación seleccionada. Workfront utiliza este valor para calcular los ingresos planificados y reales de las tareas y los problemas asociados con la función del puesto.

     Introduzca el tipo de cambio en la divisa de anulación especificada arriba. Esto también actualiza la tarifa de facturación para este rol al usar la divisa base.

     Para obtener información sobre cómo Workfront calcula los ingresos, consulte [Información general sobre facturación e ingresos](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >Al actualizar un rol existente que ya tiene una tasa de facturación asociada, Workfront calcula la tasa de anulación de moneda en función de la tasa de conversión del sistema. Si actualiza la tarifa de facturación de anulación de divisa, la tarifa de facturación del rol también se actualiza automáticamente.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indicate a name for the job role. This is the name that displays everywhere in [!DNL Workfront] where the [!UICONTROL Job Role] field displays. </p> <p>Tip: The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Enter a description for the role that indicates what is unique about it. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Select <b>[!UICONTROL Yes]</b> if you want the role to be active and available everywhere in [!DNL Workfront] to be associated with users, work items, etc. </p> </li> 
        <li> <p>Select <b>[!UICONTROL No]</b>, if you want the role to be deactivated and not available to assign to users, work items, etc. </p> </li> 
       </ul> <p><span>For information about deactivating job roles, see</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Deactivate job roles</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>This is the [!UICONTROL Base Currency], as set in the [!UICONTROL Setup] area by your Workfront administrator. For information, see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a> .</p> <p>Tip: <span>You cannot edit the [!UICONTROL Base Currency] at the job role level. This field is dimmed and serves as a reminder for what the base currency is for your system.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> 
      <p>For date effective cost rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the cost/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first cost rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> <p>For date effective billing rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the billing/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first billing rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Select a currency associated with this job role. This is the currency that [!DNL Workfront] uses for calculating costs and revenue associated with this job role. </p> 
        <p><span>This is different than the [!UICONTROL Base Currency] set up by your [!DNL Workfront] administrator in the [!UICONTROL Setup] area, and can be different than the currency associated with a project.</span> </p> 
        <p>Tip: Only currencies available in the [!UICONTROL Exchange Rates] area in your system are available in this field. If you only have one currency set up, this field is does not appear.</p> 
       <p><span>For information about setting up the [!UICONTROL Base Currency] in [!DNL Workfront], see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> <p><span>For information about changing the currency of a project, see</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Change the project currency</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>This is the cost per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role. </p> 
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Cost Rate for this job role when using the [!UICONTROL Base Currency].</span> </p> 
        <p>For information about how [!DNL Workfront] calculates cost, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> 
       <p>Tip: When updating an existing job role that already has a Cost Rate associated with it, [!DNL Workfront] calculates the [!UICONTROL Override Currency] rate based on the conversion rate in your system. If you update the [!UICONTROL Override Currency Cost Rate], the Cost Rate of the job role also updates automatically.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>This is the billing per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role. </p>
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Billing Rateate for this job role when using the [!UICONTROL Base Currency].</span> </p>
        <p>For information about how [!DNL Workfront] calculates revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p>
        <p>Tip: When updating an existing job role that already has a Billing Rate associated with it, [!DNL Workfront] calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the Billing Rate of the job role also updates automatically. </p>
       </td>
     </tr> 
    </tbody> 
   </table>
-->

>[!TIP]
>
>Las funciones son parte integral de la administración de recursos. Para utilizar las herramientas de planificación de recursos, las funciones necesitan tener asociados un coste y una tasa de facturación. Para obtener más información, consulte [Introducción a la administración de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Haga clic en **[!UICONTROL Crear función]**. La función ya está disponible para asignarse a tareas, problemas, aprobaciones o puede compartir plantillas de diseño u otros objetos con ella. Para obtener información acerca de todos los usos de las funciones en [!DNL Workfront], consulte [Información general de la función](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Para obtener información acerca de cómo eliminar una función, consulte [Eliminar funciones](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete a job role</h2>
<ol data-mc-continue="false">
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <strong>Setup</strong> <img src="assets/gear-icon-settings.png">.</li>
<li value="2">Click<strong>Job Roles.</strong></li>
<li value="3">Select the job role that you want to delete, then click <strong>Delete.</strong></li>
<li value="4">If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following:<br>
<ul>
<li><p><strong>Replace the job role with a different job role:</strong> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li>
<li><p><strong>Delete the job role and its resource allocation:</strong> Select<strong>None</strong> from the drop-down list.</p><note type="important">
Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
</note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li>
</ul></li>
<li value="5">Click  <strong>Yes, Delete It</strong>. </li>
</ol>
</div>
-->
