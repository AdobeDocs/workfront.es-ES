---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Trabajo no asignado en el Distribuidor de cargas de trabajo
description: Puede anular la asignación de usuarios a elementos de trabajo en el área de Trabajo asignado del Distribuidor de cargas de trabajo de Adobe Workfront o reasignarlos a otros usuarios, roles o equipos.
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 2%

---

# Trabajo no asignado en el Distribuidor de cargas de trabajo

Puede anular la asignación de usuarios a elementos de trabajo en el área de Trabajo asignado del Distribuidor de cargas de trabajo de Adobe Workfront o reasignarlos a otros usuarios, roles o equipos.

Puede anular la asignación de usuarios a elementos de trabajo manualmente, arrastrando y soltando o de forma masiva. Este artículo describe cómo anular la asignación de usuarios manualmente.

Para obtener información sobre cómo anular la asignación de usuarios arrastrando y soltando, consulte [Asignar trabajo en el Distribuidor de cargas de trabajo arrastrando y soltando](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Para obtener información sobre cómo anular la asignación de usuarios en lotes, consulte [Asignar trabajo en lotes mediante el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

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
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Edite el acceso a lo siguiente:</p> 
    <ul> 
     <li> <p>Administración de recursos</p> </li> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Tareas</p> </li> 
     <li> <p>Problemas</p> </li> 
    </ul> <p>Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Contribute o superiores para los proyectos, tareas y problemas que incluyen Realizar asignaciones</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

 

## Desasignar elementos de trabajo en el Distribuidor de cargas de trabajo

Puede anular la asignación de elementos de los usuarios y moverlos al área de Trabajo no asignado o reasignarlos a otros usuarios.

Para anular la asignación de elementos de trabajo a los usuarios:

1. En el Distribuidor de cargas de trabajo, vaya al área de **Trabajo asignado** y expanda un usuario.
1. Realice una de las siguientes acciones:

   * Busque el elemento cuya asignación desea anular en el área de un usuario, haga clic en él y arrástrelo y suéltelo en el área No asignada o en el área de otro usuario.
   * Haga clic en el icono **Más** ![](assets/more-icon-task-list.png) a la derecha del nombre de un elemento de trabajo, haga clic en **Asignar esto a**, quite el nombre de las entidades asignadas al elemento de trabajo o escriba otro nombre y haga clic en **Guardar**.

     ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   El elemento se muestra en el área de trabajo no asignado si coincide con los criterios de filtrado de dicha área y no está asignado a ningún otro usuario, o si está asignado a otro usuario, en el área de usuario.

   Para obtener información sobre el filtrado en el Distribuidor de cargas de trabajo, consulte [Filtrar información en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
