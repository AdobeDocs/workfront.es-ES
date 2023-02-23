---
content-type: api
navigation-topic: api-navigation-topic
title: Actualizar integraciones que utilizan versiones de API predeterminadas
description: Actualizar integraciones que utilizan versiones de API predeterminadas
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 889084f9a3740b40c84c658f9b0c17270b0a37d7
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# Actualizar integraciones que utilizan versiones de API predeterminadas

<!-- This article is going to need a complete revamp or to be removed-->

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de espacio aislado de vista previa.</span>

Lanzamos nuevas versiones de la API de Adobe Workfront cada dos años. Cada versión es compatible durante tres años después de su lanzamiento, con un año adicional en estado obsoleto en el que la versión está disponible pero no es compatible.

Las integraciones que no especifican una versión de la API en el URI se enrutan automáticamente a Default. Si desea que la llamada de API utilice una versión específica de la API, debe especificar esa versión en las solicitudes de la API de Workfront.

>[!NOTE]
>
>Si su organización está utilizando la API predeterminada, su administrador de Workfront ha recibido un mensaje del Centro de anuncios con más instrucciones sobre la API predeterminada.


<!--
Integrations that do not specify a version of the API in the URI are automatically routed to Default, which has been deprecated. In order for your Workfront integrations to be valid, you must specify a supported API version in your Workfront API requests.
-->

Para obtener más información sobre cómo especificar una versión en las solicitudes de API, consulte [Especificar una versión de API en las integraciones](../../wf-api/api/specify-api-version-integrations.md).

## Consideraciones al utilizar la API predeterminada

Tenga en cuenta lo siguiente al trabajar con la API predeterminada de Workfront:

* Después de la versión 23.2, la versión predeterminada de la API se establecerá en la versión más reciente. Cualquier llamada a la API sin la versión especificada utilizará la versión predeterminada. Cada vez que Workfront lanza una nueva versión de la API, la versión predeterminada se actualizará a la versión más reciente. **Por lo tanto, después de publicar una nueva versión de la API de Workfront, todas las llamadas a la API que utilicen la versión predeterminada deben comprobarse para asegurarse de que la funcionalidad sigue siendo compatible**.
* Si su organización está utilizando la API predeterminada obsoleta, su administrador de Workfront ha recibido un mensaje del Centro de anuncios con más instrucciones sobre la API predeterminada.
* <span class="preview">La API predeterminada del entorno de vista previa está configurada en la versión más reciente. La API predeterminada del entorno de producción se establecerá en la versión más reciente después de la versión 23.2.</span>

Para ver la versión más reciente de la API, consulte [Programación de versiones y asistencia de API](../../wf-api/api/api-version-support-schedule.md).

<!--

## Deprecating Default

In an effort to improve the Workfront API, we are in the process of removing older API versions that have exceeded our support window of three years. One of these versions is Version 2, to which Default is mapped. This version was released in 2010, and much of the logic supported in the Attask/Workfront application at that time either no longer exists or has substantially changed.

We deprecated Default in July 2017, and we will no longer designate a specific version of the API to be the default version. Instead, all Workfront API requests must specify a specific API version.

>[!IMPORTANT]
>
> By July 1, 2018 all of your Workfront integrations that use Default must be updated to call a specific supported API version. After that date, all of your Workfront API requests used by integrations that do not specify a version will fail.

To learn about the Workfront deprecation cadence, see [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md).

-->

## Actualización de las integraciones a versiones de API compatibles

Si las solicitudes de API de Workfront no especifican una versión, utilizan Predeterminado. Recomendamos sus solicitudes de API para especificar una versión compatible de la API, preferiblemente a la API más reciente admitida.

Por ejemplo, la siguiente solicitud de API de Workfront no especifica una versión de API:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Cuando se realiza esta solicitud, recibe una respuesta con texto codificado JSON que especifica los datos de su instancia de Workfront. Como no se especifica ninguna versión de API en este URI, la llamada pasa a Predeterminado.

Para convertir una solicitud de API predeterminada en una solicitud de API con versiones, simplemente llame a una versión de API compatible. Por ejemplo, el siguiente URI solicita la versión 15:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Al actualizar sus solicitudes de API de Workfront, puede especificar cualquier versión compatible de nuestra API. Para obtener más información sobre la referencia a una API específica, consulte [Especificar una versión de API en las integraciones](../../wf-api/api/specify-api-version-integrations.md).

Para garantizar la ventana de asistencia máxima, debe llamar a la versión más reciente. Puede encontrar una lista de API compatibles en [Programación de versiones y asistencia de API](../../wf-api/api/api-version-support-schedule.md).

## Historial de la versión predeterminada de la API

La intención original de la &quot;API predeterminada&quot;, o predeterminada, era asignarla a la última versión de la API de Workfront. Esto permitiría a los clientes con integraciones básicas que llamaban Predeterminado no tener que actualizar nunca sus solicitudes de API.

En 2011, Workfront lanzó la versión 3.0 de la API. El valor predeterminado se movió automáticamente a la versión 3.0, que rompió muchas integraciones de clientes que eran demasiado complejas para utilizar la versión 3.0 sin que se actualizara. Como resultado, Workfront revirtió este cambio y dejó la versión predeterminada en la Versión 2.

Desde 2011, Workfront ha aumentado sustancialmente la funcionalidad de la API. Debido a esto, hemos desaprobado versiones anteriores de nuestra API. En 2017, en lugar de actualizar Predeterminado, hemos eliminado por completo el concepto de versión predeterminada. Esto fue para animar a nuestros clientes a utilizar versiones estables de nuestras API y a mantener sus integraciones en un ciclo de, como máximo, tres años.

Workfront está restableciendo la versión de API predeterminada. La API predeterminada se establece en la versión más reciente de la API de Workfront y se actualizará a la versión más reciente cada vez que se publique una nueva versión.

