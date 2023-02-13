---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Asignar trabajo manualmente mediante el equilibrador de carga de trabajo
description: Puede asignar manualmente elementos de trabajo a los usuarios mediante el equilibrador de carga de trabajo de Adobe Workfront.
author: Alina
feature: Resource Management
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 2%

---

# Asignar trabajo manualmente mediante el equilibrador de carga de trabajo

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

## Asignación manual del trabajo en el equilibrador de carga de trabajo

Puede asignar elementos de trabajo que aún no se hayan asignado a un usuario o reasignar elementos que se hayan asignado a usuarios en el equilibrador de carga de trabajo.

1. Vaya al equilibrador de carga de trabajo donde desea asignar trabajo.

   Puede asignar trabajo a usuarios mediante el equilibrador de carga de trabajo en el área Recursos, en el proyecto o en el nivel de equipo. Para obtener más información sobre la ubicación del equilibrador de carga de trabajo en Workfront, consulte [Localizar el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Opcional) Vaya a la **Trabajo no asignado** y aplicar un filtro para ver tareas o problemas

   O

   Vaya a la **Trabajo asignado** y expanda el nombre de un usuario para ver los elementos de trabajo asignados a ellos, si desea reasignar sus elementos.

1. Haga clic en el **Más menú** ![](assets/qs-more-menu.png) a la izquierda del nombre de un elemento de trabajo y, a continuación, haga clic en **Asigne esto a**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >También puede utilizar los siguientes métodos abreviados para asignar tareas o problemas:
   >
   >* En Windows: CTRL+clic en la tarea o en la barra de problemas.
   >* En Mac: CMD+clic en la tarea o en la barra de problemas.


1. Realice una de las siguientes acciones:

   * Comience a escribir el nombre de un usuario, función de trabajo o equipo que desee asignar al elemento en la **Buscar personas, roles o equipos** , selecciónelo cuando aparezca en la lista y haga clic en **Guardar**.
   >[!TIP]
   >
   >Al agregar un usuario, observe el avatar, la función principal del usuario y su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos una función de trabajo para verla a medida que los agrega.

   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Si el administrador de Workfront o de grupo ha habilitado las delegaciones en su entorno, utilice la pestaña Asignaciones para asignar usuarios a la tarea o el problema. Utilice la pestaña Delegaciones para ver los usuarios delegados en el elemento de trabajo. Para obtener información sobre la delegación de trabajo, consulte [Administrar delegación de tareas y problemas](../../manage-work/delegate-work/how-to-delegate-work.md).


   Esto asigna o reasigna el elemento de trabajo a los asignadores especificados.

   Si asigna un artículo a un solo equipo o a una función de trabajo, el artículo solo se mostrará en el área Trabajo sin asignar. Debe asignar elementos de trabajo a los usuarios para que se muestren en el área Trabajo asignado del equilibrador de carga de trabajo.

   >[!TIP]
   >
   >Puede asignar varios usuarios, funciones de trabajo o equipos. Solo puede asignar usuarios activos, funciones de trabajo y equipos.
   >
   >
   >Si se asignó un usuario, una función de trabajo o un equipo antes de desactivarlos, se asignarán al elemento de trabajo. En este caso, se recomienda lo siguiente:
   >
   >   
   >   
   >   * Reasigne el elemento de trabajo a los recursos activos.
   >   * Asocie a los usuarios de un equipo desactivado con un equipo activo y reasigne el elemento de trabajo al equipo activo.


   * Haga clic en **Avanzadas** para acceder a Asignaciones avanzadas.

      Para obtener más información sobre cómo realizar asignaciones avanzadas, consulte [Crear asignaciones avanzadas](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).


1. (Opcional) Haga clic en el **Mostrar icono de asignaciones** ![](assets/show-allocations-icon-small.png)y, a continuación, haga clic en el botón **Más menú** ![](assets/qs-more-menu.png) > **Editar asignaciones**.

   O

   Haga doble clic en una asignación diaria o semanal para modificar la cantidad de tiempo que el usuario está asignado al elemento de trabajo.

   Para obtener información sobre la modificación de las asignaciones de usuario en el equilibrador de carga de trabajo, consulte la sección &quot;Modificar asignaciones de usuario&quot; en el artículo [Administrar asignaciones de usuario en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Para obtener información sobre cómo quitar asignaciones de un elemento de trabajo mediante el equilibrador de carga de trabajo, consulte [Anular la asignación de trabajo en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
