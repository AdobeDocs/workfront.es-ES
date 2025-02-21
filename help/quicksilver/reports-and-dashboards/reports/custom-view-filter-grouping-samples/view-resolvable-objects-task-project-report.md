---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: Objetos solucionables en un informe de tarea o proyecto"
description: Puede mostrar una lista de todos los objetos solucionables en una vista de proyecto o tarea o informe.
author: Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 17a277a5a63a521ec7285e3f5051bfd42fc204bf
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Ver: Objetos solucionables en un informe de tarea o proyecto

<!--Audited: 11/2024-->

Puede mostrar una lista de todos los objetos solucionables en una vista de proyecto o tarea o informe.

Para obtener más información acerca de los objetos solucionables, vea el artículo [Información general sobre la resolución y los objetos solucionables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![lista_de_solucionables_en_informe.png](assets/list-of-resolvables-in-report-350x54.png)

La aplicación de esta vista es idéntica para tareas y proyectos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p> Actual: 
   <ul>
   <li>Solicitud para modificar una vista</li> 
   <li>Plan para modificar un informe</li>
   </ul>
     </p>
     <p> Nuevo: 
   <ul>
   <li>Colaborador para modificar una vista</li> 
   <li>Estándar para modificar un informe</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver objetos solucionables en un informe de tarea o proyecto

1. Vaya a una lista de tareas o proyectos que se han convertido desde problemas.
1. En el menú desplegable **Vista**, haz clic en **Nueva vista**.

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
