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
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '939'
ht-degree: 1%

---

# Agregar proyectos a metas en Adobe Workfront Goals

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

Puede conectar proyectos a metas para indicar cómo progresa la meta, según el progreso real del proyecto. El proyecto se convierte en un indicador de progreso para la meta.

Al conectar los proyectos con las metas, puede vincular la planificación estratégica (las metas) de su organización al trabajo real que sus recursos realizan y completan cada día (los proyectos).

>[!IMPORTANT]
>
>Los objetivos de nivel de proyecto creados en el área de Caso comercial de un proyecto no están conectados a objetivos estratégicos creados en Objetivos de Workfront. Para obtener información sobre los objetivos del proyecto de caso empresarial, consulte [Crear metas de caso comercial](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> 
   <p>Para el nuevo plan y la estructura de licencias:
  <ul><li>Un plan definitivo </li>
  O
  <li>Licencia adicional para objetivos de Adobe Workfront para los planes Prime o Select Adobe Workfront. </li></ul> </p>
<p>Para el plan y la estructura de licencias actuales: 
<ul><li> A Pro o superior </li>
  <li>Una licencia de Adobe Workfront Goals además de una licencia de Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront*</td>
 <td>
 <p>Nueva licencia: Colaborador o superior</p>
 O
 <p>Licencia actual: Solicitud o superior</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Resumen de licencias de Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Producto*</td>
 <td>
 <p> Nuevo requisito de producto, uno de los siguientes: </p>
<ul>
<li>Un plan Select or Prime Adobe Workfront y una licencia adicional de Adobe Workfront Goals.</li>
<li>Un plan Ultimate Workfront que incluye Workfront Goals de forma predeterminada. </li></ul>
 <p>O</p>
 <p>Requisito de producto actual: un plan de Workfront y una licencia adicional para los objetivos de Adobe Workfront. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para utilizar Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Nivel de acceso</td>
 <td> <p>Editar acceso a Objetivos</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <div>
  <p>Ver o permisos superiores a la meta para verla</p>
  <p>Administrar permisos para el objetivo y editarlo</p>
  <p>Para obtener información sobre cómo compartir objetivos, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir una meta en Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área Objetivos en el menú principal. </p>  
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

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Cuando se elimina un proyecto adjunto a una meta, también se elimina de la meta.

  >[!CAUTION]
  >
  >Si la meta estaba activa antes de que eliminara el proyecto y no hay otros indicadores de progreso en la meta, la meta se vuelve Inactiva.


## Agregar proyectos a metas

1. Haga clic en **Menú principal** ![](assets/main-menu-icon.png) (redacte esto para Shell: o haga clic en el botón **Menú principal** ![](assets/three-line-main-menu-icon.png) en la esquina superior izquierda, si está disponible.) , **Metas**.
1. En la Lista de metas, haga clic en el nombre de una meta para abrir su página.
1. Clic **Indicadores de progreso** en el panel izquierdo.
1. Desde el **Nuevo indicador de progreso** , haga clic en **Agregar proyecto existente**.

   Se muestra el cuadro Agregar proyectos a la meta.
1. (Opcional) Actualice el **Ver**, **Filtrar**, o **Agrupación** haciendo clic en los iconos correspondientes en la esquina superior derecha de la lista para modificar la forma en que se muestra la lista de proyectos.
1. (Opcional) Haga clic en **Buscar** icono ![](assets/search-icon.png) y empiece a escribir el nombre de un proyecto para encontrarlo rápidamente en la lista.
1. Seleccione los proyectos que desee agregar a la meta y haga clic en **Añadir**.

   Los proyectos seleccionados se añaden a la meta y se muestran en la sección Progreso indicators de la página de la meta, bajo la etiqueta **Proyecto** agrupación.

   Después de activar la meta, su progreso se actualiza automáticamente cuando se actualiza el progreso de un proyecto. Para obtener información sobre cómo activar un objetivo, consulte [Activar metas en Adobe Workfront Goals](../goal-management/activate-goals.md).

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
| Jerarquía de metas | La jerarquía a la que pertenece un objetivo. En este campo solo se muestran los padres de la meta y la meta. Las metas secundarias no se muestran. |
| Número de metas vinculadas | Número de metas vinculadas a un proyecto. |
