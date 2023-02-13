---
product-area: resource-management
navigation-topic: resource-pools
title: Asociación de grupos de recursos con usuarios
description: Asociación de grupos de recursos con usuarios
author: Alina
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Asociación de grupos de recursos con usuarios

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

Los grupos de recursos son colecciones de usuarios que ayudan a administrar los recursos en Adobe Workfront.

Debe crear un grupo de recursos para poder asociarlo a los usuarios.

Puede asociar usuarios con grupos de recursos cuando esté creando sus grupos de recursos.

Si crea grupos de recursos sin rellenarlos con usuarios, más adelante puede asociarlos con usuarios a medida que edita o crea nuevos usuarios.

Para obtener información sobre los grupos de recursos, consulte [Resumen de los grupos de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Para obtener información sobre la creación de grupos de recursos, consulte [Crear grupos de recursos](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

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
   <td> <p>Editar el acceso a la Administración de recursos que incluye el acceso a Administrar grupos de recursos</p> <p>Editar acceso a Proyectos, Plantillas y Usuarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos para los proyectos, plantillas y usuarios con los que asocia los grupos de recursos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Asociar grupos de recursos con un usuario

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Usuarios**.
1. Marque la casilla situada junto al nombre de un usuario de la lista y haga clic en **Editar**.
1. Haga clic en **Planificación de recursos**.
1. Empiece a escribir el nombre de un grupo de recursos que desee asociar al usuario en la sección **Grupos de recursos** y, a continuación, selecciónelo en la lista, cuando aparezca.\
   Puede asociar varios grupos de recursos con un usuario.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. Haga clic en **Guardar cambios**.

Para obtener más información sobre la edición de usuarios, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Para obtener más información sobre la creación de usuarios nuevos, consulte [Agregar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Asociar grupos de recursos con usuarios de forma masiva

Puede editar varios usuarios de forma masiva y asociar los mismos grupos de recursos con todos ellos al mismo tiempo.

Para asociar grupos de recursos con varios usuarios de forma masiva:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Usuarios**.
1. Seleccione varios usuarios de la lista y haga clic en **Editar**.
1. Haga clic en **Planificación de recursos**.
1. Empiece a escribir el nombre de un grupo de recursos que desee asociar a los usuarios en la sección **Grupos de recursos** y, a continuación, selecciónelo en la lista, cuando aparezca.\
   Puede asociar varios grupos de recursos con varios usuarios.

   >[!NOTE]
   >
   >En este campo solo aparecen los grupos de recursos comunes a todos los usuarios seleccionados. Si los usuarios seleccionados no tienen grupos de recursos compartidos, este campo está vacío. Si este campo está vacío, los grupos de recursos que especifique aquí sobrescribirán sus grupos de recursos individuales.

1. Haga clic en **Guardar cambios**.

Para obtener más información sobre cómo editar usuarios de forma masiva, consulte [Editar perfiles de usuario de forma masiva](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
