---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: mostrar tareas principales'
description: Puede aplicar los filtros de tareas siguientes para mostrar las tareas de trabajo. Las tareas de trabajo son tareas que se pueden trabajar de forma independiente y no son tareas principales de otras tareas. En un ejemplo, un filtro identifica las tareas secundarias que podrían ser propias de los padres. En este caso, no están trabajando en tareas.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# Filtro: mostrar tareas principales

Puede aplicar los filtros de tareas siguientes para mostrar las tareas de trabajo. Las tareas de trabajo son tareas que se pueden trabajar de forma independiente y no son tareas principales de otras tareas. En un ejemplo, un filtro identifica las tareas secundarias que podrían ser propias de los padres. En este caso, no están trabajando en tareas.

>[!TIP]
>
>* Si tiene en cuenta la posibilidad de agregar más de un filtro a un informe, le recomendamos que agregue todos los filtros utilizando la interfaz del Creador de informes y que haga clic en Cambiar al modo Texto después de agregar todas las demás reglas de filtro. A continuación, puede añadir el código para el filtro de tareas principal como se ha indicado anteriormente. 
* También se recomienda agregar una agrupación para Nombre del proyecto para facilitar la lectura del informe. Para obtener más información sobre cómo agregar agrupaciones a los informes, consulte el artículo [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>


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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Mostrar tareas sin elementos secundarios (podrían tener un elemento principal)

Puede aplicar el siguiente filtro a un informe de tareas para mostrar tareas sin elementos secundarios. Pueden tener padres propios y ser hijos de otras tareas.

1. En el **Menú principal** ![](assets/main-menu-icon.png), haga clic en **Informes.**

1. Haga clic en **Nuevo informe**.
1. Seleccione un **Informe de tareas**.
1. Haga clic en **Filtros**.
1. Haga clic en **Agregar una regla de filtro**.
1. En el **Empiece a escribir el nombre del campo...** línea, empezar a escribir **Número de hijos**.

1. Select **Igual (con distinción de mayúsculas y minúsculas)** para el modificador, introduzca **0** para el número de hijos.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   O

   Haga clic en **Cambiar al modo de texto**, y en la ventana de edición de texto, copie y pegue el siguiente texto: 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Haga clic en **Guardar + Cerrar**.

   Esto extrae un informe para todas las tareas que están funcionando en el sistema. Algunas de estas tareas podrían tener un elemento principal, pero no son tareas principales en sí.

## Mostrar tareas con padres (podrían tener hijos)

Puede aplicar el siguiente filtro a un informe de tareas para mostrar las tareas con elementos principales, lo que significa que son tareas secundarias. Sin embargo, estas tareas también podrían tener hijos propios porque el filtro no excluye a sus hijos. Las tareas secundarias que también son padres para otras tareas no se consideran tareas de trabajo.

1. En el **Menú principal** ![](assets/main-menu-icon.png), haga clic en **Informes.
1. Haga clic en **Nuevo informe**.
1. Seleccione un **Informe de tareas**.
1. Haga clic en **Filtros**.
1. Haga clic en **Agregar una regla de filtro**.
1. En el **Empiece a escribir el nombre del campo...** línea, empezar a escribir **ID principal**.
1. Select **No está en blanco** para su modificador.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   O

   Haga clic en **Cambiar al modo de texto**, y en la ventana de edición de texto, copie y pegue el siguiente texto: 

   `parentID_Mod=notblank`

1. Haga clic en **Guardar + Cerrar**.

   Esto extrae un informe para todas las tareas del sistema que tengan padres y que sean tareas secundarias de esos padres. Algunas de estas tareas podrían ser propias de un padre.

## Mostrar tareas sin elementos secundarios y sin elementos principales (tareas independientes)

Puede aplicar el siguiente filtro a un informe de tareas para mostrar las tareas de trabajo independientes. Estas tareas no tienen un padre y no tienen hijos propios.

1. En el **Menú principal** ![](assets/main-menu-icon.png), haga clic en **Informes.**
1. Haga clic en **Nuevo informe**.
1. Seleccione un **Informe de tareas**.
1. Haga clic en **Filtros**.
1. Haga clic en **Agregar una regla de filtro** y en el **Empiece a escribir el nombre del campo...** introducción de línea **Número de hijos** select **Igual (con distinción de mayúsculas y minúsculas)** para el modificador, introduzca **0** para el número de hijos.
1. Haga clic en **Añadir otra regla de filtro** y en el **Empiece a escribir el nombre del campo...** introducción de línea **ID principal** y, a continuación, seleccione **Está en blanco**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   O

   En lugar de los pasos 6-7, haga clic en **Cambiar al modo de texto** y en la ventana de edición de texto, copie y pegue el siguiente texto: 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Haga clic en **Guardar + Cerrar**.

   Esto extrae un informe para todas las tareas del sistema que no tengan padres ni hijos. Son tareas de trabajo independientes.
