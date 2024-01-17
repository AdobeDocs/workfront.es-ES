---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Asignar trabajo en el Distribuidor de cargas de trabajo arrastrando y soltando
description: Puede asignar elementos de trabajo mediante el Distribuidor de cargas de trabajo de Adobe Workfront arrastrando y soltando elementos de trabajo a los usuarios correctos.
author: Lisa
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Asignar trabajo en el Distribuidor de cargas de trabajo arrastrando y soltando

<!--remove production and preview preferences at release-->

Puede asignar elementos de trabajo mediante el Distribuidor de cargas de trabajo de Adobe Workfront arrastrando y soltando elementos de trabajo a los usuarios correctos.

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
   <td> <p>Planificar, para asignar trabajo en el Distribuidor de cargas de trabajo en el área de Recursos</p>
   <p>Trabajar, para asignar trabajo en el Distribuidor de cargas de trabajo de un equipo o proyecto</p>
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

## Asignar un elemento arrastrando y soltando

Puede asignar un elemento del área de Trabajo no asignado a un usuario o reasignar un elemento ya asignado a otro usuario en el área de Trabajo asignado.

1. Vaya al Distribuidor de cargas de trabajo al que desea asignar el trabajo.

   Puede asignar trabajo a los usuarios mediante el Distribuidor de cargas de trabajo en el área de Recursos, en el proyecto o en el nivel de equipo. Para obtener más información sobre dónde se encuentra el Distribuidor de cargas de trabajo en Workfront, consulte [Localización del Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Opcional) Vaya a **Trabajo sin asignar** y aplicar un filtro para ver las tareas y los problemas que no están asignados a los usuarios

   O

   Vaya a la **Trabajo asignado** y expanda el nombre de un usuario para ver los elementos de trabajo asignados a él, si desea reasignar sus elementos.

1. (Condicional) En el Distribuidor de cargas de trabajo de un proyecto, haga clic en **Mostrar todos los usuarios** icono ![](assets/show-all-users-icon-project-workload-balancer.png) para mostrar todos los usuarios de Workfront.

   Esto muestra todos los usuarios a los que tiene acceso para ver.

   Los usuarios que también forman parte del equipo del proyecto y que ya están asignados a elementos del proyecto tienen el icono del proyecto a la derecha de su nombre en el área de Trabajo asignado.

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* La opción Mostrar todos los usuarios solo está disponible en el Distribuidor de cargas de trabajo de un proyecto.
   >* Utilice los filtros para mostrar solo los usuarios que son importantes para usted. Por ejemplo, utilice un filtro para mostrar solo los usuarios de sus equipos o grupos.



1. Haga clic en la barra de un elemento de trabajo que indique la escala de tiempo planificada o proyectada y arrástrela sobre el nombre de un usuario en la **Asignado** área.

   El usuario que pasa el ratón para soltar el elemento de trabajo en está resaltado.

   >[!TIP]
   >
   >Las horas planificadas del usuario al que pasa el ratón se actualizan en tiempo real con la cantidad de horas planificadas diariamente a partir del elemento de trabajo para indicar cuál puede afectar la adición de un nuevo elemento a su asignación general.

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. Cuando esté listo, suelte el elemento de trabajo seleccionado en la misma línea que el nombre del usuario en el área asignada. El elemento se asigna y las horas planificadas asignadas se actualizan para el usuario con las nuevas horas del elemento de trabajo.

   Si el elemento se ha asignado a un rol que el usuario no puede cumplir, el elemento se muestra bajo el nombre del usuario en el área Trabajo asignado y también permanece en el área Trabajo no asignado para indicar que el rol asociado a él aún no ha sido reemplazado por un usuario.

   >[!TIP]
   >
   >* Si ha habilitado Agrupar por proyecto en el área Configuración, la tarea asignada aparece debajo del proyecto correspondiente. Si la configuración está deshabilitada, la tarea asignada se muestra en el área de usuario.
   >
   >
   >     El elemento se muestra según los criterios del Distribuidor de cargas de trabajo para ordenar los elementos de trabajo. Para obtener más información, consulte [Navegación por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* Si habilitó Mostrar todos los usuarios en el Distribuidor de cargas de trabajo de un proyecto y asignó elementos a usuarios que no estaban asignados anteriormente a elementos del proyecto, los usuarios se agregan al Equipo del proyecto. Para obtener más información, consulte [Administrar equipo del proyecto](../../manage-work/projects/planning-a-project/manage-project-team.md).


1. (Opcional) Haga clic en la barra de un elemento de trabajo bajo el nombre de un usuario en el área de Trabajo asignado y arrástrelo y, a continuación, suéltelo sobre el área de Trabajo no asignado para anular la asignación. El elemento no está asignado al usuario, pero podría estar asignado a un rol, en cuyo caso se mostrará en el área de Trabajo no asignado. Si el elemento está asignado a otro usuario, permanecerá en el área Trabajo asignado bajo el nombre del usuario que aún esté asignado.
1. (Opcional) Haga clic en **Mostrar icono de asignaciones** ![](assets/show-allocations-icon-small.png), luego haga clic en **Menú Más** ![](assets/qs-more-menu.png) > **Editar asignaciones**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   O

   Haga doble clic en una asignación diaria o semanal para modificar la cantidad de tiempo que se asigna al usuario al elemento de trabajo.

   Para obtener información sobre la modificación de las asignaciones de usuarios en el Distribuidor de cargas de trabajo, consulte la sección &quot;Modificación de asignaciones de usuarios&quot; en el artículo [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Para obtener información sobre cómo quitar asignaciones de un elemento de trabajo mediante el Distribuidor de cargas de trabajo, consulte [Trabajo no asignado en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

