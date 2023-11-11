---
content-type: api
navigation-topic: api-navigation-topic
title: Certificados de suscripción de eventos
description: Certificados de suscripción de eventos
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 1%

---

# Configurar TLS de cliente para suscripción a evento

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

TLS de cliente le permite comprobar que el mensaje de suscripción de evento que recibe realmente proviene de Adobe Workfront. Para habilitar esta funcionalidad, el servidor debe estar configurado para solicitar y validar el certificado x509 de Workfront.


## Verificar el certificado de cliente de Workfront

Este procedimiento supone que el servidor está configurado para aceptar conexiones TLS. Workfront no admite certificados autofirmados.

En general, estos son los pasos necesarios para activar la autenticación de cliente en el servidor:

1. Descargue la versión PEM del certificado de CA raíz global de DigiCert.
1. Active la verificación de certificados de cliente.

   Especifique el certificado de CA del paso 1 como de confianza.

1. Establezca la profundidad de verificación en 2, ya que nuestro certificado está firmado por la CA del servidor seguro SHA2 de DigiCert, que es una CA intermedia bajo la CA raíz global de DigiCert.
1. Compruebe que el certificado de cliente proviene realmente de Workfront inspeccionando su nombre de dominio del sujeto.

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

Para obtener más información, consulte la [Documentación de NGiNX para ngx_http_ssl_module](https://nginx.org/en/docs/http/ngx_http_ssl_module.html).

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

| Entorno WF | Nombre común de certificado | Asunto del certificado (DN) |
| -- | -- | -- |
| Producción | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com |
| Vista previa | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com |
| Espacio aislado 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| Espacio aislado 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## Descargar certificados

Haga clic en los siguientes vínculos para descargar los certificados de cliente.

* [Certificado de cliente: entorno de producción](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_production.crt)
* [Certificado de cliente: entorno de vista previa](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_preview.crt)
* [Certificado de cliente: entorno de espacio aislado](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_sandboxes.crt)

>[!NOTE]
>
>Puede utilizar el mismo certificado de cliente para ambos entornos de espacio aislado.
