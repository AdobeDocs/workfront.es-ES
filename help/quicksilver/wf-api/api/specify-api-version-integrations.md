---
content-type: api
navigation-topic: api-navigation-topic
title: Especifique una versión de API en sus integraciones
description: Especifique una versión de API en sus integraciones
author: Becky
feature: Workfront API
role: Developer
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
TQID: https://experienceleague.adobe.com/GWA77t-kaVNG7tfSsg5Fe5kLtR3Ibo0YbW7Gp7wBQ0U
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 438
ht-degree: 19%

---

# Especificar una versión de API en las integraciones

Todos los URI de Adobe Workfront deben hacer referencia a una versión específica de la API después de la parte &quot;attask/api&quot; del URI. El siguiente ejemplo llama a la versión 15.0:

`attask/api/v15.0/<objectName>/<objectId>`

Asegúrese de que todas las integraciones llamen a las API de Workfront que admite actualmente.

## Programación de versiones y desuso de las API de Workfront

Las nuevas versiones de la API se publican regularmente, generalmente dos veces al año. Cada versión es compatible durante tres años después de la fecha de lanzamiento, con un año adicional en un estado obsoleto en el que la versión está disponible pero no es compatible.

Para obtener más información sobre la cadencia de lanzamiento y la programación de desaprobación de las API de Workfront, consulte [Creación de versiones de API y programación de soporte](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* La versión predeterminada de la API es la más reciente. Cualquier llamada de API sin la versión especificada utilizará la versión predeterminada. Cada vez que Workfront publica una nueva versión de la API, la versión predeterminada se actualiza a la más reciente. **Por lo tanto, después de que se publique una nueva versión de la API de Workfront, cualquier llamada de API que utilice la versión predeterminada debe comprobarse para asegurarse de que la funcionalidad sigue siendo compatible.**
>
>* Si su organización utiliza actualmente la API predeterminada, su administrador de Workfront habrá recibido un mensaje del Centro de anuncios con instrucciones adicionales sobre la API predeterminada.
>
>Para ver la versión más reciente de la API, consulte [Versiones de API y programación de soporte](../../wf-api/api/api-version-support-schedule.md).


## Determinación de la versión de la API que está utilizando

Puede determinar la versión de la API que utiliza comprobando el URI de una solicitud HTTP enviada a la API de Workfront. El siguiente ejemplo muestra un URI de solicitud de Workfront que especifica la versión 15 de la API:

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Si un URI no especifica una versión, está utilizando la versión predeterminada de la API, como se muestra en el siguiente ejemplo:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Las integraciones que no especifican una versión de la API en el URI se enrutan automáticamente a la versión predeterminada de la API.

## Actualización de integraciones para utilizar versiones de API compatibles

A medida que crea o mantiene integraciones de Workfront, debe incluir un método para actualizar dinámicamente la versión de la API y otras propiedades sujetas a cambios (como su clave de API).

Para que la actualización de las integraciones sea más eficiente, debe tener en cuenta las siguientes sugerencias para registrar los valores de integración:

* Almacena valores sujetos a cambios futuros en un archivo de propiedades que mantiene actualizado
* Creación de un servicio web para administrar propiedades en tiempo real
* Almacenar valores de propiedades en un almacén de datos que la aplicación pueda leer

El diseño de las integraciones de Workfront con esto en mente alivia la necesidad de realizar un trabajo de desarrollo exhaustivo cuando estos valores cambian inevitablemente.
