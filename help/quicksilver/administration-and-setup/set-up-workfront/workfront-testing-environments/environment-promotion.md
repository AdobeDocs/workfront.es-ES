---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Mover objetos de un entorno a otro
description: La función Promoción de entornos está diseñada para proporcionar la capacidad de mover objetos relacionados con la configuración de un entorno a otro. No admite la capacidad de mover objetos transaccionales (con excepciones limitadas).
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: d249751b78e9d40fe7a351db14cbf0f3b7c79889
workflow-type: tm+mt
source-wordcount: '2105'
ht-degree: 2%

---

# Mover objetos entre [!DNL Workfront] entornos que utilizan la variable [!DNL Workfront] API de promoción de entorno

La capacidad Promoción de entornos permite mover objetos relacionados con la configuración de un entorno a otro. Puede mover estos objetos mediante la API de Workfront como se describe en este artículo.

Para obtener instrucciones sobre cómo mover objetos entre entornos mediante la aplicación de Workfront, consulte:

* [Crear o editar un paquete de promoción de entorno](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [Instalación de un paquete de promoción de entorno](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)


## Requisitos de acceso

Debe tener lo siguiente:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> Su organización debe seguir el nuevo modelo de precios y tener un plan Prime o Ultimate.
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licencias</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Configuraciones de nivel de acceso
   </td>
   <td>Debe ser un [!DNL Workfront] administrador.
   </td>
  </tr>
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

El punto final Crear paquete promocional supone que ya ha configurado el entorno de origen. Esta llamada de API requiere la creación manual de un mapa de objetos de [!DNL Workfront] objCodes y GUID de objetos. A continuación se describe la estructura específica de este mapa.

## Objetos compatibles para la promoción del entorno

La función Promoción de entornos está diseñada para proporcionar la capacidad de mover objetos relacionados con la configuración de un entorno a otro. No admite la capacidad de mover objetos transaccionales (con excepciones limitadas).

Para ver una lista de objetos promocionales y sus subobjetos promocionales incluidos, consulte [Objetos compatibles para la promoción del entorno](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) en el artículo [Información general sobre el movimiento de objetos entre entornos de Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).

## Autenticación

La API autentica cada solicitud para garantizar que el cliente tenga acceso para ver o modificar un objeto solicitado.

La autenticación se realiza pasando un ID de sesión o una clave de API, que se pueden proporcionar mediante el siguiente método:

### Autenticación de encabezado de solicitud

El método de autenticación preferido es pasar un encabezado de solicitud denominado SessionID que contenga el token de sesión. Esto tiene la ventaja de estar seguro contra [Falsificación de solicitud en sitios múltiples (CSRF)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) ataques y no interferir con el URI con fines de almacenamiento en caché.

A continuación se muestra un ejemplo de encabezado de solicitud:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## Extremos de API

* [Creación de un paquete](#create-a-package)
* [Obtener una lista de paquetes](#get-a-list-of-packages)
* [Obtención de un paquete por ID](#get-a-package-by-id)
* [Actualización de propiedades específicas de un paquete](#update-specific-properties-of-a-package)
* [Eliminación de un paquete](#delete-a-package)
* [Ejecutar una ejecución previa](#execute-a-pre-run)
* [Ejecutar una instalación](#execute-an-installation)
* [Obtener una lista de instalaciones para un paquete específico](#get-a-list-of-installations-for-a-specific-package)
* [Obtener los detalles de instalación de una instalación](#get-the-installation-details-for-an-installation)

### Creación de un paquete

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Esta llamada ejecuta un proceso de varios pasos.

El primer paso resulta en la creación de un paquete de promoción vacío con el estado &quot;ENSAMBLANDO&quot;.

El segundo paso utiliza el `objectCollections` matriz proporcionada en el cuerpo del POST para ensamblar los registros solicitados de Workfront. Este paso puede tardar varios minutos en completarse, según la cantidad de registros solicitados y la configuración de Workfront. Al final de este proceso, el paquete de promoción vacío se actualiza con la variable `packageEntities` y el estado se establece automáticamente como &quot;BORRADOR&quot;.


>[!NOTE]
>
>Tenga en cuenta la estructura del `objectCollections`  matriz.
>
>Cada elemento de la matriz contiene un `objCode` que corresponde al código de objeto documentado en el Explorador de API de Workfront.
>
>Cada elemento también contiene un `entities` colección. Se espera el `ID` field. También puede aceptar un `name` para que sea más fácil saber qué `ID` representa.
>
>Para obtener la lista de códigos de objeto permitidos que se van a solicitar en la `objectCollections` , consulte la [Objetos compatibles para la promoción del entorno](#supported-objects-for-environment-promotion) de este artículo.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Encabezados

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

O

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Cuerpo

```json
{
    "name": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes...",
    "source": "https://{domain}.{environment}.workfront.com",
    "objectCollections": [
        {
            "objCode": "PROJ",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597ba1",
                    "name": "Agency Request"
                }
            ]
        },
        {
            "objCode": "TMPL",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597bb2",
                    "name": "New Agency Onboarding"
                },
                {
                    "ID": "6419b8b9001151ee258921a4f7597bc3",
                    "name": "New Agency Offboarding"
                }
            ]
        },
        {
            "objCode": "PTLTAB",
            "entities": [
                {
                    "ID": "645e6435000b4aaebe4776f4a42ed5ad",
                    "name": "Agency Performance and Readiness"
                }
            ]
        }
    ]
}
```

#### Respuesta

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ASSEMBLING",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
    }
}
```

### Obtener una lista de paquetes

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Esta llamada devuelve una lista sin filtrar de paquetes promocionales que pertenecen al cliente.

La respuesta incluirá todos los paquetes creados a partir de cualquiera de las instancias de zona protegida, vista previa o producción del cliente de Workfront.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Encabezados

```json
{
    "apikey": "**********"
}
```

O

```json
{
    "sessionID": "*****************"
}
```

#### Cuerpo

_Empty_

#### Respuesta

```
200
```

```json
{
    "data": [
        {
            "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
            "name": "Agency Onboarding - 2023-06-06",
            "description": "This promotion package contains configuration to support the agency onboarding processes...",
            "status": "ASSEMBLING",
            "createdAt": "2023-06-06T17:29:21.600Z",
            "deletedAt": null
},
        {...}
    ]
}
```

&lt;!—Comprobar el &quot;estado&quot; anterior—¿se añadió?—>

### Obtención de un paquete por ID

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Esta llamada devuelve como detalles un paquete promocional solicitado.

La solicitud se puede realizar a través de cualquier entorno independientemente de la fuente original del paquete de promoción.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Encabezados

```json
{
    "apikey": "**********"
}
```

O

```json
{
    "sessionID": "*****************"
}
```

#### Cuerpo

_Empty_

#### Respuesta

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "DRAFT",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "null"
                   - or -
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Actualización de propiedades específicas de un paquete

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Esta llamada actualiza cualquiera de los contenidos del paquete promocional que se proporcionan en el cuerpo del PATCH.

Los atributos editables son:

1. nombre (cadena)
1. description (cadena)
1. estado (cadena con validación de valor)

Para ver una descripción detallada de los estados disponibles, consulte [Estados de promoción del entorno](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) en el artículo [Información general sobre el movimiento de objetos entre entornos de Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).


#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### Encabezados

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

O

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Cuerpo

```json
{
    "status": "ACTIVE"
}
```

#### Respuesta

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ACTIVE",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Eliminación de un paquete

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Esta llamada elimina el registro del paquete de promoción. Esta acción no se puede deshacer.

>[!NOTE]
>
>A diferencia de eliminar un paquete de promoción, la recomendación es cambiar el estado del paquete a DESHABILITADO. Esto permite recuperar el paquete y conservar el historial de instalación del lugar donde se implementó.

#### URL

```
DELETE https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Encabezados

```json
{
    "apikey": "**********"
}
```

O

```json
{
    "sessionID": "*****************"
}
```

#### Cuerpo

_Empty_

#### Respuesta

```
200
```

```
Deleted
```

### Ejecutar una ejecución previa

>[!IMPORTANT]
>
>Antes de ejecutar una instalación, debe ejecutar esta ejecución previa. Utilizará el ID generado a partir de esta llamada cuando ejecute la instalación.

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

Esta llamada realiza una comparación entre la definición del paquete y el entorno de destino identificado en la dirección URL.

El resultado es un cuerpo JSON que identifica si un objeto de promoción se encuentra o no en el entorno de destino.

Para cada objeto de promoción, siga uno de estos procedimientos `actions`  se configurará:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>CREAR</td> 
   <td><p>Cuando no se encuentra un registro correspondiente en el entorno de destino, la acción se establece en CREATE.</p><p>Cuando esta acción se establece en la variable <code>translationmap</code> que se proporciona al <code>/install</code> extremo, el servicio de instalación creará el registro.</p></td> 
  </tr> 
  <tr> 
   <td>USEEXISTING</td> 
   <td><p>Cuando se encuentra un registro correspondiente en el entorno de destino, la acción se establece en USEEXISTING y se crea un <code>targetId</code> también se captura en el <code>translationmap</code>.</p><p>Cuando esta acción se establece en la variable <code>translationmap</code> que se proporciona al <code>/install</code> extremo, el servicio de instalación no creará el registro. Sin embargo, utilizará el <code>targetId</code> incluido en la entrada del mapa para otros objetos que puedan tener una referencia a este registro.</p><p>Por ejemplo, se puede encontrar un "Grupo predeterminado" en el entorno de destino en el que se está implementando un paquete. No es posible tener dos registros de "Grupo predeterminado", por lo que el servicio de instalación utilizará el GUID del grupo existente en cualquier otra acción de creación de objetos que incluya una referencia al "Grupo predeterminado", como un proyecto, formulario o cualquier otra entidad relacionada con este grupo.</p><p><b>Nota:</b> <ul><li><p>Cuando se asigna la acción USEEXISTING, no se modifica el registro existente en el entorno de destino. </p><p>Por ejemplo, si la descripción del "grupo predeterminado" ha cambiado en la zona protegida desde la que se creó el paquete y el valor de la descripción es diferente en el entorno de destino, el valor permanecerá sin cambios después de una instalación con este <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>SOBRESCRITURA</td> 
   <td><p>Esta acción no se establecerá automáticamente.</p><p>Esta acción permite actualizar un objeto que existe en el entorno de destino. Proporciona la capacidad de anular manualmente una acción CREATE o USEEXISTING asignada antes de ejecutar el <code>/install</code> llamada.<ul><li>Un usuario puede actualizar un objeto en el entorno de prueba y, a continuación, utilizar la acción SOBRESCRIBIR para actualizar ese objeto en el entorno de destino.</p></li><li><p>Si el usuario instala un paquete de promoción inicialmente y, posteriormente, un paquete nuevo (o actualizado) contiene cambios en los objetos del paquete inicial, el usuario puede utilizar OVERWRITING para reemplazar (anular) los objetos instalados anteriormente. </p><p>Para obtener más información sobre la sobrescritura, consulte la sección [Sobrescritura](#overwriting) en este artículo.</li><ul></td> 
  </tr> 
  <tr> 
   <td>IGNORAR</td> 
   <td><p>Esta acción no se establecerá automáticamente.</p><p>Proporciona la capacidad de anular manualmente una acción CREATE o USEEXISTING asignada antes de ejecutar el <code>/install</code> llamada.</p><p><b>Notas: </b><ul><li><p>Si un registro que originalmente se estableció en CREATE se establece en IGNORE, cualquier registro secundario también se debe establecer en IGNORE.</p><p>Por ejemplo, si un registro de plantilla se ha asignado con una acción CREAR y el usuario que lo instala desea excluirlo de la implementación, puede establecer la acción de la plantilla en IGNORAR.</p><p>En este caso, si el usuario que realiza la instalación no establece las tareas de plantilla, las asignaciones de tareas de plantilla, las predecesoras de tareas de plantilla, la definición de cola, los temas de cola, las reglas de enrutamiento, etc. en IGNORE, la implementación resultará en un intento de instalación fallido.</p></li><li><p>Si un registro que originalmente se estableció en USEEXISTING se establece en IGNORE, puede haber algunos efectos adversos durante el proceso de instalación.</p><p>Por ejemplo, si se asignó un registro de grupo con la acción USEEXISTING y el usuario que realiza la instalación cambia la acción a IGNORE, para los objetos que requieren un grupo (por ejemplo, un proyecto no puede existir sin un grupo asignado), el grupo predeterminado del sistema se asignará a ese proyecto.</p></li><li><p>Si un registro que originalmente se estableció en USEEXISTING se establece en CREATE, puede haber algunos efectos adversos durante el proceso de instalación porque muchas entidades de Workfront tienen restricciones de nombre único.</p><p>Por ejemplo, si se asignó un registro de "Grupo predeterminado" con la acción USEEXISTING y el usuario que realiza la instalación cambia la acción a CREATE, dado que ya existe un "Grupo predeterminado", el intento de instalación no podrá completar todos los pasos. Los nombres de grupo deben ser únicos.</p><p>Algunas entidades no tienen una restricción de nombre único. Para esos objetos, realizar este cambio dará como resultado dos registros con nombres idénticos. Por ejemplo, las plantillas, los proyectos, las vistas, los filtros, las agrupaciones, los informes y los paneles no requieren restricciones de nombre único. Se recomienda tener nombres únicos para estos registros, pero no se aplica.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

Actualmente no se admite una actualización `action` en las capacidades alpha de este servicio. La opción para permitir una ACTUALIZACIÓN `action` es algo que estamos investigando.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/:id/prepare-installation
```

#### Encabezados

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

O

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Cuerpo

```json
{}
```

#### Respuesta

```
200
```

```json
{
    "environmentPromotionPackageId": "45f2ae94-76c0-4b13-8f3b-f688de83043d",
    "environmentPromotionPackageVersion": 1,
    "id": "c0bc79bd-c9c1-4b5b-b118-b1241392de0e",
    "userId": "5ba38da500b752fd66439d4f6a9999a1",
    "customerId": "5ba38d9d00b74f0c7a38b1b487fc9710",
    "status": "PREPARING",
    "environment": "mmi.my.workfront.com",
    "registeredAt": "2023-10-19T20:00:16.697Z",
    "updatedAt": "2023-10-19T20:00:16.701Z",
    "translationMap": {
        "CTGY": {
            "62d9c9a0000013aeeefe7242a0a5fdb2": {
                "name": "Example Document Form",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9a0000013aeeefe7242a0a5fdb2"
            }
        },
        "PGRP": {
            "62d1eee4001c6618e6b9f9a588ba1598": {
                "name": "Asset Detail",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee4001c6618e6b9f9a588ba1598"
            }
        },
        "GROUP": {
            "5ba38da500b752b0f46d13186030b7ad": {
                "name": "Default Group",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "5ba38da500b752b0f46d13186030b7ad"
            }
        },
        "PARAM": {
            "62d1eee400f8578895166ee91a83f97a": {
                "name": "Asset Type",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee400f8578895166ee91a83f97a"
            },
            "62d1eee50001407c713514a8970b58e4": {
                "name": "Keywords",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee50001407c713514a8970b58e4"
            },
            "62d1eee5000333ac3981ea4f3df6d88e": {
                "name": "Permitted Uses",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000333ac3981ea4f3df6d88e"
            },
            "62d1eee5000b188e9ec8039a097fc7ab": {
                "name": "File Format",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000b188e9ec8039a097fc7ab"
            },
            "62d1eee500100c159fd5f838ce560507": {
                "name": "CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee500100c159fd5f838ce560507"
            },
            "62d9c988001c1f23954dbb9d646335b5": {
                "name": "Other CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c988001c1f23954dbb9d646335b5"
            },
            "62d9c9880070f546cf4c798ea6c3eaa4": {
                "name": "Other Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9880070f546cf4c798ea6c3eaa4"
            },
            "62d9c990006258baf1b40f2569c3eab7": {
                "name": "Target Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c990006258baf1b40f2569c3eab7"
            }
        }
    }
}
```

>[!NOTE]
>
>El ID que necesitará para ejecutar la instalación es el `id` field. En este ejemplo, la variable `id` el campo es el tercero desde arriba y tiene un valor que comienza por `c0bc79bd`.

### Ejecutar una instalación

>[!IMPORTANT]
>
>Antes de ejecutar una instalación, debe ejecutar una ejecución previa. Utilizará el ID generado a partir de la ejecución previa al ejecutar la instalación.
>
>Si se han realizado cambios en el entorno de destino (el entorno en el que se está implementando el paquete) después de ejecutar la preejecución, se recomienda volver a ejecutar la preejecución. Si no vuelve a ejecutar la ejecución previa, es posible que la ejecución no se complete con precisión o que la instalación falle.
>
>Para obtener instrucciones sobre cómo ejecutar una ejecución previa, consulte [Ejecutar una ejecución previa](#execute-a-pre-run).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Esta llamada inicia un intento de instalación de un paquete promocional en el entorno de destino identificado en la dirección URL del POST.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}/install
```

#### Encabezados

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

O

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Cuerpo

```json
{
}
```

#### Respuesta

```
202
```


```json
{}
```

### Obtener una lista de instalaciones para un paquete específico

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

Los resultados incluyen eventos de instalación de todos los entornos en los que se ha implementado el paquete. No se limitan a las instalaciones para el entorno a través de las cuales se realiza la solicitud. Esto le permite identificar qué entornos han recibido este paquete.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### Encabezados

```json
{
    "apikey": "**********"
}
```

O

```json
{
    "sessionID": "*****************"
}
```

#### Cuerpo

_Empty_

#### Respuesta

```
200
```

```json
[
    {
        "id": "2892b936-e09e-455a-935f-e1462ab9753c",
        "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
        "environmentPromotionPackageVersion": 1,
        "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
        "customerId": "54286d78b064451096752b99bf968481",
        "status": "INSTALLED",
        "environment": "https://{domain}.{environment}.workfront.com",
        "registeredAt": "2021-03-16T02:21:31.908Z",
        "updatedAt": null,
        "translationMap": {
            "ROLE": {
                "5f6d114f006883209828ddd9088e63b3": {
                    "name": "DAM Curator",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f4bed00028a718599f29575840053"
                },
                "ad535a9ebe647361e053a7656a0a1575": {
                    "name": "Copywriter",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f162700001ca051081c06667b14a4"
                },
                ...
            },
            "TMPL": {
                "5f9b317c00b3db5af69abcd1ed5f82aa": {
                    "name": "Digital Asset Production (Integrated)",
                    "action": "CREATE",
                    "isValid": true,
                    "targetId": "6054cda40000d5af63dc811d9c2b3a07"
                },
                ...
            },
            ...
        }
    },
    {...}
]
```

### Obtener los detalles de instalación de una instalación

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Esta llamada devolverá el `translationMap` producido por el servicio de instalación para una instalación específica.

Cada registro indicará lo prescrito `action` era y si esa acción fue exitosa o no.

Para registros con CREATE `action` el `targetId` se establecerá con el valor del registro recién creado en el sistema de destino. Además, la variable `installationStatus` El campo se establecerá en INSTALADO.

Para registros con USEEXISTING `action` el `targetId` también se establecerá el campo, y la variable `installationStatus` se establecerá en REGISTERED. Esto significa que el proceso de asignación se ha completado y el servicio de instalación reconoce que ha evaluado el registro y que no hay nada en lo que actuar.

Si el registro tiene un elemento CREATE `action` pero no crea correctamente el registro y, a continuación, el `installationStatus` se establecerá en FAILED y también se proporcionará el motivo del error.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}
```

#### Encabezados

```json
{
    "apikey": "**********"
}
```

O

```json
{
    "sessionID": "*****************"
}
```

#### Cuerpo

_Empty_

#### Respuesta

```
200
```

```json
{
    "id": "2892b936-e09e-455a-935f-e1462ab9753c",
    "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
    "environmentPromotionPackageVersion": 1,
    "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
    "customerId": "54286d78b064451096752b99bf968481",
    "status": "INSTALLED",
    "environment": "https://{domain}.{environment}.workfront.com",
    "registeredAt": "2021-03-16T02:21:31.908Z",
    "updatedAt": null,
    "translationMap": {
        "ROLE": {
            "5f6d114f006883209828ddd9088e63b3": {
                "name": "DAM Curator",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "600f4bed00028a718599f29575840053"
            },
            ...
        },
        "TMPL": {
            "5f9b317c00b3db5af69abcd1ed5f82aa": {
                "name": "Digital Asset Production (Integrated)",
                "action": "CREATE",
                "isValid": true,
                "targetId": "6054cda40000d5af63dc811d9c2b3a07"
            },
            ...
        },
        ...
    }
}
```

## Sobrescritura

Este es un proceso de tres pasos.

1. Crear un mapa de traducción (esto es análogo a la fase de &quot;preparación de la instalación&quot;).
1. Edite el mapa de traducción generado configurando la variable `action` y `targetId` campos para cualquier objeto que desee sobrescribir. La acción debe ser `OVERWRITING`, y el `targetId` debe ser el uuid del objeto que se debe sobrescribir
1. Ejecute la instalación.

* [Paso 1: Creación de un mapa de traducción](#step-1---create-a-translation-map)
* [Paso 2: Modificación del mapa de traducción](#step-2---modify-the-translation-map)
* [Paso 3: Instalación](#step-3---install)

### **Paso 1: Creación de un mapa de traducción**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/translation-map
```

#### Cuerpo

Ninguno

#### Respuesta

Un mapa de traducción, con un `202 - OK` status

```json
{
    {objcode}: {
        {object uuid}: {
            "targetId": {uuid of object in destination},
            "action": {installation action},
            "name": {name of the object},
            "isValid": true
        },
        {...more objects}
    },
    {...more objcodes}
}
```


#### Ejemplo

```json
{
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "CREATE",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
```

### Paso 2: Modificación del mapa de traducción

No hay punto final para este paso.

1. En el mapa de traducción devuelto en [Paso 1: Creación de un mapa de traducción](#step-1---create-a-translation-map), inspeccione la lista de objetos que se instalarán.
1. Actualice el campo de acción de cada objeto a la acción de instalación deseada.
1. Validar la `targetId` en cada objeto. Si la acción establecida es `USEEXISTING` o `OVERWRITING`, el `targetId` debe establecerse en el UUID del objeto de destino en el entorno de destino. Para cualquier otra acción, targetId debe ser una cadena vacía.

   >[!NOTE]
   >
   >El `targetId` ya se ha rellenado si se detecta una colisión.

### **Paso 3: Instalación**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/install
```

#### Cuerpo

Es un objeto con un solo campo `translationMap`, que debe coincidir con el mapa de traducción modificado de [Paso 2: Modificación del mapa de traducción](#step-2---modify-the-translation-map).

```json
{
    "translationMap": {
        {objcode}: {
            {object uuid}: {
                "targetId": {uuid of object in destination},
                "action": {installation action},
                "name": {name of the object},
                "isValid": true
            },
            {...more objects}
        },
        {...more objcodes}
    }
}
```


#### Ejemplo

```json
{
    "translationMap": {
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "OVERWRITING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
}
```

#### Respuesta

La respuesta incluye lo siguiente `{uuid of the created installation}` y una `202 - ACCEPTED` estado.

Ejemplo: `b6aa0af8-3520-4b25-aca3-86793dff44a6`

<!--table templates

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

<table style="table-layout:fixed"> 
 <col> 
 <tbody> 
  <tr> 
   <td><b></b></td> 
  </tr> 
  <tr> 
   <td><pre></pre></td> 
  </tr> 
  </tbody> 
</table>
-->
