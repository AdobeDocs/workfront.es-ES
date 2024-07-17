---
content-type: api
navigation-topic: api-navigation-topic
title: Actualizar integraciones que utilizan el control de versiones de API predeterminado
description: Actualizar integraciones que utilizan el control de versiones de API predeterminado
author: Becky
feature: Workfront API
role: Developer
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Actualizar integraciones que utilizan el control de versiones de API predeterminado

Lanzamos nuevas versiones de la API de Adobe Workfront cada dos años. Cada versión es compatible durante tres años después de su lanzamiento, con un año adicional en un estado obsoleto en el que la versión está disponible pero no es compatible.

Las integraciones que no especifican una versión de la API en el URI se enrutan automáticamente al valor predeterminado. Si desea que la llamada de API utilice una versión específica de la API, debe especificar esa versión en las solicitudes de API de Workfront.

>[!NOTE]
>
>Si su organización utiliza actualmente la API predeterminada, su administrador de Workfront ha recibido un mensaje del Centro de anuncios con más instrucciones sobre la API predeterminada.

Para obtener más información sobre cómo especificar una versión en sus solicitudes de API, consulte [Especificar una versión de API en sus integraciones](../../wf-api/api/specify-api-version-integrations.md).

## Consideraciones al utilizar la API predeterminada

Tenga en cuenta lo siguiente al trabajar con la API predeterminada de Workfront:

* La versión predeterminada de la API es la más reciente. Cualquier llamada de API sin la versión especificada utilizará la versión predeterminada. Cada vez que Workfront publica una nueva versión de la API, la versión predeterminada se actualiza a la más reciente. **Por lo tanto, después de que se publique una nueva versión de la API de Workfront, cualquier llamada de API que utilice la versión predeterminada debe comprobarse para asegurarse de que la funcionalidad sigue siendo compatible**.
* Si su organización utiliza actualmente la API predeterminada obsoleta anterior, su administrador de Workfront ha recibido un mensaje del Centro de anuncios con más instrucciones sobre la API predeterminada.

Para ver la versión más reciente de la API, consulte [Versiones de API y programación de soporte](../../wf-api/api/api-version-support-schedule.md).

## Actualización de las integraciones a versiones de API compatibles

Si las solicitudes de la API de Workfront no especifican una versión, se utilizan las predeterminadas. Le recomendamos que realice sus solicitudes de API para especificar una versión compatible de la API, preferiblemente a la API compatible más reciente.

Por ejemplo, la siguiente solicitud de API de Workfront no especifica una versión de API:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Cuando se realice esta solicitud, recibirá una respuesta con texto codificado en JSON que especifica los datos de la instancia de Workfront. Como no se especifica ninguna versión de API en este URI, la llamada se dirige a Predeterminado.

Para convertir una solicitud de API predeterminada en una solicitud de API con versiones, simplemente llame a una versión de API compatible. Por ejemplo, el siguiente URI solicita la versión 15:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Al actualizar las solicitudes de la API de Workfront, puede especificar cualquier versión compatible de nuestra API. Para obtener más información sobre cómo hacer referencia a una API específica, consulte [Especificar una versión de API en las integraciones](../../wf-api/api/specify-api-version-integrations.md).

Para garantizar la ventana de compatibilidad máxima, debe llamar a la versión más reciente. Puede encontrar una lista de las API admitidas en [versiones de API y programación de soporte](../../wf-api/api/api-version-support-schedule.md).

## Historial de la versión predeterminada de la API

La intención original de la &quot;API predeterminada&quot;, o predeterminada, era asignarla a la última versión de la API de Workfront. Esto permitiría a los clientes con integraciones básicas que llamaban Predeterminado no tener que actualizar nunca sus solicitudes de API.

En 2011, Workfront lanzó la versión 3.0 de la API. La versión predeterminada se movió automáticamente a la 3.0, que dañó muchas integraciones de clientes demasiado complejas para usar la 3.0 sin ser actualizadas. Como resultado, Workfront revirtió este cambio y dejó la versión predeterminada en Versión 2.

Desde 2011, Workfront ha aumentado considerablemente la funcionalidad de la API. Debido a esto, tenemos versiones anteriores obsoletas de nuestra API. En 2017, en lugar de actualizar Predeterminado, eliminamos por completo el concepto de versión predeterminada. Esto tenía por objeto animar a nuestros clientes a utilizar versiones estables de nuestras API y a mantener sus integraciones en un ciclo de, como máximo, tres años.

Workfront está restableciendo la versión de API predeterminada. La API predeterminada está configurada con la versión más reciente de la API de Workfront y se actualizará a la versión más reciente cada vez que se publique una nueva versión.

