---
title: Personalización del panel izquierdo con una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En una plantilla de diseño, puede personalizar lo que los usuarios ven en el área del panel izquierdo a través de Adobe Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 0%

---

# Personalización del panel izquierdo con una plantilla de diseño

<!--Audited: 10/2024-->

En una plantilla de diseño, puede personalizar lo que los usuarios ven en el área del panel izquierdo en [!DNL Adobe Workfront].

Por ejemplo, puede determinar cuál de los siguientes elementos ven los usuarios en el panel izquierdo al ver una tarea:

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>Los cambios realizados en el orden y la visibilidad se reflejan en la aplicación móvil.

Para obtener información sobre cómo crear plantillas de diseño, consulte [Crear y administrar plantillas de diseño](../use-layout-templates/create-and-manage-layout-templates.md).

Para obtener información acerca de las plantillas de diseño para grupos, vea [Crear y modificar plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Después de configurar una plantilla de diseño, debe asignarla a usuarios para que los cambios que ha realizado sean visibles para otros. Para obtener información acerca de cómo asignar una plantilla de diseño a los usuarios, vea [Asignar usuarios a una plantilla de diseño](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
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

## Personalizar el panel izquierdo de un área de [!DNL Workfront]:

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Haga clic en la flecha abajo ![](assets/dropdown-arrow.png) bajo **[!UICONTROL Personalizar lo que ven los usuarios]** y, a continuación, haga clic en el nombre de un tipo de objeto o un área [!DNL Workfront] cuyo panel izquierdo desee personalizar.

   Los tipos de objeto y las áreas [!DNL Workfront] cuyo panel izquierdo se puede personalizar se enumeran en la siguiente tabla:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Tipo de objeto o área [!DNL Workfront]</th> 
      <th>Cuando los usuarios hagan clic en lo siguiente...</th> 
      <th>Secciones del panel izquierdo que los usuarios ven después de mostrarlas en la plantilla de diseño:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Proyecto]</td> 
      <td>El nombre de un proyecto</td> 
      <td>[!UICONTROL Tareas], [!UICONTROL Detalles del proyecto], [!UICONTROL Caso comercial], [!UICONTROL Actualizaciones], [!UICONTROL Documentos], [!UICONTROL Problemas], [!UICONTROL Riesgos], [!UICONTROL Aprobaciones], [!UICONTROL Líneas bases], [!UICONTROL Tasas de facturación], [!UICONTROL Registros de facturación], [!UICONTROL Gastos], [!UICONTROL Horas], [!UICONTROL Distribuidor de cargas de trabajo], [!UICONTROL Personas], [!UICONTROL Utilización], [!UICONTROL Detalles de cola], [!UICONTROL Reglas de enrutamiento], [!UICONTROL Tema de cola], [!UICONTROL Grupo de temas], [!UICONTROL Métricas], [!UICONTROL Planificación]*</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tarea]</td> 
      <td>Nombre de una tarea</td> 
      <td> [!UICONTROL Actualizaciones], [!UICONTROL Documentos], [!UICONTROL Detalles de tareas], [!UICONTROL Subtarea], [!UICONTROL Problemas], [!UICONTROL Horas], [!UICONTROL Aprobaciones], [!UICONTROL Gastos], [!UICONTROL Predecesores]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Problema]</td> 
      <td>El nombre de un problema</td> 
      <td> [!UICONTROL Actualizaciones], [!UICONTROL Documentos], [!UICONTROL Detalles del problema], [!UICONTROL Horas], [!UICONTROL Aprobaciones]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>El nombre de un portafolio</td> 
      <td>[!UICONTROL Proyectos], [!UICONTROL Programas], [!UICONTROL Detalles del Portfolio], [!UICONTROL Portfolio], [!UICONTROL Optimización], [!UICONTROL Documentos], [!UICONTROL Actualizaciones], [!UICONTROL Planificación]*</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Programa]</td> 
      <td>El nombre de un programa</td> 
      <td>[!UICONTROL Proyectos], [!UICONTROL Detalles del programa], [!UICONTROL Actualizaciones], [!UICONTROL Documentos], [!UICONTROL Planificación]*</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template]</td> 
      <td>Nombre de una plantilla de proyecto</td> 
      <td>[!UICONTROL Tareas de plantilla], [!UICONTROL Detalles de plantilla], [!UICONTROL Actualizaciones], [!UICONTROL Documentos], [!UICONTROL Riesgos], [!UICONTROL Gastos], [!UICONTROL Personas], [!UICONTROL Aprobaciones], [!UICONTROL Tasas de facturación], [!UICONTROL Detalles de cola], [!UICONTROL Reglas de enrutamiento], [!UICONTROL Tema de cola], [!UICONTROL Grupo de temas]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template Task]</td> 
      <td>Nombre de una tarea de plantilla</td> 
      <td>[!UICONTROL Actualizaciones], [!UICONTROL Documentos], [!UICONTROL Detalles de tarea de plantilla], [!UICONTROL Subtareas], [!UICONTROL Gastos], [!UICONTROL Aprobaciones], [!UICONTROL Predecesores]</td>
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
      <td>Nombre de un registro de facturación de un proyecto</td> 
      <td>[!UICONTROL Detalles de registro de facturación], [!UICONTROL Horas facturables], [!UICONTROL Gastos facturables], [!UICONTROL Ingresos fijos]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Proyectos]</td> 
      <td>Proyectos <img src="assets/projects-in-main-menu.png"> en el menú principal de [!UICONTROL] <img src="assets/main-menu-icon.png"></td> 
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
      <td>[!UICONTROL Mis paneles], [!UICONTROL Paneles compartidos], [!UICONTROL Todos los paneles]<p><b>NOTA</b>: si creó fichas personalizadas para el área de [!UICONTROL Reports] usando una plantilla de diseño en [!DNL Adobe Workfront Classic], se mostrarán en la parte inferior de esta lista. Para los usuarios, se muestran en la parte inferior del panel izquierdo del área de [!UICONTROL Dashboards].</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Equipo de Scrum]</td> 
      <td>El nombre de un equipo de Scrum</td> 
      <td><p>[!UICONTROL Iteraciones], [!UICONTROL Iteración actual], [!UICONTROL Registro de pendientes], [!UICONTROL Distribuidor de cargas de trabajo], [!UICONTROL Actualizaciones], [!UICONTROL Configuración de equipo]</p> <p><strong>NOTA:</strong> El elemento <strong>[!UICONTROL Iiteración actual]</strong> solo se muestra en el panel izquierdo cuando hay al menos una tarea o un problema en la iteración.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Equipo Kanban]</td> 
      <td>El nombre de un equipo Kanban</td> 
      <td>[!UICONTROL Distribuidor de cargas de trabajo], [!UICONTROL Panel Kanban], [!UICONTROL Registro de pendientes], [!UICONTROL Actualizaciones], [!UICONTROL Configuración de equipo]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Equipo de cascada]</td> 
      <td>El nombre de un equipo de Waterfall</td> 
      <td>[!UICONTROL Distribuidor de cargas de trabajo], [!UICONTROL Actualizaciones], [!UICONTROL Solicitudes de equipo], [!UICONTROL Configuración de equipo]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iteration]</td> 
      <td>Nombre de una iteración</td> 
      <td>[!UICONTROL Historias], [!UICONTROL Problemas], [!UICONTROL Panel de historias], [!UICONTROL Información general], [!UICONTROL Forms personalizado], [!UICONTROL Actualizaciones] </td> 
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


1. En la lista **[!UICONTROL Panel izquierdo]**, realice una de las siguientes acciones para determinar qué usuarios verán en el panel izquierdo para el área [!DNL Workfront] o el tipo de objeto que ha seleccionado:

   * Haga clic en los iconos **Mostrar** ![](assets/add-secondary-nav-item.png) o **Ocultar** ![](assets/delete-secondary-nav-item.png) para mostrar u ocultar secciones en el panel izquierdo. No puede ocultar elementos que no tengan los iconos **Mostrar** o **Ocultar**.

   * Arrastre los elementos ![](assets/move-icon---dots.png) para cambiar su orden en el panel izquierdo.

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
   >* [Adobe de marca [!DNL Workfront] usando una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. (Opcional) Si desea agregar un elemento del panel izquierdo que se vincule a uno de los paneles de su organización, haga clic en **[!UICONTROL Agregar sección personalizada]**, escriba un **[!UICONTROL título de sección personalizada]** para el elemento y, a continuación, agregue el panel.

   Los elementos del panel aparecen en la parte inferior del panel izquierdo. Los usuarios ven el título de la sección personalizada que escriba junto al elemento de panel cuando pasan el ratón por encima en el panel izquierdo.

   >[!NOTE]
   >
   >Los usuarios pueden agregar elementos de tablero personalizados a su propio panel izquierdo. Cuando se agregan elementos de panel personalizados a una plantilla de diseño, los elementos se muestran además de los que agregan, sin sobrescribirlos ni restablecerlos. Esto también se aplica si asigna usuarios a una nueva plantilla de diseño con elementos de panel personalizados. Para obtener información acerca de cómo personalizar el panel izquierdo, vea [Crear fichas o secciones personalizadas](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
   >
   >Para obtener información sobre los paneles, consulte [Paneles](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Siga personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **[!UICONTROL Guardar]**.

   >[!TIP]
   >
   >Puede hacer clic en [!UICONTROL **Guardar**] en cualquier momento para guardar el progreso, lo que cierra el editor de plantillas de diseño y, a continuación, seguir modificando la plantilla más adelante.
