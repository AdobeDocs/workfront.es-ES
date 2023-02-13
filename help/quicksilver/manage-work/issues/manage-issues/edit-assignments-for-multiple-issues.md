---
product-area: projects
navigation-topic: manage-issues
title: Modificar asignaciones de usuario para varios problemas en una lista
description: Modificar asignaciones de usuario para varios problemas en una lista
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 7e77223595d3c9cf0d6592a09e893142439adb2c
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# Modificar asignaciones de usuario para varios problemas en una lista

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

Puede modificar simultáneamente las asignaciones de usuario a varios problemas. Para obtener información sobre la edición o asignación de problemas de uno en uno, consulte también los siguientes artículos:

* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Asignación de problemas](../../../manage-work/issues/manage-issues/assign-issues.md)

Para obtener información general sobre la asignación de problemas, consulte [Información general sobre la modificación de asignaciones de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Debe tener al menos permisos de Contribute para un problema para poder realizar asignaciones al problema.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el problema</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
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
1. (Opcional) Cree un filtro para mostrar solo los problemas asignados al usuario asignado que desea modificar.

   Por ejemplo, puede crear un filtro para mostrar solo los problemas con una función específica como usuario asignado. A continuación, puede reemplazar la función por un usuario específico. Haga lo siguiente:

   1. Haga clic en el **Filtro** lista desplegable y haga clic en **Nuevo filtro**.

      Aparece el cuadro de diálogo Nuevo filtro .

   1. Haga clic en **Agregar una regla de filtro.**
   1. Para filtrar por una función específica, expanda **Funciones de asignación,** a continuación, haga clic en **ID.**

      O

      Para filtrar para un usuario específico, expanda **Usuarios de asignación,** a continuación, haga clic en **ID.**

      >[!TIP]
      >
      >No use **Asignado a** porque este campo hace referencia únicamente al propietario del problema y no a todos los usuarios asignados.

   1. En la lista desplegable , seleccione **Igual** como calificador de filtro.
   1. Empiece a escribir el nombre del usuario o función que desea filtrar y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
   1. Haga clic en **Guardar filtro.**

1. Seleccione los problemas para los que desea modificar las asignaciones y haga clic en el botón **Editar** icono ![](assets/qs-edit-icon.png).

   La variable **Editar problemas** se muestra. Los elementos editados se muestran en la esquina superior izquierda de la página.

1. Vaya a la **Asignaciones** y, a continuación, seleccione **Usuario asignado**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. Realice una de las siguientes acciones:

   1. Para agregar un nuevo usuario asignado:

      1. Empiece a escribir el nombre de un usuario, función o equipo y, a continuación, selecciónelo cuando aparezca en la lista. La asignación se agrega y no reemplaza las asignaciones actuales en los problemas seleccionados.

         >[!TIP]
         Puede asignar varios usuarios, funciones de trabajo o equipos. Solo puede asignar usuarios activos, funciones de trabajo y equipos.
         Si se asignó un usuario, una función de trabajo o un equipo antes de desactivarlos, se asignarán al elemento de trabajo. En este caso, se recomienda lo siguiente:
         * Reasigne el elemento de trabajo a los recursos activos.
         * Asocie a los usuarios de un equipo desactivado con un equipo activo y reasigne el elemento de trabajo al equipo activo.


         Se muestra la información que es común en todos los problemas seleccionados. Por ejemplo, si el mismo usuario está asignado a todos los problemas, ese usuario se muestra en la **Usuario asignado** para abrir el Navegador. Si la información no es común en los problemas seleccionados, no se muestra ninguna información.
   1. Para eliminar a los usuarios asignados individuales:

      1. Haga clic en el **Icono X** junto al nombre del usuario asignado que desea eliminar si el usuario asignado aparece en la lista Asignaciones.

         O

         (Condicional) Si el usuario asignado que desea eliminar no se muestra en la sección Asignaciones porque el usuario asignado está asignado a algunos de los problemas que ha seleccionado, haga clic en **Eliminar usuario asignado** y empiece a escribir el nombre del usuario asignado que desea eliminar y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

      1. Haga clic en **Eliminar usuario asignado** para agregar otro usuario asignado para eliminarlo.
   1. Para eliminar todos los usuarios asignados existentes:

      1. Haga clic en **Eliminar todos los asignados existentes** y haga clic en **Sí, Eliminar todos los usuarios asignados**.

         Esto elimina no solo a los asignadores comunes (los asignadores que se muestran en el cuadro de diálogo de edición), sino también a todos los asignadores en todos los problemas seleccionados.



1. (Opcional) Modifique cualquiera de las siguientes opciones para los usuarios asignados que seleccionó para asociar con los problemas:

   * **Propietario del problema:** Seleccione el botón de opción para indicar qué usuario asignado está designado como propietario de problemas. Si se deja sin seleccionar, Adobe Workfront designa el primer usuario asignado como propietario del problema. Esto no está disponible para asignaciones de equipo.
   * **Función del usuario asignado**: Seleccione una función en la lista desplegable. Si se deja sin seleccionar, Workfront selecciona automáticamente la función principal del usuario.

1. Haga clic en **Guardar cambios**.
