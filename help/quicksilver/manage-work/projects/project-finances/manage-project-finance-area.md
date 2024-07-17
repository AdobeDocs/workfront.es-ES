---
product-area: projects
navigation-topic: financials
title: Administrar información en el área de finanzas del proyecto
description: Administrar información en el área de finanzas del proyecto
author: Alina
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: 647788221b4acff1cfd5e0ce14d5b99cf90ceee0
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 2%

---

# Administrar información en el área de finanzas del proyecto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

Puede ver o editar la información financiera de un proyecto accediendo al área Finanzas de la sección Detalles del proyecto. Hay un número limitado de campos que puede ver o editar en esta área. Para obtener información sobre cómo editar toda la información de un proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

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
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver o mejorar el acceso a Proyectos y Datos financieros</p> <p>Editar el acceso a Proyectos y Datos financieros para editar la información financiera del proyecto</p> <p><b>NOTA</b></p>
   <p> Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos de un proyecto o superior que incluyen permisos de Ver finanzas</p> <p>Administre permisos para el proyecto que incluyan Administrar finanzas para editar la información financiera del proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Panorama general del área de Finanzas

Tenga en cuenta lo siguiente cuando visualice o edite información en el área Finanzas:

* La información financiera que se encuentra en el área Finanzas de Detalles del proyecto representa valores que se acumulan en el nivel de proyecto a partir de las tareas, así como información introducida directamente en el proyecto. Parte de la información financiera se puede administrar tanto en el nivel de proyecto como en el de tarea.
* Debe tener permisos de visualización en el proyecto y acceso a datos financieros desde su nivel de acceso para poder ver el área de finanzas en un proyecto.
* Debe tener permisos de administración en el proyecto y acceso a datos financieros desde su nivel de acceso para poder editar la información en el área de finanzas Sin embargo, recomendamos que solo el propietario del proyecto edite la información de esta área

## Ver información de finanzas de un proyecto

1. Vaya a un proyecto.
1. Haga clic en **Detalles del proyecto** en el panel izquierdo.
1. Haga clic en el icono **Editar** ![](assets/edit-icon.png) en la esquina superior derecha de la sección Detalles y, a continuación, haga clic en **Finanzas**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >Según la configuración dada a la plantilla de diseño por el administrador de Workfront, es posible que la sección Información general no aparezca primero en la lista, en cuyo caso se contraerá. Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Vea los siguientes campos en el área Finanzas del proyecto:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Método de índice de rendimiento</td> 
      <td> Controla el método que utiliza Workfront para calcular las métricas de valor ganado. Puede basarse en el horario o en los costes. <br>Para obtener más información acerca del PIM, consulte el artículo <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Establecer el método de índice de rendimiento (PIM)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">IRC/IRCC/ICC</td> 
      <td> <p>Son métricas de rendimiento del proyecto que muestran el rendimiento del proyecto en un momento determinado. Sus valores se calculan según el método de índice de rendimiento.<br>Para obtener más información, consulte los siguientes artículos: </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calcular el índice de rendimiento de costos (CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calcular índice de rendimiento de horario (SPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calcular índice de rendimiento de horario de costos (CSI)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimar al finalizar</td> 
      <td> Costo total proyectado del proyecto, representado en horas si el método de índice de rendimiento (PIM) se basa en horas y se representa en un valor de moneda, si el método de índice de rendimiento (PIM) se basa en costos.<br>Para obtener más información acerca del cálculo de la estimación al finalizar, vea el artículo <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcular estimación al finalizar (EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Presupuesto</td> 
      <td>Este es el presupuesto establecido para el proyecto. El propietario del proyecto lo especifica manualmente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coste fijo</td> 
      <td>Son los costos fijos del proyecto, independientemente de otras actividades del proyecto. El propietario del proyecto los introduce manualmente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo planificado</td> 
      <td>El coste estimado del proyecto, basado en las horas planificadas y las tasas asociadas con los usuarios asignados de la tarea (roles de trabajo o usuarios).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo real</td> 
      <td>Todos los costes acumulados en el proyecto. Costo real es la suma de todos los costos reales: costo laboral (basado en horas reales y las tasas asociadas con los roles del puesto o los usuarios que los registran), gastos y costos fijos, que pueden asociarse con un proyecto o tarea.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresos fijos</td> 
      <td>Establezca los ingresos esperados según el calendario del proyecto. El propietario del proyecto especifica manualmente los ingresos fijos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresos planificados</td> 
      <td>Ingresos previstos basados en las horas planificadas y las tasas asociadas con los usuarios asignados a la tarea (funciones del puesto o usuarios).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresos reales</td> 
      <td>Ingresos reales del proyecto basados en las horas reales y las tasas asociadas con los usuarios asignados a la tarea (roles de trabajo o usuarios).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresos facturados</td> 
      <td> <p>Ingresos facturados a clientes u otras partes que se capturan en los registros de facturación. Para obtener más información acerca de los registros de facturación, consulte el artículo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Crear registros de facturación</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

## Edición de información financiera en un proyecto

Como propietario del proyecto, puede editar la información en la subpestaña Finanzas de un proyecto.

Para editar información en la subpestaña Project Finance:

1. Vaya a un proyecto del que sea propietario.

   >[!NOTE]
   >
   >Necesita permisos de administración en el proyecto para realizar los siguientes pasos. También recomendamos que solo el propietario del proyecto realice cambios en la subpestaña Finanzas del proyecto.

1. Haga clic en **Detalles del proyecto** en el panel izquierdo.
1. Haga clic en el icono **Editar** ![](assets/edit-icon.png) en la esquina superior derecha de la sección Detalles y, a continuación, haga clic en **Finanzas** . Se abrirá el área Finanzas para editarla.
1. Edite cualquier campo que esté disponible para la edición haciendo clic en el campo o haga clic en **+Agregar** para agregar información a un campo vacío.

   >[!TIP]
   >
   >Los campos no están disponibles para la edición si Workfront los calcula automáticamente o si no tiene permisos de edición en ellos.

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. Actualice cualquiera de los campos siguientes.

   >[!NOTE]
   >
   >Según la forma en que el administrador de Workfront configure la plantilla de diseño, los campos de la sección Detalles del proyecto podrían ser diferentes en su entorno. Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Método de índice de rendimiento</td> 
      <td> <p>Controla el método que utiliza Workfront para calcular las métricas de rendimiento del proyecto. El administrador lo configura en el nivel de sistema, pero también puede editarlo en el nivel de proyecto. Considere la posibilidad de seleccionar una de las siguientes opciones:</p> 
       <ul> 
        <li><strong>Basado en horas:</strong>Workfront usa las horas planificadas para calcular el CPI y el EAC del proyecto, y el EAC del proyecto se muestra como un número en horas. </li> 
        <li><strong>Basado en costos:</strong>Workfront usa el costo de mano de obra planificado para calcular el CPI y el EAC del proyecto, y el EAC se muestra como un valor de moneda. Al seleccionar esta opción, asegúrese de que las personas asignadas a la tarea (funciones del puesto o usuarios) estén asociadas a las tasas de coste.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimar al finalizar</td> 
      <td> <p>Representa el costo total proyectado del proyecto o tarea cuando se completa. El administrador lo configura en el nivel de sistema, pero también puede editarlo en el nivel de proyecto. Considere la posibilidad de seleccionar una de las siguientes opciones:</p> 
       <ul> 
        <li><strong>Calcular en el nivel de proyecto</strong>: el EAC de la tarea y el proyecto principales se determina especificando las horas reales/el costo laboral real en las fórmulas EAC. Este cálculo incluye las horas, los costos y los gastos reales agregados directamente a la tarea o al proyecto principal.</li> 
        <li><strong>Resumir a partir de tareas/ subtareas</strong>: el EAC de la tarea y el proyecto principales se determina resumiendo el EAC de cada tarea secundaria. Este cálculo excluye las horas, los costos y los gastos reales agregados directamente a la tarea o al proyecto principal.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Presupuesto</td> 
      <td>Especifique el presupuesto para este proyecto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coste fijo</td> 
      <td>Especifique el coste fijo de este proyecto. Esto no debe incluir costes laborales o de gastos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresos fijos</td> 
      <td> <p>Especifique los ingresos fijos de este proyecto. Esto no debe incluir los ingresos procedentes de ningún registro de facturación facturado a socios o terceros.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Divisa del proyecto</td> 
      <td> <p>Especifique una moneda para este proyecto, si es diferente de la moneda predeterminada en el sistema. El administrador de Workfront define la moneda predeterminada del sistema. Para obtener más información acerca de la configuración de tasas de cambio en Workfront, consulte el artículo <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tasas de cambio</a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. Haga clic en **Guardar cambios**.
