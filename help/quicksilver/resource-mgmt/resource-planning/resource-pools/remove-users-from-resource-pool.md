---
product-area: resource-management
navigation-topic: resource-pools
title: Eliminar usuarios de grupos de recursos
description: Aunque no hay límite para cuántos usuarios puede tener en un grupo de recursos, la lista de usuarios solo muestra los primeros 2000 usuarios enumerados alfabéticamente.
author: Alina
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# Eliminar usuarios de grupos de recursos

Aunque no hay límite para cuántos usuarios puede tener en un grupo de recursos, la lista de usuarios solo muestra los primeros 2000 usuarios enumerados alfabéticamente.

Le recomendamos que elimine los usuarios que hayan sido desactivados o que hayan movido funciones o departamentos para asegurarse de que siempre tiene una lista precisa de usuarios en todos los grupos de recursos.

Para obtener más información sobre los grupos de recursos, consulte [Resumen de los grupos de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Pro y superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a la Administración de recursos que incluye el acceso a Administrar grupos de recursos</p> <p>Ver o acceso superior a Usuarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>(NOTE:&nbsp;I don't think this is needed for removing users from the pool)</p> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Eliminar usuarios de un grupo de recursos

Puede quitar usuarios de un grupo de recursos cuando esos usuarios ya no se necesiten en ese grupo.

Para quitar un usuario de un grupo de recursos:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Recurso**.
1. Haga clic en **Grupos de recursos** en el panel izquierdo.
1. Seleccione un grupo de recursos y haga clic en **Editar.**O\
   Haga clic en el nombre de un grupo de recursos.

1. Comience a escribir el nombre de un usuario que desee eliminar en la **Buscar en este grupo de recursos** campo .\
   O\
   Empiece a escribir el nombre de una empresa, función de trabajo, equipo o grupo, si desea eliminar todos los usuarios asociados a esas entidades.\
   ![search_interior_NEW_resource_pool.png](assets/search-inside-new-resource-pool-350x314.png)

1. Haga clic en el icono &quot;x&quot; en el nivel de usuario para eliminar un usuario del grupo de recursos. Se eliminan de todas las listas en las que aparecen.\
   O\
   Para eliminar todos los usuarios asociados a una función de trabajo, grupo, equipo o empresa, haga clic en **Eliminar** en el nivel de rol de trabajo, grupo, equipo o empresa. Esto elimina de la agrupación de recursos a todos los usuarios asociados a esa función de trabajo, grupo, equipo o empresa.

1. Haga clic en **Guardar**.
