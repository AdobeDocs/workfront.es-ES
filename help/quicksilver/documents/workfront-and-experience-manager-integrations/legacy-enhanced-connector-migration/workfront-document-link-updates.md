---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migración de carpetas y documentos vinculados
description: Puede utilizar la API para migrar carpetas y documentos vinculados a Adobe Experience Manager Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: aad8f4648a57c93047a1a691d5e608c327d78c1b
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Migración de carpetas y documentos vinculados

Puede utilizar la API para migrar carpetas y documentos vinculados a Adobe Experience Manager Assets.

## Procedimiento

1. Identifique todos los documentos y carpetas vinculados con el proveedor de almacenamiento de documentos externo anterior, teniendo en cuenta sus identificadores de carpeta o documento interno de Workfront, así como el ID de carpeta de cualquier carpeta contenedora.

   >[!NOTE]
   >
   > Debe comprobar todas las carpetas o documentos detectados para comprobar que aún no han creado un vínculo para ellos con el nuevo proveedor.

1. Busque los documentos y carpetas en el nuevo repositorio por ruta y, a continuación, busque su identidad en el sistema externo.

1. Cree una asignación del Workfront ID interno al ID en el nuevo almacén externo. Esto es necesario para crear un vínculo nuevo en el siguiente paso.

1. Cree un nuevo documento o vínculo de carpeta de documentos en Workfront que señale al recurso en su nueva ubicación mediante su nuevo ID externo.

   1. **Documentos**: agregue una nueva versión del documento existente con el nuevo proveedor de documentos externo.
   1. **Carpetas**: cree una carpeta nueva en el mismo lugar con el mismo nombre.

>[!CAUTION]
>
>   No elimine las carpetas vinculadas existentes. Esto podría causar la pérdida de datos. Para quitar vínculos de carpetas antiguas de la aplicación de Workfront, deshabilite la integración de documentos personalizada en el área de Configuración.


## Proceso de ejemplo para migrar vínculos

![flujo de vínculo simplificado](assets/links-flow-simplified.png)

## Información de API

Para obtener más información sobre las API de Workfront en esta sección, consulte [Documentación para desarrolladores:Documentos](https://developer.workfront.com/documents.html).

### Buscar todos los documentos

Buscar todos los **documentos (DOCU)** vinculados a **proveedor de documentos** de **providerType** con **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[Referencia de DOCUMENTOS DE API](https://developer.workfront.com/documents.html#get-/docu/search)

### Buscar todas las carpetas

Buscar todas las **carpetas de documentos (DOCFDR)** vinculadas al proveedor de documentos de **providerType** con **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

DOCUMENTOS DE API: (Puntos finales de carpeta de documentos no cubiertos actualmente en developer.workfront.com)

### Enlazar documentos

Vincular **documentos (DOCU)** de **proveedor de documentos externos** de **providerType** con **documentProviderID**.

>[!IMPORTANT]
>
>Los documentos se almacenan temporalmente. Esto significa que tiene acceso a todas las versiones del documento. Al crear el vínculo, puede especificar el ID del documento existente, por lo que simplemente está escribiendo una nueva versión en ese documento, con los datos alojados externamente en el nuevo proveedor. Este ID de documento es el mismo que el ID de documento encontrado en el vínculo de documento que está reemplazando. Es el mismo documento conceptual. Simplemente indica que los bytes de esta nueva versión se almacenan con un proveedor diferente.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

DOCUMENTOS DE API: (Puntos finales de vínculo interno no cubiertos actualmente en developer.workfront.com)

### Vincular carpetas

Vincular **carpetas de documentos (DOCFDR)** de **proveedor de documentos externos** de **providerType** con **documentProviderID**.

>[!IMPORTANT]
>
>Para los vínculos de carpeta, a diferencia de los vínculos de documento, necesita el &quot;documentFolderId&quot; de la carpeta en Workfront en la que desea colocar el nuevo vínculo. Es muy probable que se trate de la misma carpeta principal que la carpeta vinculada que estamos copiando.

>[!CAUTION]
>
>Las carpetas no se almacenan temporalmente. No elimine las carpetas antiguas. Deshabilite la integración de documentos personalizada en el área de configuración para quitar carpetas antiguas.


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

DOCUMENTOS DE API: (Puntos finales de vínculo interno no cubiertos actualmente en developer.workfront.com)

## Términos importantes

* **Documento**: Un recurso digital en Workfront

* **Carpeta de documentos**: Un contenedor para recursos digitales en Workfront

* **ID de documento**: ID interno de Workfront para un recurso digital

* **ID de carpeta de documentos**: ID interno de Workfront para una carpeta de recursos digitales

* **ID de proveedor de documentos**: ID asociado con proveedores de documentos específicos

>[!IMPORTANT]
>
> Para cualquier tipo de proveedor de documentos determinado, un cliente puede tener varias instancias conectadas. AEM Por ejemplo, pueden tener varios repositorios de datos enlazados, por ejemplo. O varias instancias de Google Drive vinculadas. El ID del proveedor de documentos indica la instancia específica del tipo de conexión que se desea reemplazar o cambiar.

* **Tipo de proveedor de almacenamiento de documentos (también &quot;Tipo de integración externa&quot;)**: Tipo de integración de proveedor de almacenamiento de documentos que admite Workfront. Mediante una integración dedicada o una &quot;integración personalizada&quot;.

* **Tipos de proveedor de almacenamiento de documentos actuales ( providerType)**:

  ```
  ATTASK
  BOX
  GOOGLE
  SHAREPOINT
  WEBDAM
  WORKFRONTDAM
  INFERNO
  WIDEN
  DROPBOX
  DROPBOX_BUSINESS
  ONEDRIVE
  QUIP
  WEBHOOKS
  AEM
  MOCK
  ```

* **Documento vinculado**: Un recurso digital alojado en un proveedor de almacenamiento de documentos externo. Workfront tendrá su propio &quot;ID de documento&quot; interno para el recurso, pero los bytes se almacenan externamente. Para facilitarlo, Workfront también almacena un &quot;ID de documento externo&quot; para ayudar a localizar el recurso al que se hace referencia externamente en el repositorio o almacén remoto.

* **Carpeta de documentos vinculados**: Un contenedor para recursos digitales hospedados en un proveedor de almacenamiento de documentos externo. Workfront tendrá su propio &quot;ID de carpeta de documentos&quot; interno para el recurso, pero los bytes se almacenan externamente. Para facilitarlo, Workfront también almacena un &quot;ID de documento externo&quot; para ayudar a localizar el recurso al que se hace referencia externamente en el repositorio o almacén remoto.

* **ID de documento externo**: ID asignado cuando los recursos se almacenan fuera de Workfront. Workfront asigna su identificador interno al identificador utilizado para localizar el recurso en el sistema externo, a través de este campo &quot;identificador de documento externo&quot;. Por lo tanto, al vincular el documento o la carpeta desde un nuevo almacén externo, se debe crear un nuevo identificador de documento externo, en el formato adecuado para que el proveedor de documentos externos identifique el documento en el nuevo repositorio o almacén.

  >[!NOTE]
  >
  > Workfront todavía no tiene un estándar para identificadores de documentos externos. AEM Se está utilizando una nueva especificación para ID de, pero para otros ID, el ID del documento externo puede adoptar diferentes formas según el tipo de proveedor.


* **Tipo de objeto**: se trata de un término de API únicamente para los fines de este documento. Es un tipo de objeto genérico dentro de Workfront con el que desea interactuar. En estos casos, interactuará con documentos y carpetas que tengan los tipos &quot;DOCU&quot; y &quot;DOCFDR&quot; respectivamente.

* **Id. de objeto**: El identificador Workfront interno del objeto genérico con el que desea interactuar. Interactuará con documentos y carpetas, por lo que será el ID del documento o el ID de la carpeta del documento respectivamente.
