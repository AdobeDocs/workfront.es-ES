---
title: Crear o personalizar grupos de problemas
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Los usuarios pueden usar gravámenes para definir la gravedad de un problema. Puede personalizar cualquiera de las cinco gravedad predeterminadas que existen en Adobe Workfront o crear una nueva gravedad para los usuarios.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 4%

---

# Crear o personalizar grupos de problemas

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Los usuarios pueden usar gravámenes para definir la gravedad de un problema. Puede personalizar cualquiera de las cinco gravedad predeterminadas que existen en Adobe Workfront o crear una nueva gravedad para los usuarios.

>[!NOTE]
>
>Las tareas y los proyectos no tienen seriedad.

## Requisitos de acceso

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Grupos de problemas integrados

Workfront tiene cinco grupos de problemas integrados:

* Cosmético
* Causa confusión
* Error con solución
* Error sin solución
* Error fatal

<p>Puede editar lo siguiente para estos grupos:</p>

* Nombre
* Color

   El color de una gravedad se conserva en un informe de gráfico si se agrupan los resultados por gravedad del problema. Para obtener información sobre los informes de gráficos, consulte [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* ¿Qué gravedad es la predeterminada?

   Para obtener más información sobre la gravedad predeterminada, consulte [Crear o editar una gravedad de problema](#create-or-edit-an-issue-severity) en este artículo.
* Descripción
* Si una gravedad está oculta en Workfront

   Para obtener más información sobre cómo ocultar una gravedad, consulte [Crear o editar una gravedad de problema](#create-or-edit-an-issue-severity")

* Eliminar una gravedad

   Al hacerlo, debe seleccionar una gravedad de reemplazo.

## Crear o editar una gravedad de problema {#create-or-edit-an-issue-severity}

Como administrador de Workfront, puede crear y editar grupos de problemas para adaptarlos a las necesidades de sus usuarios.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Preferencias de proyecto** > **Versiones**.

1. Si está creando una nueva gravedad, haga clic en **Agregar una nueva gravedad**.
1. Configure las siguientes opciones para la nueva gravedad o edítelas para una existente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de gravedad</td> 
      <td>Escriba un nombre para la gravedad</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importancia</td> 
      <td>Aumente o disminuya el nivel de gravedad, asignado originalmente por Workfront, para la gravedad.
      <p>El número de importancia de cada gravedad debe ser único. El número más alto corresponde al nivel más alto de gravedad.</p> <p>No puede editar este número después de guardar la gravedad.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Color</td> 
      <td> <p>Elija un color para la gravedad.</p> 
      <p>El color de la gravedad se utiliza en los informes de gráficos cuando se agrupan los resultados por gravedad del problema. Para obtener información sobre los informes de gráficos, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Agregar un gráfico a un informe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gravedad predeterminada</td> 
      <td>Seleccione la gravedad que desea que Workfront seleccione automáticamente todos los problemas recién creados.</p>
      <p>La métrica es la gravedad predeterminada para los problemas en Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba una descripción de la gravedad para explicar su función.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar</td> 
      <td> Oculte una gravedad que ya no sea necesaria. 
      <p>Una gravedad oculta no se muestra en ninguna parte de Workfront, por lo que los usuarios no pueden seleccionarla para sus problemas.</p> 
      <p><b>IMPORTANTE</b>: En lugar de eliminar gravámenes que ya no desea utilizar, le sugerimos que los oculte. De este modo, se mantienen todos los datos históricos de los objetos que ya se han completado con la gravedad, al tiempo que se evita que las personas utilicen la gravedad en el futuro.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Cambie el orden de las listas de sus gravedad arrastrándolas y soltándolas en el orden que desee.

   Esto cambia el orden en que se muestran para los problemas. No cambia la variable **Importancia** número.

1. Haga clic en **Guardar**.

Para obtener más información sobre cómo utilizar las gravedad mientras se trabaja con problemas, consulte [Actualizar gravedad del problema](../../../manage-work/issues/issue-information/update-issue-severity.md).
