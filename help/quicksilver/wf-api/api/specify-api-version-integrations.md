---
content-type: api
navigation-topic: api-navigation-topic
title: Especificar una versión de API en las integraciones
description: Especificar una versión de API en las integraciones
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 889084f9a3740b40c84c658f9b0c17270b0a37d7
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# Especificar una versión de API en las integraciones

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de espacio aislado de vista previa.</span>

Todos los URI de Adobe Workfront son necesarios para hacer referencia a una versión específica de la API después de la porción &quot;attask/api&quot; del URI. El siguiente ejemplo llama a la versión 15.0:

`attask/api/v15.0/<objectName>/<objectId>`

Asegúrese de que todas sus integraciones llamen a las API de Workfront compatibles actualmente.

## Calendario de versiones y desaprobaciones de las API de Workfront

Las nuevas versiones de la API se publican periódicamente, normalmente dos veces al año. Cada versión es compatible durante tres años después de la fecha de lanzamiento, con un año adicional en estado obsoleto, donde la versión está disponible pero no es compatible.

Para obtener más información sobre la cadencia de la versión y la programación de desaprobación de las API de Workfront, consulte [Programación de versiones y asistencia de API](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* Después de la versión 23.2, la versión predeterminada de la API se establecerá en la versión más reciente. Cualquier llamada a la API sin la versión especificada utilizará la versión predeterminada. Cada vez que Workfront lanza una nueva versión de la API, la versión predeterminada se actualizará a la versión más reciente. Por lo tanto, después de publicar una nueva versión de la API de Workfront, todas las llamadas a la API que utilicen la versión predeterminada deben comprobarse para asegurarse de que la funcionalidad sigue siendo compatible.
>
>* Si su organización está utilizando la API predeterminada, su administrador de Workfront ha recibido un mensaje del Centro de anuncios con más instrucciones sobre la API predeterminada.
>
>* <span class="preview">La API predeterminada del entorno de vista previa se establece en la versión más reciente. La API predeterminada del entorno de producción se establecerá en la versión más reciente después de la versión 23.2 (abril de 2023)</span>.
>
>Para ver la versión más reciente de la API, consulte [Programación de versiones y asistencia de API](../../wf-api/api/api-version-support-schedule.md).


## Determinación de la versión de API que utiliza

Puede determinar la versión de la API que está utilizando comprobando el URI de una solicitud HTTP enviada a la API de Workfront. El siguiente ejemplo muestra un URI de solicitud de Workfront que especifica la versión 15 de la API:

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Si un URI no especifica una versión, entonces está utilizando la versión predeterminada de la API, como se muestra en el siguiente ejemplo:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Las integraciones que no especifican una versión de la API en el URI se enrutan automáticamente a la versión predeterminada de la API.

## Actualización de integraciones para utilizar versiones de API compatibles

Al crear o mantener integraciones de Workfront, debe incluir un método para actualizar dinámicamente la versión de la API y otras propiedades sujetas a cambios (como su clave de API).

Para que la actualización de integraciones sea más eficaz, debe considerar las siguientes sugerencias para registrar los valores de integración:

* Almacene valores sujetos a cambios futuros en un archivo de propiedades que mantenga actualizado
* Crear un servicio web para administrar propiedades en tiempo real
* Almacenar valores de propiedades en un almacén de datos que su aplicación pueda leer

Diseñar las integraciones de Workfront con esto en mente alivia la necesidad de un trabajo de desarrollo extenso cuando esos valores cambian inevitablemente.
