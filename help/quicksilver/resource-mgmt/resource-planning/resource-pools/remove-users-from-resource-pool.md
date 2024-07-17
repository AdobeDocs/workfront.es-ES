---
product-area: resource-management
navigation-topic: resource-pools
title: Quitar usuarios de conjuntos de recursos
description: Aunque no hay límite para la cantidad de usuarios que puede tener en un conjunto de recursos, la lista de usuarios sólo muestra los primeros 2000 usuarios, enumerados alfabéticamente.
author: Alina
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 1%

---

# Quitar usuarios de conjuntos de recursos

Aunque no hay límite para la cantidad de usuarios que puede tener en un conjunto de recursos, la lista de usuarios sólo muestra los primeros 2000 usuarios, enumerados alfabéticamente.

Se recomienda eliminar los usuarios que se han desactivado o que han movido funciones o departamentos, para garantizar que siempre tenga una lista precisa de los usuarios en todos los conjuntos de recursos.

Para obtener más información acerca de los conjuntos de recursos, vea [Resumen de los conjuntos de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Pro y superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Administración de recursos que incluye acceso a Administrar conjuntos de recursos</p> <p>Acceso de visualización o superior a los usuarios</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>(NOTE:&nbsp;I don't think this is needed for removing users from the pool)</p> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Quitar usuarios de un conjunto de recursos

Puede quitar usuarios de un conjunto de recursos cuando ya no los necesite en dicho conjunto.

Para eliminar un usuario de un conjunto de recursos:

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Recursos**.
1. Haga clic en **Conjuntos de recursos** en el panel izquierdo.
1. Seleccione un conjunto de recursos y haga clic en **Editar.**O\
   Haga clic en el nombre de un conjunto de recursos.

1. Empiece a escribir el nombre de un usuario que desee quitar en el campo **Buscar en este conjunto de recursos**.\
   O\
   Empiece a escribir el nombre de una empresa, función de trabajo, equipo o grupo si desea quitar todos los usuarios asociados a esas entidades.\
   ![search_inside_NEW_resource_pool.png](assets/search-inside-new-resource-pool-350x314.png)

1. Haga clic en el icono &quot;x&quot; en el nivel de usuario para eliminar un usuario del conjunto de recursos. Se eliminan de todas las listas en las que aparecen.\
   O\
   Para quitar todos los usuarios asociados con un rol, grupo, equipo o compañía, haga clic en **Quitar** en el rol, grupo, nivel de equipo o nivel de compañía del trabajo. Esto elimina del conjunto de recursos a todos los usuarios asociados a ese rol, grupo, equipo o compañía.

1. Haga clic en **Guardar**.
