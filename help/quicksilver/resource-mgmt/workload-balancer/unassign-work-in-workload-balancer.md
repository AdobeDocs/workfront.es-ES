---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Anular la asignación de trabajo en el equilibrador de carga de trabajo
description: Puede anular la asignación de usuarios de elementos de trabajo en el área Trabajo asignado del equilibrador de carga de trabajo de Adobe Workfront o reasignarlos a otros usuarios, funciones o equipos.
author: Alina
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 2%

---

# Anular la asignación de trabajo en el equilibrador de carga de trabajo

Puede anular la asignación de usuarios de elementos de trabajo en el área Trabajo asignado del equilibrador de carga de trabajo de Adobe Workfront o reasignarlos a otros usuarios, funciones o equipos.

Puede desasignar usuarios de elementos de trabajo manualmente, arrastrándolos y soltándolos o de forma masiva. Este artículo describe cómo anular la asignación de usuarios manualmente.

Para obtener información sobre cómo anular la asignación de usuarios arrastrando y soltando, consulte [Asignar trabajo en el equilibrador de carga de trabajo arrastrando y soltando](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Para obtener información sobre cómo anular la asignación de usuarios de forma masiva, consulte [Asignar trabajo de forma masiva mediante el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

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
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Edite el acceso a lo siguiente:</p> 
    <ul> 
     <li> <p>Administración de recursos</p> </li> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Tareas</p> </li> 
     <li> <p>Problemas</p> </li> 
    </ul> <p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Contribute o superior a los proyectos, tareas y problemas que incluyen Realizar asignaciones</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

 

## Anular la asignación de elementos de trabajo en el equilibrador de carga de trabajo

Puede anular la asignación de elementos de usuarios y moverlos al área Trabajo no asignado, o bien reasignarlos a otros usuarios.

Para anular la asignación de elementos de trabajo de los usuarios:

1. En el equilibrador de carga de trabajo, vaya a la **Trabajo asignado** y expandir un usuario.
1. Realice una de las siguientes acciones:

   * Busque el elemento que desea anular la asignación en el área de un usuario, haga clic en él y arrástrelo y suéltelo en el área No asignado o en el área de otro usuario.
   * Haga clic en el **Más** icono ![](assets/more-icon-task-list.png) a la derecha del nombre de un elemento de trabajo, haga clic en **Asigne esto a** y, a continuación, elimine el nombre de las entidades asignadas al elemento de trabajo o introduzca otro nombre, y haga clic en **Guardar**.

      ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)
   El elemento se muestra en el área Trabajo no asignado si coincide con los criterios de filtrado de esa área y no está asignado a ningún otro usuario, o si se muestra en el área de usuario si está asignado a otro usuario.

   Para obtener información sobre el filtrado de información en el equilibrador de carga de trabajo, consulte [Filtrar información en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
