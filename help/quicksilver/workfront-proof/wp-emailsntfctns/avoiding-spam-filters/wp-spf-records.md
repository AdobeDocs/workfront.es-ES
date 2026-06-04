---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Registros de Workfront Proof SPF
description: Workfront Proof envía notificaciones por correo electrónico a los revisores desde una dirección de correo electrónico de Workfront Proof como notification@proofing.yourdomain.com. Para garantizar que los servidores de correo de los destinatarios confíen en todas las notificaciones de correo electrónico de Workfront Proof, debe configurar un registro de  [!DNL Sender Policy] Framework (SPF) para el dominio personalizado conectado a la cuenta  [!DNL Workfront Proof] por ejemplo, proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
TQID: https://experienceleague.adobe.com/LTZzs99Zzsn5dbOlu4wP1coyJAMDnnCZZ1pTTbEjT24
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 181
ht-degree: 100%

---

# Registros de Workfront Proof SPF

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] envía notificaciones por correo electrónico a los revisores desde una dirección de correo electrónico de [!DNL Workfront Proof], como notification@proofing.yourdomain.com. Para garantizar que los servidores de correo de los destinatarios confíen en todas las notificaciones de correo electrónico de [!DNL Workfront Proof], debe configurar un registro de [!UICONTROL Marco de directivas de remitente] (SPF) para el dominio personalizado conectado a la cuenta de [!DNL Workfront Proof] (por ejemplo, **proofing.yourdomain.com**).

Para configurar un registro de SPF, deberá incluir el registro de SPF utilizado para nuestro dominio principal.

1. Añada una entrada **[!UICONTROL DNS TXT]** para su dominio con el siguiente valor:

   `v=spf1 a:mx.proofhq.com -all`

   El administrador de correo electrónico o el personal de TI pueden ayudarle a configurarlo.

   >[!TIP]
   >
   >Puede usar la herramienta gratuita en [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) para revisar registros SPF de [!DNL Workfront].
