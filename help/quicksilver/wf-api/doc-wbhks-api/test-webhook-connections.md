---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Comprobar conexiones de webhook
description: Comprobar conexiones de webhook
author: Becky
feature: Workfront API
role: Developer
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
TQID: https://experienceleague.adobe.com/08obyXZ-MxoG1JqSrG-skblpHIudRUTeCcZ3vsUocBs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 809
ht-degree: 96%

---

# Comprobar conexiones de webhook

Para comprobar que la implementación del webhook del documento funcione correctamente, ejecute las pruebas manuales en esta sección. Estos pasos van a través de la interfaz web de Adobe Workfront e indirectamente llegan a los puntos finales de la implementación del webhook.

## Requisitos previos

Se requieren los siguientes requisitos previos para ejecutar las pruebas:

* Una cuenta de Workfront con la administración avanzada de documentos (ADM) habilitada

* Un usuario de Workfront para esta cuenta con derechos de administrador del sistema

* Una instancia de Document Webhook con puntos finales HTTP accesibles para Workfront

Estas pruebas también presuponen que la instancia del webhook de documentos está registrada. (Puede registrar la instancia en Workfront en Configuración > Documentos > Integraciones personalizadas).

**Prueba 1: aprovisionar el servicio de webhook de documentos para un usuario**

Comprueba la URL de autenticación y la URL del punto final del token para proveedores de webhook basados en OAuth.

1. En Workfront, vaya a la página principal de Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Haga clic en el menú desplegable Añadir documentos y seleccione el servicio de webhook de documentos en Añadir servicio.
1. (Solo servicios de OAuth) Después de completar el paso anterior, verá cómo se carga la página de autenticación OAuth2 del servicio en una ventana emergente. (Nota: es posible que se le pida que inicie sesión en el servicio primero.) En la página de autenticación, conceda acceso a Workfront a la cuenta del usuario haciendo clic en el botón Confiar o Permitir.
1. Compruebe que el servicio se haya añadido a la lista desplegable Añadir documentos. Si no lo ve al principio, intente actualizar el explorador.

**Prueba 2: vincular un documento a Workfront comprueba los siguientes puntos finales: /files, /metadata**

1. En Workfront, vaya a la página principal de Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Seleccione el servicio de webhook de documentos en Añadir documentos.
1. En el modal, navegue por la estructura de carpetas.
1. Compruebe que pueda desplazarse por la estructura de carpetas.
1. Seleccionar y vincular un documento a Workfront

**Prueba 3: desplazarse hasta un documento en el sistema de administración de contenido**

Comprueba los siguientes puntos finales: /metadata (específicamente viewLink)

1. Vincular un documento a Workfront
1. Seleccione el documento y haga clic en el vínculo Abrir.
1. Compruebe que el documento se abra en una nueva pestaña.

**Prueba 4: vaya a un documento en el sistema de administración de contenido (con inicio de sesión)**

Comprueba los siguientes puntos finales: /metadata (específicamente viewLink)

1. Asegúrese de haber cerrado la sesión del sistema de administración de contenido.
1. Vincule un documento a Workfront.
1. Seleccione el documento y haga clic en el vínculo Abrir.
1. Compruebe que la pantalla de inicio de sesión del sistema de administración de contenido se cargue en una nueva pestaña.
1. Inicie sesión y compruebe que haya accedido al documento

**Prueba 5: descargar el documento desde el sistema de administración de contenido**

Comprueba los siguientes puntos finales (específicamente el vínculo de descarga): /metadatos 

1. Vincule un documento a Workfront.
1. Seleccione el documento y haga clic en el vínculo Descargar.
1. Compruebe que se inicie la descarga.

**Prueba 6: buscar contenido**

Comprueba los siguientes puntos finales: /search

1. En Workfront, vaya a la página principal de Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Seleccione el servicio de webhook de documentos en Añadir documentos.
1. En el modal, realice una búsqueda.
1. Compruebe que los resultados de la búsqueda sean correctos.

**Prueba 7: enviar documento de Workfront al sistema de administración de contenido**

Comprueba los siguientes puntos finales: /files, /uploadInit, /upload

1. En Workfront, vaya a la página principal de Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Cargar un documento a Workfront desde el equipo
1. Vaya a la página de detalles del documento
1. En el menú desplegable Acciones del documento, seleccione el servicio de webhook de documentos en Enviar a…
1. Vaya a la carpeta de destino deseada y haga clic en el botón Guardar.
1. Compruebe que el documento se haya cargado en la ubicación correcta del sistema de administración de contenido.

**Prueba 8: ver miniaturas en Workfront**

Comprueba los siguientes puntos finales: /thumbnail

1. Vincule un documento a Workfront.
1. Seleccione el documento en la lista.
1. Compruebe que la miniatura aparezca en el panel derecho.

**Prueba 9: obtener los bytes de contenido**

Comprueba los siguientes puntos finales: /download

1. Vincule un documento a Workfront.
1. Vaya a la página de detalles del documento.
1. Envíe el documento a Workfront seleccionando Acciones del documento > Enviar a… > Workfront. Se crea una nueva versión del documento en Workfront.
1. Descargue el documento desde Workfront haciendo clic en el vínculo Descargar.

**Prueba 10: actualizar el token de acceso (solo proveedores de webhook de OAuth2)**

Comprueba los siguientes puntos finales: URL de punto final del token

1. Aprovisionamiento del servicio de webhook de documentos para un usuario
1. Invalide el token de acceso del usuario 1) esperando a que se agote el tiempo de espera o 2) invalidándolo manualmente en el sistema externo.
1. Actualice el token de acceso en Workfront. Para ello, por ejemplo, puede vincular un documento a Workfront. Sabrá que el token de acceso se actualizó correctamente si pudo desplazarse a un documento y vincularlo.

>[!NOTE]
>
>Actualmente, la opción Enviar a… no está disponible para documentos vinculados. Esta se añadirá mediante Workfront. Puede comprobar el punto final /descarga presionando el punto final manualmente con un cliente REST, como Postman. Como alternativa, el punto final /download se puede probar generando una revisión digital. Para habilitar la revisión digital, póngase en contacto con Workfront.
