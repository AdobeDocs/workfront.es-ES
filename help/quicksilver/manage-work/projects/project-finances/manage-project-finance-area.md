---
product-area: projects
navigation-topic: financials
title: Administrar información en el área de finanzas del proyecto
description: Administrar información en el área de finanzas del proyecto
author: Alina
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 2%

---

# Administrar información en el área de finanzas del proyecto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

Puede ver o editar la información financiera de un proyecto accediendo al área Finanzas de la sección Detalles del proyecto . Hay un número limitado de campos que puede ver o editar en esta área. Para obtener información sobre cómo editar toda la información de un proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

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
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver o tener más acceso a Proyectos y Datos financieros</p> <p>Editar el acceso a Proyectos y Datos Financieros para editar la información financiera del proyecto</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos de un proyecto o superior que incluyen permisos de Ver finanzas</p> <p>Administre los permisos del proyecto que incluyen Administrar finanzas para editar la información financiera del proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Descripción general del área de finanzas

Tenga en cuenta lo siguiente cuando visualice o edite información en el área de finanzas:

* La información financiera que puede encontrar en el área Finanzas de Detalles del proyecto representa valores que se resumen al nivel del proyecto desde las tareas, así como información introducida directamente en el proyecto. Parte de la información financiera se puede administrar en el proyecto, así como en el nivel de tarea.
* Debe tener permisos de visualización en el proyecto, así como acceso a datos financieros desde el nivel de acceso para poder ver el área de finanzas de un proyecto.
* Debe tener permisos de administración en el proyecto, así como acceso a datos financieros desde el nivel de acceso para poder editar la información en el área de finanzas . Sin embargo, recomendamos que solo el propietario del proyecto edite la información de esta área .

## Ver información financiera de un proyecto

1. Vaya a un proyecto.
1. Haga clic en **Detalles del proyecto** en el panel izquierdo.
1. Haga clic en el **Editar** icono ![](assets/edit-icon.png) en la esquina superior derecha de la sección Detalles , haga clic en **Finanzas**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >Según la configuración del administrador de Workfront de la plantilla de diseño, es posible que la sección Información general no aparezca en primer lugar, en cuyo caso se contraerá. Para obtener más información, consulte [Personalización de la vista Detalles mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Vea los campos siguientes en el área Finanzas del proyecto:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Método de índice de rendimiento</td> 
      <td> Controla el método que utiliza Workfront para calcular las métricas de Valor acumulado. Puede basarse en horas o en costes. <br>Para obtener más información sobre el PIM, consulte el artículo <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Definir el método del índice de rendimiento (PIM)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">IRC / IRCC / ICC</td> 
      <td> <p>Son métricas de rendimiento del proyecto que muestran el rendimiento del proyecto en un momento determinado. Sus valores se calculan según el método del índice de rendimiento.<br>Para obtener más información, consulte los siguientes artículos: </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calcular el índice de rendimiento de costes (CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calcular el índice de rendimiento de la programación (SPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calcular el Índice de Rendimiento del Programa de Costes (CSI)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimar al finalizar</td> 
      <td> El coste total proyectado de su proyecto, representado en horas si el método de índice de rendimiento (PIM) está basado en horas y se representa en un valor de moneda, si el método de índice de rendimiento (PIM) está basado en costes.<br>Para obtener más información sobre el cálculo de la estimación al completarse, consulte el artículo <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcular estimación al finalizar (CAO)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Presupuesto</td> 
      <td>Este es el presupuesto establecido para el proyecto. El propietario del proyecto lo especifica manualmente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo fijo</td> 
      <td>Estos son los costes fijos del proyecto, independientemente de otras actividades del proyecto. El propietario del proyecto las introduce manualmente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo planificado</td> 
      <td>El coste estimado del proyecto, basado en el horario planificado y en las tasas asociadas con los asignadores de tareas (funciones o usuarios).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Costo real</td> 
      <td>Todos los costes acumulados en el proyecto. Costo real es la suma de todos los costos reales: coste laboral (en función de las horas reales y las tasas asociadas con las funciones de trabajo o los usuarios que las registran), gastos y costes fijos, que se pueden asociar a un proyecto o tarea.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresos fijos</td> 
      <td>Establezca los ingresos esperados en función del calendario del proyecto. El propietario del proyecto especifica manualmente los ingresos fijos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresos planificados</td> 
      <td>Se esperan ingresos previstos basados en el horario planificado y en las tasas asociadas con los asignadores de tareas (funciones o usuarios).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresos reales</td> 
      <td>Ingresos reales del proyecto basados en el horario real y en las tasas asociadas con los asignadores de tareas (funciones o usuarios).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresos facturados</td> 
      <td> <p>Ingresos facturados a clientes u otras partes que se capturan en Registros de facturación. Para obtener más información sobre los registros de facturación, consulte el artículo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Crear registros de facturación</a>. </p> </td> 
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

## Editar información financiera en un proyecto

Como propietario del proyecto, puede editar la información en la subficha Finanzas de un proyecto.

Para editar información en la subficha Finanzas del proyecto:

1. Vaya a un proyecto del que sea propietario.

   >[!NOTE]
   >
   >Para realizar los siguientes pasos, debe administrar los permisos del proyecto. También recomendamos que solo el propietario del proyecto realice cambios en la subficha Finanzas del proyecto.

1. Haga clic en **Detalles del proyecto** en el panel izquierdo.
1. Haga clic en el **Editar** icono ![](assets/edit-icon.png) en la esquina superior derecha de la sección Detalles , haga clic en **Finanzas** . Se abre el área Finanzas para editarlo.
1. Edite cualquier campo que esté disponible para edición haciendo clic en él o haciendo clic en él. **+Añadir** para añadir información a un campo vacío.

   >[!TIP]
   >
   >Los campos no están disponibles para edición si Workfront los calcula automáticamente o si no tiene permisos de edición en ellos.

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. Actualice cualquiera de los campos siguientes.

   >[!NOTE]
   >
   >Según la configuración de la plantilla de diseño que configure el administrador de Workfront, los campos de la sección Detalles del proyecto pueden ser diferentes en el entorno. Para obtener más información, consulte [Personalización de la vista Detalles mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Método de índice de rendimiento</td> 
      <td> <p>Controla el método que utiliza Workfront para calcular las métricas de rendimiento del proyecto. El administrador lo configura en el nivel del sistema, pero también puede editarlo en el nivel del proyecto. Considere la posibilidad de seleccionar una de las siguientes opciones:</p> 
       <ul> 
        <li><strong>Basado en horas:</strong>Workfront utiliza las horas planificadas para calcular el CPI y la CAO del proyecto, y el CAO del proyecto se muestra como un número, en horas. </li> 
        <li><strong>Basado en los costos:</strong>Workfront utiliza el Costo de trabajo planificado para calcular el IPC y la CAO del proyecto, y el EAC se muestra como un valor de moneda. Cuando seleccione esta opción, asegúrese de que los asignadores de tareas (funciones de trabajo o usuarios) estén asociados a tasas de coste.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimar al finalizar</td> 
      <td> <p>Representa el coste total previsto del proyecto o la tarea cuando se completa. El administrador lo configura en el nivel del sistema, pero también puede editarlo en el nivel del proyecto. Considere la posibilidad de seleccionar una de las siguientes opciones:</p> 
       <ul> 
        <li><strong>Calcular en el nivel de proyecto</strong>: Las CAO para la tarea principal y el proyecto se determinan introduciendo las horas/coste laboral real en las Fórmulas de CAO. Este cálculo incluye horas/costes reales y gastos añadidos directamente a la tarea o proyecto principal.</li> 
        <li><strong>Resumen de tareas/subtareas</strong>: Las CAO para la tarea principal y el proyecto se determinan sumando la CAO para cada tarea secundaria. Este cálculo excluye las horas/costes reales y los gastos añadidos directamente a la tarea o proyecto principal.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Presupuesto</td> 
      <td>Especifique el presupuesto de este proyecto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Costo fijo</strong> </td> 
      <td>Especifique el coste fijo para este proyecto. Esto no debe incluir ningún costo laboral o de gastos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ingresos fijos</strong> </td> 
      <td> <p>Especifique los ingresos fijos de este proyecto. Esto no debe incluir los ingresos procedentes de registros de facturación facturados a socios o terceros.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Divisa del proyecto</td> 
      <td> <p>Especifique una moneda para este proyecto si es diferente de la moneda predeterminada del sistema. El administrador de Workfront define la moneda predeterminada del sistema. Para obtener más información sobre la configuración de las tasas de cambio en Workfront, consulte el artículo <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tipos de cambio</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar***Cambios**.
