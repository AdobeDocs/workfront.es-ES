---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: HTTP &gt; Otros módulos
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 84%

---

# HTTP > Otros módulos

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [HTTP > Otros módulos](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/universal-connectors/http-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] requiere una licencia de [!UICONTROL Adobe Workfront Fusion] además de una licencia de [!UICONTROL Adobe Workfront].

La aplicación [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] proporciona varios módulos de comunicación basados en el protocolo HTTP (Protocolo de transferencia de hipertexto). HTTP es la base de la comunicación de datos para la Internet. Puede utilizar los módulos para descargar páginas web y archivos, llamar a webhooks y extremos de API, etc.

La elección correcta del módulo depende del mecanismo de autenticación/autorización que emplee el recurso al que desea acceder. A continuación, se muestran ejemplos de módulos

* Realizar una solicitud: módulo universal destinado principalmente a recursos que no utilizan ningún tipo de autenticación o autorización
* Realizar una solicitud de autenticación básica: para recursos que emplean la autenticación básica (BA) [!DNL HTTP]
* Realizar una solicitud de OAuth 2.0: para recursos que emplean el protocolo de autorización de OAuth 2.0
* Realizar una solicitud de autenticación de certificado de cliente: para recursos que emplean un protocolo de autorización que requiere un certificado del lado del cliente.
* Realizar una solicitud de autorización de clave API: para recursos que utilizan claves de API para la autorización.

>[!NOTE]
>
>Si se está conectando a un producto de Adobe que actualmente no tiene un conector dedicado, le recomendamos utilizar el módulo de Adobe Authenticator.
>
>Para obtener más información, consulte [Módulo de Adobe Authenticator](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

## Módulos de solicitud

Consulte los siguientes artículos para obtener instrucciones específicas sobre los módulos de solicitud:

* [Módulo [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [Módulo [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud de autorización básica]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [Módulo [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud OAuth 2.0]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [Módulo [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud de autorización de certificado de cliente]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud de autorización de clave API]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## Otros módulos de acción

* [[!UICONTROL Obtener un archivo]](#get-a-file)
* [[!UICONTROL Resolver una dirección URL de destino]](#resolve-a-target-url)

### [!UICONTROL Obtener un archivo]

Este módulo de acción descarga un archivo desde la dirección URL especificada. Una vez descargado el archivo, puede procesarlo aún más (asignar los datos del archivo) mediante otros módulos en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Introduzca o asigne la dirección URL del archivo que desea descargar. </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Resolver una dirección URL de destino]

Este módulo de acción resuelve una cadena de redirecciones HTTP y devuelve una dirección URL de destino.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Escriba o asigne la dirección URL que desea resolver, como una dirección URL de [!DNL bit.ly].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method] </td> 
   <td> <p>Seleccione si desea utilizar el método [!UICONTROL HEAD] o el método [!UICONTROL GET].</p> </td> 
  </tr> 
 </tbody> 
</table>

## Módulos de iterador

### [!UICONTROL Recuperar encabezados]

Este módulo devuelve cada encabezado (nombre y valor) del módulo HTTP especificado en un paquete independiente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Seleccione el módulo del que desee recuperar los encabezados.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Generación de tokens web JSON (JWT)

Es posible generar un token JWT con la ayuda de funciones integradas:

Encabezado:

![](assets/jwt-header-350x19.png)

Código para copiar y pegar:

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Carga útil:

![](assets/jwt-payload-350x17.png)

Código para copiar y pegar:

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Token:

![](assets/jwt-token-350x15.png)

Código para copiar y pegar:

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```
