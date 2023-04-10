---
content-type: reference
product-area: workfront-integrations
keywords: nativa,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Métodos de integración de Adobe Workfront
description: Puede integrar [!DNL Adobe Workfront] con aplicaciones de terceros. Estas integraciones pueden ampliar la utilidad de [!DNL Workfront] y adaptarlo a las necesidades de su organización. Puede utilizar cualquiera o todas estas integraciones, en función de cuál sea la más útil para una tarea determinada.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 328d3a8d16ace22100d86efc127874d7edd6cb6d
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Métodos de integración de Adobe Workfront

Puede integrar [!DNL Adobe Workfront] con aplicaciones de terceros, así como otras [!DNL Adobe] productos. Estas integraciones pueden ampliar la utilidad de [!DNL Workfront] y adaptarlo a las necesidades de su organización. Puede utilizar cualquiera o todas estas integraciones, en función de cuál sea la más útil para una tarea determinada.

## Integraciones integradas

Workfront proporciona varias integraciones que puede configurar directamente desde Workfront o desde otra aplicación instalando el complemento de Workfront para esa aplicación. Estas integraciones incorporadas cubren muchos casos de uso comunes y se centran en ampliar y conectar las experiencias de usuario para los usuarios finales.

Las integraciones integradas de Workfront se centran principalmente en la productividad personal y la colaboración. Estas integraciones reducen las interrupciones en el flujo de trabajo de un usuario individual, lo que les permite recibir notificaciones de Workfront, acceder a información y actuar sobre elementos de trabajo de Workfront sin salir de la aplicación integrada.

Las ventajas de las integraciones integradas pueden incluir lo siguiente:

* Muchas de estas integraciones integradas están disponibles sin coste adicional. (Otros requieren una compra adicional).
* Las integraciones integradas cubren muchas de las aplicaciones más comunes utilizadas por las empresas, como [!DNL Slack], [!DNL Google Drive]o [!DNL Adobe] productos como [!DNL Adobe Creative Cloud] o [!DNL Adobe Experience Manager] Recursos. Si su empresa ya utiliza estas aplicaciones, la integración se integrará sin problemas en el flujo de trabajo existente de los usuarios.
* Integración [!DNL Workfront] con una aplicación utilizada con frecuencia puede aumentar la adopción entre los usuarios.

>[!INFO]
>
>**Ejemplo:**
>
>Con la variable [!DNL Workfront for Microsoft Teams integration], puede recibir notificaciones en [!DNL Microsoft Teams] acerca de su [!DNL Workfront] elementos de trabajo. Sin salir [!DNL Microsoft Teams], puede realizar acciones como aprobar, comentar o cambiar el estado de los elementos de trabajo. Cualquier cambio que realice en los elementos de trabajo [!DNL Microsoft Teams] se reflejan en [!DNL Workfront] también.

Para obtener más información sobre las integraciones integradas, incluida una lista de las integraciones integradas actualmente disponibles, consulte [[!DNL Adobe Workfront] información general sobre integraciones integradas](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Aplicaciones OAuth2 personalizadas

Adobe [!DNL Workfront] los administradores pueden crear aplicaciones OAuth2 para su instancia de [!DNL Workfront], que permiten acceder a otras aplicaciones [!DNL Workfront]. Los usuarios pueden dar permiso a esas otras aplicaciones para acceder a sus [!DNL Workfront] datos. De este modo, puede integrar Workfront con las aplicaciones que elija, incluidas sus propias aplicaciones internas.

>[!NOTE]
>
>En el contexto de OAuth2, &quot;crear una aplicación&quot; se refiere al proceso de creación de este tipo de vínculo de acceso entre una aplicación y un servidor como Workfront.

Ventajas de crear una [!UICONTROL OAuth2] la solicitud podrá incluir lo siguiente:

* Los usuarios pueden utilizar estas integraciones directamente en [!DNL Workfront], similar a las integraciones integradas.
* Configuración o uso de un [!UICONTROL OAuth2] la aplicación no requiere conocimientos técnicos adicionales, como la familiaridad con el [!DNL Workfront] API.
* Su organización puede utilizar software que no se ofrezca como [!DNL Workfront] aplicación integrada. Aún puede integrar este software con [!DNL Workfront] mediante una [!UICONTROL OAuth2] , incluso si el software es propiedad de su organización.

Para obtener más información, consulte [Creación de aplicaciones OAuth2 para integraciones de Workfront](../administration-and-setup/configure-integrations/create-oauth-application.md).

## [!DNL Workfront] API

[!DNL Workfront] ofrece una API pública (interfaz de programación de aplicaciones) que le permite ampliar y mejorar su experiencia con Workfront. El objetivo de [!DNL Workfront] La API es simplificar la creación de sus propias integraciones con [!DNL Workfront] introduciendo una arquitectura compatible con REST que funciona a través de HTTP. La variable [!DNL Workfront] La API requiere conocimientos técnicos, pero es una herramienta muy eficaz para recuperar, crear y modificar datos. Puede personalizar las llamadas a la API para realizar funciones muy específicas.

Además, [!DNL Workfront] ofrece una API de suscripción de evento. Cuando se produce una acción en un [!DNL Workfront] objeto compatible con suscripciones de eventos, puede configurar [!DNL Workfront] para enviar una respuesta al punto final deseado. Esto significa que las aplicaciones de terceros pueden recibir actualizaciones de [!DNL Workfront] interacciones a través de la variable [!DNL Workfront] API poco después de que se produzcan.

Ventajas de usar la variable [!DNL Workfront] La API puede incluir lo siguiente:

* Puede usar la variable [!DNL Workfront] para conectarse a casi cualquier otro servicio web o aplicación que ofrezca una API pública. Por lo tanto, es posible integrar [!DNL Workfront] con casi cualquier servicio web o aplicación que desee utilizar.
* La variable [!DNL Workfront] La flexibilidad de API también se extiende al software propietario de su empresa. Puede usar y modificar [!DNL Workfront] datos de su propio software.
* Dado que las API son tan comunes al software, es probable que los desarrolladores internos estén familiarizados con ellas. [!DNL Workfront] utiliza una API completa de REST, el tipo de API más común, lo que facilita aún más a los desarrolladores la actualización rápida.

>[!INFO]
>
>**Ejemplo:**
>
>La siguiente llamada de API coloca un comentario en el flujo de actualización de la tarea con el ID especificado.
>
>
```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Para obtener más información sobre la variable [!DNL Workfront] API, consulte [Conceptos básicos de API](../wf-api/general/api-basics.md).

Para obtener más información sobre las suscripciones a eventos, consulte [API de suscripción de evento](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] permite automatizar flujos de trabajo. Con la variable [!DNL Workfront Fusion for Work Automation and Integration] licencia, puede crear estas automatizaciones en varias aplicaciones y servicios web, creando escenarios en los que las aplicaciones trabajan juntas para ejecutar una tarea. Un escenario es una representación visual de la tarea o el flujo de trabajo que se crea mediante módulos, que son tareas discretas como &quot;Descargar un documento&quot; o &quot;Crear un proyecto&quot;. Los módulos se agrupan para definir el flujo de trabajo y este se ejecuta automáticamente cuando se cumple una condición de déclencheur.

Ventajas para [!DNL Workfront Fusion] puede incluir lo siguiente:

* [!DNL Workfront Fusion] no requiere tantos conocimientos técnicos como la API, ya que la interfaz visual ayuda a comprender y configurar el flujo de trabajo. Esto significa que puede ser utilizado por personas ajenas a un equipo de desarrollo, lo que puede ahorrar tiempo y dinero a su organización.
* Since [!DNL Workfront Fusion] funciona a través de la API de , puede acceder a la mayoría de las aplicaciones y servicios web. Muchas aplicaciones tienen módulos para realizar llamadas a la API, o puede usar los módulos HTTP, SOAP o JSON para interactuar con servicios web que no tengan una [!DNL Workfront Fusion] conector.

>[!INFO]
>
>**Ejemplo:**
>
>Lo siguiente [!DNL Workfront] módulo en [!DNL Workfront Fusion] está configurado para agregar un comentario al proyecto seleccionado. Una vez ejecutado el módulo, el comentario se puede ver en el flujo de actualización del proyecto en Workfront.
>
>![](assets/fusion-example-comment-350x416.png)

Para obtener más información, consulte [!DNL Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md).
