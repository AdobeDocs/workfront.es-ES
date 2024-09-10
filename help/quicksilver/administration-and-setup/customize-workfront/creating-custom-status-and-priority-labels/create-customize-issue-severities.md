---
title: Crear o personalizar gravedades de problemas
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Los usuarios pueden usar gravedades para definir la gravedad de un problema. Puede personalizar cualquiera de las cinco gravedades predeterminadas existentes en Adobe Workfront o crear una nueva gravedad para los usuarios.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 5%

---

# Crear o personalizar la gravedad de los problemas

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Los usuarios pueden usar gravedades para definir la gravedad de un problema. Puede personalizar cualquiera de las cinco gravedades predeterminadas existentes en Adobe Workfront o crear una nueva gravedad para los usuarios.

>[!NOTE]
>
>Las tareas y los proyectos no tienen gravedades.

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
     <p>Nuevo: estándar</p>
     <p>o</p>
     <p>Actual: plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gravedades de problemas integradas

Workfront tiene cinco gravedades de problemas integradas:

* Cosmético
* Causa confusión
* Error con solución
* Error sin solución
* Error fatal

<p>Puede editar lo siguiente para estas gravedades:</p>

* Nombre
* Color

  El color de una gravedad se conserva en un informe de gráfico si se agrupan los resultados por Gravedad del problema. Para obtener información sobre los informes de gráficos, consulte [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Qué gravedad es la predeterminada

  Para obtener más información acerca de las gravedades predeterminadas, vea [Crear o editar una gravedad de problema](#create-or-edit-an-issue-severity) en este artículo.
* Descripción
* Si una gravedad está oculta en Workfront

  Para obtener más información acerca de cómo ocultar una gravedad, vea [Crear o editar una gravedad de problema](#create-or-edit-an-issue-severity")

* Eliminar una gravedad

  Al hacerlo, debe seleccionar una gravedad de reemplazo.

## Crear o editar una gravedad de problema {#create-or-edit-an-issue-severity}

Como administrador de Workfront, puede crear y editar gravedades de problemas para adaptarlas a las necesidades de los usuarios.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Preferencias del proyecto** > **Gravedades**.

1. Si está creando una gravedad nueva, haga clic en **Agregar una gravedad nueva**.
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
      <td>Aumente o reduzca el nivel de gravedad, asignado originalmente por Workfront, para la gravedad.
      <p>El número de importancia de cada gravedad debe ser único. El número más alto corresponde al nivel más alto de gravedad.</p> <p>No puede editar este número después de guardar la gravedad.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Color</td> 
      <td> <p>Elija un color para la gravedad.</p> 
      <p>El color de la gravedad se utiliza en los informes de gráficos al agrupar los resultados por gravedad del problema. Para obtener información sobre los informes de gráficos, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Agregar un gráfico a un informe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gravedad predeterminada</td> 
      <td>Seleccione la gravedad en la que desea que Workfront seleccione automáticamente todos los problemas recién creados.</p>
      <p>La gravedad cosmética es la predeterminada para los problemas en Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba una descripción de la gravedad para explicar su función.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar</td> 
      <td> Oculte una gravedad que ya no sea necesaria. 
      <p>Una gravedad oculta no se muestra en ninguna parte de Workfront, por lo que los usuarios no pueden elegirla para sus problemas.</p> 
      <p><b>IMPORTANTE</b>: En lugar de eliminar gravedades que ya no desea usar, le sugerimos que las oculte. De este modo, se conservan todos los datos históricos de los objetos ya completados con la gravedad, al tiempo que se evita que las personas utilicen la gravedad en el futuro.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Para cambiar el orden en que aparecen las gravedades, arrastre y suelte las gravedades en el orden que desee.

   Esto cambia el orden en que se muestran para los problemas. No cambia el número **Importance**.

1. Haga clic en **Guardar**.

Para obtener más información sobre cómo usar gravedades mientras se trabaja con problemas, consulte [Actualizar la gravedad del problema](../../../manage-work/issues/issue-information/update-issue-severity.md).
