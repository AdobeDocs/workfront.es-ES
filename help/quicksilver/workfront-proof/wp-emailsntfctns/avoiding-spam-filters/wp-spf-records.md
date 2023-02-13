---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Registros de Workfront Proof SPF
description: Workfront Proof envía notificaciones por correo electrónico a los revisores desde una dirección de correo electrónico de Workfront Proof como notification@proofing.yourdomain.com. Para asegurarse de que los servidores de correo de los destinatarios confían en todas las notificaciones de correo electrónico de Workfront Proof, debe configurar un [!DNL Sender Policy] Registro de marco (SPF) para su dominio personalizado conectado al [!DNL Workfront Proof] (por ejemplo, proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Registros de Workfront Proof SPF

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] envía notificaciones por correo electrónico a los revisores desde un [!DNL Workfront Proof] dirección de correo electrónico como notification@proofing.yourdomain.com. Para garantizar que los servidores de correo de los destinatarios confíen en todo [!DNL Workfront Proof] notificaciones por correo electrónico, debe configurar un [!UICONTROL Marco de políticas del remitente] (SPF) registro para su dominio personalizado conectado al [!DNL Workfront Proof] (por ejemplo, **proofing.yourdomain.com**).

Para configurar un registro SPF, deberá incluir el registro SPF utilizado para nuestro dominio principal.

1. Agregue un **[!UICONTROL TXT de DNS]** para su dominio con el siguiente valor:

   `v=spf1 a:mx.proofhq.com -all`

   El administrador de correo electrónico o el personal de TI pueden ayudarle a configurarlo.

   >[!TIP]
   >
   >Puede utilizar la herramienta gratuita en [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) para revisar [!DNL Workfront] Registros SPF.
