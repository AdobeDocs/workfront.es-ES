---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Crear y administrar funciones de trabajo
description: Como [!DNL Adobe Workfront] o un usuario con acceso administrativo a Funciones de trabajo, puede crear funciones de trabajo que se pueden asignar a usuarios y eliminar funciones de trabajo predeterminadas que no sean relevantes para su organización.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# Crear y administrar funciones de trabajo

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como [!DNL Adobe Workfront] o un usuario con acceso administrativo a Funciones de trabajo, puede crear funciones de trabajo que se pueden asignar a usuarios y eliminar funciones de trabajo predeterminadas que no sean relevantes para su organización. Para obtener información sobre el acceso administrativo en [!DNL Workfront], consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a las funciones de trabajo</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Crear una función de trabajo

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y, a continuación, haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en &#x200B; **[!UICONTROL Funciones del trabajo].**
1. Haga clic en **[!UICONTROL Nueva función de trabajo].**
1. Configure lo siguiente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indique un nombre para la función de trabajo. Este es el nombre que aparece en todas partes en [!DNL Workfront] donde se muestra el campo [!UICONTROL Job Role]. </p> <p>Sugerencia: El nombre de una función de trabajo puede contener hasta 255 caracteres. Sin embargo, es posible que los nombres más largos se trunquen en determinadas áreas de [!DNL Workfront]. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Está Activo]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Select <b>[!UICONTROL Sí]</b> si desea que la función esté activa y disponible en todas partes en [!DNL Workfront] para asociarse con usuarios, elementos de trabajo, etc. </p> </li> 
        <li> <p>Select <b>[!UICONTROL No]</b>, si desea desactivar la función y no está disponible para asignarla a usuarios, elementos de trabajo, etc. </p> </li> 
       </ul> <p><span>Para obtener información sobre la desactivación de funciones de trabajo, consulte</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Desactivar funciones de trabajo</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descripción]</td> 
      <td>Escriba una descripción para la función que indique lo que es único sobre ella. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Moneda básica]</span> </td> 
      <td> <p><span>Esta es la [!UICONTROL Base Currency], tal como lo establece el administrador de Workfront en el área [!UICONTROL Setup]. Para obtener más información, consulte</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tipos de cambio</a> .</p> <p>Sugerencia: <span>No puede editar la [!UICONTROL Base Currency] en el nivel de rol de trabajo. Este campo está tenue y sirve como recordatorio de cuál es la moneda base para su sistema.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Costo/ Hora.]</td> 
      <td>Es la tasa de costo por hora de la función de trabajo. Este valor calcula los costes previstos y reales de las tareas y los problemas asociados con la función, y en última instancia los costes previstos y reales de los proyectos. <span>Introduzca la tasa utilizando la [!UICONTROL Base Currency].</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Bill/ Hr.] </td> 
      <td>Es la tasa de facturación por hora de la función de trabajo. Este valor calcula los ingresos previstos y reales de las tareas y los problemas asociados con la función, y en última instancia los ingresos previstos y reales de los proyectos. Introduzca la tasa utilizando la [!UICONTROL Base Currency]. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Anular moneda]</span> </td> 
      <td> 
       <div> 
        <p>Seleccione una moneda asociada a esta función de trabajo. Esta es la moneda que [!DNL Workfront] utiliza para calcular costes e ingresos asociados a esta función de trabajo. </p> 
        <p><span>Es distinto de la [!UICONTROL Base Currency] configurada por su [!DNL Workfront] administrador en el área [!UICONTROL Setup] y puede ser diferente a la moneda asociada a un proyecto.</span> </p> 
        <p>Sugerencia: En este campo solo están disponibles las monedas disponibles en el área [!UICONTROL Exchange Rates] del sistema.</p> 
       </div> <p><span>Para obtener información sobre la configuración de la [!UICONTROL Base Currency] en [!DNL Workfront], consulte</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tipos de cambio</a>.</p> <p><span>Para obtener información sobre cómo cambiar la moneda de un proyecto, consulte</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Cambiar la moneda del proyecto</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Anular costo/hora de moneda]</span> </td> 
      <td> 
       <div> 
        <p>Es la tasa de coste por hora del rol de trabajo que utiliza la [!UICONTROL Override Currency] seleccionada. [!DNL Workfront] utiliza este valor para calcular los costes planificados y reales de las tareas y los problemas asociados a la función de trabajo. </p> 
        <p><span>Introduzca la tasa en la [!UICONTROL Override Currency] especificada arriba. Esto también actualiza la tasa de coste/hora para esta función de trabajo al utilizar la [!UICONTROL Base Currency].</span> </p> 
        <p>Para obtener información sobre cómo [!DNL Workfront] calcula el coste, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> 
       </div> <p>Sugerencia: Al actualizar una función de trabajo existente que ya tiene asociada una tasa de costo/hora, [!DNL Workfront] calcula la tasa de [!UICONTROL Override Currency] en función de la tasa de conversión del sistema. Si actualiza el [!UICONTROL Override Currency Cost/ Hour], el coste/ hora de la función de trabajo también se actualiza automáticamente.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Anular Facturación de Moneda/ Hora]</span> </td> 
      <td> 
       <div> 
        <p>Esta es la tasa de facturación por hora del rol de trabajo utilizando la [!UICONTROL Override Currency] seleccionada. [!DNL Workfront] utiliza este valor para calcular los ingresos previstos y reales de las tareas y los problemas asociados con la función de trabajo. </p> 
        <p><span>Introduzca la tasa en la [!UICONTROL Override Currency] especificada arriba. Esto también actualiza la tasa de facturación/hora para esta función de trabajo al utilizar la [!UICONTROL Base Currency].</span> </p> 
        <p>Para obtener información sobre cómo [!DNL Workfront] calcula los ingresos, consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a>.</p> 
       </div> <p>Sugerencia: Al actualizar una función de trabajo existente que ya tiene asociada una tasa de facturación/hora, [!DNL Workfront] calcula la tasa de cambio de divisa en función de la tasa de conversión del sistema. Si actualiza la Facturación/Hora de Anulación de Moneda, la función Facturación/Hora del trabajo también se actualiza automáticamente. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Las funciones de trabajo son una parte integral de la administración de recursos. Para utilizar las herramientas de planificación de recursos, las funciones de trabajo necesitan una tasa de costo y facturación asociada a ellas. Para obtener más información, consulte [Introducción a la administración de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Haga clic en **[!UICONTROL Crear función de trabajo]**. La función de trabajo ya está disponible para asignarse a tareas, problemas, aprobaciones o puede compartir plantillas de diseño u otros objetos con ella. Para obtener información sobre todos los usos de las funciones de trabajo en [!DNL Workfront], consulte [Información general sobre la función de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Para obtener información sobre cómo eliminar una función de trabajo, consulte [Eliminar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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
