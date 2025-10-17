---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Ver y administrar los elementos eliminados recientemente de un grupo
description: Cuando visualiza un grupo que administra en el área Grupos, puede ver, filtrar, restaurar y exportar los elementos de trabajo, documentos y plantillas eliminados recientemente.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 91%

---

# Ver y administrar los elementos eliminados recientemente de un grupo

Cuando visualiza un grupo que administra en el área de Grupos, puede ver y trabajar con los proyectos, tareas, problemas, documentos y plantillas eliminados recientemente de las siguientes maneras:

* Ver, filtrar y agrupar una lista de elementos eliminados recientemente
* Restaurar los elementos eliminados recientemente que seleccione
* Exportar una lista de elementos eliminados recientemente

Si hay grupos por encima del suyo, sus administradores también pueden hacer estas cosas por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Para obtener más información sobre los elementos eliminados, consulte [Administrar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr>
   <td>Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
  </tr>
  <tr> 
   <td>Permisos de objeto</td>
   <td>Los elementos eliminados deben estar asociados al grupo o a cualquiera de sus subgrupos.</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver y administrar los elementos eliminados recientemente de un grupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

1. Haga clic en el nombre del grupo.
1. En el panel izquierdo, haga clic en **Eliminados recientemente**.
1. Abra una de las siguientes pestañas en las que quiera ver y administrar los elementos eliminados recientemente del grupo:

   * Proyectos
   * Tareas
   * Problemas
   * Documentos
   * Plantillas

   Cada pestaña enumera elementos del tipo de objeto correspondiente que pertenecen al grupo actual o a sus subgrupos y que se eliminaron en los últimos 30 días.

   >[!NOTE]
   >
   >Si alguien eliminó un proyecto, todas sus tareas, problemas y documentos individuales se eliminaron con él. No se muestran individualmente en las pestañas Tareas, Problemas, Documentos o Plantillas. Sin embargo, al restaurar el proyecto también se restauran todos estos objetos secundarios en el proyecto.
   >
   >
   >Si alguien ha eliminado una tarea, un problema, un documento o una plantilla de forma individual, puede verlo y administrarlo en la pestaña correspondiente.

1. Complete cualquiera de las siguientes acciones:

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
      <td> <p>En la esquina superior derecha, sobre la lista, utilice <strong>Filtrar</strong> para definir lo que se mostrará según los criterios que proporcione. Utilice <strong>Ver</strong> para definir qué campos se muestran como columnas. Utilice <strong>Agrupación</strong> para agrupar los elementos en categorías.</p> </td> 
     </tr> 
    </tbody> 
   </table>
