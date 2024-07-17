---
content-type: api
product-area: user-management
navigation-topic: general-api
title: Desactivar un usuario mediante la API
description: Desactivar un usuario mediante la API
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# Desactivar un usuario mediante la API

Cuando un usuario abandona la organización, puede desactivarlo, haciendo que su licencia de Adobe Workfront esté disponible para otro usuario y evitando que se le asigne trabajo de forma involuntaria. Al desactivar un usuario, conserva su historial laboral, incluidas sus asignaciones de trabajo y su asociación con notas, horas y documentos.

Para obtener más información sobre cómo desactivar un usuario, consulte &quot; [Desactivar o reactivar un usuario](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Para obtener información acerca del uso de la API principal, consulte [Conceptos básicos de la API](../../wf-api/general/api-basics.md).

Para desactivar un usuario a través de la API:

1. Genere una clave de API mediante la siguiente solicitud de API:

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. Busque el GUID del usuario que desea desactivar.

   1. Utilice la siguiente solicitud de API para recuperar el GUID de todos los usuarios del sistema. Tenga en cuenta que el campo **isActive** muestra **true** para los usuarios que están activos actualmente y **false** para los usuarios que se han desactivado:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. Busque el GUID del usuario que desea desactivar. Use la siguiente solicitud de **PUT** para cambiar el valor del campo **isActive** del usuario a **false**:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. La respuesta mostrará que el valor del campo **isActive** ha cambiado de **true** a **false** indicando que el usuario ha sido desactivado:

<!-- [Copy](javascript:void(0);) -->
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>
