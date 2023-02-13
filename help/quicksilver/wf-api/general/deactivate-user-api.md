---
content-type: api
product-area: user-management
navigation-topic: general-api
title: Desactivar un usuario a través de la API
description: Desactivar un usuario a través de la API
author: John
feature: Workfront API
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: 50675b7af3fcd2188a18391732a93a7b67454db9
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# Desactivar un usuario a través de la API

Cuando un usuario abandona la organización, puede desactivar el usuario, haciendo que su licencia de Adobe Workfront esté disponible para otro usuario e impidiendo que se le asigne trabajo de forma inadvertida. Al desactivar un usuario, se preserva su historial de trabajo, incluidas sus asignaciones de trabajo y su asociación con notas, horas y documentos.

Para obtener más información sobre la desactivación de un usuario, consulte &quot; [Desactivar o reactivar un usuario](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Para obtener información sobre el uso de la API principal, consulte [Conceptos básicos de API](../../wf-api/general/api-basics.md).

Para desactivar un usuario a través de la API:

1. Genere una clave de API mediante la siguiente solicitud de API:

```
<domain>.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. Busque el GUID del usuario que desea desactivar.

   1. Utilice la siguiente solicitud de API para recuperar el GUID de todos los usuarios del sistema, tenga en cuenta que la variable **isActive** se muestra el campo **true** para usuarios que están activos actualmente y **false** para usuarios desactivados:

```
<domain>`.my.workfront.com/attask/api/v7.0/USER/search?fields=isActive
```

1. Localice el GUID del usuario que desea desactivar, utilice lo siguiente **PUT** solicitud para cambiar el **isActive** valor de campo a **false**:

```
<domain>`.my.workfront.com/attask/api/v7.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. La respuesta mostrará que la variable **isActive** el valor de campo ha cambiado de **true** a **false** indicando que el usuario ha sido desactivado:

<!-- [Copy](javascript:void(0);) -->
<pre></pre>
