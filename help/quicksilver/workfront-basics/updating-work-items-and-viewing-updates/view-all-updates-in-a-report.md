---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Ver todas las actualizaciones en un informe de notas
description: Para ver todas las actualizaciones que cualquiera de los usuarios ha introducido para un objeto, puede crear un informe de nota que muestre todas las actualizaciones.
author: Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 15%

---

# Ver todas las actualizaciones en un informe de notas

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

El área Actualizaciones de un objeto muestra un número máximo de 200 actualizaciones de forma predeterminada. Para ver todas las actualizaciones que cualquiera de los usuarios ha introducido para un objeto, puede crear un informe de nota que muestre todas las actualizaciones.

>[!NOTE]
>
>Puede crear un informe para ver las actualizaciones de los objetos en Vista previa con el informe Entrada de cuaderno. Para obtener más información, consulte [Informe sobre el área de actualizaciones con un informe de entrada de diario](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: estándar </p>
   <p>Actual: plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a:</p> 
    <ul> 
     <li> <p>Creación de informes, paneles de control y calendarios</p> </li> 
     <li> <p>Creación de filtros, vistas y agrupaciones</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver</p>
    <p>Nota: Si no tiene permiso de visualización o superior para un objeto, la información de ese objeto no se muestra en el informe.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Creación de un informe de notas

La creación de un informe para Notas para cualquier objeto es idéntica, independientemente del objeto.

Por ejemplo, para crear un informe de notas para todas las notas de un proyecto:

{{step1-to-reports}}

1. En la esquina superior izquierda de la página, haga clic en **Nuevo informe** y, a continuación, seleccione **Nota**.

1. (Opcional) Haga clic en **(Columnas) Ver**, luego en **Agregar columna** para agregar el **Nombre** del **Proyecto** en la vista del informe. 

1. (Opcional) Si realiza informes sobre varios proyectos al mismo tiempo, haga clic en **Agrupaciones** y, a continuación, en **Agregar agrupación** al grupo por el **Nombre** del **Proyecto**. Esto garantiza que las notas se agrupen por sus respectivos proyectos, lo que facilita la lectura del informe. 

1. (Opcional) Haga clic en **Filtros** y, a continuación, **Agregar una regla de filtro**.
1. Agregar un filtro para **Nota** > **Texto de la nota** > **No está en blanco**.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Si se actualizó un campo de proyecto pero no se agregó ninguna nota en el momento de la actualización, el **Texto de la nota** de la actualización se muestra como **(No se agregó texto para la actualización)**.


1. (Opcional) Agregue otro filtro para **Proyecto** > **Nombre** > **Es igual a** y agregue uno o varios nombres de proyecto para los que desee ver notas.
1. Haga clic en **Guardar + Cerrar**. Todas las actualizaciones introducidas en el proyecto por todos los usuarios con permisos para Ver el proyecto se muestran en el informe.
