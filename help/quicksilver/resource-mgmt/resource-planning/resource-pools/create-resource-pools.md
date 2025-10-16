---
product-area: resource-management
navigation-topic: resource-pools
title: Crear conjuntos de recursos
description: Los conjuntos de recursos son conjuntos de usuarios que ayudan a administrar recursos con mayor facilidad en Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 95%

---

# Crear conjuntos de recursos {#create-resource-pools}

>[!CONTEXTUALHELP]
>id="wf_resource_pools"
>title="Conjuntos de recursos"
>abstract="Un conjunto de recursos es una colección de usuarios que se necesitan al mismo tiempo para la finalización de un proyecto. Después de crear un conjunto de recursos, puede asociarlo a proyectos y plantillas."

Los conjuntos de recursos son conjuntos de usuarios que ayudan a administrar recursos con mayor facilidad en Adobe Workfront. Para obtener más información acerca de los conjuntos de recursos, consulte [Información general sobre los conjuntos de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

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
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a la administración de recursos, que incluye el acceso a la administración de conjuntos de recursos</p> <p>Editar acceso a proyectos, plantillas y usuarios</p></td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Administre permisos para los proyectos, plantillas y usuarios con los que desee asociar los conjuntos de recursos</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear un conjunto de recursos {#create-a-resource-pool}

{{step1-to-resourcing}}

1. Haga clic en **Conjuntos de recursos** en el panel de la izquierda.
1. Haga clic en **Nuevo conjunto de recursos**.

   ![Conjuntos de recursos](assets/list-of-resource-pools.png)

1. Especifique lo siguiente:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nombre</strong></td>
      <td>Este es el nombre del conjunto de recursos.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descripción</strong></td>
      <td>Esta es una breve descripción sobre este conjunto de recursos. Por ejemplo, especifique para qué propósito se debería utilizar.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Miembros del conjunto</strong></td>
      <td><p> Añada usuarios al conjunto de recursos individualmente.<br>O <br>para añadir una gran cantidad de usuarios al conjunto de recursos al mismo tiempo. Es posible añadir una de las siguientes entidades asociadas con usuarios o colecciones de usuarios:
        <ul>
         <li><strong>Equipos</strong>: todos los miembros del equipo se añaden al conjunto de recursos.</li>
         <li><strong>Grupos</strong>: todos los miembros del grupo se añaden al conjunto de recursos.</li>
         <li><strong>Funciones</strong>: todos los usuarios asociados con esa función se añaden al conjunto de recursos.</li>
         <li><strong>Compañías</strong>: todos los usuarios de la compañía se añaden al conjunto de recursos.</li>
        </ul><p>Sugerencia: solo es posible añadir usuarios, equipos, <span>funciones</span> o compañías activos.</p><br>Es posible que tenga que desplazarse hacia abajo en el cuadro de diálogo para ver a todos los usuarios del conjunto de recursos.
        <p>Nota: si un usuario se convierte en miembro de un grupo, equipo, empresa o estuviera asociado a una función después de que el grupo, equipo, empresa o función se añadieran al conjunto de recursos, el nuevo miembro no se añadirá automáticamente al conjunto de recursos. <br>Si un usuario perteneciera al equipo, grupo, compañía y función que está añadiendo, al mismo tiempo, el usuario se añadirá solo una vez al conjunto de recursos.<br>Los usuarios que se desactivan después de haber sido añadidos al conjunto de recursos aparecen atenuados en la lista de usuarios y se marcan como desactivados.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Opcional) Use el vínculo **Deshacer** para quitar a los usuarios añadidos mediante grupos, equipos, compañías o funciones.

   >[!NOTE]
   >
   >No hay límite en cuanto a la cantidad de usuarios que se pueden tener en un conjunto de recursos. Sin embargo, se recomienda no añadir demasiados usuarios a un conjunto de recursos, ya que de lo contrario la administración de recursos se convertiría en un desafío. La lista de usuarios solo muestra los 2000 primeros usuarios del conjunto de recursos y se enumeran alfabéticamente.

   ![Usuarios añadidos al conjunto de recursos](assets/users-in-resource-pool2.png)

1. (Opcional) Haga clic en el icono de la X de la derecha del nombre de un usuario para eliminarlo. Para obtener más información acerca de cómo quitar usuarios de un conjunto de recursos, consulte [Quitar usuarios de conjuntos de recursos](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Opcional) Use la opción **Buscar** para encontrar a usuarios del conjunto de recursos.
1. Haga clic en **Crear**.
