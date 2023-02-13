---
content-type: api
navigation-topic: api-navigation-topic
title: Actualizar integraciones que utilizan versiones de API predeterminadas
description: Actualizar integraciones que utilizan versiones de API predeterminadas
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Actualizar integraciones que utilizan versiones de API predeterminadas

Lanzamos nuevas versiones de la API de Adobe Workfront cada dos años. Cada versión es compatible durante tres años después de su lanzamiento, con un año adicional en estado obsoleto en el que la versión está disponible pero no es compatible.

Las integraciones que no especifican una versión de la API en el URI se enrutan automáticamente a Default, que ha quedado obsoleta. Para que las integraciones de Workfront sean válidas, debe especificar una versión de API compatible en las solicitudes de API de Workfront.

Para obtener más información sobre cómo especificar una versión en las solicitudes de API, consulte [Especificar una versión de API en las integraciones](../../wf-api/api/specify-api-version-integrations.md).

## Explicación de la versión predeterminada de la API

La intención original de la &quot;API predeterminada&quot;, o predeterminada, era asignarla a la última versión de la API de Workfront. Esto permitiría a los clientes con integraciones básicas que llamaban Predeterminado no tener que actualizar nunca sus solicitudes de API.

En 2011, Workfront lanzó la versión 3.0 de la API. El valor predeterminado se movió automáticamente a la versión 3.0, que rompió muchas integraciones de clientes que eran demasiado complejas para utilizar la versión 3.0 sin que se actualizara. Como resultado, Workfront revirtió este cambio y dejó la versión predeterminada en la Versión 2.

Lamentablemente, este tema nunca se volvió a examinar y ahora que planeamos aumentar sustancialmente la funcionalidad de la API, nos vemos obligados a eliminar versiones anteriores de nuestra API, incluido Default. En lugar de actualizar Default, que indudablemente rompería más integraciones, eliminamos por completo el concepto de versión predeterminada. Esto es para animar a nuestros clientes a utilizar versiones estables de nuestras API y a mantener sus integraciones en un ciclo de, como máximo, tres años.

## Obsoleto predeterminado

En un esfuerzo por mejorar la API de Workfront, estamos eliminando las versiones de API anteriores que han superado nuestra ventana de asistencia de tres años. Una de estas versiones es Versión 2, a la que se asigna Predeterminado. Esta versión se publicó en 2010 y gran parte de la lógica admitida en la aplicación Attask/Workfront en ese momento ya no existe o ha cambiado sustancialmente.

En julio de 2017 se dejó de utilizar el valor predeterminado y ya no designaremos una versión específica de la API para que sea la versión predeterminada. En su lugar, todas las solicitudes de API de Workfront deben especificar una versión de API específica.

>[!IMPORTANT]
>
> Para el 1 de julio de 2018, todas las integraciones de Workfront que utilicen Default deben actualizarse para llamar a una versión de API compatible específica. Después de esta fecha, todas las solicitudes de API de Workfront que utilicen integraciones que no especifiquen una versión fallarán.

Para obtener más información sobre la cadencia de desaprobación de Workfront, consulte [Programación de versiones y asistencia de API](../../wf-api/api/api-version-support-schedule.md).

## Actualización de las integraciones a versiones de API compatibles

Si las solicitudes de API de Workfront no especifican una versión, utilizan Predeterminado. Debe actualizar sus solicitudes de API para especificar una versión compatible de la API, preferiblemente a la API más reciente admitida.

Por ejemplo, la siguiente solicitud de API de Workfront no especifica una versión de API:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Cuando se realiza esta solicitud, recibe una respuesta con texto codificado JSON que especifica los datos de su instancia de Workfront. Como no se especifica ninguna versión de API en este URI, la llamada pasa a Predeterminado.

Para convertir una solicitud de API predeterminada en una solicitud de API con versiones, simplemente llame a una versión de API compatible. Por ejemplo, el siguiente URI solicita la versión 9:

`https://davidwhite.my.workfront.com/attask/api/`**v9.0**`/project/metadata`

Al actualizar sus solicitudes de API de Workfront, puede especificar cualquier versión compatible de nuestra API. Para obtener más información sobre la referencia a una API específica, consulte [Especificar una versión de API en las integraciones](../../wf-api/api/specify-api-version-integrations.md).

Para garantizar la ventana de asistencia máxima, debe llamar a la versión más reciente (versión 9). Puede encontrar una lista de API compatibles en [Programación de versiones y asistencia de API](../../wf-api/api/api-version-support-schedule.md).

Es imperativo que actualice las integraciones que tenga que utilicen Predeterminado. Si actualmente tiene integraciones que no especifican una versión, puede recibir notificaciones de su vendedor de Workfront, gestor de éxito de clientes o representante de asistencia, o bien un mensaje del centro de anuncios.

Asegúrese de que sus integraciones se actualicen lo antes posible para llamar a una versión compatible de nuestra API.
