---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Ver y administrar los elementos eliminados recientemente de un grupo
description: Cuando vea un grupo que administra en el área Grupos, puede ver, filtrar, restaurar y exportar los elementos de trabajo, documentos y plantillas eliminados recientemente.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 1%

---

# Ver y administrar los elementos eliminados recientemente de un grupo

Cuando está viendo un grupo que administra en el área de Grupos, puede ver y trabajar con los proyectos, tareas, problemas, documentos y plantillas eliminados recientemente de las siguientes maneras:

* Ver, filtrar y agrupar una lista de elementos eliminados recientemente
* Restaurar los elementos eliminados recientemente que seleccione
* Exportar una lista de elementos eliminados recientemente

Si hay grupos por encima de su grupo, sus administradores también pueden hacer estas cosas por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Para obtener más información sobre los elementos eliminados, vea [Administrar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Los elementos eliminados deben estar asociados al grupo o a cualquiera de sus subgrupos. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

+++

## Ver y administrar los elementos eliminados recientemente de un grupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo.
1. En el panel izquierdo, haga clic en **Eliminados recientemente**.
1. Abra una de las siguientes pestañas donde desee ver y administrar los elementos eliminados recientemente del grupo:

   * Proyectos
   * Tareas
   * Problemas
   * Documentos
   * Plantillas

   Cada ficha enumera elementos del tipo de objeto correspondiente que pertenecen al grupo actual o a sus subgrupos y que se eliminaron en los últimos 30 días.

   >[!NOTE]
   >
   >Si alguien eliminó un proyecto, todas sus tareas, problemas y documentos individuales se eliminaron con él. No se muestran individualmente en las fichas Tareas, Problemas, Documentos o Plantillas. Sin embargo, al restaurar el proyecto también se restauran todos estos objetos secundarios en el proyecto.
   >
   >
   >Si alguien ha eliminado una tarea, un problema, un documento o una plantilla de forma individual, puede verla y administrarla en la pestaña correspondiente.

1. Realice una de las siguientes acciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Restaurar objetos</p> </td> 
      <td> <p>Seleccione hasta 10 objetos y luego haga clic en <strong>Restaurar</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Exportar toda la lista de objetos en la pestaña</p> </td> 
      <td> <p>Haga clic en <strong>Exportar</strong>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>Cambiar la visualización de la información en la lista</p> </td> 
      <td> <p>En la esquina superior derecha sobre la lista, usa <strong>Filter</strong> para definir lo que se mostrará según los criterios que proporciones. Use <strong>Ver</strong> para definir qué campos se muestran como columnas. Use <strong>Agrupación</strong> para agrupar los elementos en categorías.</p> </td> 
     </tr> 
    </tbody> 
   </table>
