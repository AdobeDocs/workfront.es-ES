---
product-area: projects
navigation-topic: manage-issues
title: Modificar asignaciones de usuarios para varios problemas en una lista
description: Modificar asignaciones de usuarios para varios problemas en una lista
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 7aa420946115fc612ad1d9e310583e5453ae0678
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 97%

---

# Modificar asignaciones de usuarios para varios problemas en una lista

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

Puede modificar simultáneamente las asignaciones de usuarios a varios problemas. Para obtener información sobre cómo editar problemas o asignarlos de uno en uno, consulte los siguientes artículos:

* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Asignar problemas](../../../manage-work/issues/manage-issues/assign-issues.md)

Para obtener información general sobre la asignación de problemas, consulte [Información general sobre la modificación de asignaciones de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Debe tener al menos permisos de aportación para resolver un problema y poder realizar asignaciones al mismo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Acceso de visualización o superior a proyectos y tareas para asignar un problema</p> </td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td> <p>Permisos de administración para el problema</p> <p>Permisos de contribución o superiores para el proyecto o la tarea donde se encuentra el problema, al asignar varios problemas.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

   1. Haga clic en **Añadir una regla de filtro.**
   1. Para filtrar por una función específica, expanda **Funciones de la asignación,** y luego haga clic en **ID.**

      O

      Para filtrar por un usuario específico, expanda **Usuarios de la asignación,** y luego haga clic en **ID.**

      >[!TIP]
      >
      >No utilice **Asignado a**, ya que este campo hace referencia solamente al propietario del problema y no a todos los usuarios asignados.

   1. En la lista desplegable, seleccione **Igual** como calificador de filtro.
   1. Empiece a escribir el nombre del usuario o función que desea filtrar y, a continuación, haga clic sobre el nombre cuando aparezca en la lista desplegable.
   1. Haga clic en **Guardar filtro.**

1. Seleccione los problemas para los que desea modificar las asignaciones y, a continuación, haga clic en el icono **Editar** ![Editar icono](assets/qs-edit-icon.png).

   Se muestra la opción **Editar problemas**. Los elementos editados se muestran en la esquina superior izquierda de la página.

1. Vaya a la sección **Asignaciones** y, a continuación, seleccione **Usuario asignado**.

   ![Área de asignaciones](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. Realice una de las siguientes acciones:

   1. Para añadir un nuevo usuario asignado:

      1. Empiece a escribir el nombre de un usuario, función o equipo y, a continuación, selecciónelo cuando aparezca en la lista. La asignación se añade y no sustituye a las asignaciones actuales en los problemas seleccionados.

         >[!TIP]
         >
         >Puede asignar varios usuarios, funciones o equipos. Solo puede asignar usuarios, funciones y equipos activos.
         >
         >Si se asignó un usuario, una función o un equipo antes de desactivarlos, permanecen asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
         >
         >* Reasignar el elemento de trabajo a los recursos activos.
         >* Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.

         Se muestra la información común a todos los problemas seleccionados. Por ejemplo, si se asigna el mismo usuario a todos los problemas, ese usuario se muestra en la columna **Usuario asignado**. Si la información no es común a los problemas seleccionados, no se muestra ninguna información.

   1. Para quitar usuarios asignados individuales:

      1. Haga clic en el **icono X** junto al nombre del usuario asignado que desee eliminar si este aparece en la lista Asignaciones.

         O

         (Condicional) Si el usuario asignado que desea quitar no se muestra en la sección Asignaciones porque solo se le ha asignado a algunos de los problemas seleccionados, haga clic en **Quitar usuario asignado** y empiece a escribir el nombre del usuario asignado que desea quitar; a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

      1. Vuelva a hacer clic en **Quitar usuario asignado** para añadir otro que quiera quitar.

   1. Para quitar todos los usuarios asignados existentes:

      1. Haga clic en **Quitar todos los usuarios asignados existentes** y, a continuación, en **Sí, eliminar todos los usuarios asignados**.

         Esta acción elimina no solo los usuarios asignados comunes (los usuarios asignados que se muestran en el cuadro de diálogo de edición), sino también todos los usuarios asignados de todos los problemas seleccionados.

1. (Opcional) Modifique cualquiera de las siguientes opciones para los usuarios asignados que ha seleccionado para asociar a los problemas:

   * **Propietario de problemas:** seleccione el botón de opción para indicar qué usuario asignado se ha designado como propietario de problemas. Si se deja sin seleccionar, Adobe Workfront designa como propietario de problemas al primer usuario asignado. Esto no está disponible para asignaciones de equipo.
   * **Función de usuario asignado**: seleccione una función de la lista desplegable. Si se deja sin seleccionar, Workfront selecciona automáticamente la función principal del usuario.

1. Haga clic en **Guardar cambios**.
