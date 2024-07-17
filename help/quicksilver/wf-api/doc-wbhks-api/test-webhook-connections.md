---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Prueba de conexiones de webhook
description: Prueba de conexiones de webhook
author: Becky
feature: Workfront API
role: Developer
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---


# Prueba de conexiones de webhook

Para comprobar que la implementación del webhook de documentos funciona correctamente, ejecute las pruebas manuales en esta sección. Estos pasos pasan por la interfaz web de Adobe Workfront e indirectamente llegan a los extremos de la implementación del webhook.

## Requisitos previos

Se requieren los siguientes requisitos previos para ejecutar las pruebas:

* Una cuenta de Workfront con la administración avanzada de documentos (ADM) habilitada

* Un usuario de Workfront para esta cuenta con derechos de administrador del sistema

* Una instancia de Document Webhook con extremos HTTP accesibles para Workfront

Estas pruebas también suponen que la instancia de Document Webhook está registrada. (Puede registrar la instancia en Workfront en Configuración > Documentos > Integraciones personalizadas).

**Prueba 1: aprovisionar el servicio de webhook de documentos para un usuario**

Prueba la URL de autenticación y la URL de extremo de token para proveedores de webhook basados en OAuth.

1. En Workfront, vaya a la página principal de Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Haga clic en el menú desplegable Agregar documentos y seleccione el servicio de webhook de documentos en Agregar servicio.
1. (Solo servicios de OAuth) Después de completar el paso anterior, verá cómo se carga la página de autenticación OAuth2 del servicio en una ventana emergente. (Nota: es posible que se le pida que inicie sesión en el servicio primero.) En la página de autenticación, conceda acceso a Workfront a la cuenta del usuario haciendo clic en el botón Confiar o Permitir.
1. Compruebe que el servicio se haya agregado a la lista desplegable Agregar documentos. Si no lo ve al principio, intente actualizar el explorador.

**Prueba 2: vincular un documento a Workfront Prueba los siguientes extremos: /files, /metadata**

1. En Workfront, vaya a la página principal de Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Seleccione el servicio webhook de documentos en Agregar documentos.
1. En el modal, navegue por la estructura de carpetas.
1. Compruebe que puede desplazarse por la estructura de carpetas.
1. Seleccionar y vincular un documento a Workfront

**Prueba 3: desplácese a un documento en el sistema de administración de contenido**

Prueba los siguientes extremos: /metadata (específicamente viewLink)

1. Vinculación de documentos a Workfront
1. Seleccione el documento y haga clic en el vínculo Open.
1. Compruebe que el documento se abre en una nueva ficha.

**Prueba 4: Vaya a un documento en el sistema de administración de contenido (con inicio de sesión)**

Prueba los siguientes extremos: /metadata (específicamente viewLink)

1. Asegúrese de haber cerrado la sesión del sistema de administración de contenido.
1. Vincule un documento a Workfront.
1. Seleccione el documento y haga clic en el vínculo Open.
1. Compruebe que la pantalla de inicio de sesión del sistema de administración de contenido se carga en una nueva pestaña.
1. Inicie sesión y compruebe que ha accedido al documento

**Prueba 5: descargar el documento desde el sistema de administración de contenido**

Prueba los siguientes extremos (específicamente el vínculo de descarga): /metadata 

1. Vincule un documento a Workfront.
1. Seleccione el documento y haga clic en el vínculo Descargar.
1. Compruebe que comienza la descarga.

**Prueba 6: buscar contenido**

Prueba los siguientes extremos: /search

1. En Workfront, vaya a la página principal de Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Seleccione el servicio webhook de documentos en Agregar documentos.
1. En el modal, realice una búsqueda.
1. Compruebe que los resultados de la búsqueda son correctos.

**Prueba 7: enviar documento de Workfront al sistema de administración de contenido**

Prueba los siguientes extremos: /files, /uploadInit, /upload

1. En Workfront, vaya a la página principal de Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Cargar un documento a Workfront desde el equipo
1. Ir a la página de detalles del documento
1. En el menú desplegable Acciones de documento, seleccione el servicio Webhook de documentos en Enviar a...
1. Vaya a la carpeta de destino deseada y haga clic en el botón Save.
1. Compruebe que el documento se ha cargado en la ubicación correcta del sistema de administración de contenido.

**Prueba 8: Ver miniaturas en Workfront**

Prueba los siguientes extremos: /thumbnail

1. Vincule un documento a Workfront.
1. Seleccione el documento en la lista.
1. Compruebe que la miniatura aparece en el panel derecho.

**Prueba 9: Obtener los bytes de contenido**

Prueba los siguientes extremos: /download

1. Vincule un documento a Workfront.
1. Vaya a la página de detalles del documento.
1. Envíe el documento a Workfront seleccionando Acciones de documento > Enviar a... > Workfront. Se creará una nueva versión del documento en Workfront.
1. Descargue el documento desde Workfront haciendo clic en el vínculo Descargar.

**Prueba 10: Actualizar token de acceso (solo proveedores de webhook de OAuth2)**

Prueba los siguientes extremos: URL de extremo de token

1. Aprovisionamiento del servicio Document Webhook para un usuario
1. Invalide el token de acceso del usuario (1 ) esperando a que se agote el tiempo de espera o (2) invalidándolo manualmente en el sistema externo.
1. Actualice el token de acceso en Workfront. Para ello, por ejemplo, puede vincular un documento a Workfront. Sabrá que el token de acceso se actualizó correctamente si pudo desplazarse a un documento y vincularlo.

>[!NOTE]
>
>Actualmente, Enviar a... no está disponible para documentos vinculados. Esto se agregará mediante Workfront. Puede probar el extremo /download presionando el extremo manualmente con un cliente REST, como Postman. Como alternativa, el punto final /download se puede probar generando una prueba digital. Para habilitar la revisión digital, póngase en contacto con Workfront.
