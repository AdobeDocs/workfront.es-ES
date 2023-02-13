---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: HTTP &gt; Otros módulos
description: La variable [!DNL Adobe Workfront Fusion] La aplicación HTTP proporciona varios módulos de comunicación basados en el protocolo de transferencia de hipertexto (HTTP). HTTP es la base de la comunicación de datos para la World Wide Web. Puede utilizar los módulos para descargar páginas web y archivos, llamar a enlaces web y extremos de API, etc.
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# HTTP > Otros módulos

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] requiere un [!UICONTROL Adobe Workfront Fusion] además de una [!UICONTROL Adobe Workfront] licencia.

La variable [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] La aplicación proporciona varios módulos de comunicación basados en el protocolo de transferencia de hipertexto (HTTP). HTTP es la base de la comunicación de datos para la World Wide Web. Puede utilizar los módulos para descargar páginas web y archivos, llamar a enlaces web y extremos de API, etc.

La elección correcta del módulo depende del mecanismo de autenticación/autorización que emplee el recurso al que desee acceder. Los siguientes son ejemplos de módulos

* Realizar una solicitud:módulo universal destinado principalmente a recursos que no emplean ningún tipo de autenticación/autorización
* Realizar una solicitud de autenticación básica:para recursos que empleen [!DNL HTTP] Autenticación básica (BA)
* Realice una solicitud de OAuth 2.0: para recursos que utilizan el protocolo de autorización de OAuth 2.0
* Realizar una solicitud de autenticación de certificado de cliente: para recursos que emplean el protocolo de autorización que requiere un certificado del lado del cliente.
* Realice una solicitud de autorización de clave de API: para recursos que utilizan claves de API para la autorización.

## Módulos de solicitud

Consulte los siguientes artículos para obtener instrucciones específicas sobre el módulo de solicitudes:

* [[!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud] módulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud de autorización básica] módulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud de OAuth 2.0] módulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud de autorización de certificado de cliente] módulo](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud de autorización de clave de API]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## Otros módulos de acción

* [[!UICONTROL Obtener un archivo]](#get-a-file)
* [[!UICONTROL Resolución de una dirección URL de destino]](#resolve-a-target-url)

### [!UICONTROL Obtener un archivo]

Este módulo de acción descarga un archivo desde la dirección URL especificada. Una vez descargado el archivo, puede seguir procesándolo (asigne los datos del archivo) utilizando otros módulos en el escenario.

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

### [!UICONTROL Resolución de una dirección URL de destino]

Este módulo de acción resuelve una cadena de redirecciones HTTP y devuelve una dirección URL de destino.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Introduzca o asigne la dirección URL que desea resolver, como un [!DNL bit.ly] URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método] </td> 
   <td> <p>Seleccione si desea utilizar el método [!UICONTROL HEAD] o el método [!UICONTROL GET].</p> </td> 
  </tr> 
 </tbody> 
</table>

## Módulos de iteración

### [!UICONTROL Recuperar encabezados]

Este módulo devuelve cada encabezado (nombre y valor) del módulo HTTP especificado en un paquete independiente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Seleccione el módulo desde el que desea recuperar los encabezados.</p> </td> 
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
