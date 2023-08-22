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
hide: true
hidefromtoc: true
source-git-commit: 4042384f4e3c70bb23d585d5a5e392d624ac6cb4
workflow-type: tm+mt
source-wordcount: '2407'
ht-degree: 2%

---

# Mover objetos de uno [!DNL Workfront] entorno a otro

<!-- 
TO DO

Overview of value
Check for any code changes
Fix {}
Add to tocs
-->

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plan</td> 
   <td> <p>Enterprise, Prime o Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] licencia</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>Debe ser un [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Permisos de objeto</p> </td> 
   <td> <p>Todas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paquete de soporte</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL preferido] o [!UICONTROL Enterprise]</p> <p>El paquete de soporte estándar no tiene acceso a la zona protegida de actualización personalizada, pero sí tiene acceso a la de vista previa.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Requisitos previos

El punto final Crear paquete promocional supone que ya ha configurado el entorno de origen. Esta llamada de API requiere la creación manual de un mapa de objetos de [!DNL Workfront] objCodes y GUID de objetos. A continuación se describe la estructura específica de este mapa.

## Objetos compatibles para la promoción del entorno

La función Promoción de entornos está diseñada para proporcionar la capacidad de mover objetos relacionados con la configuración de un entorno a otro. No admite la capacidad de mover objetos transaccionales (con excepciones limitadas).

* [Objetos de trabajo](#work-objects)
* [Objetos de informes](#reporting-objects)
* [Objetos de datos personalizados](#custom-data-objects)
* [Objetos de organización](#organization-objects)
* [Otros objetos de configuración](#other-configuration-objects)


### Objetos de trabajo

| Objeto promocionable | Subobjetos incluidos |
| --- | --- |
| Proyecto (PROJ) | Proyecto<br>Tarea<br>Asignación<br>Predecesora<br>Compañía<br>Tasa de anulación<br>Grupo<br>Rol<br>Equipo<br>Proceso de aprobación<br>Ruta de aprobación<br>Paso de aprobación<br>Aprobador de etapa<br>Programación<br>Día no laborable<br>Definición de cola<br>Grupo de temas de cola<br>Tema de cola<br>Regla de enrutamiento<br>Ruta de hitos<br>Hito<br>Tipo de hora<br>Conjunto de recursos<br>Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Opción de parámetro<br>Lógica de visualización de categoría |
| Plantilla (TMPL) | Plantilla<br>Tarea de plantilla<br>Asignación de tarea de plantilla<br>Tarea de plantilla predecesora<br>Compañía<br>Tasa de anulación<br>Grupo<br>Rol<br>Equipo<br>Proceso de aprobación<br>Ruta de aprobación<br>Paso de aprobación<br>Aprobador de etapa<br>Programación<br>Día no laborable<br>Definición de cola<br>Grupo de temas de cola<br>Tema de cola<br>Regla de enrutamiento<br>Ruta de hitos<br>Hito<br>Tipo de hora<br>Conjunto de recursos<br>Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Opción de parámetro<br>Lógica de visualización de categoría |

### Objetos de informes

| Objeto promocionable | Subobjetos incluidos |
| --- | --- |
| Plantilla de diseño (UITMPL) | Plantilla de diseño<br>Tablero<br>Calendario<br>Sección de calendario<br>Página externa<br>Informe<br>Filtrar<br>Agrupación<br>Ver<br>Parámetro |
| Tablero (PTLTAB) | Tablero<br>Calendario<br>Sección de calendario<br>Página externa<br>Informe<br>Filtrar<br>Agrupación<br>Ver<br>Parámetro |
| Calendario (CALEND) | Calendario<br>Sección de calendario |
| Página externa (EXTSEC) | Página externa |
| Informe (PTLSEC) | Informe<br>Filtrar<br>Agrupación<br>Ver<br>Parámetro |
| Filtro (UIFT) | Filtrar<br>Parámetro |
| Agrupación (UIGB) | Agrupación<br>Parámetro |
| Vista (UIVW) | Ver<br>Parámetro |

### Objetos de datos personalizados

| Objeto promocionable | Subobjetos incluidos |
| --- | --- |
| Categoría (CTGY) | Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Opción de parámetro<br>Lógica de visualización de categoría<br>Grupo |
| Parámetro (PARAM) | Parámetro<br>Opción de parámetro |
| Grupo de parámetros (PGRP) | Grupo de parámetros |

### Objetos de organización

| Objeto promocionable | Subobjetos incluidos |
| --- | --- |
| Grupo (GROUP) | Grupo <br>Subgrupos (hasta 5 niveles)<br>Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Opción de parámetro<br>Lógica de visualización de categoría |
| Rol (ROLE) | Rol |
| Equipo (EQUIPO) | Equipo<br>Grupo |
| Empresa (CMPY) | Compañía<br>Tasa de anulación<br>Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Parámetro <br>Lógica de visualización de categoría<br>Grupo |
| Portfolio (PUERTO) | Portfolio<br>Programa<br>Grupo<br>Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Opción de parámetro<br>Lógica de visualización de categoría |
| Programa (PRGM) | Programa<br>Portfolio<br>Grupo<br>Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Opción de parámetro<br>Lógica de visualización de categoría |

### Otros objetos de configuración

| Objeto promocionable | Subobjetos incluidos |
| --- | --- |
| Proceso de aprobación (ARVPRC) | Proceso de aprobación<br>Ruta de aprobación<br>Paso de aprobación<br>Aprobador de etapa<br>Rol<br>Equipo<br>Grupo |
| Programa (SCHED) | Programación<br>Día no laborable<br>Grupo |
| Ruta de hitos (MPATH) | Ruta de hitos<br>Hito |
| Perfil de hoja de horas (TSPRO) | Perfil de hoja de horas<br>Tipo de hora |
| Tipo de hora (HOURT) | Tipo de hora |
| Tipo de gasto (EXPTYPE) | Tipo de gasto |
| Tipo de riesgo (RSKTYPE) | Tipo de riesgo |
| Conjunto de recursos (RSPL) | Conjunto de recursos |

## Autenticación

La API autentica cada solicitud para garantizar que el cliente tenga acceso para ver o modificar un objeto solicitado.

La autenticación se realiza pasando un ID de sesión que se puede proporcionar mediante uno de los métodos siguientes:

### Autenticación de encabezado de solicitud

El método de autenticación preferido es pasar un encabezado de solicitud denominado SessionID que contenga el token de sesión. Esto tiene la ventaja de estar seguro contra [Falsificación de solicitud en sitios múltiples (CSRF)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) ataques y no interferir con el URI con fines de almacenamiento en caché.

A continuación se muestra un ejemplo de encabezado de solicitud:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

### Solicitar autenticación de parámetro

Puede autenticarse pasando un parámetro de solicitud denominado sessionID, como se muestra en el siguiente ejemplo: 

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0?sessionID=abc1234
```

### Autenticación basada en cookies

La API utiliza la misma autenticación basada en cookies que la IU web utiliza para configurar el sistema. En el que, si un cliente inicia sesión en Workfront AJAX mediante la interfaz de usuario web, cualquier llamada a la red realizada desde el mismo explorador utiliza la misma autenticación.

>[!NOTE]
>
>Para protegerse contra la posibilidad de ataques CSRF (Falsificación de solicitud en sitios múltiples), este método de autenticación solo está disponible para operaciones de solo lectura.

## Extremos de API

* [Creación de un paquete](#create-a-package)
* [Obtener una lista de paquetes](#get-a-list-of-packages)
* [Obtención de un paquete por ID](#get-a-package-by-id)
* [Obtener la definición de configuración de un paquete](#get-a-packages-configuration-definition)
* [Reemplazar detalles y definición del paquete](#replace-package-details-and-definition)
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
Tenga en cuenta la estructura del `objectCollections`  matriz.
>
Cada elemento de la matriz contiene un `objCode` que corresponde al código de objeto documentado en el Explorador de API de Workfront.
>
Cada elemento también contiene un `entities` colección. Se espera el `ID` y `name` claves para estar presentes.
>
Para obtener la lista de códigos de objeto permitidos que se van a solicitar en la `objectCollections` , consulte la [Objetos compatibles para la promoción del entorno](#supported-objects-for-environment-promotion) de este artículo.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Encabezados

```json
{
    "Authorization": "Bearer ****************",
    "Content-Type": "application/json"
}
```

#### Cuerpo

```json
{
    "packageName": "Agency Onboarding - 2023-06-06",
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

#### respuesta

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ASSEMBLING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "isPrivate": true,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
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
    "Authorization": "Bearer ****************"
}
```

#### Cuerpo

_Empty_

#### respuesta

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
            "version": 1,
            "installationCounts": {},
            "createdAt": "2023-06-06T17:29:21.600Z",
            "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
            "publishedAt": null,
            "isPrivate": true,
            "customerId": "61aa9d090005fa42152c1cb66659f38d"
        },
        {...}
    ]
}
```

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
    "Authorization": "Bearer ****************"
}
```

#### Cuerpo

_Empty_

#### respuesta

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "DRAFT",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "isPrivate": true,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "metadata": {
            "displayOrder": ["GROUP","ROLE","TMPL","PROJ","PTLTAB"], 
            "historyOrder": ["GROUP","ROLE","TMPL","TTSK","PROJ","PTLTAB"], 
            "installOrder": ["GROUP","ROLE","TMPL","TTSK","TPRED","TASSGN","PROJ","QUED","RRUL","QUET","UIFT","UIGB","UIVW","PTLTAB"], 
            "summaryOrder": ["GROUP","ROLE","TMPL"], 
            "shapeVersion": 2
        },
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description"
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

### Obtener la definición de configuración de un paquete

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}/definition</code></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/definition
```

#### Encabezados

```json
{
    "Authorization": "Bearer ****************"
}
```

#### Cuerpo

_Empty_

#### respuesta

```
200
```

```json
{
    "metadata": {
        "displayOrder": ["GROUP","ROLE","TMPL","PROJ","PTLTAB"], 
        "historyOrder": ["GROUP","ROLE","TMPL","TTSK","PROJ","PTLTAB"], 
        "installOrder": ["GROUP","ROLE","TMPL","TTSK","TPRED","TASSGN","PROJ","QUED","RRUL","QUET","UIFT","UIGB","UIVW","PTLTAB"], 
        "summaryOrder": ["GROUP","ROLE","TMPL"], 
        "shapeVersion": 2
    },
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID" null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

### Reemplazar detalles y definición del paquete

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PUT /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Esta llamada reemplaza todo el contenido del paquete de promoción.

La solicitud espera que se proporcionen todos los campos editables.

Los atributos editables son:

1. nombre (cadena)
2. description (cadena)
3. origen (cadena con validación de URL)
4. estado (cadena con validación de valor)
5. versión (entero)
6. metadata (colección)
7. packageEntities (colección)

Las opciones de estado incluyen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>MONTAJE</td> 
   <td><p>Este estado se asigna automáticamente mientras se montan los objetos.</p><p>Un cliente no puede establecer directamente este estado.</p></td> 
  </tr> 
  <tr> 
   <td>BORRADOR</td> 
   <td><p>Este estado se asigna al final de un proceso de ensamblado o al crear un paquete de promoción vacío.</p><p>Un cliente puede volver a mover el paquete de promoción a este estado.</p><p>Mientras que en este estado el paquete de promoción no se puede instalar en ningún entorno.</p></td> 
  </tr> 
  <tr> 
   <td>PRUEBAS</td> 
   <td><p>Este estado permite instalar un paquete de promoción en cualquier zona protegida de vista previa o actualización personalizada. Mientras esté en este estado, el paquete no se puede instalar en Producción.</p></td> 
  </tr> 
  <tr> 
   <td>ACTIVO</td> 
   <td><p>Este estado permite instalar un paquete de promoción en cualquier entorno, incluido el de producción.</p><p>Cuando el estado de un paquete se establece en ACTIVO, la variable <code>publishedAt</code> La fecha se establece automáticamente en la marca de tiempo actual de la solicitud.</p></td> 
  </tr> 
  <tr> 
   <td>DESACTIVADO</td> 
   <td><p>Este estado se utilizará para ocultar los paquetes de promoción utilizados anteriormente que no se instalarán en ningún entorno en el futuro.</p><p>Cuando un paquete se encuentra en este estado, no se puede instalar en ningún entorno.</p><p>Cuando el estado de un paquete se establece en DESHABILITADO, la variable <code>retiredAt</code> La fecha se establece automáticamente en la marca de tiempo actual de la solicitud.</p><p>Se recomienda usar este estado en lugar de usar el<code>DELETE /package</code> extremo porque se puede recuperar y el historial de instalación se conserva para cualquier implementación realizada con este paquete.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>El paquete de promoción pasa automáticamente a este estado si falla la fase de MONTAJE.</p><p>Para devolver el paquete a la fase de MONTAJE, se debe almacenar en déclencheur de nuevo el proceso de extracción.</p></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
PUT https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Encabezados

```json
{
    "Authorization": "Bearer ****************",
    "Content-Type": "application/json"
}
```

#### Cuerpo

```json
{
    "packageName": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes... with a description change",
    "source": "https://{domain}.{environment}.workfront.com",
    "status": "TESTING",
    "version": 1,
    "metadata": {
        "displayOrder": ["GROUP","ROLE","TMPL","PROJ","PTLTAB"],
        "historyOrder": ["GROUP","ROLE","TMPL","TTSK","PROJ","PTLTAB"], 
        "installOrder": ["GROUP","ROLE","TMPL","TTSK","TPRED","TASSGN","PROJ","QUED","RRUL","QUET","UIFT","UIGB","UIVW","PTLTAB"], 
        "summaryOrder": ["GROUP","ROLE","TMPL"], 
        "shapeVersion": 2
    },
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID" null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

#### respuesta

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "TESTING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "isPrivate": true,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "metadata": {
            "displayOrder": ["GROUP","ROLE","TMPL","PROJ","PTLTAB"], 
            "historyOrder": ["GROUP","ROLE","TMPL","TTSK","PROJ","PTLTAB"], 
            "installOrder": ["GROUP","ROLE","TMPL","TTSK","TPRED","TASSGN","PROJ","QUED","RRUL","QUET","UIFT","UIGB","UIVW","PTLTAB"], 
            "summaryOrder": ["GROUP","ROLE","TMPL"], 
            "shapeVersion": 2
        },
        "displayEntities": {
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
1. origen (cadena con validación de URL)
1. estado (cadena con validación de valor)
1. versión (entero)
1. metadata (colección)
1. packageEntities (colección)

   o

   objectCollections, matriz

Proporcionar el `packageEntities` actualizará el paquete de promoción con la definición de configuración proporcionada.

Proporcionar el `objectCollections` iniciará una reextracción desde el `source` entorno asociado con el paquete de promoción. El `source` debe proporcionarse cuando la variable `objectCollections` se proporciona.

#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### Encabezados

```json
{
    "Authorization": "Bearer ****************",
    "Content-Type": "application/json"
}
```

#### Cuerpo

```json
{
    "status": "ACTIVE"
}
```

#### respuesta

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ACTIVE",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "isPrivate": true,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "metadata": {
            "displayOrder": ["GROUP","ROLE","TMPL","PROJ","PTLTAB"], 
            "historyOrder": ["GROUP","ROLE","TMPL","TTSK","PROJ","PTLTAB"], 
            "installOrder": ["GROUP","ROLE","TMPL","TTSK","TPRED","TASSGN","PROJ","QUED","RRUL","QUET","UIFT","UIGB","UIVW","PTLTAB"], 
            "summaryOrder": ["GROUP","ROLE","TMPL"], 
            "shapeVersion": 2
        },
        "displayEntities": {
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
A diferencia de eliminar un paquete de promoción, la recomendación es cambiar el estado del paquete a DESHABILITADO. Esto permite recuperar el paquete y conservar el historial de instalación del lugar donde se implementó.

#### URL

```
DELETE https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Encabezados

```json
{
    "Authorization": "Bearer ****************"
}
```

#### Cuerpo

_Empty_

#### respuesta

```
200
```

```
Deleted
```

### Ejecutar una ejecución previa

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
   <td>IGNORAR</td> 
   <td><p>Esta acción no se establecerá automáticamente.</p><p>Proporciona la capacidad de anular manualmente una acción CREATE o USEEXISTING asignada antes de ejecutar el <code>/install</code> llamada.</p><p><b>Notas: </b><ul><li><p>Si un registro que originalmente se estableció en CREATE se establece en IGNORE, cualquier registro secundario también se debe establecer en IGNORE.</p><p>Por ejemplo, si un registro de plantilla se ha asignado con una acción CREAR y el usuario que lo instala desea excluirlo de la implementación, puede establecer la acción de la plantilla en IGNORAR.</p><p>En este caso, si el usuario que realiza la instalación no establece las tareas de plantilla, las asignaciones de tareas de plantilla, las predecesoras de tareas de plantilla, la definición de cola, los temas de cola, las reglas de enrutamiento, etc. en IGNORE, la implementación resultará en un intento de instalación fallido.</p></li><li><p>Si un registro que originalmente se estableció en USEEXISTING se establece en IGNORE, puede haber algunos efectos adversos durante el proceso de instalación.</p><p>Por ejemplo, si se asignó un registro de grupo con la acción USEEXISTING y el usuario que realiza la instalación cambia la acción a IGNORE, para los objetos que requieren un grupo (por ejemplo, un proyecto no puede existir sin un grupo asignado), el grupo predeterminado del sistema se asignará a ese proyecto.</p></li><li><p>Si un registro que originalmente se estableció en USEEXISTING se establece en CREATE, puede haber algunos efectos adversos durante el proceso de instalación porque muchas entidades de Workfront tienen restricciones de nombre único.</p><p>Por ejemplo, si se asignó un registro de "Grupo predeterminado" con la acción USEEXISTING y el usuario que realiza la instalación cambia la acción a CREATE, dado que ya existe un "Grupo predeterminado", el intento de instalación no podrá completar todos los pasos. Los nombres de grupo deben ser únicos.</p><p>Algunas entidades no tienen una restricción de nombre único. Para esos objetos, realizar este cambio dará como resultado dos registros con nombres idénticos. Por ejemplo, las plantillas, los proyectos, las vistas, los filtros, las agrupaciones, los informes y los paneles no requieren restricciones de nombre único. Se recomienda tener nombres únicos para estos registros, pero no se aplica.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

Actualmente no se admite una actualización `action` en las capacidades alpha de este servicio. La opción para permitir una ACTUALIZACIÓN `action` es algo que estamos investigando.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/translationmap
```

#### Encabezados

```json
{
    "Authorization": "Bearer ****************",
    "Content-Type": "application/json"
}
```

#### Cuerpo

```json
{}
```

#### respuesta

```
200
```

```json
{}
```

### Ejecutar una instalación

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Esta llamada inicia un intento de instalación de un paquete promocional en el entorno de destino identificado en la dirección URL del POST.

#### Opciones

Si un `translationmap` no se proporciona en el cuerpo del POST, el proceso iniciará automáticamente el `/translationmap` llamada. El `translationmap` que se devuelva se utilizará tal cual, sin oportunidad de revisarlo ni realizar ajustes en él.

Si un `translationmap` se proporciona en el cuerpo del POST, el proceso de instalación utilizará la asignación proporcionada. Esto ofrece al usuario que realiza la instalación la oportunidad de revisar y realizar los ajustes necesarios antes de ejecutar un intento de instalación.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/install
```

#### Encabezados

```json
{
    "Authorization": "Bearer ****************",
    "Content-Type": "application/json"
}
```

#### Cuerpo

```json
{
}
```

#### respuesta

```
200
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
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### Encabezados

```json
{
    "Authorization": "Bearer ****************"
}
```

#### Cuerpo

_Empty_

#### respuesta

```
200
```

```json
[
    {
        "id": "2892b936-e09e-455a-935f-e1462ab9753c",
        "blueprintId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
        "blueprintVersion": 1,
        "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
        "customerId": "54286d78b064451096752b99bf968481",
        "status": "COMPLETED",
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
    "Authorization": "Bearer ****************"
}
```

#### Cuerpo

_Empty_

#### respuesta

```
200
```

```json
{
    "id": "2892b936-e09e-455a-935f-e1462ab9753c",
    "blueprintId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
    "blueprintVersion": 1,
    "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
    "customerId": "54286d78b064451096752b99bf968481",
    "status": "COMPLETED",
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