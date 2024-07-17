---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtener tokens de OAuth2
description: Obtener tokens de OAuth2
author: Becky
feature: Workfront API
role: Developer
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 3%

---


# Obtener tokens de OAuth2

## Obteniendo tokens de OAuth2

Devuelve el token de actualización de OAuth2 y el token de acceso de un usuario autenticado. Se invoca una vez cuando el usuario aprovisiona un proveedor de documentos. Se realizan llamadas posteriores para obtener un token de acceso actualizado.

**URL**

POST /any/url

La dirección URL es configurable y corresponde al valor URL de extremo de token en la página Configuración de integración personalizada.

### Parámetros de consulta

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>Nombre</th>
   <th>Requerido</th>
   <th>Descripción</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>grant_type</td>
   <td>yes</td>
   <td><p>Los valores incluyen "authorization_code" o "refresh_token". El valor especificado indica cuál de los dos parámetros se pasará a esta llamada de API: code o refresh_token.</p></td>
  </tr>
  <tr>
   <td>código</td>
   <td>depende</td>
   <td><p>El código de autorización se envía a Adobe Workfront justo después de que el usuario haga clic en el botón Conceder. Esto solo es necesario cuando el tipo de concesión es "authorization_code". El código de autorización debe ser de corta duración y normalmente caduca en 10 minutos o menos.</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>depende</td>
   <td><p>Esto solo es necesario cuando se realizan llamadas subsiguientes para recuperar un nuevo access_token, dado que el access_token anterior ha caducado. Al enviar este valor, establezca el parámetro grant_type en "refresh_token".</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>yes</td>
   <td>El ID de cliente configurado en Workfront para esta integración personalizada.</td>
  </tr>
  <tr>
   <td>client_secret</td>
   <td>yes</td>
   <td> Secreto de cliente configurado en Workfront para esta integración personalizada.</td>
  </tr>
 </tbody>
</table>

 

## Respuesta

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>Nombre</th>
   <th>Tipo </th>
   <th>Descripción</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>access_token </td>
   <td>Cadena</td>
   <td><p>Un token utilizado para hacer llamadas de API autorizadas en nombre del usuario. Esto debería caducar para evitar llamadas de API no autorizadas.</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>Cadena</td>
   <td><p>Un token de larga duración que se utiliza para recuperar un nuevo access_token llamando a este método de API.</p></td>
  </tr>
  <tr>
   <td>expires_in </td>
   <td>largo</td>
   <td><p>(opcional) Tiempo (en segundos) antes de que access_token caduque, por lo general, 3600.</p></td>
  </tr>
 </tbody>
</table>

**Ejemplo**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```

## Respuesta

```
{
access_token:"ad8af5ad5ads759",
refresh_token:"9a0h5d87d808ads",
expires_id:3600
}
```
