---
content-type: api
navigation-topic: api-navigation-topic
title: Certificados de suscripción de eventos
description: Certificados de suscripción de eventos
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: 2c5a4ff65088652b67099d187e6ee4c11d80a3b3
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 88%

---

# Configuración de TLS de cliente para suscripción a eventos

<!--Configuring Client TLS for Event Subscription
Steps to Verify Workfront's Client Certificate
Examples for Server configuration
NGINX
Apache
Certificate to Environment Mapping
Certificates
Production
Preview
Sandbox 1
Sandbox 2
-->

La TLS de cliente permite comprobar que el mensaje de suscripción a un evento que recibe proviene, en efecto, de Adobe Workfront. Para habilitar esta funcionalidad, el servidor debe estar configurado para solicitar y validar el certificado x509 de Workfront.


>[!NOTE]
>
>Las suscripciones de eventos utilizan TLS versión 1.3 si el servidor al que la suscripción de eventos envía eventos es compatible con la versión 1.3. Si el servidor de conexión no es compatible con la versión 1.3, la suscripción de evento utiliza la versión 1.2 de TLS.



## Verificación del certificado de cliente de Workfront

Este procedimiento supone que el servidor está configurado para aceptar conexiones TLS. Workfront no admite certificados autofirmados.

En general, estos son los pasos necesarios para activar la autenticación de cliente en el servidor:

1. Descargue la versión PEM del certificado de CA raíz global de DigiCert.
1. Active la verificación de certificados de cliente.

   Especifique el certificado de CA del paso 1 como de confianza.

1. Establezca la profundidad de verificación en 2, ya que nuestro certificado está firmado por la CA de servidor seguro SHA2 de DigiCert, que es una CA intermedia bajo la CA raíz global de DigiCert.
1. Compruebe que el certificado de cliente proviene, en efecto, de Workfront inspeccionando su nombre de dominio del asunto.

## Ejemplos de configuración del servidor

### NGINX

```
server {

    listen 443 ssl default_server;
    # ... existing SSL configuration for server authentication ...

    ssl_verify_client on;
    ssl_client_certificate /path/to/DigiCert_Global_Root_CA.pem;
    ssl_verify_depth 2;

        # ... existing location configuration ...
    }
}
```

Para obtener más información, consulte la [documentación de NGiNX para ngx_http_ssl_module](https://nginx.org/en/docs/http/ngx_http_ssl_module.html).

### Apache

```
Listen 443
<VirtualHost *:443>
    # ... existing SSL configuration for server authentication ...

    SSLVerifyClient require
    SSLCACertificateFile "/path/to/DigiCert_Global_Root_CA.pem"
    SSLVerifyDepth 2
</VirtualHost>

<Directory /var/www/>
    Require expr "%{SSL_CLIENT_S_DN_CN} == <>"

    # ... existing directory configuration ...
</Directory>
```

Para obtener más información, consulte

* [Autenticación de cliente y control de acceso](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Módulo Apache mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## Asignación de certificado a entorno

| Entorno WF | Nombre común del certificado | Asunto del certificado (DN) |
| -- | -- | -- |
| Producción | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com |
| Vista previa | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com |
| Zona protegida 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| Zona protegida 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## Descarga de certificados

Haga clic en los siguientes vínculos para descargar los certificados de cliente.

* [Certificado de cliente: entorno de producción](assets/prod-environment-nov-2024.crt)
* [Certificado de cliente: entorno de vista previa](assets/preview-environment-nov-2024.crt)
* [Certificado de cliente: entorno de zona protegida](assets/sandbox-environment-nov-2024.crt)

>[!NOTE]
>
>Puede utilizar el mismo certificado de cliente para ambos entornos de zona protegida.
