---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Asignación de trabajo por lotes mediante el Distribuidor de cargas de trabajo
description: Puede asignar recursos a varias tareas y problemas de forma masiva mediante el Distribuidor de cargas de trabajo de Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '1551'
ht-degree: 94%

---

# Asignar trabajo de forma masiva mediante el Distribuidor de cargas de trabajo

<!--Audited: 07/2024-->

Puede asignar recursos a varias tareas y problemas de forma masiva mediante el Distribuidor de cargas de trabajo de Adobe Workfront.

Para obtener información general acerca de cómo asignar trabajo a los usuarios mediante el Distribuidor de cargas de trabajo, consulte [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>o</p>
       <p>Actual: Planificar, al usar el Distribuidor de cargas de trabajo en el área de Recursos;</br>
       Trabaje con el Distribuidor de cargas de trabajo de un equipo o proyecto</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a los siguientes elementos:</p> 
    <ul> 
     <li>Administración de recursos</li> 
     <li>Proyectos</li> 
     <li>Tareas</li> 
     <li>Problemas</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Permisos de contribuir o superiores para los proyectos, tareas y problemas que incluyan asignar tareas</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones a la hora de realizar asignaciones masivas en el Distribuidor de cargas de trabajo

* Puede administrar rápidamente las asignaciones de usuarios para varias tareas y problemas en uno o varios proyectos. Los cambios en las asignaciones se pueden ver inmediatamente en el Distribuidor de cargas de trabajo.
* No puede asignar recursos a elementos de trabajo que se hayan completado ni a elementos que se encuentren en un proyecto completado.
* Al asignar usuarios de forma masiva, puede hacer lo siguiente:

   * Asignar un usuario a todos los elementos de trabajo asignados actualmente a una función.
   * Reemplazar asignaciones de usuarios entre usuarios.
   * Anular la asignación de un usuario a todos sus elementos de trabajo.

**EJEMPLOS**

* La realización de asignaciones de usuarios en varios proyectos nuevos es responsabilidad suya. Los proyectos se han creado originalmente a partir de plantillas y las funciones ya están asignadas a las distintas tareas de los proyectos. Por ejemplo, desea asignar una usuaria específica, María López, a todas las tareas actualmente asignadas a una función. Puede utilizar la función Asignar para asignar estas tareas a María López.
* Se asignan 45 tareas de 3 proyectos diferentes a María López. María deja la organización y ahora debe reasignar sus tareas a otro usuario. Puede utilizar la función Reemplazar para asignar estas tareas a la nueva persona.
* Se asignan 10 tareas de 2 proyectos diferentes a otro usuario, Juan García. Advierte que a Juan se le asignaron estas tareas por error, pero no tiene la certidumbre de a quién deben asignarse en este momento. Tiene que anular la asignación de Juan a todas las tareas al mismo tiempo. Puede utilizar la función Anular asignación para quitar a Juan de estas tareas.

## Asignar trabajo de forma masiva en el Distribuidor de cargas de trabajo

1. Ir al Distribuidor de cargas de trabajo al que desea asignar el trabajo.

   Puede asignar trabajo a los usuarios mediante el Distribuidor de cargas de trabajo en el área de Recursos, en el proyecto o en el nivel de equipo. Para obtener más información sobre dónde se encuentra el Distribuidor de cargas de trabajo en Workfront, consulte [Buscar el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).


1. Haga clic en **Asignaciones en lotes** ![Asignaciones en lotes](assets/bulk-assignments-wb.png) en la parte superior del Distribuidor de cargas de trabajo.

   El panel Asignaciones masivas se abrirá a la derecha del Distribuidor de cargas de trabajo.

1. (Condicional) Si accede al Distribuidor de cargas de trabajo desde el área Recursos o para un equipo, expanda el menú desplegable **Proyecto: nombre** y utilice los modificadores de filtro para seleccionar el o los proyectos para los que desea realizar asignaciones. Puede seleccionar proyectos por Nombre (esta es la opción predeterminada) o por Estado.

   Para obtener información acerca de los modificadores de filtro de Workfront, vea [Filtros y modificadores de condición](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >El nombre del proyecto está seleccionado de forma predeterminada al acceder al Distribuidor de cargas de trabajo de un proyecto.

   ![Nombre de proyecto en asignaciones masivas](assets/project-name-status-dropdown-bulk-assignments-wb-nwe-350x133.png)

1. (Opcional) Haga clic en **Seleccionar tareas de proyecto** para seleccionar la tarea o tareas para las que desea realizar asignaciones y, a continuación, en el menú desplegable **Tarea: Nombre**, seleccione tareas por Nombre (esta es la opción predeterminada) o Estado y utilice los modificadores de filtro para buscar tareas específicas.

   Para obtener información acerca de los modificadores de filtro de Workfront, consulte [Filtros y modificadores de condición](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >No puede seleccionar tareas en estado Completo.

   ![Estado de la tarea en asignaciones masivas](assets/task-name-status-dropdown-bulk-assignments-wb-nwe-350x102.png)

   >[!TIP]
   >
   >Deje esta selección en blanco si desea realizar asignaciones masivas tanto para problemas como para tareas.

1. (Opcional) Haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete.png) junto a uno de los criterios seleccionados

   O

   Haga clic en **Borrar todo** en la esquina superior derecha del panel Asignaciones masivas para eliminar todas las selecciones.

1. Seleccione una de las siguientes opciones y continúe con los pasos que se describen a continuación:

   * [Asignar usuario](#assign-user)
   * [Reemplazar usuario](#replace-user)
   * [Quitar asignación de usuario](#unassign-user)

   >[!TIP]
   >
   >Si ningún elemento coincide con los filtros seleccionados, estas opciones aparecen atenuadas.

### Asignar usuario {#assign-user}

Cuando asigna un usuario mediante Asignaciones masivas en el Distribuidor de cargas de trabajo, sucede lo siguiente:

* Un usuario está asignado a todos los elementos de trabajo asignados actualmente a una función especificada dentro de los proyectos seleccionados.
* El usuario no está asignado a los siguientes tipos de elementos de trabajo:

   * Elementos que ya se han asignado a un usuario.
   * Elementos completados.

* Si el usuario seleccionado no está asociado con la función especificada, la función será reemplazada por el usuario en la Función principal del usuario.

Para asignar un usuario a elementos de trabajo previamente asignados a funciones:

1. Comience a asignar elementos de trabajo mediante asignaciones masivas en el Distribuidor de cargas de trabajo como se ha descrito anteriormente y seleccione **Asignar**.

1. En el campo **Asignación de funciones**, haga clic en la flecha desplegable para elegir entre una lista de funciones. Solo se muestran las funciones asignadas actualmente en los proyectos especificados. Este campo es obligatorio.

   ![Asignación de funciones](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. En el campo **Usuario para asignar**, haga clic en la flecha desplegable para elegir de una lista de usuarios sugeridos o para escribir el nombre de otro usuario.

   Seleccione los usuarios de las siguientes áreas:

   * **Asignaciones sugeridas**: usuarios que pueden cumplir la función seleccionada y que coinciden con los criterios de Asignaciones inteligentes. Para más información, consulte [Información general de las asignaciones inteligentes](../../manage-work/tasks/assign-tasks/smart-assignments.md).
   * **Otras asignaciones**: todos los usuarios del sistema que pueden cumplir la función seleccionada.

     >[!TIP]
     >
     >Solo los 50 primeros usuarios aparecen en el área Otras asignaciones.


   Después de seleccionar un usuario, Workfront muestra una nota sobre el número de elementos donde se asignará al usuario especificado y la función que reemplazará.

   >[!TIP]
   >
   >Todos los roles del usuario se muestran en la lista, bajo el nombre del usuario.


1. Haga clic en **Asignar**.

   Las funciones especificadas se reemplazarán por los usuarios seleccionados.

   Recibirá una confirmación sobre cuántos elementos de trabajo han reemplazado la función seleccionada con el usuario seleccionado.

   ![Confirmación de asignación masiva](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

### Reemplazar usuario {#replace-user}

Puede reemplazar a un usuario que ya esté asignado a elementos de trabajo con otro usuario en los proyectos seleccionados.

Cuando reemplaza un usuario por otro con Asignaciones masivas en el Distribuidor de cargas de trabajo, sucede lo siguiente:

* El usuario de reemplazo se asigna a todos los elementos de trabajo que estén asignados a un usuario original dentro de los proyectos seleccionados.

* El nuevo usuario no está asignado a ningún elemento de trabajo que ya esté marcado como Completado.
* Si la función asociada al primer usuario no coincide con ninguna de las funciones del segundo usuario, se asigna al segundo usuario en su función principal.

Para reemplazar a un usuario por otro:

1. Empiece a asignar elementos de trabajo en el Distribuidor de cargas de trabajo como se describe más arriba y seleccione **Reemplazar**.
1. En el campo **Usuario asignado actualmente**, haga clic en la flecha desplegable para elegir uno de una lista de usuarios. Solo se muestran los usuarios asignados actualmente a elementos de trabajo incompletos dentro de los proyectos especificados. Este campo es obligatorio.

   ![Reemplazar usuario](assets/bulk-assignments-workload-balancer-replace-selected-350x345.png)

1. En el campo **Usuario para asignar**, haga clic en la flecha desplegable para elegir uno de una lista de usuarios sugeridos o para escribir otro nombre de usuario. Los usuarios enumerados en la lista coinciden de forma predeterminada con los criterios de Asignaciones inteligentes. Para obtener más información, consulte [Información general sobre las asignaciones inteligentes](../../manage-work/tasks/assign-tasks/smart-assignments.md).

   Workfront muestra una nota sobre el número de elementos en los que el usuario asignado actualmente reemplazará al segundo usuario y las funciones a las que reemplazará.

   ![Confirmación de usuario de reemplazo masivo](assets/bulk-replace-user-confirmation-before-replacing-nwe-350x49.png)

1. Haga clic en **Reemplazar**.

   El primer usuario seleccionado se reemplaza por el segundo usuario en todos los elementos de trabajo del proyecto seleccionado.

   Recibirá una confirmación de cuántos elementos de trabajo se han reemplazado en la asignación de usuario original por el segundo usuario seleccionado.

### Quitar asignación de usuario {#unassign-user}

Se puede anular la asignación de un usuario a todos los elementos de trabajo a los que esté asignado en los proyectos seleccionados.

Cuando se anula la asignación de un usuario a todas sus asignaciones mediante asignaciones masivas en el Distribuidor de cargas de trabajo, se producen los siguientes problemas:

* El usuario especificado se elimina de todos los elementos de trabajo a los que está asignado.
* Si el usuario para el que se ha anulado la asignación está asociado a funciones de trabajo, estas funciones de trabajo permanecen asignadas a los elementos de trabajo cuando se quita el usuario.

* Si el usuario especificado está asignado a elementos de trabajo completados, el usuario permanece asignado a esos elementos de trabajo.

Para obtener más información sobre las asignaciones y funciones de usuarios, consulte [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Para anular la asignación de un usuario a elementos de trabajo en los proyectos seleccionados o a tareas o problemas seleccionados donde se hayan asignado:

1. Empiece a asignar elementos de trabajo en el Distribuidor de cargas de trabajo como se ha descrito anteriormente y seleccione **Anular asignación**.

1. En el campo **Usuario para anular la asignación**, haga clic en la flecha desplegable para elegir uno de una lista de usuarios. Solo se muestran los usuarios asignados actualmente a elementos de trabajo incompletos dentro de los proyectos especificados. Este campo es obligatorio.

   ![Quitar la asignación del usuario](assets/bulk-assignments-workload-balancer-unassign-selected-350x318.png)

   Workfront muestra una nota sobre el número de elementos para los que se anulará la asignación del usuario asignado actualmente.

   ![Confirmación de anulación de asignación masiva](assets/bulk-unassign-user-confirmation-before-assigning-nwe-350x45.png)

1. Haga clic en **Anular asignación**.\
   Recibirá una confirmación sobre el número de elementos de trabajo para los que se eliminó el usuario especificado.


