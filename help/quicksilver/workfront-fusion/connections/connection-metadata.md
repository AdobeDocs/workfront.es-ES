---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Metadatos de conexión en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: af260c63-3385-4d5c-abc2-d5c23175be40
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 78%

---

# Metadatos de conexión en Adobe Workfront Fusion

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Metadatos de conexión](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/connections/connection-metadata.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requiere una licencia de [!DNL Adobe Workfront Fusion] además de una licencia de [!DNL Adobe Workfront].

No todas las conexiones son iguales. Comprender las diferencias entre conexiones es muy importante para conocer su contexto empresarial. Fusion utiliza metadatos para identificar los atributos importantes de una conexión.

Los metadatos de la conexión se pueden establecer al crear una nueva conexión. Estos atributos se encuentran en el mismo cuadro de diálogo que sirve para configurar una conexión:

![Metadatos de conexión](assets/connection-metadata-setup.png)

Los usuarios de Fusion pueden ver y editar conexiones desde el área Conexiones.

![Metadatos de conexión en el área Conexiones](assets/connections-area-metadata.png)

## Tipo de entorno

Las conexiones de Fusion las pueden utilizar tanto los sistemas de producción como los sistemas que no son de producción. Conocer la diferencia es muy importante para proteger los entornos de producción. Tenga en cuenta que el tipo de entorno, al igual que otros metadatos de conexión, se utiliza únicamente con fines informativos. Los usuarios siguen siendo responsables de configurar este atributo con precisión.

## Tipo de autenticación

Las conexiones de Fusion se pueden utilizar tanto para cuentas de servicio como para cuentas personales. Las cuentas de servicio se utilizan para la autenticación cuando un escenario se automatiza como Fusion. Las cuentas personales son una autenticación basada en una persona específica. El tipo de autenticación que se use depende de los requisitos del escenario. Las cuentas personales deben utilizarse para las acciones automatizadas de los usuarios. Por ejemplo, si un escenario de Fusion automatiza la aprobación por parte de una persona específica, el tipo de autenticación debe ser para esa persona. De lo contrario, Fusion actúa como Fusion y el tipo debe ser &quot;Cuenta de servicio&quot;.

Tenga en cuenta que, al igual que otros metadatos de conexión, solo se utiliza con fines informativos. Los usuarios siguen siendo responsables de configurar este atributo de forma manual con precisión.

Para obtener más información sobre los tipos de autenticación, consulte [Autenticación](https://developer.adobe.com/developer-console/docs/guides/authentication/) en la Guía de autenticación de Adobe.
