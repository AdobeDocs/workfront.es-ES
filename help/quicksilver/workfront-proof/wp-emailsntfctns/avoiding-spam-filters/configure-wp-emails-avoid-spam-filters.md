---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Configurar  [!DNL Workfront Proof] correos electrónicos para evitar filtros de spam
description: '"El filtro de spam de su cliente de correo electrónico tiene un propósito importante: protegerle de correos electrónicos spam molestos y posiblemente maliciosos. Sin embargo, si no tiene la configuración correcta en el filtro de correo no deseado, no podrá ver los siguientes  [!DNL Workfront Proof] correos electrónicos importantes: notificaciones de prueba por correo electrónico, boletines informativos y comunicaciones especiales".'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Configurar [!DNL Workfront Proof] correos electrónicos para evitar filtros de spam

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

El filtro de correo no deseado de su cliente de correo electrónico tiene un propósito importante: protegerle de mensajes de correo electrónico no deseado molestos y posiblemente malintencionados. Sin embargo, si no tiene la configuración correcta en el filtro de correo no deseado, puede impedir que vea los siguientes [!DNL Workfront Proof] correos electrónicos importantes: notificaciones de prueba por correo electrónico, boletines informativos y comunicaciones especiales.

Para asegurarse de que los mensajes de correo electrónico de [!DNL Workfront Proof] siempre se enruten a la bandeja de entrada en lugar de a la carpeta de correo no deseado, debe agregar lo siguiente a la lista de permitidos:

* [!DNL Workfront Proof] servidor de correo: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] direcciones de correo electrónico &quot;[!UICONTROL de]&quot; (por ejemplo, notification@proofhq.com)

Para obtener más información acerca de las direcciones URL que se agregarán a la lista de permitidos, consulte [Configuración de la lista de permitidos del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) en el artículo [Configuración de la lista de permitidos del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] direcciones de correo electrónico &quot;[!UICONTROL de]&quot;

Según el tipo de cliente de correo electrónico, es posible que deba agregar [!DNL Workfront Proof] direcciones de correo electrónico &quot;[!UICONTROL de]&quot; a una de las siguientes direcciones para evitar que el filtro de correo no deseado enrute los mensajes de correo electrónico a la carpeta de correo no deseado en el futuro:

* Su lista de contactos
* Su lista de [!UICONTROL remitentes seguros]
* Un filtro que crea para enviar correos electrónicos desde esas direcciones a la bandeja de entrada

También es posible que tenga que eliminar cualquier correo electrónico existente de [!DNL Workfront Proof] de su carpeta de correo no deseado y comprobar si alguna de las direcciones &quot;[!UICONTROL de]&quot; está en la lista de direcciones bloqueadas. Esta página de ayuda enumera las direcciones &quot;[!UICONTROL de]&quot; de [!DNL Workfront Proof] y muestra cómo agregarlas al filtro de correo no deseado en los siguientes clientes de correo electrónico:

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Si tiene alguna pregunta sobre un procedimiento descrito aquí, consulte la ayuda de su cliente de correo electrónico.

Para obtener más información, consulte [Configuración de correo no deseado para clientes de correo electrónico comunes](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## Las [!DNL Workfront Proof] direcciones de correo electrónico &quot;[!UICONTROL de]&quot; que se van a copiar

Para asegurarse de que los correos electrónicos de [!DNL Workfront Proof] lleguen a la bandeja de entrada, deberá agregar dos direcciones de correo electrónico de [!DNL Workfront Proof] por separado al filtro de correo no deseado del cliente de correo electrónico:

* La dirección de soporte general [!DNL support@proofhq.com], desde la cual [!DNL Workfront Proof] envía muchas comunicaciones por correo electrónico
* Una dirección de notificación desde la cual [!DNL Workfront Proof] envía correos electrónicos de notificación de prueba al creador de la prueba y a los revisores con vínculos a la prueba. Puede ser una dirección general, notification@support.proofhq.com o una dirección específica si tiene un subdominio personalizado o un dominio de etiqueta blanca.

Para agregar [!DNL Workfront Proof] direcciones &quot;[!UICONTROL from]&quot; al filtro del cliente de correo electrónico:

1. Copie la dirección de correo electrónico general [!DNL Workfront Proof] de soporte &quot;[!UICONTROL from]&quot; (support@proofhq.com) y péguela en el campo indicado para su cliente de correo electrónico.
1. Copie una de las siguientes [!DNL Workfront Proof] direcciones de correo electrónico &quot;[!UICONTROL de]&quot; y péguela POR SEPARADO en el campo indicado para su cliente de correo electrónico:

   * notification@support.proofhq.com si NO tiene un subdominio personalizado o un dominio de etiqueta blanca
   * notification@yoursubdomain.proofhq.com si tiene un subdominio personalizado; sustituya el nombre de subdominio en esta dirección
   * notification@yoursubdomain.yourdomain.com si tiene un dominio de marca blanca; sustituya su nombre de subdominio y nombre de dominio en esta dirección

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
