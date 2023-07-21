---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Asignar trabajo manualmente mediante el Distribuidor de cargas de trabajo
description: Puede asignar manualmente elementos de trabajo a los usuarios mediante el Distribuidor de cargas de trabajo de Adobe Workfront.
author: Alina
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 1%

---

# Asignar trabajo manualmente mediante el Distribuidor de cargas de trabajo

Puede asignar manualmente elementos de trabajo a los usuarios mediante el Distribuidor de cargas de trabajo de Adobe Workfront.

Para obtener información general sobre la asignación de trabajo a los usuarios mediante el Distribuidor de cargas de trabajo, consulte [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

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
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar, al utilizar el Distribuidor de cargas de trabajo en el área de Recursos</p>
   <p>Trabaje con el Distribuidor de cargas de trabajo de un equipo o proyecto</p>
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

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Aportar permisos o niveles superiores a los proyectos, tareas y problemas que incluyen Realizar asignaciones</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Asignar trabajo manualmente en el Distribuidor de cargas de trabajo

Puede asignar elementos de trabajo que aún no se hayan asignado a un usuario o reasignar elementos que se hayan asignado a usuarios en el Distribuidor de cargas de trabajo.

1. Vaya al Distribuidor de cargas de trabajo al que desea asignar el trabajo.

   Puede asignar trabajo a los usuarios mediante el Distribuidor de cargas de trabajo en el área de Recursos, en el proyecto o en el nivel de equipo. Para obtener más información sobre dónde se encuentra el Distribuidor de cargas de trabajo en Workfront, consulte [Localización del Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Opcional) Vaya a **Trabajo sin asignar** y aplicar un filtro para ver tareas o problemas

   O

   Vaya a la **Trabajo asignado** y expanda el nombre de un usuario para ver los elementos de trabajo asignados a él, si desea reasignar sus elementos.

1. Haga clic en **Menú Más** ![](assets/qs-more-menu.png) a la izquierda del nombre de un elemento de trabajo y haga clic en **Asignar esto a**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >También puede utilizar los siguientes métodos abreviados para asignar tareas o problemas:
   >
   >* En Windows: CTRL + clic en la barra de tareas o problemas.
   >* En Mac: CMD + clic en la barra de tareas o problemas.

1. Realice una de las siguientes acciones:

   * Empiece a escribir el nombre de un usuario, rol o equipo que desee asignar al elemento en la **Buscar personas, funciones o equipos** , selecciónelo cuando se muestre en la lista y haga clic en **Guardar**.

   >[!TIP]
   >
   >Al agregar un usuario, observe el avatar, la función principal del usuario y su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos.
   >
   >Los usuarios deben estar asociados con al menos un rol para verlo a medida que los agregue.
   >
   > Debe tener activada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Concesión de acceso a los usuarios](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Si el administrador de su Workfront o de su grupo ha habilitado las delegaciones en su entorno, utilice la pestaña Asignaciones para asignar usuarios a la tarea o al problema. Utilice la pestaña Delegaciones para ver los usuarios delegados al elemento de trabajo. Para obtener información sobre la delegación de trabajo, consulte [Administrar delegación de tareas y problemas](../../manage-work/delegate-work/how-to-delegate-work.md).


   Esto asigna o reasigna el elemento de trabajo a los usuarios asignados especificados.

   Si asigna un elemento a un equipo o rol, el elemento solo se muestra en el área Trabajo no asignado. Debe asignar elementos de trabajo a los usuarios para mostrarlos en el área de Trabajo asignado del Distribuidor de cargas de trabajo.

   >[!TIP]
   >
   >Puede asignar varios usuarios, roles o equipos. Solo puede asignar usuarios activos, roles y equipos.
   >
   >
   >Si se asignó un usuario, un rol o un equipo antes de desactivarlos, permanecen asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
   >
   >   
   >   
   >   * Reasignar el elemento de trabajo a los recursos activos.
   >   * Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.
   >   
   >

   * Clic **Avanzadas** para acceder a Asignaciones avanzadas.

     Para obtener más información sobre cómo realizar asignaciones avanzadas, consulte [Crear asignaciones avanzadas](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. (Opcional) Haga clic en **Mostrar icono de asignaciones** ![](assets/show-allocations-icon-small.png), luego haga clic en **Menú Más** ![](assets/qs-more-menu.png) > **Editar asignaciones**.

   O

   Haga doble clic en una asignación diaria o semanal para modificar la cantidad de tiempo que se asigna al usuario al elemento de trabajo.

   Para obtener información sobre la modificación de las asignaciones de usuarios en el Distribuidor de cargas de trabajo, consulte la sección &quot;Modificación de asignaciones de usuarios&quot; en el artículo [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Para obtener información sobre cómo quitar asignaciones de un elemento de trabajo mediante el Distribuidor de cargas de trabajo, consulte [Trabajo no asignado en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
