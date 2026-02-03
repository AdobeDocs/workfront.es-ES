---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Ver todas las actualizaciones en un informe de notas
description: Para ver todas las actualizaciones que cualquiera de los usuarios ha introducido para un objeto, puede crear un informe de nota que muestre todas las actualizaciones.
author: Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 11%

---

# Ver todas las actualizaciones en un informe de notas

<!-- Audited: 10/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

El área Actualizaciones de un objeto muestra un número máximo de 200 actualizaciones de forma predeterminada. Para ver todas las actualizaciones que cualquiera de los usuarios ha introducido para un objeto, puede crear un informe de nota que muestre todas las actualizaciones.

>[!NOTE]
>
>Puede crear un informe para ver las actualizaciones de los objetos en Vista previa con el informe Entrada de cuaderno. Para obtener más información, consulte [Informe sobre el área de actualizaciones con un informe de entrada de diario](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso con capacidad para crear lo siguiente:</p> 
    <ul> 
     <li> <p>Informes, paneles de control y calendarios</p> </li> 
     <li> <p>Filtros, vistas y agrupaciones</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver los permisos de los objetos en el informe</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View</p>
    <p>Note: If you do not have View permission or higher to an object, information for that object doesn't display in the report.</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Creación de un informe de notas

La creación de un informe para Notas para cualquier objeto es idéntica, independientemente del objeto.

Por ejemplo, para crear un informe de notas para todas las notas de un proyecto:

{{step1-to-reports}}

1. En la esquina superior izquierda de la página, haga clic en **Nuevo informe** y, a continuación, seleccione **Nota**.

1. (Opcional) Haga clic en **(Columnas) Ver**, luego en **Agregar columna** para agregar el **Nombre** del **Proyecto** en la vista del informe.

1. (Opcional) Si realiza informes sobre varios proyectos al mismo tiempo, haga clic en **Agrupaciones** y, a continuación, en **Agregar agrupación** al grupo por el **Nombre** del **Proyecto**. Esto garantiza que las notas se agrupen por sus respectivos proyectos, lo que facilita la lectura del informe.

1. (Opcional) Haga clic en **Filtros** y, a continuación, **Agregar una regla de filtro**.
1. Agregar un filtro para **Nota** > **Texto de la nota** > **No está en blanco**.

   ![El campo de texto de nota no está vacío](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Si se actualizó un campo de proyecto pero no se agregó ninguna nota en el momento de la actualización, el **Texto de la nota** de la actualización se muestra como **(No se agregó texto para la actualización)**.


1. (Opcional) Agregue otro filtro para **Proyecto** > **Nombre** > **Es igual a** y agregue uno o varios nombres de proyecto para los que desee ver notas.
1. Haga clic en **Guardar + Cerrar**. Todas las actualizaciones introducidas en el proyecto por todos los usuarios con permisos para Ver el proyecto se muestran en el informe.
