---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Metadatos de conexión en Adobe Workfront Fusion
description: Adobe Workfront Fusion requiere una licencia Adobe Workfront Fusion además de una licencia Adobe Workfront.
author: Becky
feature: Workfront Fusion
source-git-commit: 3a7983279a38c30cb58078d129ea22dee137d9a5
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Metadatos de conexión en Adobe Workfront Fusion

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requiere un [!DNL Adobe Workfront Fusion] además de una licencia de [!DNL Adobe Workfront] licencia.

No todas las conexiones son iguales. Comprender las diferencias entre conexiones es muy importante para conocer su contexto empresarial. Fusion utiliza metadatos para identificar atributos importantes de una conexión.

Los metadatos de la conexión se pueden establecer al crear una nueva conexión. Estos atributos se encuentran en el mismo cuadro de diálogo utilizado para configurar una conexión:

![Metadatos de conexión](assets/connection-metadata-setup.png)

Los usuarios de Fusion pueden ver y editar conexiones desde el área Conexiones.

![Metadatos de conexión en el área Conexiones](assets/connections-area-metadata.png)

## Tipo de entorno

Las conexiones Fusion pueden ser utilizadas tanto por los sistemas de producción como por los sistemas que no son de producción. Conocer la diferencia es muy importante para proteger los entornos de producción. Tenga en cuenta que el tipo de entorno, al igual que otros metadatos de conexión, se utiliza únicamente con fines informativos. Los usuarios siguen siendo responsables de configurar este atributo con precisión.

## Tipo de autenticación

Las conexiones de Fusion se pueden utilizar tanto para cuentas de servicio como para cuentas personales. Las cuentas de servicio se utilizan para la autenticación cuando un escenario se automatiza como Fusion. Las cuentas personales son una autenticación basada en una persona específica. El tipo de autenticación que se use depende de los requisitos del escenario. Las cuentas personales deben utilizarse para acciones automatizadas de los usuarios. Por ejemplo, si un escenario de Fusion automatiza la aprobación por parte de una persona específica, el tipo de autenticación debe ser para esa persona. De lo contrario, Fusion actúa como Fusion y el tipo debe ser &quot;Cuenta de servicio&quot;.

Tenga en cuenta que, al igual que otros metadatos de conexión, solo se utiliza con fines informativos. Los usuarios siguen siendo responsables de configurar este atributo de forma manual con precisión.

Para obtener más información sobre los tipos de autenticación, consulte [Autenticación](https://developer.adobe.com/developer-console/docs/guides/authentication/) en la Guía de autenticación de Adobe.



