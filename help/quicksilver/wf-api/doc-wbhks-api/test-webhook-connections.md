---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Probar conexiones de Weblock
description: Probar conexiones de Weblock
author: Becky
feature: Workfront API
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---


# Probar conexiones de Weblock

Para verificar que la implementación del weblock del documento funciona correctamente, ejecute las pruebas manuales en esta sección. Estos pasos pasan por la interfaz web de Adobe Workfront y llegan indirectamente a los puntos finales de su implementación de weblink.

## Requisitos previos

Se requieren los siguientes requisitos previos para ejecutar las pruebas:

* Una cuenta de Workfront con la administración avanzada de documentos (ADM) habilitada

* Un usuario de Workfront para esta cuenta con derechos de administrador del sistema

* Una instancia de Document Weblock con extremos HTTP a los que se puede acceder desde Workfront

Estas pruebas también suponen que la instancia de Document Weblock está registrada. (Puede registrar la instancia en Workfront en Configuración > Documentos > Integraciones personalizadas).

**Prueba 1: Aprovisionar el servicio Document Weblock para un usuario**

Prueba la URL de autenticación y la URL del extremo del token para los proveedores de Weblock basados en OAuth.

1. En Workfront, vaya a la página principal Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Haga clic en la lista desplegable Add Documents y seleccione el servicio Document Weblock en Add Service.
1. (Solo servicios de OAuth) Después de completar el paso anterior, verá la carga de la página de autenticación OAuth2 de su servicio en una ventana emergente. (Nota: es posible que se le pida que inicie sesión en su servicio primero). En la página de autenticación, conceda a Workfront acceso a la cuenta del usuario haciendo clic en el botón Confiar o Permitir .
1. Verifique que su servicio se haya agregado a la lista desplegable Agregar documentos . Si no lo ve inicialmente, intente actualizar el explorador.

**Prueba 2: Vincular un documento a pruebas de Workfront con los siguientes extremos: /archivos, /metadatos**

1. En Workfront, vaya a la página principal Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Seleccione el servicio Document Weblock en Añadir documentos.
1. Desde el modal, navegue por la estructura de carpetas.
1. Compruebe que puede desplazarse por la estructura de carpetas.
1. Seleccionar y vincular un documento a Workfront

**Prueba 3: Vaya a un documento del sistema de gestión de contenido**

Prueba los puntos finales siguientes: /metadata (específicamente el viewLink)

1. Vinculación de un documento a Workfront
1. Seleccione el documento y haga clic en el vínculo Open .
1. Compruebe que el documento se abre en una nueva ficha.

**Prueba 4: Vaya a un documento del sistema de administración de contenido (con inicio de sesión)**

Prueba los puntos finales siguientes: /metadata (específicamente el viewLink)

1. Asegúrese de haber cerrado la sesión del sistema de administración de contenido.
1. Vincular un documento a Workfront.
1. Seleccione el documento y haga clic en el vínculo Open .
1. Compruebe que la pantalla de inicio de sesión del sistema de administración de contenido se carga en una pestaña nueva.
1. Inicie sesión y verifique que ha accedido al documento.

**Prueba 5: Descargue el documento desde el sistema de administración de contenido**

Prueba los siguientes puntos finales (específicamente el vínculo de descarga): /metadata 

1. Vincular un documento a Workfront.
1. Seleccione el documento y haga clic en el vínculo Descargar .
1. Compruebe que la descarga comience.

**Prueba 6: Buscar contenido**

Prueba los puntos finales siguientes: /search

1. En Workfront, vaya a la página principal Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Seleccione el servicio Document Weblock en Añadir documentos.
1. Desde el modal, realice una búsqueda.
1. Compruebe que los resultados de la búsqueda sean correctos.

**Prueba 7: Enviar documento desde Workfront al sistema de administración de contenido**

Prueba los puntos finales siguientes: /files, /uploadInit, /upload

1. En Workfront, vaya a la página principal Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Cargar un documento a Workfront desde el equipo
1. Vaya a la página de detalles del documento
1. En el menú desplegable Acciones de documento , seleccione el servicio de Weblock de documento en Enviar a...
1. Vaya a la carpeta de destino deseada y haga clic en el botón Save .
1. Compruebe que el documento se haya cargado en la ubicación correcta del sistema de administración de contenido.

**Prueba 8: Ver miniaturas en Workfront**

Prueba los puntos finales siguientes: /thumbnail

1. Vincular un documento a Workfront.
1. Seleccione el documento en la lista.
1. Compruebe que la miniatura aparece en el panel derecho.

**Prueba 9: Obtención de los bytes de contenido**

Prueba los puntos finales siguientes: /download

1. Vincular un documento a Workfront.
1. Vaya a la página de detalles del documento.
1. Envíe el documento a Workfront seleccionando Acciones de documento > Enviar a... > Workfront. Esto creará una nueva versión del documento en Workfront.
1. Descargue el documento desde Workfront haciendo clic en el vínculo Descargar .

**Prueba 10: Actualizar token de acceso (solo proveedores de Weblock de OAuth2)**

Prueba los puntos finales siguientes: URL del extremo del token

1. Aprovisionar un servicio de Document Weblock para un usuario
1. Invalide el token de acceso del usuario en 1 ) esperando que se agote el tiempo de espera o 2) invalidándolo manualmente en el sistema externo.
1. Actualice el token de acceso en Workfront. Puede hacerlo, por ejemplo, vinculando un documento a Workfront. Sabdrá que el token de acceso se actualizó correctamente si pudo navegar a un documento y vincularlo.

>[!NOTE]
>
>Actualmente, Send To... no está disponible para documentos vinculados. Workfront lo agregará. Puede probar el extremo /download pulsando el extremo manualmente usando un cliente REST, como Postman. Alternativamente, el extremo /download se puede probar generando una prueba digital. Para habilitarlo, póngase en contacto con Workfront.
