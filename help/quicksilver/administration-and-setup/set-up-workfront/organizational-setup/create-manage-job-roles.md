---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Crear y administrar roles
description: Como  [!DNL Adobe Workfront] administrador o usuario con acceso administrativo a los roles, puede crear roles que se pueden asignar a usuarios y eliminar roles predeterminados que no sean relevantes para su organización.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 0%

---

# Crear y administrar funciones de trabajo

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como administrador de [!DNL Adobe Workfront] o usuario con acceso administrativo a los roles, puede crear roles que se puedan asignar a los usuarios y eliminar los roles predeterminados que no sean relevantes para su organización. Para obtener información acerca del acceso administrativo en [!DNL Workfront], vea [Conceder acceso administrativo a los usuarios a ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>
   <p>Nuevo: [!UICONTROL Standard]</p>
   <p>O</p>
   <p>Actual: [!UICONTROL plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Acceso administrativo a los roles</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear un rol

Para crear un rol:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en&#x200B; **[!UICONTROL Funciones del puesto].**
1. Haga clic en **[!UICONTROL Nuevo rol].**
1. Configure lo siguiente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre]</td> 
      <td> <p>Indique un nombre para el rol. Este es el nombre que se muestra en todas partes en [!DNL Workfront] donde aparece el campo [!UICONTROL Rol]. </p> <p>Sugerencia: El nombre de un rol puede contener hasta 255 caracteres. Sin embargo, los nombres más largos podrían truncarse en ciertas áreas de [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Descripción]</td> 
      <td>Escriba una descripción para la función que indique lo que tiene de único. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Está Activo]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Seleccione <b>[!UICONTROL Yes]</b> si desea que el rol esté activo y disponible en todas partes en [!DNL Workfront] para asociarlo a usuarios, elementos de trabajo, etc. </p> </li> 
        <li> <p>Seleccione <b>[!UICONTROL No]</b>, si desea que el rol se desactive y no esté disponible para asignarlo a usuarios, elementos de trabajo, etc. </p> </li> 
       </ul> <p><span>Para obtener información sobre cómo desactivar roles, consulte</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Desactivar roles</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Moneda base]</span> </td> 
      <td> <p><span>Es la [!UICONTROL Base Currency], tal como la estableció el administrador de Workfront en el área [!UICONTROL Setup]. Para obtener más información, vea </span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tasas de cambio</a> .</p> <p>Sugerencia: <span>No puede editar la [!UICONTROL Base Currency] en el nivel de rol. Este campo está atenuado y sirve como recordatorio de cuál es la divisa base del sistema.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tasa de costo]</td> 
      <td><p>tarifa de coste por hora del rol. Este valor calcula los costos planificados y reales de las tareas y problemas asociados con la función y, en última instancia, los costos planificados y reales de los proyectos. Introduzca la tasa utilizando la [!UICONTROL Moneda base].</p> 
      <p>Para ver las tasas de costo efectivas por fecha, haga clic en <strong>[!UICONTROL Agregar tasa]</strong>. Introduzca el valor del coste/hora para el período de tiempo y asigne una [!UICONTROL Fecha de inicio] y una [!UICONTROL Fecha de finalización] según sea necesario. La primera tasa de coste no tendrá una fecha de inicio y la última tasa de coste no tendrá una fecha de finalización.</p> <p>Algunas fechas se añaden automáticamente. Por ejemplo, si la primera tasa de coste no tiene una fecha de finalización y agrega una segunda tasa de coste con una fecha de inicio del 1 de mayo de 2023, se agrega una fecha de finalización del 30 de abril de 2023 a la primera tasa de coste para que no haya espacios.</p> <p>Sugerencia: al editar un rol existente, puede seleccionar <strong>Ordenar por fecha de inicio</strong> para ver la fecha de inicio más reciente en la parte superior de la lista de tarifas.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tarifa de facturación] </td> 
      <td><p>tarifa de facturación por hora de la función del puesto. Este valor calcula los ingresos planificados y reales de las tareas y problemas asociados con la función y, en última instancia, los ingresos planificados y reales de los proyectos. Introduzca la tasa utilizando la [!UICONTROL Moneda base].</p> <p>Para ver las tarifas de facturación efectivas por fecha, haga clic en <strong>[!UICONTROL Agregar tarifa]</strong>. Introduzca el valor de facturación/hora para el período de tiempo y asigne una [!UICONTROL Fecha de inicio] y una [!UICONTROL Fecha de finalización] según sea necesario. La primera tarifa de facturación no tendrá fecha de inicio y la última tarifa de facturación no tendrá fecha de finalización.</p> <p>Algunas fechas se añaden automáticamente. Por ejemplo, si la primera tarifa de facturación no tiene una fecha de finalización y agrega una segunda con una fecha de inicio del 1 de mayo de 2023, se agrega una fecha de finalización del 30 de abril de 2023 a la primera tarifa de facturación para que no haya espacios.</p> <p>Sugerencia: al editar un rol existente, puede seleccionar <strong>Ordenar por fecha de inicio</strong> para ver la fecha de inicio más reciente en la parte superior de la lista de tarifas.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Anular moneda]</span> </td> 
      <td>
        <p>Seleccione una divisa asociada a este rol. Esta es la moneda que [!DNL Workfront] usa para calcular los costos e ingresos asociados con este rol. </p> 
        <p><span>Es diferente a la [!UICONTROL Moneda base] configurada por el administrador de [!DNL Workfront] en el área [!UICONTROL Configuración] y puede ser diferente a la moneda asociada a un proyecto.</span> </p> 
        <p>Sugerencia: En este campo solo están disponibles las monedas disponibles en el área [!UICONTROL Exchange Rates] del sistema. Si solo tiene una moneda configurada, este campo no aparece.</p> 
       <p><span>Para obtener información acerca de cómo configurar la [!UICONTROL Moneda base] en [!DNL Workfront], vea</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tasas de cambio</a>.</p> <p><span>Para obtener información acerca de cómo cambiar la moneda de un proyecto, vea</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Cambiar la moneda del proyecto</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Anular tasa de costo de moneda]</span> </td> 
      <td>
        <p>tarifa de coste por hora de la función con la [!UICONTROL Anular moneda] seleccionada. [!DNL Workfront] utiliza este valor para calcular los costos planificados y reales de las tareas y los problemas asociados con el rol. </p> 
        <p><span>Escriba la tarifa en la [!UICONTROL Anular moneda] especificada arriba. Esto también actualiza la tasa de costo para este rol cuando se usa la [!UICONTROL Moneda base].</span> </p> 
        <p>Para obtener información acerca de cómo [!DNL Workfront] calcula el costo, vea <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear costos</a>.</p> 
       <p>Sugerencia: al actualizar un rol existente que ya tiene asociada una tasa de costo, [!DNL Workfront] calcula la tasa de [!UICONTROL Anular moneda] en función de la tasa de conversión del sistema. Si actualiza la [!UICONTROL Anular tasa de coste de divisa], la tasa de coste de la función también se actualiza automáticamente.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Anular tarifa de facturación de moneda]</span> </td> 
      <td>
        <p>Es la tarifa de facturación por hora del rol usando la [!UICONTROL Anular moneda] seleccionada. [!DNL Workfront] utiliza este valor para calcular los ingresos planificados y reales de las tareas y los problemas asociados con el rol. </p>
        <p><span>Escriba la tarifa en la [!UICONTROL Anular moneda] especificada arriba. Esto también actualiza la tarifa de facturación para este rol cuando se usa la [!UICONTROL Moneda base].</span> </p>
        <p>Para obtener información acerca de cómo [!DNL Workfront] calcula los ingresos, vea <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a>.</p>
        <p>Sugerencia: Al actualizar un rol existente que ya tiene asociado un tipo de cambio de facturación, [!DNL Workfront] calcula el tipo de cambio de anulación de divisa en función del tipo de cambio del sistema. Si actualiza la tarifa de facturación de anulación de divisa, la tarifa de facturación de la función de puesto también se actualiza automáticamente. </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Las funciones del puesto son parte integral de la administración de recursos. Para utilizar las herramientas de planificación de recursos, las funciones del puesto necesitan tener asociados un coste y una tasa de facturación. Para obtener más información, consulte [Introducción a la administración de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Haga clic en **[!UICONTROL Crear rol]**. La función ya está disponible para asignarse a tareas, problemas, aprobaciones o puede compartir plantillas de diseño u otros objetos con ella. Para obtener información acerca de todos los usos de los roles en [!DNL Workfront], vea [Descripción general del rol](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Para obtener información acerca de cómo eliminar un rol, vea [Eliminar roles](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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
