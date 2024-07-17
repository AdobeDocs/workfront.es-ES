---
content-type: reference
product-area: workfront-integrations
keywords: nativo,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Métodos de integración de Adobe Workfront
description: Puede integrar [!DNL Adobe Workfront] con aplicaciones de terceros. Estas integraciones pueden ampliar la utilidad de  [!DNL Workfront]  y adaptarla a las necesidades de su organización. Puede utilizar cualquiera o todas estas integraciones, según cuál sea más útil para una tarea determinada.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 328d3a8d16ace22100d86efc127874d7edd6cb6d
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Métodos de integración de Adobe Workfront

Puede integrar [!DNL Adobe Workfront] con aplicaciones de terceros, así como otros [!DNL Adobe] productos. Estas integraciones pueden ampliar la utilidad de [!DNL Workfront] y adaptarla a las necesidades de su organización. Puede utilizar cualquiera o todas estas integraciones, según cuál sea más útil para una tarea determinada.

## Integraciones integradas

Workfront proporciona varias integraciones que puede configurar directamente desde Workfront o desde otra aplicación instalando el complemento de Workfront para esa aplicación. Estas integraciones integradas cubren muchos casos de uso comunes y se centran en ampliar y conectar las experiencias de los usuarios para los usuarios finales.

Las integraciones integradas de Workfront se centran principalmente en la productividad personal y la colaboración. Estas integraciones reducen las interrupciones en el flujo de trabajo de un usuario individual, lo que le permite recibir notificaciones de Workfront, acceder a información y actuar en elementos de trabajo de Workfront sin salir de la aplicación integrada.

Las ventajas de las integraciones integradas pueden incluir las siguientes:

* Muchas de estas integraciones integradas están disponibles sin coste adicional. (Otros requieren una compra adicional).
* Las integraciones integradas cubren muchas de las aplicaciones más comunes que usan las empresas, como [!DNL Slack], [!DNL Google Drive] o [!DNL Adobe] productos como [!DNL Adobe Creative Cloud] o [!DNL Adobe Experience Manager] Assets. Si su empresa ya utiliza estas aplicaciones, la integración se realizará sin problemas en el flujo de trabajo existente de los usuarios.
* Al integrar [!DNL Workfront] con una aplicación usada con frecuencia, puede aumentar la adopción entre los usuarios.

>[!INFO]
>
>**Ejemplo:**
>
>Con [!DNL Workfront for Microsoft Teams integration], puede recibir notificaciones en [!DNL Microsoft Teams] sobre sus [!DNL Workfront] elementos de trabajo. Sin salir de [!DNL Microsoft Teams], puede realizar acciones como aprobar, comentar o cambiar el estado de los elementos de trabajo. Cualquier cambio que realice en los elementos de trabajo de [!DNL Microsoft Teams] también se reflejará en [!DNL Workfront].

Para obtener más información acerca de las integraciones integradas, incluida una lista de las integraciones integradas disponibles actualmente, consulte [[!DNL Adobe Workfront] información general sobre las integraciones integradas](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Aplicaciones OAuth2 personalizadas

Adobe [!DNL Workfront] los administradores pueden crear aplicaciones OAuth2 para su instancia de [!DNL Workfront], que permiten que otras aplicaciones tengan acceso a [!DNL Workfront]. Los usuarios pueden dar permiso a esas otras aplicaciones para tener acceso a sus datos de [!DNL Workfront]. De este modo, puede integrar Workfront con las aplicaciones de su elección, incluidas las aplicaciones internas.

>[!NOTE]
>
>En el contexto de OAuth2, &quot;creación de una aplicación&quot; hace referencia al proceso de creación de este tipo de vínculo de acceso entre una aplicación y un servidor como Workfront.

Las ventajas de crear una aplicación [!UICONTROL OAuth2] pueden incluir las siguientes:

* Los usuarios pueden usar estas integraciones directamente en [!DNL Workfront], de forma similar a las integraciones integradas.
* Configurar o usar una aplicación [!UICONTROL OAuth2] no requiere conocimientos técnicos adicionales, como estar familiarizado con la API [!DNL Workfront].
* Su organización puede utilizar software que no se ofrece como aplicación integrada de [!DNL Workfront]. Aún puede integrar este software con [!DNL Workfront] mediante una aplicación [!UICONTROL OAuth2], aunque el software pertenezca a su organización.

Para obtener más información, consulte [Crear aplicaciones OAuth2 para integraciones de Workfront](../administration-and-setup/configure-integrations/create-oauth-application.md).

## API [!DNL Workfront]

[!DNL Workfront] ofrece una API pública (interfaz de programación de aplicaciones) que le permite ampliar y mejorar su experiencia con Workfront. El objetivo de la API [!DNL Workfront] es simplificar la creación de sus propias integraciones con [!DNL Workfront] mediante la introducción de una arquitectura REST-ful que funcione a través de HTTP. La API [!DNL Workfront] requiere algunos conocimientos técnicos, pero es una herramienta muy eficaz para recuperar, crear y modificar datos. Puede personalizar las llamadas a la API para realizar funciones muy específicas.

Además, [!DNL Workfront] ofrece una API de suscripción a evento. Cuando se produce una acción en un objeto [!DNL Workfront] compatible con las suscripciones de evento, puede configurar [!DNL Workfront] para que envíe una respuesta al extremo deseado. Esto significa que las aplicaciones de terceros pueden recibir actualizaciones de las interacciones de [!DNL Workfront] a través de la API [!DNL Workfront] poco después de que se produzcan.

Las ventajas de usar la API [!DNL Workfront] pueden incluir las siguientes:

* Puede usar la API [!DNL Workfront] para conectarse a casi cualquier otro servicio web o aplicación que ofrezca una API pública. Por lo tanto, es posible integrar [!DNL Workfront] con casi cualquier servicio web o aplicación que desee utilizar.
* La flexibilidad de la API [!DNL Workfront] también se extiende al software propietario de su empresa. Puede usar y modificar los datos de [!DNL Workfront] desde su propio software.
* Dado que las API son tan comunes en el software, es probable que los desarrolladores internos estén familiarizados con ellas. [!DNL Workfront] usa una API REST-ful, el tipo de API más común, lo que facilita aún más a los desarrolladores la tarea de ponerse al día rápidamente.

>[!INFO]
>
>**Ejemplo:**
>
>La siguiente llamada de API coloca un comentario en el flujo de actualización de la tarea con el ID especificado.
>
>```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Para obtener más información acerca de la API [!DNL Workfront], consulte [Conceptos básicos de la API](../wf-api/general/api-basics.md).

Para obtener más información sobre las suscripciones a eventos, consulte [API de suscripción a eventos](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] le permite automatizar flujos de trabajo. Con la licencia [!DNL Workfront Fusion for Work Automation and Integration], puede crear esas automatizaciones en varias aplicaciones y servicios web, creando escenarios donde las aplicaciones trabajen juntas para ejecutar una tarea. Un escenario es una representación visual de la tarea o del flujo de trabajo creado mediante módulos, que son tareas discretas como &quot;Descargar un documento&quot; o &quot;Crear un proyecto&quot;. Los módulos se encadenan para definir el flujo de trabajo, que se ejecuta automáticamente cuando se cumple una condición de déclencheur.

Entre las ventajas de [!DNL Workfront Fusion] se incluyen las siguientes:

* [!DNL Workfront Fusion] no requiere tantos conocimientos técnicos como la API, ya que la interfaz visual ayuda a comprender y configurar el flujo de trabajo. Esto significa que puede ser utilizado por individuos fuera de un equipo de desarrollo, lo que puede ahorrar tiempo y dinero a su organización.
* Dado que [!DNL Workfront Fusion] funciona a través de la API, puede acceder a la mayoría de las aplicaciones y servicios web. SOAP Muchas aplicaciones tienen módulos para realizar llamadas API, o bien puede utilizar los módulos HTTP, o JSON para interactuar con servicios web que no tienen un conector [!DNL Workfront Fusion] dedicado.

>[!INFO]
>
>**Ejemplo:**
>
>El siguiente módulo [!DNL Workfront] de [!DNL Workfront Fusion] está configurado para agregar un comentario al proyecto seleccionado. Una vez ejecutado el módulo, el comentario es visible en el flujo de actualización del proyecto en Workfront.
>
>![](assets/fusion-example-comment-350x416.png)

Para obtener más información acerca de [!DNL Workfront Fusion], vea [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md).
