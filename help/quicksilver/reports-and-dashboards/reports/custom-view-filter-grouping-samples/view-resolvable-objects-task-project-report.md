---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Objetos solucionables en un informe de tarea o proyecto'
description: Puede mostrar una lista de todos los objetos solucionables en una vista de proyecto o tarea o informe.
author: Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 30%

---

# Vista: objetos que se pueden resolver en un informe de tarea o proyecto

<!--Audited: 11/2024-->

Puede mostrar una lista de todos los objetos solucionables en una vista de proyecto o tarea o informe.

Para obtener más información acerca de los objetos solucionables, vea el artículo [Información general sobre la resolución y los objetos solucionables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![lista_de_solucionables_en_informe.png](assets/list-of-resolvables-in-report-350x54.png)

La aplicación de esta vista es idéntica para tareas y proyectos.

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
   <p>Colaborador o solicitud para modificar una vista </p>
   <p>Estándar o Plan para modificar un informe</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Edición del acceso a Filtros, Vistas y Agrupaciones para modificar una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Ver objetos solucionables en un informe de tarea o proyecto

1. Vaya a una lista de tareas o proyectos que se han convertido desde problemas.
1. En el menú desplegable **Vista**, haga clic en **Nueva vista**.

1. En el área **Vista previa de columna**, haga clic en **Agregar columna**.

1. Haga clic en el encabezado de la nueva columna y, a continuación, haga clic en **Cambiar al modo de texto** > **Editar modo de texto**.
1. Elimine el texto que encuentre en el cuadro **Editar modo de texto** y reemplácelo por el siguiente código:

   ```
   displayname=Resolvables
   listdelimiter=<br>
   listmethod=nested(resolvables).lists
   textmode=true
   type=iterate
   valuefield=name
   valueformat=HTML
   ```

1. Haga clic en **Listo** > **Guardar vista**.\
   Se muestra una lista de todos los objetos solucionables en la nueva columna. Los nombres de los objetos de la lista no se pueden vincular directamente a los objetos.
