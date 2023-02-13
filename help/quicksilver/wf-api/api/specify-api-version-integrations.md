---
content-type: api
navigation-topic: api-navigation-topic
title: Especificar una versión de API en las integraciones
description: Especificar una versión de API en las integraciones
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Especificar una versión de API en las integraciones

Todos los URI de Adobe Workfront son necesarios para hacer referencia a una versión específica de la API después de la porción &quot;attask/api&quot; del URI. El siguiente ejemplo llama a la versión 7.0:
`attask/api/v7.0/<objectName>/<objectId>` Asegúrese de que todas sus integraciones llamen a las API de Workfront compatibles actualmente.

## Calendario de versiones y desaprobaciones de las API de Workfront

Las nuevas versiones de la API se publican cada dos años, cada seis a ocho meses. Cada versión es compatible durante tres años después de la fecha de lanzamiento, con un año adicional en estado obsoleto, donde la versión está disponible pero no es compatible.

Para obtener más información sobre la cadencia de la versión y la programación de desaprobación de las API de Workfront, consulte [Programación de versiones y asistencia de API](../../wf-api/api/api-version-support-schedule.md).

Workfront dejó de utilizar la versión predeterminada de la API en julio de 2017. Esto significa que Workfront ya no designa una versión específica de la API para que sea la versión predeterminada. Todos los URI de API futuros deben especificar una versión de la API para que sea válida.

>[!IMPORTANT]
>
> Todas las integraciones que utilicen la versión de API predeterminada deben actualizarse para llamar a una versión de API compatible específica antes del 1 de julio de 2018.

## Determinación de la versión de API que utiliza

Puede determinar la versión de la API que está utilizando comprobando el URI de una solicitud HTTP enviada a la API de Workfront. El siguiente ejemplo muestra un URI de solicitud de Workfront que especifica la versión 7 de la API:

`https://<domainname>.my.workfront.com/attask/api/v7.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Si un URI no especifica una versión, entonces está utilizando la versión predeterminada de la API, como se muestra en el siguiente ejemplo:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Las integraciones que no especifican una versión de la API en el URI se enrutan automáticamente a la versión predeterminada de la API y no funcionarán después del 1 de julio de 2018.

## Actualización de integraciones para utilizar versiones de API compatibles

Al crear o mantener integraciones de Workfront, debe incluir un método para actualizar dinámicamente la versión de la API y otras propiedades sujetas a cambios (como su clave de API).

Para que la actualización de integraciones sea más eficaz, debe considerar las siguientes sugerencias para registrar los valores de integración:

* Almacene valores sujetos a cambios futuros en un archivo de propiedades que mantenga actualizado
* Crear un servicio web para administrar propiedades en tiempo real
* Almacenar valores de propiedades en un almacén de datos que su aplicación pueda leer

Diseñar las integraciones de Workfront con esto en mente alivia la necesidad de un trabajo de desarrollo extenso cuando esos valores cambian inevitablemente.
