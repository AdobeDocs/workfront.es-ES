---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Asignar trabajo de forma masiva mediante el equilibrador de carga de trabajo
description: Puede asignar manualmente elementos de trabajo a los usuarios mediante el equilibrador de carga de trabajo de Adobe Workfront.
author: Alina
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
source-git-commit: 10b905c8a66f2507cbfac7c15a01f38d40ab3e00
workflow-type: tm+mt
source-wordcount: '1545'
ht-degree: 2%

---

# Asignar trabajo de forma masiva mediante el equilibrador de carga de trabajo

<!--drafted
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 
-->

Puede asignar manualmente elementos de trabajo a los usuarios mediante el equilibrador de carga de trabajo de Adobe Workfront.

Para obtener información general sobre la asignación de trabajo a usuarios mediante el equilibrador de carga de trabajo, consulte [Información general sobre la asignación de trabajo en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

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
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar, al utilizar el equilibrador de carga de trabajo para un equipo o en el área de recursos </p>
   <p>Trabajar, al utilizar el equilibrador de carga de trabajo de un proyecto </p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Edite el acceso a lo siguiente:</p> 
    <ul> 
     <li> <p>Administración de recursos</p> </li> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Tareas</p> </li> 
     <li> <p>Problemas</p> </li> 
    </ul> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Contribute o superior a los proyectos, tareas y problemas que incluyen Realizar asignaciones</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones para realizar asignaciones masivas en el equilibrador de carga de trabajo

* Puede administrar rápidamente las asignaciones de usuario para varias tareas y problemas en uno o varios proyectos. Los cambios en las asignaciones se pueden ver inmediatamente en el equilibrador de carga de trabajo.
* No se pueden asignar recursos a elementos de trabajo completados o a elementos de un proyecto completado.
* Al asignar usuarios de forma masiva, puede hacer lo siguiente:

   * Asigne un usuario a todos los elementos de trabajo que estén asignados a una función de trabajo.
   * Reemplazar asignaciones de usuario entre usuarios.
   * Anule la asignación de un usuario de todos sus elementos de trabajo.

**EJEMPLOS**

* Usted es el responsable de realizar asignaciones de usuario en varios proyectos nuevos. Los proyectos se crearon originalmente a partir de plantillas y las funciones de trabajo ya están asignadas a las distintas tareas dentro de los proyectos. Desea asignar un usuario específico, Jackie Simms, a todas las tareas que actualmente están asignadas a una función de trabajo. Puede utilizar la función Assign para asignar estas tareas a Jackie Simms.
* A Jackie Simms se le asignan 45 tareas en 3 proyectos diferentes. Jackie deja la organización, y ahora necesitas reasignar sus tareas a otro usuario. Puede utilizar la función Reemplazar para asignar estas tareas a la nueva persona.
* 10 tareas en 2 proyectos diferentes se asignan a otro usuario, Rick Kuvec. Te das cuenta de que Rick fue asignado a estas tareas por error, pero no estás seguro de a quién necesitan ser asignados en este momento. Debe anular la asignación de Rick a todas las tareas al mismo tiempo. Puede utilizar la función Unassign para eliminar a Rick de estas tareas.

## Asignar trabajo de forma masiva en el equilibrador de carga de trabajo

1. Vaya al equilibrador de carga de trabajo donde desea asignar trabajo.

   Puede asignar trabajo a usuarios mediante el equilibrador de carga de trabajo en el área Recursos, en el proyecto o en el nivel de equipo. Para obtener más información sobre la ubicación del equilibrador de carga de trabajo en Workfront, consulte [Localizar el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).


1. Haga clic en **Asignaciones masivas** ![](assets/bulk-assignments-wb.png) en la parte superior del equilibrador de carga de trabajo.

   El panel Asignaciones masivas se abre a la derecha del equilibrador de carga de trabajo.

1. (Condicional) Si accede al equilibrador de carga de trabajo desde el área Recursos o para un equipo, expanda el **Proyecto: Nombre** menú desplegable y utilice los modificadores de filtro para seleccionar el proyecto o los proyectos para los que desea realizar asignaciones. Puede seleccionar proyectos por Nombre (esta es la opción predeterminada) o por Estado.

Para obtener información sobre los modificadores de filtros de Workfront, consulte [Filtros y modificadores de condición](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

>[!NOTE]
>
>El nombre del proyecto está seleccionado de forma predeterminada cuando se accede al equilibrador de carga de trabajo de un proyecto.

![](assets/project-name-status-dropdown-bulk-assignments-wb-nwe-350x133.png)

1. (Opcional) Haga clic en **Seleccionar tareas de proyecto** para seleccionar la tarea o tareas para las que desea realizar asignaciones y, a continuación, en el **Tarea: Nombre** menú desplegable, seleccione tareas por Nombre (esta es la opción predeterminada) o Estado y utilice los modificadores de filtro para buscar tareas específicas.

Para obtener información sobre los modificadores de filtros de Workfront, consulte [Filtros y modificadores de condición](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

>[!NOTE]
>
>No puede seleccionar tareas en un estado de Finalización.

![](assets/task-name-status-dropdown-bulk-assignments-wb-nwe-350x102.png)

>[!TIP]
>
>Deje esta selección en blanco si desea realizar asignaciones masivas para problemas así como tareas.

1. (Opcional) Haga clic en el **Eliminar** icono ![](assets/delete.png) junto a uno de los criterios seleccionados

   O

   Haga clic en **Borrar todo** en la esquina superior derecha del panel Asignaciones masivas para eliminar todas las selecciones.

1. Seleccione una de las siguientes opciones y continúe con los pasos que se describen a continuación:

   * [Asignar usuario](#assign-user)
   * [Reemplazar usuario](#replace-user)
   * [Quitar asignación de usuario](#unassign-user)

   >[!TIP]
   >
   >Si no hay elementos que coincidan con los filtros seleccionados, estas opciones aparecerán atenuadas.

### Asignar usuario {#assign-user}

Cuando asigna un usuario mediante asignaciones masivas en el equilibrador de carga de trabajo, ocurren las siguientes cosas:

* Se asigna un usuario a todos los elementos de trabajo que están asignados a una función específica dentro de los proyectos seleccionados.
* El usuario no está asignado a los siguientes tipos de elementos de trabajo:

   * Elementos que ya están asignados a un usuario.
   * Elementos completados.

* Si el usuario seleccionado no está asociado con la función especificada, la función se reemplaza por el usuario en la función principal del usuario.

Para asignar un usuario a elementos de trabajo previamente asignados a funciones de trabajo:

1. Comience a asignar elementos de trabajo mediante asignaciones masivas en el equilibrador de carga de trabajo como se describe anteriormente y seleccione **Asignar**.

1. En el **Asignación de funciones** , haga clic en la flecha desplegable para elegir entre una lista de funciones. Solo se muestran las funciones asignadas actualmente en los proyectos especificados. Este campo es obligatorio.

   ![](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. En el **Usuario al que asignar** , haga clic en la flecha desplegable para elegir entre una lista de usuarios sugeridos o para escribir el nombre de otro usuario.

   Seleccione usuarios de las siguientes áreas:

   * **Asignaciones sugeridas**: Usuarios que pueden cumplir la función seleccionada y que coinciden con los criterios de las asignaciones inteligentes. Para obtener más información, consulte [Información general sobre asignaciones inteligentes](../../manage-work/tasks/assign-tasks/smart-assignments.md).
   * **Otras asignaciones**: Todos los usuarios del sistema que puedan cumplir la función seleccionada.

      >[!TIP]
      >
      >En el área Otras asignaciones solo se muestran los primeros 50 usuarios.
   Después de seleccionar un usuario, Workfront muestra una nota sobre el número de elementos a los que se asignará el usuario especificado y la función de trabajo que reemplazarán.

   >[!TIP]
   >
   >Todas las funciones del usuario se muestran en la lista, bajo el nombre del usuario.


1. Haga clic en **Asignar**.

   Las funciones especificadas se reemplazan con los usuarios seleccionados.

   Recibirá una confirmación sobre cuántos elementos de trabajo han reemplazado la función seleccionada por el usuario seleccionado.

   ![](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

### Reemplazar usuario {#replace-user}

Puede reemplazar un usuario que ya esté asignado a elementos de trabajo por otro usuario en los proyectos seleccionados.

Cuando se reemplaza un usuario por otro mediante asignaciones masivas en el equilibrador de carga de trabajo, ocurren las siguientes cosas:

* El usuario de reemplazo se asigna a todos los elementos de trabajo que están asignados a un usuario original dentro de los proyectos seleccionados.

* El nuevo usuario no está asignado a ningún elemento de trabajo que ya esté marcado como Completado.
* Si la función asociada al primer usuario no coincide con ninguna de las funciones del segundo usuario, se asigna al segundo usuario en su función principal.

Para reemplazar un usuario por otro usuario:

1. Inicie la asignación de elementos de trabajo en el equilibrador de carga de trabajo como se describe anteriormente y seleccione **Reemplazar**.
1. En el **Usuario asignado actualmente** , haga clic en la flecha desplegable para elegir entre una lista de usuarios. Solo se muestran los usuarios asignados actualmente a elementos de trabajo incompletos dentro de los proyectos especificados. Este campo es obligatorio.

   ![](assets/bulk-assignments-workload-balancer-replace-selected-350x345.png)

1. En el **Usuario al que asignar** , haga clic en la flecha desplegable para elegir entre una lista de usuarios sugeridos o para escribir otro nombre de usuario. Los usuarios que aparecen en la lista de forma predeterminada coinciden con los criterios de las asignaciones inteligentes. Para obtener más información, consulte [Información general sobre asignaciones inteligentes](../../manage-work/tasks/assign-tasks/smart-assignments.md).

   Workfront muestra una nota sobre el número de elementos en los que el usuario asignado actualmente reemplazará al segundo usuario y qué funciones reemplazarán.

   ![](assets/bulk-replace-user-confirmation-before-replacing-nwe-350x49.png)

1. Haga clic en **Reemplazar**.

   El primer usuario seleccionado se sustituye por el segundo usuario en todos los elementos de trabajo del proyecto seleccionado.

   Recibirá una confirmación sobre cuántos elementos de trabajo han tenido que reemplazar la asignación de usuario original por el segundo usuario seleccionado.

### Quitar asignación de usuario {#unassign-user}

Puede anular la asignación de un usuario de todos los elementos de trabajo asignados al usuario en los proyectos seleccionados.

Cuando se anula la asignación de un usuario de todas sus asignaciones mediante asignaciones masivas en el equilibrador de carga de trabajo, ocurren las siguientes cosas:

* El usuario especificado se elimina de todos los elementos de trabajo a los que está asignado.
* Si el usuario no asignado está asociado con funciones de trabajo, las funciones de trabajo permanecen asignadas a los elementos de trabajo cuando se elimina al usuario.

* Si el usuario especificado está asignado a elementos de trabajo completados, el usuario permanece asignado a esos elementos de trabajo.

Para obtener más información sobre las asignaciones de funciones de usuario y trabajo, consulte [Información general sobre la asignación de trabajo en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Para anular la asignación de un usuario de elementos de trabajo de los proyectos seleccionados o de las tareas o problemas seleccionados a los que se les asigna:

1. Inicie la asignación de elementos de trabajo en el equilibrador de carga de trabajo como se describe anteriormente y seleccione **Anulación de asignación**.

1. En el **Usuario que desea anular la asignación** , haga clic en la flecha desplegable para elegir entre una lista de usuarios. Solo se muestran los usuarios asignados actualmente a elementos de trabajo incompletos dentro de los proyectos especificados. Este campo es obligatorio.

   ![](assets/bulk-assignments-workload-balancer-unassign-selected-350x318.png)

   Workfront muestra una nota sobre el número de elementos a los que el usuario asignado actualmente no estará asignado.

   ![](assets/bulk-unassign-user-confirmation-before-assigning-nwe-350x45.png)

1. Haga clic en **Anulación de asignación**.\
   Recibirá una confirmación sobre el número de elementos de trabajo en los que se eliminó el usuario especificado.

 
