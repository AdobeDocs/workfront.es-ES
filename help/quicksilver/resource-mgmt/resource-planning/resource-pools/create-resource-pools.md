---
product-area: resource-management
navigation-topic: resource-pools
title: Crear conjuntos de recursos
description: Los conjuntos de recursos son conjuntos de usuarios que le ayudan a administrar recursos con mayor facilidad en Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: 854197fcb8c4d3a87e4d93fe2ae9e968a3254027
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 8%

---

# Crear conjuntos de recursos {#create-resource-pools}

>[!CONTEXTUALHELP]
>id="wf_resource_pools"
>title="Conjuntos de recursos"
>abstract="Un conjunto de recursos es una colección de usuarios que se necesitan al mismo tiempo para la finalización de un proyecto. Después de crear un conjunto de recursos, puede asociarlo a proyectos y plantillas."

Los conjuntos de recursos son conjuntos de usuarios que le ayudan a administrar recursos con mayor facilidad en Adobe Workfront. Para obtener más información acerca de los conjuntos de recursos, vea [Resumen de los conjuntos de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td><p>Nuevo: Cualquiera</p>
       <p>o</p>
       <p>Actual: Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>o</p>
       <p>Actual: plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Administración de recursos que incluye acceso a Administrar conjuntos de recursos</p> <p>Editar el acceso a Proyectos, Plantillas y Usuarios</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Administre permisos para los proyectos, plantillas y usuarios con los que desee asociar los conjuntos de recursos</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear un conjunto de recursos {#create-a-resource-pool}

{{step1-to-resourcing}}

1. Haga clic en **Conjuntos de recursos** en el panel izquierdo.
1. Haga clic en **Nuevo conjunto de recursos**.

   ![Conjuntos de recursos](assets/list-of-resource-pools.png)

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
        </ul><p>Sugerencia: solo puede agregar usuarios, equipos, <span>roles,</span> o compañías activos.</p><br>Es posible que tenga que desplazarse hacia abajo en el cuadro de diálogo para ver todos los usuarios del conjunto de recursos.
        <p>Nota: Si un usuario se convierte en miembro de un grupo, equipo, empresa o está asociado a un rol después de que el grupo, equipo, empresa o rol se hayan agregado al conjunto de recursos, el nuevo miembro no se agrega automáticamente al conjunto de recursos. <br>Si un usuario pertenece al equipo, grupo, compañía y rol que está agregando, al mismo tiempo, el usuario se agregará solo una vez al conjunto de recursos.<br>Los usuarios que se desactivan después de haber sido agregados al conjunto de recursos aparecen atenuados en la lista de usuarios y se marcan como desactivados.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Opcional) Use el vínculo **Deshacer** para quitar los usuarios agregados mediante un grupo, equipo, compañía o rol.

   >[!NOTE]
   >
   >No hay límite en cuanto a la cantidad de usuarios que puede tener en un Conjunto de recursos. Sin embargo, se recomienda no agregar demasiados usuarios a un Conjunto de recursos, ya que de lo contrario la Administración de recursos podría convertirse en un desafío. La lista de usuarios sólo muestra los 2.000 primeros usuarios del Conjunto de recursos y se enumeran alfabéticamente.

   ![Usuarios agregados al conjunto de recursos](assets/users-in-resource-pool2.png)

1. (Opcional) Haga clic en el icono X a la derecha del nombre de un usuario para eliminarlo. Para obtener más información acerca de cómo quitar usuarios de un conjunto de recursos, vea [Quitar usuarios de conjuntos de recursos](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Opcional) Use la opción **Buscar** para encontrar un usuario en el conjunto de recursos.
1. Haga clic en **Crear**.
