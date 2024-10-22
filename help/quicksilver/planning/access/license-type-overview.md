---
title: Información general sobre el tipo de licencia al usar Adobe Workfront Planning
description: El acceso a Adobe Workfront Planning depende del tipo de licencia, además de los permisos para los objetos. No todos los usuarios de la organización tienen el mismo acceso y permisos para utilizar Adobe Workfront Planning. En este artículo se describen los niveles de acceso que los usuarios podrían tener a Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---


# Información general sobre el tipo de licencia al usar Adobe Workfront Planning

{{planning-important-intro}}

El tipo de licencia de Adobe Workfront funciona junto con los permisos de Adobe Workfront Planning para proporcionar el siguiente acceso:

* Ver, contribuir o administrar espacios de trabajo
* Ver o administrar vistas.

Para obtener información acerca de los permisos de los objetos en Workfront Planning, vea [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Para obtener información sobre el acceso a Workfront Planning, consulte [Descripción general del acceso a Adobe Planning](/help/quicksilver/planning/access/access-overview.md).

## La relación entre los tipos de licencia de Workfront y los permisos de Workfront Planning

En la tabla siguiente se describe la relación entre el tipo de licencia de un usuario en Adobe Workfront y el nivel de permisos que puede concederles a los objetos de Adobe Workfront Planning basados en esa licencia.

Al conceder permisos de usuario a un espacio de trabajo, también se les conceden permisos para tipos de registros, registros y campos.

Debe conceder a los usuarios permisos independientes a las vistas, además de los que tienen para los espacios de trabajo, para poder acceder y administrar las vistas.

| Tipo de licencia de Adobe Workfront* | Permisos más altos permitidos en Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Estándar | <p>Los usuarios pueden administrar espacios de trabajo y vistas. Pueden crear, editar o eliminar espacios de trabajo, tipos de registros, registros, campos y vistas.</p> <br> <p>Los administradores del sistema tienen permisos de administración en todos los espacios de trabajo, incluidos los que no han creado.</p> |
| Ligero o colaborador | <p>Los usuarios pueden ver los espacios de trabajo compartidos con ellos, así como los tipos de registro, registros y campos de dichos espacios de trabajo.</p> <br> <p>Los usuarios pueden ver las vistas que se han compartido con ellos, pero no pueden crear las suyas. </p><br> <p>Los usuarios no pueden crear, editar ni eliminar espacios de trabajo, tipos de registros, registros o campos.</p> |

*Workfront Planning no está disponible para licencias de Workfront heredadas.
Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


<!--OLD 

| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

### Tipos de licencias y permisos de Workspace

Solo los usuarios con una licencia estándar pueden tener permisos de Contribute o Administrar en los espacios de trabajo. Los usuarios con todos los demás tipos de licencia pueden tener permisos de visualización en los espacios de trabajo compartidos con ellos.

Los administradores del sistema pueden ver todos los espacios de trabajo del sistema, incluso los que no han creado.

>[!INFO]
>
>**EJEMPLO:**
>
>Los colaboradores o los usuarios con licencia básica no pueden contribuir ni administrar espacios de trabajo y sus objetos.
>
>Hay una indicación en el cuadro de diálogo de uso compartido de que no se pueden conceder permisos a los usuarios para contribuir o administrar un espacio de trabajo cuando tienen una licencia de nivel inferior, ya que estos niveles de permisos están atenuados.
>
>![](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### Tipos de licencias y permisos de visualización

Solo los usuarios con una licencia Standard pueden tener permisos de administración en las vistas. Los usuarios con todos los demás tipos de licencia pueden tener permisos de visualización para las vistas compartidas con ellos.

>[!INFO]
>
>**EJEMPLO:**
>
>Los colaboradores o los usuarios con licencia básica no pueden administrar las vistas. Pueden aplicar filtros, ordenaciones o agrupaciones temporales a las vistas a las que pueden acceder.
>
>Hay una indicación en el cuadro de uso compartido de que no se pueden conceder permisos a los usuarios para administrar una vista cuando tienen una licencia de nivel inferior, ya que estos niveles de permisos están atenuados.
>
>![](assets/permissions-grayed-out-for-light-user.png)
