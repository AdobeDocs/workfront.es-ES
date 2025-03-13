---
title: Información general sobre el tipo de licencia al usar Adobe Workfront Planning
description: El acceso a Adobe Workfront Planning depende del tipo de licencia, además de los permisos para los objetos. No todos los usuarios de la organización tienen el mismo acceso y permisos para utilizar Adobe Workfront Planning. En este artículo se describen los niveles de acceso que los usuarios podrían tener a Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: a3c82d8be6945a91a249d64923c6377a5edfa268
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 42%

---


# Información general sobre el tipo de licencia al usar Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

El tipo de licencia de Adobe Workfront funciona junto con los permisos de Adobe Workfront Planning para proporcionar el siguiente acceso:

* Ver, contribuir o administrar espacios de trabajo <!--<span class="preview">or record types</span>-->
* Ver o administrar vistas.

Para obtener información acerca de los permisos de los objetos en Workfront Planning, consulte [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Para obtener información sobre el acceso a Workfront Planning, consulte [Información general sobre el acceso a Adobe Planning](/help/quicksilver/planning/access/access-overview.md).

## La relación entre los tipos de licencia de Workfront y los permisos de Workfront Planning

En la tabla siguiente se describe la relación entre el tipo de licencia de un usuario en Adobe Workfront y el nivel de permisos que puede concederles a los objetos de Adobe Workfront Planning basados en esa licencia.

Al conceder permisos de usuario a un espacio de trabajo, también se les conceden permisos para tipos de registros, registros y campos.

Debe conceder a los usuarios permisos independientes a las vistas, además de los que tienen para los espacios de trabajo, para poder acceder y administrar las vistas.

<!--

<div class="preview">

Consider the following when working with record type permissions: 

* Users automatically inherit record type permissions from workspaces. 
* When a user has Manage permissions to a workspace, they cannot have a lesser access to record type. 
* Users cannot have greater permissions to a record type than they have for the workspace the record type belongs to.

</div>
-->

| Tipo de licencia de Adobe Workfront* | Permisos más altos permitidos en Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Estándar | <p>Los usuarios pueden administrar los espacios de trabajo <!--<span class="preview">, record types, </span> --> y las vistas. Pueden crear, editar o eliminar espacios de trabajo, tipos de registros, registros, campos y vistas.</p> <br> <p>Los administradores del sistema tienen permisos de administración en todos los espacios de trabajo, incluidos los que no han creado.</p> |
| Ligero o colaborador | <p>Los usuarios pueden ver los espacios de trabajo compartidos con ellos, así como los tipos de registro, registros y campos de dichos espacios de trabajo.</p> <br> <p>Los usuarios pueden ver las vistas que se han compartido con ellos, pero no pueden crear las suyas. </p><br> <p>Los usuarios no pueden crear, editar ni eliminar espacios de trabajo, tipos de registros, registros o campos.</p> |

*Workfront Planning no está disponible para licencias de Workfront heredadas.
Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


### Tipos de licencias y permisos para espacios de trabajo

<!--should we add "record types" in the title above and to this section?-->

Solo los usuarios con una licencia estándar pueden tener permisos de contribución o administración en los espacios de trabajo <!--<span class="preview">and record types</span>-->. Los permisos de Contribuir y Administrar en los espacios de trabajo <!--<span class="preview">and record types</span>--> también se transfieren a los tipos de registro, registros y campos.

<!--take "record types" out from the end of the sentence above when we release record type-level access-->

Los usuarios con todos los demás tipos de licencia pueden tener permisos de visualización en los espacios de trabajo <!--<span class="preview"> and record types </span> --> compartidos con ellos, así como en sus tipos de registro, registros y campos.

<!--take "record types" out from the end of the sentence above when we release record type-level access-->

Los administradores del sistema pueden ver todos los espacios de trabajo del sistema, incluidos los que no han creado.

<!--does the shot below need to be replaced for record types??-->

>[!INFO]
>
>**Ejemplo:**
>
>Los colaboradores o los usuarios con licencia básica no pueden contribuir ni administrar espacios de trabajo y sus objetos.
>
>Hay una indicación en el cuadro de diálogo de uso compartido de que no se pueden conceder permisos a los usuarios para contribuir o administrar un espacio de trabajo cuando tienen una licencia de nivel inferior, ya que estos niveles de permisos están atenuados.
>
>![Permisos atenuados para el usuario colaborador en el espacio de trabajo](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### Tipos de licencias y permisos para vistas

Solo los usuarios con una licencia Standard pueden tener permisos de administración en las vistas. Los usuarios con todos los demás tipos de licencia pueden tener permisos de visualización para las vistas compartidas con ellos.

>[!INFO]
>
>**Ejemplo:**
>
>Los colaboradores o los usuarios con licencia básica no pueden administrar las vistas. Pueden aplicar filtros, ordenaciones o agrupaciones temporales a las vistas a las que pueden acceder.
>
>Hay una indicación en el cuadro de uso compartido de que no se pueden conceder permisos a los usuarios para administrar una vista cuando tienen una licencia de nivel inferior, ya que estos niveles de permisos están atenuados.
>
>![Permisos atenuados para el usuario ligero al compartir la vista](assets/permissions-grayed-out-for-light-user.png)
