---
title: Información general
description: Información general
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 1%

---

# Información general

**Bienvenido a la API de Workfront Proof**

La API de Workfront Proof es un servicio HTTP sencillo que se protege mediante SSL. El objetivo de la API es proporcionarle toda la funcionalidad que se utiliza en su propia aplicación.

## Formatos compatibles

La interfaz pública es compatible con SOAP 1.1 y con WSDL. Por lo tanto, todas las solicitudes se ejecutan mediante XML a través de HTTPS.

## Versiones de API

A fin de preservar la compatibilidad con las integraciones de cliente existentes, hemos introducido el control de versiones de API desde nuestra versión 12.1. Consulte la  [Actualizaciones de API](https://api.proofhq.com/new-updates.html) para obtener más información. Si un método o parámetro no tiene información de versión, significa que lo encontrará como parte de nuestra API estándar, consulte la sección &quot;Introducción a la API&quot; a continuación.

## Introducción a la API

El punto de entrada de API:

`https://soap.proofhq.com/soap` (tenga en cuenta el uso de HTTPS)

El WSDL se puede encontrar aquí:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**Este WSDL contiene todos los cambios hasta la versión 12.1, después de lo cual hemos introducido el control de versiones de la API. Consulte la página Actualizaciones de API para obtener más información sobre las distintas versiones de WSDL y los cambios futuros**

Cada solicitud de API requiere una clave de sesión. Esta clave de sesión identifica al usuario de Workfront Proof que realiza las acciones y se obtiene llamando al método doLogin() y pasando la dirección de correo electrónico y la contraseña del usuario. El método doLogin() solo debe llamarse una vez antes de una secuencia de solicitudes de API. La clave de sesión permanece activa durante un corto periodo de tiempo y se renueva en cada llamada al método. *Muy pronto añadiremos la compatibilidad con la autenticación basada en token.*

Todas las solicitudes utilizan el siguiente formato de sobre, encabezado y cuerpo:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

