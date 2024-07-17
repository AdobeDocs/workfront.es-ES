---
product-area: projects
navigation-topic: manage-tasks
title: Administrar finanzas de tareas en la sección Detalles de tareas
description: Administrar finanzas de tareas en la sección Detalles de tareas
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 4%

---

# Administrar finanzas de tareas en la sección Detalles de tareas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

Puede ver o editar la información financiera de una tarea accediendo al área Información general de la sección Detalles de la tarea Hay un número limitado de campos que puede ver o editar en esta área. Para obtener información sobre cómo editar toda la información financiera de una tarea, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos y tareas</p> <p>Ver acceso a datos financieros o superior</p> <p>Debe tener acceso de edición a los datos financieros para editar la información financiera sobre las tareas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos de la tarea que incluyen Ver finanzas o superior</p> <p>Debe tener permisos de Administración en la tarea que incluya Editar finanzas para editar la información financiera de las tareas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Edite las finanzas de la tarea en la sección Detalles de la tarea

1. Vaya a un proyecto en el que desee ver una tarea.

   >[!NOTE]
   >
   >Para encontrar una tarea, también puede buscarla y hacer clic en el nombre para acceder a la tarea. Para obtener más información sobre cómo buscar objetos en Workfront, consulte [Buscar en Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. Haga clic en **Tareas** en el panel izquierdo.
1. Haga clic en el nombre de una tarea que desee ver.
1. Haga clic en **Detalles de la tarea**.
1. (Opcional) Haga clic en el icono **Contraer todo** en la parte superior derecha de la página Detalles de la tarea.

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >Según la forma en que el administrador de Workfront o el administrador del grupo configuren la plantilla de diseño, los campos de la sección Detalles de la tarea podrían volver a organizarse o no mostrarse. Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Haga clic en **Finanzas** para expandir y ver la información financiera de la tarea.

   Haga clic en el icono **Editar** ![](assets/edit-icon.png) en la esquina superior derecha de la sección Detalles y, a continuación, haga clic en **Finanzas**.

1. Edite cualquier campo que esté disponible para la edición haciendo clic en el campo o haga clic en **+Agregar** para agregar información a un campo vacío.
1. Revise o edite la siguiente información en el área **Finanzas**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo de costo</td> 
      <td> <p>Especifique el Tipo de coste de la tarea. Esto determina cómo se calcula el coste de la tarea, en función del número de horas de las tareas. </p> <p>Seleccione entre las siguientes opciones: </p> 
       <ul> 
        <li> <p>Sin coste</p> </li> 
        <li> <p>Fijo por hora </p> </li> 
        <li> <p> Usuario por hora </p> </li> 
        <li> <p> Rol por hora</p> </li> 
       </ul> <p>Para obtener más información sobre los costos de seguimiento, vea <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costos de seguimiento</a> . El administrador de Workfront o de un grupo selecciona la configuración predeterminada Tipo de coste para las tareas del sistema o del grupo. Para obtener información sobre cómo establecer los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de ingresos</td> 
      <td> <p>Especifique el Tipo de ingresos para la tarea. Esto determina cómo se calculan los ingresos de la tarea, en función del número de horas de las tareas. </p> <p>Seleccione entre las siguientes opciones: </p> 
       <ul> 
        <li> <p> No facturable </p> </li> 
        <li> <p>Usuario por hora </p> </li> 
        <li> <p>Rol por hora </p> </li> 
        <li> <p>Fijo por hora </p> </li> 
        <li> <p>Usuario por hora sin límite </p> </li> 
        <li> <p>Rol por hora con límite </p> </li> 
        <li> <p>Usuario por hora más fijos </p> </li> 
        <li> <p>Rol por hora más fijos </p> </li> 
        <li> <p>Ingresos fijos </p> </li> 
       </ul> <p>Para obtener más información sobre el seguimiento de los ingresos, consulte<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a> . </p> <p>El administrador de Workfront o del grupo selecciona la configuración predeterminada Tipo de ingresos para las tareas del sistema o del grupo. Para obtener información sobre cómo establecer los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo planificado</td> 
      <td> <p>Se trata de un cálculo que muestra el coste de la tarea en función de las horas planificadas, el tipo de coste y la tasa por hora para los usuarios o los roles. Para obtener más información sobre los costos de seguimiento, vea <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costos de seguimiento</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo real</td> 
      <td> <p> Se trata de un cálculo que muestra el coste de la tarea en función de las horas reales, el tipo de coste y la tarifa por hora de los usuarios o los roles. Para obtener más información sobre los costos de seguimiento, vea <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costos de seguimiento</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresos planificados</td> 
      <td> <p>Se trata de un cálculo que muestra los ingresos asociados con la tarea en función de las horas planificadas, el tipo de ingresos y la tasa por hora para los usuarios o los roles. Para obtener más información sobre los costos de seguimiento, vea <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costos de seguimiento</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresos reales</td> 
      <td> <p>Se trata de un cálculo que muestra los ingresos asociados con la tarea en función de las horas reales, el tipo de ingresos y la tarifa por hora de los usuarios o los roles. Para obtener más información sobre los costos de seguimiento, vea <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costos de seguimiento</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>IRC/IRCC/CSI</strong> </td> 
      <td> <p>Son métricas de rendimiento de tareas que muestran el rendimiento de la tarea en un momento determinado. Sus valores se calculan según el método de índice de rendimiento del proyecto.<br>Para obtener más información, consulte los siguientes artículos:</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calcular el índice de rendimiento de costos (CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calcular índice de rendimiento de horario (SPI) </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calcular índice de rendimiento de horario de costos (CSI)</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimar al finalizar (EAC)</td> 
      <td> <p>Es un cálculo que muestra el costo total de la tarea, al finalizar. Para obtener más información acerca de la estimación al finalizar, vea <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcular estimación al finalizar (EAC)</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Si está editando los campos en la sección Finanzas, haga clic en **Guardar****Cambios**.
