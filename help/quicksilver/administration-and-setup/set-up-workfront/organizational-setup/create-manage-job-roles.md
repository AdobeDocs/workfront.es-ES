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
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 99%

---

# Crear y administrar funciones de trabajo

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

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
1. Configure lo siguiente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indique un nombre para la función. Este es el nombre que se muestra en todas partes en [!DNL Workfront] donde aparece el campo [!UICONTROL Job Role]. </p> <p>Sugerencia: el nombre de una función puede contener hasta 255 caracteres. Sin embargo, los nombres más largos podrían truncarse en ciertas áreas de [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Escriba una descripción de la función que indique lo que la hace única. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Seleccione <b>[!UICONTROL Yes]</b> si desea que la función esté activa y disponible en todas partes en [!DNL Workfront] para asociarla a usuarios, elementos de trabajo, etc. </p> </li> 
        <li> <p>Seleccione <b>[!UICONTROL No]</b>, si desea que la función se desactive y no esté disponible para que se asigne a usuarios, elementos de trabajo, etc. </p> </li> 
       </ul> <p><span>Para obtener información sobre cómo desactivar funciones, consulte</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Desactivar funciones</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>Esta es la [!UICONTROL Base Currency], tal como la estableció el administrador de Workfront en el área [!UICONTROL Setup]. Para obtener más información, consulte</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tipos de cambio</a> .</p> <p>Sugerencia: <span>No puede editar la [!UICONTROL Base Currency] en el nivel de función. Este campo está atenuado y sirve como recordatorio de cuál es la divisa base del sistema.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>Esta es la tarifa de coste por hora de la función. Este valor calcula los costes planificados y reales de las tareas y problemas asociados con la función y, en última instancia, los costes planificados y reales de los proyectos. Introduzca la tarifa utilizando la [!UICONTROL Base Currency].</p> 
      <p>Para ver las tarifas de coste de fecha efectiva, haga clic en <strong>[!UICONTROL Add Rate]</strong>.  Introduzca el valor del coste u hora para el período de tiempo y asigne una [!UICONTROL Start Date] y una [!UICONTROL End Date] según sea necesario. La primera tarifa de coste no tendrá una fecha de inicio y la última tarifa de coste no tendrá una fecha de finalización.</p> <p>Algunas fechas se añaden automáticamente. Por ejemplo, si la primera tarifa de coste no tiene una fecha de finalización y añade una segunda tarifa de coste con una fecha de inicio del 1 de mayo de 2023, se añade una fecha de finalización del 30 de abril de 2023 a la primera tarifa de coste para que no haya huecos.</p> <p>Sugerencia: al editar una función existente, puede seleccionar <strong>Ordenar por fecha de inicio</strong> para ver la fecha de inicio más reciente en la parte superior de la lista de tarifas.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>Esta es la tarifa de facturación por hora de la función. Este valor calcula los ingresos planificados y reales de las tareas y los problemas asociados a la función, y, en última instancia, los ingresos planificados y reales de los proyectos. Introduzca la tarifa utilizando la [!UICONTROL Base Currency].</p> <p>Para ver las tarifas de facturación efectivas por fecha, haga clic en <strong>[!UICONTROL Add Rate]</strong>. Introduzca el valor de facturación/hora para el período de tiempo y asigne una [!UICONTROL Start Date] y una [!UICONTROL End Date] según sea necesario. La primera tarifa de facturación no tendrá fecha de inicio y la última tarifa de facturación no tendrá fecha de finalización.</p> <p>Algunas fechas se añaden automáticamente. Por ejemplo, si la primera tarifa de facturación no tiene una fecha de finalización y añade una segunda con una fecha de inicio del 1 de mayo de 2023, se añade una fecha de finalización del 30 de abril de 2023 a la primera tarifa de facturación para que no existan huecos.</p> <p>Sugerencia: al editar una función existente, puede seleccionar <strong>Ordenar por fecha de inicio</strong> para ver la fecha de inicio más reciente en la parte superior de la lista de tarifas.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Seleccione una divisa asociada a esta función. Esta es la moneda que [!DNL Workfront] utiliza para calcular los costes e ingresos asociados con esta función. </p> 
        <p><span>Es diferente a la [!UICONTROL Base Currency] configurada por el administrador de [!DNL Workfront] en el área [!UICONTROL Setup] y puede ser diferente a la divisa asociada a un proyecto.</span> </p> 
        <p>Sugerencia: en este campo solo están disponibles las divisas disponibles en el área [!UICONTROL Exchange Rates] del sistema. Si solo tiene una divisa configurada, este campo no aparece.</p> 
       <p><span>Para obtener información acerca de cómo configurar la [!UICONTROL Base Currency] en [!DNL Workfront], consulte</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tipos de cambio</a>.</p> <p><span>Para obtener información acerca de cómo cambiar la divisa de un proyecto, consulte</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Cambiar la divisa del proyecto</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>Este es el coste por hora de la función con la [!UICONTROL Override Currency] seleccionada. [!DNL Workfront] utiliza este valor para calcular los costes planificados y reales de las tareas y los problemas asociados con la función. </p> 
        <p><span>Escriba la tarifa en la [!UICONTROL Override Currency] especificada más arriba. Esto también actualiza la tarifa de coste para esta función cuando se usa la [!UICONTROL Base Currency].</span> </p> 
        <p>Para obtener información acerca de cómo [!DNL Workfront] calcula el coste, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> 
       <p>Sugerencia: al actualizar una función existente que ya tiene asociada una tarifa de coste, [!DNL Workfront] calcula la tasa de [!UICONTROL Override Currency] en función de la tasa de conversión del sistema. Si actualiza la [!UICONTROL Override Currency Cost Rate], la tarifa de coste de la función también se actualiza automáticamente.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>Es la tarifa de facturación por hora de la función usando la [!UICONTROL Override Currency] seleccionada. [!DNL Workfront] utiliza este valor para calcular los ingresos planificados y reales de las tareas y los problemas asociados con la función. </p>
        <p><span>Escriba la tarifa en la [!UICONTROL Override Currency] especificada más arriba. Esto también actualiza la tarifa de facturación para esta función cuando se usa la [!UICONTROL Base Currency].</span> </p>
        <p>Para obtener información acerca de cómo [!DNL Workfront] calcula los ingresos, consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a>.</p>
        <p>Sugerencia: al actualizar una función existente que ya tiene asociado un tipo de cambio de facturación, [!DNL Workfront] calcula el tipo de cambio de anulación de divisa en función de la tasa de conversión del sistema. Si actualiza la tarifa de facturación de anulación de divisa, la tarifa de facturación de la función también se actualiza automáticamente. </p>
       </td>
     </tr> 
    </tbody> 
   </table>

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
