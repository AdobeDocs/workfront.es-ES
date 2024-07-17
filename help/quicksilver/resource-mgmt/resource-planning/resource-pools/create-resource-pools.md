---
product-area: resource-management
navigation-topic: resource-pools
title: Crear conjuntos de recursos
description: Los conjuntos de recursos son conjuntos de usuarios que le ayudan a administrar recursos con mayor facilidad en Adobe Workfront. Para obtener más información sobre conjuntos de recursos, consulte Información general sobre conjuntos de recursos
author: Alina
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 1%

---

# Crear conjuntos de recursos

Los conjuntos de recursos son conjuntos de usuarios que le ayudan a administrar recursos con mayor facilidad en Adobe Workfront. Para obtener más información acerca de los conjuntos de recursos, vea [Resumen de los conjuntos de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

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
   <td> <p>Editar acceso a Administración de recursos que incluye acceso a Administrar conjuntos de recursos</p> <p>Editar el acceso a Usuarios, Proyectos y Plantillas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos para los proyectos y las plantillas con los que desea asociar los conjuntos de recursos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear un conjunto de recursos {#create-a-resource-pool}

1. Inicie sesión como un usuario que tenga acceso para editar Conjuntos de recursos.\
   Para obtener más información, consulte [Crear un conjunto de recursos](#create-a-resource-pool).

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Recursos**.
1. Haga clic en **Conjuntos de recursos** en el panel izquierdo.\
   ![resource_pools_tab.png](assets/resource-pools-tab-350x198.png)

1. Haga clic en **Nuevo conjunto de recursos**.
1. Especifique lo siguiente:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nombre</strong></td>
      <td>Es el nombre del conjunto de recursos.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descripción</strong></td>
      <td>Esta es una breve descripción de este conjunto de recursos. Por ejemplo, puede especificar para qué propósito se debe utilizar.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Miembros del conjunto</strong></td>
      <td><p> Agregue usuarios al Conjunto de recursos individualmente.<br>O <br>Para agregar una gran cantidad de usuarios al conjunto de recursos al mismo tiempo. Puede agregar una de las siguientes entidades asociadas con usuarios o una colección de usuarios:
        <ul>
         <li><strong>Equipos</strong>: todos los miembros del equipo se agregan al Conjunto de recursos.</li>
         <li><strong>Grupos</strong>: todos los miembros del grupo se agregan al Conjunto de recursos.</li>
         <li><strong>Roles</strong>: todos los usuarios asociados con ese rol se agregan al Conjunto de recursos.</li>
         <li><strong>Compañías</strong>: todos los usuarios de la compañía se agregan al Conjunto de recursos.</li>
        </ul><p>Sugerencia: solo puede agregar usuarios, equipos, <span>roles,</span> o compañías activos.</p><p>Nota: Si un usuario se convierte en miembro de un grupo, equipo, empresa o está asociado a un rol después de que el grupo, equipo, empresa o rol se hayan agregado al conjunto de recursos, el nuevo miembro no se agrega automáticamente al conjunto de recursos. <br>Si un usuario pertenece al equipo, grupo, compañía y rol que está agregando, al mismo tiempo, el usuario se agregará solo una vez al conjunto de recursos.<br>Los usuarios que se desactivan después de haber sido agregados al conjunto de recursos aparecen atenuados en la lista de usuarios y se marcan como desactivados.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Opcional) Use el vínculo **Deshacer** para quitar los usuarios agregados mediante un grupo, equipo, compañía o rol.

   >[!NOTE]
   >
   >No hay límite en cuanto a la cantidad de usuarios que puede tener en un Conjunto de recursos. Sin embargo, se recomienda no agregar demasiados usuarios a un Conjunto de recursos, ya que de lo contrario la Administración de recursos podría convertirse en un desafío. La lista de usuarios sólo muestra los 2.000 primeros usuarios del Conjunto de recursos y se enumeran alfabéticamente.

   ![Resource_pools_NEW___UNDO_button_for_team_groups_etc.png](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. (Opcional) Haga clic en el icono X a la derecha del nombre de un usuario para eliminarlo. Para obtener más información acerca de cómo quitar usuarios de un conjunto de recursos, vea [Quitar usuarios de conjuntos de recursos](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Opcional) Use la opción **Buscar** para encontrar un usuario en el conjunto de recursos.
1. Haga clic en **Crear**.
