---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Agregar proyectos a metas en Adobe Workfront Goals
description: Puede conectar proyectos a metas para indicar cómo progresa la meta, según el progreso real del proyecto. El proyecto se convierte en un indicador de progreso para la meta.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 26%

---

# Agregar proyectos a metas en Adobe Workfront Goals

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

Puede conectar proyectos a metas para indicar cómo progresa la meta, según el progreso real del proyecto. El proyecto se convierte en un indicador de progreso para la meta.

Al conectar los proyectos con las metas, puede vincular la planificación estratégica (las metas) de su organización al trabajo real que sus recursos realizan y completan cada día (los proyectos).

>[!IMPORTANT]
>
>Los objetivos de nivel de proyecto creados en el área de Caso comercial de un proyecto no están conectados a objetivos estratégicos creados en Objetivos de Workfront. Para obtener información acerca de los objetivos del proyecto de caso empresarial, vea [Crear metas de caso empresarial](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> 
   <p>Para la nueva estructura de plan y licencias:
  <ul><li>Un plan Ultimate </li></ul>
   </p>
<p>Para la estructura actual de plan y licencias: 
<ul><li> Pro o superior </li>
  <li>Una licencia de Adobe Workfront Goals además de una licencia de Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront*</td>
 <td>
 <p>Nueva licencia: Contributor o superior</p>
 O
 <p>Licencia actual: Request o superior</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre las licencias de Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Producto*</td>
 <td>
 <p> Nuevo requisito de producto, uno de los siguientes: </p>
<ul>
<li>Un plan Select or Prime Adobe Workfront y una licencia adicional de Adobe Workfront Goals.</li>
<li>Un plan Ultimate Workfront que incluye Workfront Goals de forma predeterminada. </li></ul>
 <p>O</p>
 <p>Requisito de producto actual: un plan de Workfront y una licencia adicional para Adobe Workfront Goals. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Nivel de acceso</td>
 <td> <p>Editar acceso a Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <div>
  <p>Permisos Ver o superiores para la meta que desea ver</p>
  <p>Permisos de administración para la meta y poder editarla</p>
  <p>Para obtener información acerca de cómo compartir metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir una meta en Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área Metas en el menú principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Consideraciones sobre la conexión de proyectos a objetivos

* Puede agregar a un objetivo un proyecto que cumpla los siguientes criterios:

   * Debe tener al menos permisos para verlo.

     >[!NOTE]
     >
     >Si pierde los permisos para ver el proyecto después de haber adjuntado el proyecto a la meta, aún podrá ver información del proyecto en la meta, pero ya no podrá acceder al proyecto.

   * El proyecto no debe tener el estado Inactivo.

* Puede asociar varios proyectos con una meta.
* Puede asociar el mismo proyecto con varios objetivos.
* No se puede actualizar manualmente el progreso de un proyecto desde el objetivo al que está adjunto. En su lugar, Workfront calcula el porcentaje completado del proyecto y Workfront Goals calcula el progreso de la meta usando este porcentaje completado. Esto actualiza el objetivo en tiempo real después de actualizar el porcentaje del proyecto.
* La duración del proyecto puede estar fuera del período de tiempo de un objetivo. Si un proyecto dura más que la fecha límite de la meta, aún puede cerrar la meta y considerar que se ha completado, pero el porcentaje de objetivo completado no será del 100%. El porcentaje completado del proyecto ya no se actualiza en la meta.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![Goal closed](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Cuando se elimina un proyecto adjunto a una meta, también se elimina de la meta.

  >[!CAUTION]
  >
  >Si la meta estaba activa antes de que eliminara el proyecto y no hay otros indicadores de progreso en la meta, la meta se vuelve Inactiva.


## Agregar proyectos a metas

1. Haga clic en el **Menú principal** ![icono del menú principal](assets/main-menu-icon.png) (borrador de esto para Shell: o haga clic en el **Menú principal** ![Líneas del menú principal](assets/three-line-main-menu-icon.png) en la esquina superior izquierda, si está disponible.) , a continuación **Metas**.
1. En la Lista de metas, haga clic en el nombre de una meta para abrir su página.
1. Haga clic en **Indicadores de progreso** en el panel de la izquierda.
1. En el menú desplegable **Nuevo indicador de progreso**, haga clic en **Agregar proyecto existente**.

   Se muestra el cuadro Agregar proyectos a la meta.
1. (Opcional) Actualice **Ver**, **Filtro** o **Agrupación** haciendo clic en los iconos respectivos en la esquina superior derecha de la lista para modificar la forma en que se muestra la lista de proyectos.
1. (Opcional) Haga clic en el icono **Buscar** ![Icono de búsqueda](assets/search-icon.png) y empiece a escribir el nombre de un proyecto para encontrarlo rápidamente en la lista.
1. Seleccione los proyectos que desee agregar a la meta y luego haga clic en **Agregar**.

   Los proyectos seleccionados se agregan a la meta y se muestran en la sección Indicadores de progreso de la página de la meta, en la agrupación **Proyecto**.

   Después de activar la meta, su progreso se actualiza automáticamente cuando se actualiza el progreso de un proyecto. Para obtener información sobre cómo activar una meta, consulte [Activar metas en Adobe Workfront Goals](../goal-management/activate-goals.md).

## Buscar información del proyecto en las metas

<p>
La siguiente información del proyecto está visible a nivel de objetivo en la sección Indicadores de progreso de la página de un objetivo:

</p>

<table>
  <tr>
   <td>Nombre del proyecto
   </td>
   <td>Cualquier cambio en el nombre del proyecto también se reflejará en el proyecto conectado.
   </td>
  </tr>
  <tr>
   <td>Propietario del proyecto
   </td>
   <td>Cualquier cambio en el propietario del proyecto también se reflejará en el proyecto conectado.
   </td>
  </tr>
    <tr>
   <td>Progreso actual
   </td>
   <td> <p>Porcentaje completado del proyecto. No puede actualizar manualmente el porcentaje completado del proyecto desde el objetivo. Workfront lo calcula automáticamente en función del porcentaje completado de las tareas. </p>
   </td>
  </tr>
  <tr>
   <td>Progreso
   </td>
   <td>Porcentaje completado del proyecto representado por una barra. Cualquier cambio en el porcentaje completado del proyecto actualiza automáticamente el progreso de la meta a menos que se cierre la meta.
   </td>
  </tr>

</table>

## Buscar información de objetivos en proyectos

La siguiente información de objetivos es visible en una lista de proyectos o un informe:

| Información del objetivo | Descripción |
|---|---|
| Metas | Una lista de todas las metas que tienen un proyecto asociado. |
| Jerarquía de metas | La jerarquía a la que pertenece un objetivo. En este campo solo se muestran los elementos principales de la meta y la meta. Las metas secundarias no se muestran. |
| Número de metas vinculadas | Número de metas vinculadas a un proyecto. |
