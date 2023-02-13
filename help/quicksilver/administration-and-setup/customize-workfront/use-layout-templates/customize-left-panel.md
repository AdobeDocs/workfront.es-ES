---
title: Personalización del panel izquierdo mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En una plantilla de diseño, puede personalizar lo que los usuarios ven en el área del panel izquierdo a través de Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: c0b0102eb1e1f45e794f962f7e905349f9e241eb
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---

# Personalización del panel izquierdo mediante una plantilla de diseño

En una plantilla de diseño, puede personalizar lo que los usuarios ven en el área del panel izquierdo mediante [!DNL Adobe Workfront].

Por ejemplo, puede determinar cuál de los siguientes elementos ven los usuarios en el panel izquierdo cuando ven una tarea:

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>Los cambios realizados en el orden y la visibilidad se reflejan en la aplicación móvil.

Para obtener información sobre plantillas de diseño para grupos, consulte [Creación y modificación de las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> Para realizar estos pasos a nivel de sistema, necesita el nivel de acceso de [!UICONTROL System Administrator].<p>Para realizarlos para un grupo, debe ser administrador de dicho grupo.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalización del panel izquierdo de un área de [!DNL Workfront]:

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Haga clic en la flecha hacia abajo ![](assets/dropdown-arrow.png) under **[!UICONTROL Personalización de lo que ven los usuarios]** y, a continuación, haga clic en el panel izquierdo que desee personalizar.

   >[!NOTE]
   >
   >Para obtener información sobre la variable [!UICONTROL Página principal] en esta lista desplegable, consulte [Personalizar [!UICONTROL Página principal] y [!UICONTROL Resumen] uso de una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md). Para obtener información sobre la opción Listas , consulte [Personalización de filtros, vistas y grupos mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. En el **[!UICONTROL Panel izquierdo]** , realice una de las acciones siguientes para determinar qué verán los usuarios en el panel izquierdo para la opción ([!DNL Workfront] área o tipo de objeto) que haya seleccionado:

   * Show ![](assets/add-secondary-nav-item.png) u ocultar ![](assets/delete-secondary-nav-item.png) elementos. Cualquier elemento sin ![](assets/add-secondary-nav-item.png) o ![](assets/delete-secondary-nav-item.png) no se puede ocultar.

   * Arrastrar elementos ![](assets/move-icon---dots.png) para cambiar su orden en el panel izquierdo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Opción</th> 
      <th>Cuando los usuarios hacen clic en lo siguiente...</th> 
      <th>Verán los elementos del panel izquierdo que elija entre los siguientes:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Project]</td> 
      <td>El nombre de un proyecto</td> 
      <td>[!UICONTROL Tasks], [!UICONTROL Project Details], [!UICONTROL Business Case], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Issues], [!UICONTROL Riss], [!UICONTROL Approvals], [!UICONTROL Baselines], [!UICONTROL Billing Rates], [!UICONTROL Billing Records], UICONTROL Expenses], [!UICONTROL Hours], [!UICONTROL Workload Balancer], [!UICONTROL People], [!UICONTROL Utilization], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic Topic Topic], [!UICONTROL Metrics]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Task]</td> 
      <td>El nombre de una tarea</td> 
      <td> [!UICONTROL Actualizaciones], [!UICONTROL Documents], [!UICONTROL Task Details], [!UICONTROL Subtask], [!UICONTROL Issues], [!UICONTROL Hours], [!UICONTROL Approvals], [!UICONTROL Expenses], [!UICONTROL Predecesors]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Problema]</td> 
      <td>El nombre de un problema</td> 
      <td> [!UICONTROL Actualizaciones], [!UICONTROL Documentos], [!UICONTROL Detalles del problema], [!UICONTROL Hours], [!UICONTROL Aprobaciones]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>El nombre de un portafolio</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Programs], [!UICONTROL Portfolio Details], [!UICONTROL Portfolio], [!UICONTROL Optimization], [!UICONTROL Documents], [!UICONTROL Updates]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>El nombre de un programa</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Program Details], [!UICONTROL Updates], [!UICONTROL Documents]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template]</td> 
      <td>El nombre de una plantilla de proyecto</td> 
      <td>[!UICONTROL Template Tasks], [!UICONTROL Template Details], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Risks], [!UICONTROL Expenses], [!UICONTROL People], [!UICONTROL Approvals], [!UICONTROL Billing Rates], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Routing Rules], Tema de cola UICONTROL], [!UICONTROL Grupo de temas]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template Task]</td> 
      <td>El nombre de una tarea de plantilla</td> 
      <td>[!UICONTROL Actualizaciones], [!UICONTROL Documents], [!UICONTROL Template Task Details], [!UICONTROL Subtasks], [!UICONTROL Expenses], [!UICONTROL Approvals], [!UICONTROL Predecesors]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Registro de facturación]</td> 
      <td>El nombre de un registro de facturación de un proyecto</td> 
      <td>[!UICONTROL Detalles de registro de facturación], [!UICONTROL Horario facturable], [!UICONTROL Gastos facturables], [!UICONTROL Ingresos fijos]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Proyectos]</td> 
      <td>Proyectos <img src="assets/projects-in-main-menu.png"> en el [!UICONTROL menú principal] <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Proyectos]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Solicitudes]</td> 
      <td>El nombre de una solicitud</td> 
      <td>[!UICONTROL Nueva solicitud], [!UICONTROL Solicitudes enviadas], [!UICONTROL Todas las solicitudes], [!UICONTROL Borradores]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tableros]</td> 
      <td>El nombre de un tablero</td> 
      <td>[!UICONTROL Mis tableros], [!UICONTROL Tableros compartidos], [!UICONTROL Todos los tableros]<p><b>NOTA</b>: Si ha creado fichas personalizadas para el área [!UICONTROL Reports] con una plantilla de diseño en [!DNL Adobe Workfront Classic], se muestran en la parte inferior de esta lista. Para los usuarios, se muestran en la parte inferior del panel izquierdo del área [!UICONTROL Tableros].</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Scrum Team]</td> 
      <td>El nombre de un equipo de Scrum</td> 
      <td><p>[!UICONTROL Iterations], [!UICONTROL Current iteration], [!UICONTROL Backlog], [!UICONTROL Workload Balancer], [!UICONTROL Actualizaciones], [!UICONTROL Team Settings]</p> <p><strong>NOTA:</strong> La variable <strong>[!UICONTROL iteración actual]</strong> el elemento solo aparece en el panel izquierdo cuando hay al menos una tarea o problema en la iteración.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Kanban Team]</td> 
      <td>El nombre de un equipo kanban</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Kanban board], [!UICONTROL Backlog], [!UICONTROL Updates], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Waterfall Team]</td> 
      <td>El nombre de un equipo de Waterfall</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Requests], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iteración]</td> 
      <td>El nombre de una iteración</td> 
      <td>[!UICONTROL Stories], [!UICONTROL Issues], [!UICONTROL Story Board], [!UICONTROL Overview], [!UICONTROL Custom Forms], [!UICONTROL Updates] </td> 
     </tr> 
     <!--
      <tr> 
       <td>Company</td> 
       <td>The name of the company</td> 
       <td> <p>People (cannot be hidden), Billing Rates, Custom Forms </p> </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Timesheets</td> 
       <td>The name of the timesheet</td> 
       <td>My Timesheets, Timesheets I Approve, All Timesheets (cannot be hidden) </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Resourcing</td> 
       <td>The name of the resource</td> 
       <td>Planner (cannot be hidden), Workload Balancer, Utilization, Resource Pools </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>User Details</td> 
       <td>____________</td> 
       <td>Details (cannot be hidden), Org Chart, Time Off, Custom Forms </td> 
      </tr>
     --> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Los últimos 3 elementos de la sección **[!UICONTROL Personalización de lo que ven los usuarios]** lista desplegable ([!UICONTROL Listas], [!UICONTROL Inicio y resumen]y [!UICONTROL Marcas]) son para configurar áreas que no sean el panel izquierdo. Para obtener más información, consulte estos artículos:
>   * [Personalización de filtros, vistas y grupos mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
>* [Personalizar [!UICONTROL Página principal] y [!UICONTROL Resumen] uso de una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
* [Brand Adobe [!DNL Workfront] uso de una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)



1. (Opcional) Si desea agregar un elemento del panel izquierdo que se vincule a uno de los tableros de su organización, haga clic en **[!UICONTROL Agregar sección personalizada]**, escriba a **[!UICONTROL Título de sección personalizado]** para el elemento, luego agregue el tablero.

   Los elementos del panel aparecen en la parte inferior del panel izquierdo. Los usuarios ven el título de la sección personalizada que escribe junto al elemento del tablero cuando pasan el ratón por encima del panel izquierdo.

   >[!NOTE]
   Los usuarios pueden agregar elementos de tablero personalizados a su propio panel izquierdo. Al agregar elementos de tablero personalizados en una plantilla de diseño, los elementos se combinan con los suyos, sin sobrescribirlos ni restablecerlos. Esto también ocurre si asigna usuarios a una nueva plantilla de diseño con elementos de tablero personalizados. Para obtener información sobre cómo los usuarios pueden personalizar el panel izquierdo, consulte [Crear fichas o secciones personalizadas](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

   Para obtener información sobre los tableros, consulte [Tableros](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Continúe personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **[!UICONTROL Guardar]**.

   >[!TIP]
   Puede hacer clic en [!UICONTROL Guardar] en cualquier momento para guardar el progreso, siga modificando la plantilla más adelante.
