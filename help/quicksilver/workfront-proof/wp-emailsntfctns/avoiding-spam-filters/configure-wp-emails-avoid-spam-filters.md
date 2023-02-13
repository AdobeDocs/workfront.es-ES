---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Configurar [!DNL Workfront Proof] correos electrónicos para evitar filtros de correo no deseado
description: '"El filtro de correo no deseado de su cliente de correo electrónico tiene un propósito importante: protegerle de los correos electrónicos no deseados y posiblemente malintencionados. Pero, si no tiene la configuración correcta en el filtro de correo no deseado, puede evitar ver lo siguiente importante [!DNL Workfront Proof] correos electrónicos: prueba de notificaciones por correo electrónico, boletines informativos y comunicaciones especiales".'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Configurar [!DNL Workfront Proof] correos electrónicos para evitar filtros de correo no deseado

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

El filtro de correo no deseado de su cliente de correo electrónico tiene un propósito importante: protegerle de los correos electrónicos no deseados y posiblemente malintencionados. Pero, si no tiene la configuración correcta en el filtro de correo no deseado, puede evitar ver lo siguiente importante [!DNL Workfront Proof] correos electrónicos: probar notificaciones por correo electrónico, boletines informativos y comunicaciones especiales.

Para asegurarse de que su [!DNL Workfront Proof] Los correos electrónicos siempre se dirigen a la bandeja de entrada en lugar de a la carpeta de correo no deseado, debe añadir lo siguiente a la lista de permitidos :

* [!DNL Workfront Proof] servidor de correo: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; direcciones de correo electrónico (por ejemplo, notification@proofhq.com)

Para obtener más información sobre las direcciones URL que se agregarán a la lista de permitidos, consulte [Configurar la lista de permitidos del cortafuegos](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) en el artículo [Configurar la lista de permitidos del cortafuegos](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; direcciones de correo electrónico

Según el tipo de cliente de correo electrónico, es posible que tenga que agregar [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; direcciones de correo electrónico a una de las siguientes para evitar que el filtro de correo no deseado dirija sus correos electrónicos a su carpeta de correo no deseado en el futuro:

* Su lista de contactos
* Su [!UICONTROL Remitentes seguros] list
* Un filtro que crea para enviar correos electrónicos de esas direcciones a la bandeja de entrada

También es posible que tenga que eliminar cualquier [!DNL Workfront Proof] correos electrónicos de su carpeta de correo no deseado y compruebe si alguno de los[!UICONTROL from]&quot; las direcciones están en la lista de direcciones bloqueadas. Esta página de ayuda enumera las [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; y muestra cómo agregarlos al filtro de correo no deseado en los siguientes clientes de correo electrónico:

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Si tiene alguna pregunta sobre un procedimiento descrito aquí, consulte la ayuda de su cliente de correo electrónico.

Para obtener más información, consulte [Configuración de correo no deseado para clientes de correo electrónico comunes](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## La variable [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; direcciones de correo electrónico para copiar

Para asegurarse de que su [!DNL Workfront Proof] los correos electrónicos llegan a la bandeja de entrada; deberá agregar dos [!DNL Workfront Proof] direcciones de correo electrónico por separado para el filtro de correo no deseado de su cliente de correo electrónico:

* La dirección general de apoyo, [!DNL support@proofhq.com], a partir de las cuales [!DNL Workfront Proof] envía muchas comunicaciones por correo electrónico
* Una dirección de notificación desde la que [!DNL Workfront Proof] envía correos electrónicos de notificación de prueba al creador de pruebas y a los revisores con vínculos a la prueba. Puede ser una dirección general, notification@support.proofhq.com o una dirección específica si tiene un subdominio personalizado o un dominio de etiqueta blanca.

Para agregar [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; al filtro de su cliente de correo electrónico:

1. Copiar el general [!DNL Workfront Proof] soporte &quot;[!UICONTROL from]&quot; dirección de correo electrónico (support@proofhq.com) y péguela en el campo indicado para su cliente de correo electrónico.
1. Copie el que corresponda de la siguiente manera [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; direcciones de correo electrónico y péguelas SEPARADAMENTE en el campo indicado para su cliente de correo electrónico:

   * notification@support.proofhq.com si NO tiene un subdominio personalizado o un dominio de etiqueta blanca
   * notification@yoursubdomain.proofhq.com si tiene un subdominio personalizado; sustituya su nombre de subdominio por esta dirección
   * notification@yoursubdomain.yourdomain.com si tiene un dominio de etiqueta blanca; sustituya el nombre de subdominio y el nombre de dominio por esta dirección

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
