---
product-area: resource-management
navigation-topic: resource-pools
title: Asociar conjuntos de recursos a los usuarios
description: Debe crear un conjunto de recursos para poder asociarlo a los usuarios. Puede asociar usuarios con conjuntos de recursos al crear los conjuntos de recursos.
author: Lisa
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: 36599722aafadcbbc630650a94005fd73b3e517e
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# Asociar conjuntos de recursos a los usuarios

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

Los conjuntos de recursos son colecciones de usuarios que le ayudan a administrar los recursos en Adobe Workfront.

Debe crear un conjunto de recursos para poder asociarlo a los usuarios.

Puede asociar usuarios con conjuntos de recursos al crear los conjuntos de recursos.

Si crea conjuntos de recursos sin rellenarlos con los usuarios, más adelante puede asociarlos a los usuarios mientras edita o crea nuevos usuarios.

Para obtener información acerca de los conjuntos de recursos, vea [Resumen de los conjuntos de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Para obtener información acerca de cómo crear conjuntos de recursos, vea [Crear conjuntos de recursos](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

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
   <td> <p>Editar acceso a Administración de recursos que incluye acceso a Administrar conjuntos de recursos</p> <p>Editar el acceso a Proyectos, Plantillas y Usuarios</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para los proyectos, plantillas y usuarios con los que asocia los conjuntos de recursos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Asociar conjuntos de recursos a un usuario

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Usuarios**.
1. Marque la casilla junto al nombre de un usuario en la lista y luego haga clic en **Editar**.
1. Haga clic en **Planificación de recursos**.
1. Empiece a escribir el nombre de un conjunto de recursos que desee asociar con el usuario en el campo **Conjuntos de recursos** y, a continuación, selecciónelo en la lista cuando aparezca.\
   Puede asociar varios conjuntos de recursos a un usuario.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. Haga clic en **Guardar cambios**.

Para obtener más información sobre cómo editar usuarios, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Para obtener más información sobre cómo crear usuarios nuevos, consulte [Agregar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Asociar conjuntos de recursos a usuarios de forma masiva

Puede editar varios usuarios de forma masiva y asociar los mismos conjuntos de recursos a todos ellos al mismo tiempo.

Para asociar conjuntos de recursos a varios usuarios de forma masiva:

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Usuarios**.
1. Seleccione varios usuarios en la lista y haga clic en **Editar**.
1. Haga clic en **Planificación de recursos**.
1. Empiece a escribir el nombre de un conjunto de recursos que desee asociar con los usuarios en el campo **Conjuntos de recursos** y, a continuación, selecciónelo en la lista cuando aparezca.\
   Puede asociar varios conjuntos de recursos con varios usuarios.

   >[!NOTE]
   >
   >En este campo solo aparecen los conjuntos de recursos que son comunes a todos los usuarios seleccionados. Si los usuarios seleccionados no tienen conjuntos de recursos compartidos, este campo está vacío. Si este campo está vacío, los conjuntos de recursos que especifique aquí sobrescribirán sus conjuntos de recursos individuales.

1. Haga clic en **Guardar cambios**.

Para obtener más información sobre cómo editar usuarios en lotes, consulte [Editar perfiles de usuario en lotes](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
