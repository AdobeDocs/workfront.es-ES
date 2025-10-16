---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Asignar trabajo manualmente mediante el Distribuidor de cargas de trabajo
description: Puede asignar manualmente elementos de trabajo a los usuarios mediante el Distribuidor de cargas de trabajo de Adobe Workfront.
author: Lisa
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: e1580f7b9065fce7bb31ab0c7edb00fd2856e1df
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 81%

---

# Asignar trabajo manualmente mediante el Distribuidor de cargas de trabajo

Puede asignar manualmente elementos de trabajo a los usuarios mediante el Distribuidor de cargas de trabajo de Adobe Workfront.

Para obtener información general acerca de cómo asignar trabajo a los usuarios mediante el Distribuidor de cargas de trabajo, consulte [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

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
       <p>Planificar, al utilizar el Distribuidor de cargas de trabajo en el área de Recursos; Trabajar, al utilizar el Distribuidor de cargas de trabajo de un equipo o proyecto</p></td>
  </tr>
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
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
   <td>Permisos de objeto</td> 
   <td>Permisos de contribuir o superiores para los proyectos, tareas y problemas que incluyan asignar tareas</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Asignación manual de trabajo en el Distribuidor de cargas de trabajo

Puede asignar elementos de trabajo que aún no se hayan asignado a un usuario o reasignar elementos que se hayan asignado a usuarios en el Distribuidor de cargas de trabajo.

1. Ir al Distribuidor de cargas de trabajo al que desea asignar el trabajo.

   Puede asignar trabajo a los usuarios mediante el Distribuidor de cargas de trabajo en el área de Recursos, en el proyecto o en el nivel de equipo. Para obtener más información sobre dónde se encuentra el Distribuidor de cargas de trabajo en Workfront, consulte [Buscar el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Opcional) Vaya al área **Trabajo sin asignar** y aplique un filtro para ver tareas, problemas o asignaciones de funciones.

   O

   Vaya al área **Trabajo asignado** y expanda el nombre de un usuario para ver los elementos de trabajo asignados a él, si desea reasignar sus elementos.

   >[!NOTE]
   >
   >Las asignaciones de roles se muestran en elementos de trabajo en el área Trabajo no asignado cuando la opción Mostrar asignaciones de roles está activada. Para obtener más información, consulte [Personalizar la vista](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md#customize-the-view) en [Navegar por el Distribuidor de cargas de trabajo](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Haga clic en el **menú Más** ![menú Más](assets/qs-more-menu.png) que se encuentra a la izquierda del nombre de un elemento de trabajo o de la asignación de funciones y, a continuación, haga clic en **Asignar esto a**.

   ![Asignar esto a](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >También puede utilizar los siguientes métodos abreviados para asignar tareas o problemas:
   >
   >* En Windows: CTRL + clic en la barra de tareas o problemas.
   >* En Mac: CMD + clic en la barra de tareas o problemas.

1. Realice una de las siguientes acciones:

   * Comience a escribir el nombre de un usuario, función laboral o equipo que desee asignar al elemento en el campo **Buscar personas, funciones o equipos**, selecciónelo cuando aparezca en la lista y luego haga clic en **Guardar**.

   >[!TIP]
   >
   >Al añadir un usuario, observe el avatar, la función principal del usuario y su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos.
   >
   >Los usuarios deben estar asociados con al menos una función para verla a medida que los añade.
   >
   > Debe tener habilitada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Conceder acceso a usuarios](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


   ![Asignaciones avanzadas](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Si el administrador de su Workfront o de su grupo ha habilitado las delegaciones en su entorno, utilice la pestaña Asignaciones para asignar usuarios a la tarea o al problema. Utilice la pestaña Delegaciones para ver los usuarios delegados al elemento de trabajo. Para obtener información sobre la delegación de trabajo, consulte [Delegar tareas y problemas](../../manage-work/delegate-work/how-to-delegate-work.md).


   Esto asigna o reasigna el elemento de trabajo a los usuarios asignados especificados.

   Si asigna un elemento a un equipo o rol, el elemento solo se muestra en el área Trabajo no asignado. Debe asignar elementos de trabajo a los usuarios para mostrarlos en el área de Trabajo asignado del Distribuidor de cargas de trabajo.

   >[!TIP]
   >
   >Puede asignar varios usuarios, funciones o equipos. Solo puede asignar usuarios, funciones y equipos activos.
   >
   >
   >Si se asignó un usuario, una función o un equipo antes de desactivarlos, permanecen asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
   >
   >   
   >   
   >   * Reasignar el elemento de trabajo a los recursos activos.
   >   * Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.
   >   
   >

   * Haga clic en **Avanzadas** para acceder a las Asignaciones avanzadas.

     Para obtener más información sobre cómo realizar asignaciones avanzadas, consulte [Crear asignaciones avanzadas](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. (Opcional) Haga clic en el icono **Mostrar asignaciones** ![Mostrar asignaciones](assets/show-allocations-icon-small.png) y, a continuación, haga clic en el **menú Más** ![menú Más](assets/qs-more-menu.png) > **Editar asignaciones**.

   O

   Haga doble clic en una asignación diaria o semanal para modificar la cantidad de tiempo que se asigna al usuario al elemento de trabajo.

   Para obtener información sobre cómo modificar las asignaciones de usuarios en el Distribuidor de cargas de trabajo, consulte la sección “Modificar asignaciones de usuarios” en el artículo [Administrar asignaciones de usuario en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Para obtener información sobre cómo eliminar asignaciones de un elemento de trabajo utilizando el Distribuidor de cargas de trabajo, consulte [Desasignar trabajo en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
