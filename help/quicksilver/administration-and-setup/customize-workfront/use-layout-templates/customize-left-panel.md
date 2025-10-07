---
title: Personalizar el panel izquierdo con una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En una plantilla de diseño, puede personalizar lo que los usuarios ven en el área del panel izquierdo a través de Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: 58567104d88e7e1363d4196aec8a36ee0566b95a
workflow-type: tm+mt
source-wordcount: '1120'
ht-degree: 52%

---

# Personalizar el panel izquierdo con una plantilla de diseño

<!--Audited: 10/2024-->

En una plantilla de diseño, puede personalizar lo que los usuarios ven en el área del panel izquierdo en [!DNL Adobe Workfront].

Por ejemplo, puede determinar cuál de los siguientes elementos ven los usuarios en el panel izquierdo al ver un proyecto:

![Panel izquierdo de un proyecto](assets/left-panel-in-project.png)

>[!IMPORTANT]
>
>Los cambios realizados en el orden y la visibilidad se reflejan en la aplicación móvil.

Para obtener información sobre cómo crear plantillas de diseño, consulte [Crear y administrar plantillas de diseño](../use-layout-templates/create-and-manage-layout-templates.md).

Para obtener información acerca de las plantillas de diseño para grupos, consulte [Creación y modificación de las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Después de configurar una plantilla de diseño, debe asignarla a usuarios para que los cambios que ha realizado sean visibles para otros. Para obtener información acerca de cómo asignar una plantilla de diseño a los usuarios, consulte [Asignar usuarios a una plantilla de diseño](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td><p>Cualquiera</p>
   <p>Añadir aplicaciones personalizadas al menú principal solo está disponible para organizaciones con licencia para Adobe App Builder.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td><p>Nuevo: estándar</p>
  <p> Actual: plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.
Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar en el panel de navegación izquierdo de un área de [!DNL Workfront]:

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Haga clic en la flecha abajo ![Flecha abajo](assets/dropdown-arrow.png) bajo **[!UICONTROL Personalice lo que ven los usuarios]** y, a continuación, haga clic en el nombre de un tipo de objeto o un área [!DNL Workfront] cuyo panel izquierdo desee personalizar.

   Los tipos de objeto y las áreas [!DNL Workfront] cuyo panel izquierdo se puede personalizar se enumeran en la siguiente tabla:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Tipo de objeto o área [!DNL Workfront]</th> 
      <th>Cuando los usuarios hagan clic en lo siguiente…</th> 
      <th>Secciones del panel izquierdo que los usuarios ven después de mostrarlas en la plantilla de diseño:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Project]</td> 
      <td>El nombre de un proyecto</td> 
      <td>[!UICONTROL Tareas], [!UICONTROL Detalles del proyecto], [!UICONTROL Caso comercial], [!UICONTROL Actualizaciones], [!UICONTROL Documentos], [!UICONTROL Problemas], [!UICONTROL Riesgos], [!UICONTROL Aprobaciones], [!UICONTROL Líneas bases], [!UICONTROL Tasas de facturación], [!UICONTROL Registros de facturación], [!UICONTROL Gastos], [!UICONTROL Horas], [!UICONTROL Distribuidor de cargas de trabajo], [!UICONTROL Personas], [!UICONTROL Utilización], [!UICONTROL Detalles de cola], [!UICONTROL Reglas de enrutamiento], [!UICONTROL Tema de cola], [!UICONTROL Grupo de temas], [!UICONTROL Métricas], [!UICONTROL Planificación]*, [!UICONTROL Aplicación personalizada]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Task]</td> 
      <td>Nombre de una tarea</td> 
      <td> [!UICONTROL Actualizaciones], [!UICONTROL Documentos], [!UICONTROL Detalles de tareas], [!UICONTROL Subtarea], [!UICONTROL Problemas], [!UICONTROL Horas], [!UICONTROL Aprobaciones], [!UICONTROL Gastos], [!UICONTROL Predecesores], [!UICONTROL Aplicación personalizada]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Issue]</td> 
      <td>El nombre de un problema</td> 
      <td> [!UICONTROL Actualizaciones], [!UICONTROL Documentos], [!UICONTROL Detalles del problema], [!UICONTROL Horas], [!UICONTROL Aprobaciones], [!UICONTROL Aplicación personalizada]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>El nombre de un portafolio</td> 
      <td>[!UICONTROL Proyectos], [!UICONTROL Programas], [!UICONTROL Detalles de Portfolio], [!UICONTROL Portfolio], [!UICONTROL Optimización], [!UICONTROL Documentos], [!UICONTROL Actualizaciones], [!UICONTROL Planificación]*, [!UICONTROL Aplicación personalizada]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>Nombre de un programa</td> 
      <td>[!UICONTROL Proyectos], [!UICONTROL Detalles del programa], [!UICONTROL Actualizaciones], [!UICONTROL Documentos], [!UICONTROL Planificación]*, [!UICONTROL Aplicación personalizada]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template]</td> 
      <td>Nombre de una plantilla de proyecto</td> 
      <td>[!UICONTROL Template Tasks], [!UICONTROL Template Details], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Risks], [!UICONTROL Expenses], [!UICONTROL People], [!UICONTROL Approvals], [!UICONTROL Billing Rates], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic], [!UICONTROL Topic Group]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template Task]</td> 
      <td>Nombre de una tarea de plantilla</td> 
      <td>[!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Template Task Details], [!UICONTROL Subtasks], [!UICONTROL Expenses], [!UICONTROL Approvals], [!UICONTROL Predecessors]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Billing Record]</td> 
      <td>Nombre de un registro de facturación de un proyecto</td> 
      <td>[!UICONTROL Billing Record Details], [!UICONTROL Billable Hours], [!UICONTROL Billable Expenses], [!UICONTROL Fixed Revenues]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Projects]</td> 
      <td>Proyectos <img src="assets/projects-in-main-menu.png"> en el [!UICONTROL Main menu] <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Projects]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Requests]</td> 
      <td>El nombre de una solicitud</td> 
      <td>[!UICONTROL New Request], [!UICONTROL Submitted requests], [!UICONTROL All Requests], [!UICONTROL Drafts]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Dashboards]</td> 
      <td>El nombre de un panel de control</td> 
      <td>[!UICONTROL My Dashboards], [!UICONTROL Shared Dashboards], [!UICONTROL All Dashboards]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Scrum Team]</td> 
      <td>El nombre de un equipo de Scrum</td> 
      <td><p>[!UICONTROL Iterations], [!UICONTROL Current iteration], [!UICONTROL Backlog], [!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Settings]</p> <p><strong>NOTA:</strong> El elemento <strong>[!UICONTROL Current iteration]</strong> solo se muestra en el panel izquierdo cuando hay al menos una tarea o un problema en la iteración.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Kanban Team]</td> 
      <td>El nombre de un equipo Kanban</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Kanban board], [!UICONTROL Backlog], [!UICONTROL Updates], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Waterfall Team]</td> 
      <td>El nombre de un equipo de Waterfall</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Requests], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iteration]</td> 
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

   *Su empresa debe adquirir una licencia adicional para Workfront Planning a fin de poder agregar esta área al panel izquierdo de proyectos, portafolios y programas. Para obtener más información, consulte [Descripción general de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)

   **Las aplicaciones personalizadas deben crearse por separado antes de que estén disponibles como opciones del menú principal. Para obtener más información, consulte [Crear una aplicación personalizada para Workfront con Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).


1. En la lista **[!UICONTROL Panel izquierdo]**, realice una de las siguientes acciones para determinar qué usuarios verán en el panel izquierdo para el área [!DNL Workfront] o el tipo de objeto que ha seleccionado:

   * Haga clic en los iconos **Mostrar** ![Mostrar icono](assets/add-secondary-nav-item.png) o **Ocultar** ![Ocultar icono](assets/delete-secondary-nav-item.png) para mostrar u ocultar secciones en el panel izquierdo. No puede ocultar elementos que no tengan los iconos **Mostrar** o **Ocultar**.

   * Arrastre los elementos ![Icono de mover](assets/move-icon---dots.png) para cambiar su orden en el panel izquierdo.

   >[!NOTE]
   >
   >Los siguientes elementos de la lista desplegable **[!UICONTROL Personalizar lo que ven los usuarios]** se refieren a áreas distintas del panel izquierdo:
   >* [!UICONTROL Listas]
   >* [!UICONTROL Panel de resumen]
   >* [!UICONTROL Inicio]
   >* [!UICONTROL Marca]
   > 
   >Para obtener información sobre cómo personalizar las áreas adicionales, consulte los siguientes artículos:
   >
   >* [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >* [Personalizar el [!UICONTROL panel de resumen] mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   >* [Personalizar página de inicio mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   >* [Personalización de la marca Adobe  [!DNL Workfront]  usando una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. (Opcional) Si desea agregar un elemento del panel izquierdo que se vincule a uno de los paneles de su organización, haga clic en **[!UICONTROL Agregar panel]**, escriba el **[!UICONTROL nombre del vínculo rápido]** para el elemento y, a continuación, elija el panel.

   Debe generar el tablero antes de que aparezca en la lista.

   Los elementos del panel aparecen en la parte inferior del panel izquierdo.

   >[!NOTE]
   >
   >Los usuarios pueden añadir elementos de panel de control personalizados a su propio panel izquierdo. Cuando se agregan elementos de panel personalizados a una plantilla de diseño, los elementos se muestran además de los que agregan, sin sobrescribirlos ni restablecerlos. Esto también se aplica si asigna usuarios a una nueva plantilla de diseño con elementos de panel de control personalizados. Para obtener información acerca de cómo los usuarios pueden personalizar el panel izquierdo, vea [Agregar un panel en el panel izquierdo de un objeto o área de Workfront](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
   >
   >Para obtener información sobre los paneles de control, consulte [Paneles de control](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Siga personalizando la plantilla de diseño.

   O

   Si ha finalizado la personalización, haga clic en **[!UICONTROL Guardar]**.

   >[!TIP]
   >
   >Puede hacer clic en [!UICONTROL **Guardar**] en cualquier momento para guardar el progreso, lo que cierra el editor de plantillas de diseño y, a continuación, seguir modificando la plantilla más adelante.
