---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupación: desglose de porcentaje de tarea 2'
description: 'En esta agrupación de tareas personalizada, puede mostrar las tareas agrupadas por un rango de sus valores de porcentaje completado. Los desgloses muestran un valor de porcentaje completado de incrementos de 10 puntos porcentuales: 1-10%, 11-20%, etc.'
author: Nolan
feature: Reports and Dashboards
exl-id: 7d5a40dd-d451-48c7-9323-af52aa387709
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 59%

---

# Agrupación: desglose de porcentaje de tarea 2

<!--Audited: 10/2024-->

En esta agrupación de tareas personalizada, puede mostrar las tareas agrupadas por un rango de sus valores de porcentaje completado. Los desgloses muestran un valor de porcentaje completado de incrementos de 10 puntos porcentuales: 1-10%, 11-20%, etc.

La siguiente agrupación organiza los proyectos por el valor de porcentaje completado en una de estas agrupaciones:

* 0 %
* 1-10 %
* 11-20 %
* 21-30 %
* 31-40 %
* 41-50 %
* 51-60 %
* 61-70 %
* 71-80 %
* 81-90 %
* 91-99 %
* 100 %

![task_10__desglose_grouping.png](assets/task-10--breakdown-grouping-350x547.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o solicitud para modificar un filtro </p>
   <p>Estándar o Plan para modificar un informe</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Acceso de edición a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agrupar por desglose de porcentaje de tareas

Para aplicar esta agrupación:

1. Vaya a una lista de tareas.
1. En el menú desplegable **Agrupación**, seleccione **Nueva agrupación**.
1. Haga clic en **Agregar agrupación**.

1. Haga clic en **Cambiar a modo de texto**.
1. Quitar el texto del área **Agrupar por**.
1. Reemplace el texto por el código siguiente :

   ```
   group.0.linkedname=direct
   group.0.name=Percent Breakdown
   group.0.notime=false
   group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=11,"1-10 %",IF({percentComplete}<=21,"11-20 %",IF({percentComplete}<=31,"21-30 %",IF({percentComplete}<41,"31-40 %",IF({percentComplete}<51,"41-50 %",IF({percentComplete}<61,"51-60 %",IF({percentComplete}<71,"61-70 %",IF({percentComplete}<81,"71-80 %",IF({percentComplete}<91,"81-90 %",IF({percentComplete}<100,"91-99 %","100 %")))))))))))
   textmode=true
   ```

1. Haga clic en **Listo** > **Guardar agrupación**.
1. (Opcional) Actualice el nombre de la agrupación y, a continuación, haga clic en **Guardar agrupación**.
