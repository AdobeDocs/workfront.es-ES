---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Ver todas las actualizaciones en un informe de notas
description: Ver todas las actualizaciones en un informe de notas
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 36bdacb5f6d04245552aeeb4ab82d210597645a2
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 1%

---

# Ver todas las actualizaciones en un informe de notas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

El área Actualizaciones de un objeto muestra un número máximo de 200 actualizaciones de forma predeterminada. Para ver todas las actualizaciones que cualquiera de los usuarios ha introducido para un objeto, puede crear un informe de nota que muestre todas las actualizaciones.

>[!NOTE]
>
>Puede crear un informe para ver las actualizaciones de los objetos en Vista previa con el informe Entrada de cuaderno. Para obtener más información, consulte [Informe sobre el área de actualizaciones](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Nuevo: estándar </p>
   <p>Actual: plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>Editar acceso a:</p> 
    <ul> 
     <li> <p>Creación de informes, tableros y calendarios</p> </li> 
     <li> <p>Creación de filtros, vistas y agrupaciones</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver</p> <p><b>NOTA</b></p>
   <p>Si no tiene permiso de visualización o superior para un objeto, la información de ese objeto no se muestra en el informe.</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Creación de un informe de notas

La creación de un informe para Notas para cualquier objeto es idéntica, independientemente del objeto.

Por ejemplo, para crear un informe de notas para todas las notas de un proyecto:

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, elija **Nota**.

1. (Opcional) Haga clic en **Vistas**, luego en **Agregar columna** para agregar el **Nombre** del **Proyecto** en la vista del informe. 

1. (Opcional) Haga clic en **Agrupaciones** y, a continuación, en **Agregar agrupación** al grupo por el **Nombre del proyecto**, si realiza informes sobre varios proyectos al mismo tiempo.\
   Esto garantiza que las notas se agrupen por sus respectivos proyectos, lo que facilita la lectura del informe. 

1. (Opcional) Haga clic en **Filtros,** y después en **Agregar una regla de filtro**.
1. Agregar un filtro para **Nota** > **Texto de la nota** > **No está en blanco**.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Si se actualizó un campo de proyecto pero no se agregó ninguna nota en el momento de la actualización, el **Texto de la nota** de la actualización se muestra como **(No se agregó texto para la actualización)**.


1. (Opcional) Agregue otro filtro para **Proyecto** > **Nombre** > **Es igual a** y agregue uno o varios nombres de proyecto para los que desee ver notas.
1. Haga clic en **Guardar + Cerrar**.\
   Todas las actualizaciones introducidas en el proyecto por todos los usuarios con permisos de al menos Ver el proyecto se muestran en el informe.
