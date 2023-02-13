---
product-area: projects
navigation-topic: manage-tasks
title: Administrar finanzas de tarea en la sección Detalles de la tarea
description: Administrar finanzas de tarea en la sección Detalles de la tarea
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 5%

---

# Administrar finanzas de tarea en la sección Detalles de la tarea

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

Puede ver o editar la información financiera de una tarea accediendo al área Información general de la sección Detalles de la tarea . Hay un número limitado de campos que puede ver o editar en esta área. Para obtener información sobre cómo editar toda la información financiera de una tarea, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos y tareas</p> <p>Ver acceso a datos financieros o superior</p> <p>Debe tener acceso de edición a los datos financieros para editar la información financiera sobre las tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos para la tarea que incluyen Ver finanzas o superior</p> <p>Debe tener permisos de gestión en la tarea que incluyen Editar finanzas para editar información financiera sobre tareas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Editar finanzas de tareas en la sección Detalles de la tarea

1. Vaya a un proyecto en el que desee ver una tarea.

   >[!NOTE]
   >
   >Para buscar una tarea, también puede buscarla y hacer clic en el nombre para acceder a la tarea. Para obtener más información sobre la búsqueda de objetos en Workfront, consulte [Buscar en Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. Haga clic en **Tareas** en el panel izquierdo.
1. Haga clic en el nombre de una tarea que desee ver.
1. Haga clic en **Detalles de la tarea**.
1. (Opcional) Haga clic en el **Contraer todo** en la parte superior derecha de la página Detalles de la tarea .

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >Dependiendo de cómo configure el administrador de Workfront o el administrador de grupo nuestra plantilla de diseño, los campos de la sección Detalles de la tarea podrían reorganizarse o no mostrarse. Para obtener más información, consulte [Personalización de la vista Detalles mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Haga clic en **Finanzas** para expandir y ver la información financiera de la tarea.

   Haga clic en el **Editar** icono ![](assets/edit-icon.png) en la esquina superior derecha de la sección Detalles , haga clic en **Finanzas**.

1. Edite cualquier campo que esté disponible para edición haciendo clic en él o haciendo clic en él. **+Añadir** para añadir información a un campo vacío.
1. Revise o edite la siguiente información en la sección **Finanzas** área :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo de costo</td> 
      <td> <p>Especifique el tipo de coste para la tarea. Esto determinará cómo se calcula el coste de la tarea, en función del número de horas en las tareas. </p> <p>Seleccione entre las siguientes opciones: </p> 
       <ul> 
        <li> <p>Sin costo</p> </li> 
        <li> <p>Fijo por hora </p> </li> 
        <li> <p> Usuario por hora </p> </li> 
        <li> <p> Rol por hora</p> </li> 
       </ul> <p>Para obtener más información sobre el seguimiento de costes, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a> . El administrador de Workfront o un administrador de grupos selecciona la configuración predeterminada Tipo de coste para las tareas del sistema o del grupo. Para obtener información sobre la configuración de los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de ingresos</td> 
      <td> <p>Especifique el tipo de ingresos para la tarea. Esto determina cómo se calcula el resultado de la tarea, en función del número de horas que haya en las tareas. </p> <p>Seleccione entre las siguientes opciones: </p> 
       <ul> 
        <li> <p> No facturable </p> </li> 
        <li> <p>Usuario por hora </p> </li> 
        <li> <p>Rol por hora </p> </li> 
        <li> <p>Fijo por hora </p> </li> 
        <li> <p>Usuario por hora sin tope </p> </li> 
        <li> <p>Rol por hora con tope </p> </li> 
        <li> <p>Usuario por hora más fijos </p> </li> 
        <li> <p>Rol por hora más fijos </p> </li> 
        <li> <p>Ingresos fijos </p> </li> 
       </ul> <p>Para obtener más información sobre el seguimiento de ingresos, consulte<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a> . </p> <p>El administrador de Workfront o el administrador de grupos seleccionan la configuración predeterminada Tipo de ingresos para las tareas del sistema o del grupo. Para obtener información sobre la configuración de los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo planificado</td> 
      <td> <p>Se trata de un cálculo que muestra el coste de la tarea en función de las horas planificadas, el tipo de coste y la tasa por hora para los usuarios o las funciones de trabajo. Para obtener más información sobre el seguimiento de costes, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo real</td> 
      <td> <p> Se trata de un cálculo que muestra el coste de la tarea en función de las horas reales, el tipo de coste y la tasa por hora para los usuarios o las funciones de trabajo. Para obtener más información sobre el seguimiento de costes, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresos planificados</td> 
      <td> <p>Se trata de un cálculo que muestra los ingresos asociados con la tarea en función de las horas planificadas, el tipo de ingresos y la tasa por hora para los usuarios o las funciones de trabajo. Para obtener más información sobre el seguimiento de costes, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresos reales</td> 
      <td> <p>Se trata de un cálculo que muestra los ingresos asociados con la tarea en función de las horas reales, el tipo de ingresos y la tasa por hora para los usuarios o las funciones de trabajo. Para obtener más información sobre el seguimiento de costes, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>IRC / IRCC / ICC</strong> </td> 
      <td> <p>Son métricas de rendimiento de tareas que muestran el rendimiento de su tarea en un momento determinado. Sus valores se calculan según el método de índice de rendimiento del proyecto.<br>Para obtener más información, consulte los siguientes artículos:</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calcular el índice de rendimiento de costes (CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calcular el índice de rendimiento de la programación (SPI) </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calcular el Índice de Rendimiento del Programa de Costes (CSI)</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimación al finalizar (CAO)</td> 
      <td> <p>Se trata de un cálculo que muestra el coste total de la tarea al finalizar. Para obtener más información sobre la estimación al finalizar, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcular estimación al finalizar (CAO)</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Si está editando los campos en la sección Finanzas, haga clic en **Guardar***Cambios**.
