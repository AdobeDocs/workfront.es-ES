---
product-area: projects
navigation-topic: manage-issues
title: Modificar asignaciones de usuarios para varios problemas de una lista
description: Modificar asignaciones de usuarios para varios problemas de una lista
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 1%

---

# Modificar asignaciones de usuarios para varios problemas de una lista

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

Puede modificar simultáneamente las asignaciones de usuarios a varios problemas. Para obtener información sobre cómo editar problemas o asignarlos de uno en uno, consulte los siguientes artículos:

* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Asignar problemas](../../../manage-work/issues/manage-issues/assign-issues.md)

Para obtener información general sobre la asignación de problemas, consulte [Información general sobre la modificación de asignaciones de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Debe tener al menos permisos de Contribute para resolver un problema y poder realizar asignaciones a este.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el problema</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:&nbsp;drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:</p>
<ul>
<li>Users join or leave&nbsp;your team</li>
<li>A user takes a vacation that extends beyond the issue&nbsp;due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Modificar asignaciones para varios problemas

1. Vaya a la lista de problemas que contiene los problemas cuyas asignaciones desea modificar.
1. (Opcional) Cree un filtro para mostrar solo los problemas asignados al usuario asignado que desee modificar.

   Por ejemplo, puede crear un filtro para mostrar solo los problemas con una función específica como usuario asignado. A continuación, puede reemplazar la función por un usuario específico. Haga lo siguiente:

   1. Haga clic en la lista desplegable **Filtro** y luego haga clic en **Nuevo filtro**.

      Aparece el cuadro de diálogo Nuevo filtro.

   1. Haga clic en **Agregar una regla de filtro.**
   1. Para filtrar por un rol específico, expanda **Roles de asignación,** y luego haga clic en **ID.**

      O

      Para filtrar por un usuario específico, expanda **Usuarios de asignación,** y luego haga clic en **ID.**

      >[!TIP]
      >
      >No use **Asignado a** porque este campo hace referencia solamente al Propietario del problema y no a todas las personas asignadas.

   1. En la lista desplegable, seleccione **Equal** como calificador de filtro.
   1. Empiece a escribir el nombre del usuario o función para el que desea filtrar y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
   1. Haga clic en **Guardar filtro.**

1. Seleccione los problemas para los que desea modificar las asignaciones y, a continuación, haga clic en el icono **Editar** ![](assets/qs-edit-icon.png).

   Se muestra **Editar problemas**. Los elementos editados se muestran en la esquina superior izquierda de la página.

1. Vaya a la sección **Asignaciones** y, a continuación, seleccione **Usuario asignado**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. Realice una de las siguientes acciones:

   1. Para agregar un nuevo usuario asignado:

      1. Empiece a escribir el nombre de un usuario, rol o equipo y, a continuación, selecciónelo cuando aparezca en la lista. La asignación se agrega y no reemplaza las asignaciones actuales en los problemas seleccionados.

         >[!TIP]
         >
         >Puede asignar varios usuarios, roles o equipos. Solo puede asignar usuarios activos, roles y equipos.
         >
         >Si se asignó un usuario, un rol o un equipo antes de desactivarlos, permanecen asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
         >
         >* Reasignar el elemento de trabajo a los recursos activos.
         >* Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.

         Se muestra la información que es común en todos los problemas seleccionados. Por ejemplo, si se asigna el mismo usuario a todos los problemas, ese usuario se muestra en la columna **Usuario asignado**. Si la información no es común en los problemas seleccionados, no se muestra ninguna información.

   1. Para eliminar usuarios asignados individuales:

      1. Haga clic en el **icono X** junto al nombre del usuario asignado que desee eliminar si este aparece en la lista Asignaciones.

         O

         (Condicional) Si el usuario asignado que desea eliminar no aparece en la sección Asignaciones porque el usuario asignado solo está asignado a algunos de los problemas que ha seleccionado, haga clic en **Quitar usuario asignado** y empiece a escribir el nombre del usuario asignado que desea eliminar; a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

      1. Vuelva a hacer clic en **Quitar usuario asignado** para agregar otro usuario asignado que eliminar.

   1. Para eliminar todas las personas asignadas actualmente:

      1. Haga clic en **Quitar todas las personas asignadas existentes** y, a continuación, haga clic en **Sí, eliminar todas las personas asignadas**.

         Esto elimina no solo los usuarios asignados comunes (los usuarios asignados que se muestran en el cuadro de diálogo de edición), sino también todos los usuarios asignados de todos los problemas seleccionados.

1. (Opcional) Modifique cualquiera de las siguientes opciones para los usuarios asignados que seleccionó para asociar con los problemas:

   * **Propietario del problema:** Seleccione el botón de opción para indicar qué usuario asignado está designado como Propietario del problema. Si no se selecciona, Adobe Workfront designa al primer usuario asignado como propietario del problema. Esto no está disponible para asignaciones de equipo.
   * **Rol de asignado**: seleccione un rol de la lista desplegable. Si no se selecciona, Workfront selecciona automáticamente la función principal del usuario.

1. Haga clic en **Guardar cambios**.
