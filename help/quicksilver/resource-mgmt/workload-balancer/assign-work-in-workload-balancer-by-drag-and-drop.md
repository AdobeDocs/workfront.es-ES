---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Asignar trabajo en el equilibrador de carga de trabajo arrastrando y soltando
description: Puede asignar elementos de trabajo mediante el equilibrador de carga de trabajo de Adobe Workfront arrastrando y soltando elementos de trabajo a los usuarios correctos.
author: Alina
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: a1ffec0d8a50ff7f025ff23370afa746cf0d6d3f
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 1%

---

# Asignar trabajo en el equilibrador de carga de trabajo arrastrando y soltando

<!--remove production and preview preferences at release-->

Puede asignar elementos de trabajo mediante el equilibrador de carga de trabajo de Adobe Workfront arrastrando y soltando elementos de trabajo a los usuarios correctos.

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

## Asignar un elemento arrastrando y soltando

Puede asignar un elemento del área Trabajo no asignado a un usuario, o puede reasignar un elemento ya asignado a otro usuario del área Trabajo asignado.

1. Vaya al equilibrador de carga de trabajo donde desea asignar trabajo.

   Puede asignar trabajo a usuarios mediante el equilibrador de carga de trabajo en el área Recursos, en el proyecto o en el nivel de equipo. Para obtener más información sobre la ubicación del equilibrador de carga de trabajo en Workfront, consulte [Localizar el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Opcional) Vaya a la **Trabajo no asignado** y aplique un filtro para ver las tareas y los problemas que no están asignados a los usuarios

   O

   Vaya a la **Trabajo asignado** y expanda el nombre de un usuario para ver los elementos de trabajo asignados a ellos, si desea reasignar sus elementos.

1. (Condicional) En el equilibrador de carga de trabajo de un proyecto, haga clic en el **Mostrar todos los usuarios** icono ![](assets/show-all-users-icon-project-workload-balancer.png) para mostrar todos los usuarios de Workfront.

   Esto muestra todos los usuarios a los que tiene acceso para ver.

   Los usuarios que también forman parte del equipo del proyecto y que ya están asignados a elementos del proyecto tienen el icono del proyecto a la derecha de su nombre en el área Trabajo asignado .

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* La opción Mostrar todos los usuarios solo está disponible en el equilibrador de carga de trabajo de un proyecto.
   >* Utilice filtros para mostrar solo los usuarios que sean importantes para usted. Por ejemplo, utilice un filtro para mostrar solo los usuarios de sus equipos o grupos.




1. Haga clic en la barra de un elemento de trabajo que indica la cronología planificada o proyectada y arrástrela sobre el nombre de un usuario en la **Asignado** .

   Se resaltará el usuario al que pasa el ratón para soltar el elemento de trabajo.

   >[!TIP]
   >
   >Las horas planificadas para el usuario que está actualizando en tiempo real con el número de horas planificadas diarias desde el elemento de trabajo, para indicar cuál podría ser el impacto de agregar un nuevo elemento a su asignación general.

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. Cuando esté listo, suelte el elemento de trabajo seleccionado en la misma línea que el nombre del usuario en el área asignada. El artículo se asigna y las horas programadas asignadas se actualizan para el usuario con las nuevas horas del elemento de trabajo.

   Si el artículo se asignó a una función de trabajo que el usuario no puede cumplir, el artículo se muestra bajo el nombre del usuario en el área Trabajo asignado y también permanece en el área Trabajo no asignado para indicar que la función de trabajo asociada a él no ha sido reemplazada por un usuario todavía.

   >[!TIP]
   >
   >* Si ha activado Agrupar por proyecto en el área Configuración , la tarea asignada se muestra debajo del proyecto correspondiente. Si la configuración está deshabilitada, la tarea asignada se muestra en el área de usuario.
      >
      >
      >     El elemento se muestra según los criterios del equilibrador de carga de trabajo para ordenar los elementos de trabajo. Para obtener más información, consulte [Navegar por el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* Si habilitó Mostrar todos los usuarios del equilibrador de carga de trabajo de un proyecto y asignó elementos a usuarios que no se habían asignado previamente a elementos del proyecto, los usuarios se agregarán al equipo del proyecto. Para obtener más información, consulte [Administrar equipo de proyecto](../../manage-work/projects/planning-a-project/manage-project-team.md).



1. (Opcional) Haga clic en la barra de un elemento de trabajo bajo el nombre de un usuario en el área Trabajo asignado y arrástrela y, a continuación, suéltela sobre el área Trabajo sin asignar para anular la asignación. El elemento no está asignado por el usuario, pero podría estar asignado a una función de trabajo en cuyo caso se mostrará en el área Trabajo no asignado. Si el elemento está asignado a otro usuario, permanece en el área Trabajo asignado bajo el nombre del usuario que aún está asignado.
1. (Opcional) Haga clic en el **Mostrar icono de asignaciones** ![](assets/show-allocations-icon-small.png)y, a continuación, haga clic en el botón **Más menú** ![](assets/qs-more-menu.png) > **Editar asignaciones**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   O

   Haga doble clic en una asignación diaria o semanal para modificar la cantidad de tiempo que el usuario está asignado al elemento de trabajo.

   Para obtener información sobre la modificación de las asignaciones de usuario en el equilibrador de carga de trabajo, consulte la sección &quot;Modificar asignaciones de usuario&quot; en el artículo [Administrar asignaciones de usuario en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Para obtener información sobre cómo quitar asignaciones de un elemento de trabajo mediante el equilibrador de carga de trabajo, consulte [Anular la asignación de trabajo en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

