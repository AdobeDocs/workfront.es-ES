---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: mostrar tareas principales'
description: Puede aplicar los filtros de tareas siguientes para mostrar las tareas de trabajo. Las tareas de trabajo son tareas que se pueden trabajar de forma independiente y no son tareas principales de otras tareas. En un ejemplo, un filtro identifica las tareas secundarias que podrían ser principales a su vez. En este caso, no son tareas de trabajo.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 63%

---

# Filtro: mostrar tareas principales

<!--Audited: 10/2024-->

Puede aplicar los filtros de tareas siguientes para mostrar las tareas de trabajo. Las tareas de trabajo son tareas que se pueden trabajar de forma independiente y no son tareas principales de otras tareas. En un ejemplo, un filtro identifica las tareas secundarias que podrían ser principales a su vez. En este caso, no son tareas de trabajo.

>[!TIP]
>
>* Si tiene en cuenta la posibilidad de añadir más de un filtro a un informe, le recomendamos que añada todos los filtros mediante la interfaz de Report Builder y que haga clic en Cambiar al modo de texto después de haber añadido todas las demás reglas de filtro. A continuación, puede añadir el código para el filtro de tarea principal tal como se indica más arriba. 
>* También se recomienda añadir una agrupación para Nombre del proyecto para facilitar la lectura del informe. Para obtener más información sobre cómo añadir agrupaciones a los informes, consulte el artículo [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>

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

## Mostrar tareas sin tareas secundarias (podrían tener una principal)

Puede aplicar el siguiente filtro a un informe de tareas para mostrar tareas sin tareas secundarias. Podrían tener padres propios y ser hijos de otras tareas.

1. Desde el **Menú principal** ![icono del Menú principal](assets/main-menu-icon.png) en la esquina superior derecha, o desde el **Menú principal** ![Líneas del menú principal](assets/lines-main-menu.png) en la esquina superior izquierda, si están disponibles, haga clic en **Informes**.

1. Haga clic en **Nuevo informe**.
1. Seleccione un **Informe de tareas**.
1. Haga clic en **Filtros**.
1. Haga clic en **Añadir regla de filtro**.
1. En la línea **Empiece a escribir el nombre del campo ...**, empiece a escribir **Número de elementos secundarios** y, a continuación, haga clic en **Tarea >> Número de elementos secundarios** cuando se muestre en la lista.

1. Seleccione **Igual (con distinción de mayúsculas y minúsculas)** para el modificador y, a continuación, escriba **0** para el número de elementos tareas secundarias.\
   ![Filtro de tarea principal](assets/parent-task-filter-from-the-ui-350x76.png)

   O

   Haga clic en **Cambiar al modo de texto** y, en la ventana de edición de texto, copie y pegue el texto siguiente

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Haga clic en **Guardar + Cerrar**.

   Esto extrae un informe de todas las tareas que son tareas de trabajo en su sistema. Algunas de estas tareas podrían tener una tarea principal, pero no son tareas principales en sí mismas.

## Mostrar tareas con las tareas principales (podrían ser secundarias)

Puede aplicar el siguiente filtro a un informe de tareas para mostrar las tareas con las principales, lo que significa que son tareas secundarias. Sin embargo, estas tareas también podrían tener tareas secundarias propias porque el filtro no excluye a sus tareas secundarias. Las tareas secundarias, que también son principales respecto a otras tareas, no se consideran laborales.

1. Desde el **Menú principal** ![icono del Menú principal](assets/main-menu-icon.png) en la esquina superior derecha, o desde el **Menú principal** ![Líneas del menú principal](assets/lines-main-menu.png) en la esquina superior izquierda, si están disponibles, haga clic en **Informes**.

1. Haga clic en **Nuevo informe**.
1. Seleccione un **Informe de tareas**.
1. Haga clic en **Filtros**.
1. Haga clic en **Añadir regla de filtro**.
1. En la línea **Empiece a escribir el nombre del campo ...**, empiece a escribir **Id. principal** y, a continuación, seleccione **Tarea >> Id. principal** cuando se muestre en la lista.
1. Seleccione **No está en blanco** para el modificador.

   ![El identificador principal no está en blanco](assets/filter-parent-id-not-blank-350x100.png)

   O

   Haga clic en **Cambiar al modo de texto** y, en la ventana de edición de texto, copie y pegue el texto siguiente: 

   `parentID_Mod=notblank`

1. Haga clic en **Guardar + Cerrar**.

   Se extraerá un informe de todas las tareas del sistema que tienen tareas principales y son tareas secundarias de esas tareas principales. Algunas de estas tareas podrían ser ellas mismas principales.

## Mostrar tareas sin tareas secundarias ni principales (tareas independientes)

Puede aplicar el siguiente filtro a un informe de tareas para mostrar las tareas de trabajo independientes. Estas tareas no tienen padres y no tienen hijos propios.

1. Desde el **Menú principal** ![icono del Menú principal](assets/main-menu-icon.png) en la esquina superior derecha, o desde el **Menú principal** ![Líneas del menú principal](assets/lines-main-menu.png) en la esquina superior izquierda, si están disponibles, haga clic en **Informes**.

1. Haga clic en **Nuevo informe**.
1. Seleccione un **Informe de tareas**.
1. Haga clic en **Filtros**.
1. Haga clic en **Añadir regla de filtro**.
1. En el **Empiece a escribir el nombre del campo ...**, empiece a escribir la línea **Número de tareas secundarias** y, a continuación, seleccione **Tarea >> Número de tareas secundarias** en la lista.
1. Seleccione **Igual (con distinción de mayúsculas y minúsculas)** para el modificador y, a continuación, escriba **0** para el número de elementos tareas secundarias.
1. Haga clic en **Agregar otra regla de filtro**.
1. En el **Empiece a escribir el nombre del campo ...**, empiece a escribir la línea **Id. principal** y, a continuación, seleccione **Tarea >> Id. principal** en la lista.
1. Seleccione **Está en blanco** para el modificador.

   ![El identificador principal está en blanco y no hay elementos secundarios](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   O

   En lugar de los pasos 6-10 <!--ensure steps above stay accurate-->, haga clic en **Cambiar al modo de texto** y en la ventana de edición de texto, copie y pegue el siguiente texto:

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Haga clic en **Guardar + Cerrar**.

   Se extrae un informe de todas las tareas del sistema que no tienen tareas principales ni secundarias. Son tareas de trabajo independientes.
