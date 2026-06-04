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
TQID: https://experienceleague.adobe.com/dspQLWwqjYdo3y9Trqv70ylGd1hFE-ynJaBU7-xLyxg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 254
ht-degree: 100%

---

# Obtener tokens de OAuth2

## Cómo obtener tókenes de OAuth2

Devuelve el token de actualización de OAuth2 y el token de acceso de un usuario autenticado. Se invoca una vez cuando el usuario aprovisiona un proveedor de documentos. Se realizan llamadas posteriores para obtener un token de acceso actualizado.

**URL**

POST /any/url

La dirección URL es configurable y corresponde al valor URL del punto final de token en la página Configuración de integración personalizada.

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
   <td>sí</td>
   <td><p>Los valores incluyen “authorization_code” o “refresh_token”. El valor especificado indica cuál de los dos parámetros se pasará a esta llamada de API: code o refresh_token.</p></td>
  </tr>
  <tr>
   <td>code</td>
   <td>depende</td>
   <td><p>El código de autorización se envía a Adobe Workfront justo después de que el usuario haga clic en el botón Conceder. Solo es necesario cuando el tipo de concesión es “authorization_code”. El código de autorización debe ser de corta duración y normalmente caduca en 10 minutos o menos.</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>depende</td>
   <td><p>Solo es necesario cuando se realizan llamadas subsiguientes para recuperar un nuevo access_token, dado que el access_token anterior ha caducado. Al enviar este valor, establezca el parámetro grant_type en "refresh_token".</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>sí</td>
   <td>El ID de cliente configurado en Workfront para esta integración personalizada.</td>
  </tr>
  <tr>
   <td>client_secret</td>
   <td>sí</td>
   <td> El secreto de cliente configurado en Workfront para esta integración personalizada.</td>
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
   <td><p>Un token utilizado para hacer llamadas de API autorizadas en nombre del usuario. Debería caducar para evitar llamadas de API no autorizadas.</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>Cadena</td>
   <td><p>Un token de larga duración que se utiliza para recuperar un nuevo access_token llamando a este método de API.</p></td>
  </tr>
  <tr>
   <td>expires_in </td>
   <td>long</td>
   <td><p>(opcional) El tiempo (en segundos) antes de que access_token caduque, por lo general, 3.600.</p></td>
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
