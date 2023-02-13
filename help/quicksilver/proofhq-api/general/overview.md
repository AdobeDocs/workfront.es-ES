---
title: Información general
description: Información general
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 1%

---

# Información general

**Bienvenido a la API de prueba de Workfront**

La API de prueba de Workfront es un servicio HTTP sencillo que se asegura mediante SSL. La API pretende proporcionarle toda la funcionalidad que utilizó en nuestra propia aplicación.

## Formatos compatibles

La interfaz pública es compatible con SOAP 1.1 y con WSDL. Por lo tanto, todas las solicitudes se ejecutan utilizando XML sobre HTTPS.

## Versiones de API

Para preservar la compatibilidad con las integraciones de cliente existentes, hemos introducido el control de versiones de API a partir de nuestra versión 12.1. Consulte la  [Actualizaciones de API](http://api.proofhq.com/new-updates) para obtener más información. Si un método o parámetro no tiene información de versión, significa que lo encontrará como parte de nuestra API estándar, consulte la sección &quot;Introducción a la API&quot; más abajo.

## Introducción a la API

El punto de entrada de la API:

`https://soap.proofhq.com/soap` (tenga en cuenta el uso de HTTPS)

El WSDL se puede encontrar aquí:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**Este WSDL contiene todos los cambios hasta la versión 12.1, tras lo cual hemos introducido el control de versiones de API. Consulte la página de actualizaciones de API para obtener más información sobre las distintas versiones de WSDL y los próximos cambios**

Cada solicitud de API requiere una clave de sesión. Esta clave de sesión identifica al usuario de Workfront Proof que realiza la acción o acciones y se obtiene llamando al método doLogin() y pasando la dirección de correo electrónico y contraseña del usuario. El método doLogin() solo necesita llamarse una vez antes de una secuencia de solicitudes de API. La clave de sesión permanece activa durante un breve periodo de tiempo y se renueva en cada llamada al método. *Muy pronto, añadiremos compatibilidad con la autenticación basada en token.*

Todas las solicitudes utilizan el siguiente formato de sobre, encabezado y cuerpo:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
	   ... API function and data inserted here ...
	</soapenv:Body>
	</soapenv:Envelope>
```

## Preguntas frecuentes

Si desea consultar una colección de preguntas frecuentes, visite [this](http://api.proofhq.com/faqs) página.
