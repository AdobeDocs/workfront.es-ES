---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: No se aceptan correos electrónicos no autenticados debido a la directiva DMARC del dominio
description: Si un correo electrónico enviado desde el sistema  [!DNL Workfront]  no se acepta debido a la directiva DMARC del dominio, el administrador del correo electrónico puede solucionar el problema configurando el sistema de correo electrónico para permitir todos los correos electrónicos de workfront.com.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
TQID: https://experienceleague.adobe.com/f44Wkid-gwfXgHKmSKa6oevhN5jA6720JTlOcH8kJKY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 177
ht-degree: 94%

---

# No se aceptan correos electrónicos no autenticados debido a la política DMARC del dominio

## Problema

[Prueba] Me han devuelto el siguiente correo electrónico:

550-5.7.1 El correo electrónico no autenticado de &quot;customer domain.com&quot; no se acepta debido a\
550-5.7.1 la directiva DMARC del dominio. Póngase en contacto con el administrador del dominio &quot;customer domain.com&quot;\
550-5.7.1 si se trata de un correo legítimo. Visite\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) para obtener más información sobre la iniciativa\
550 5.7.1 de DMARC.

## Solución

DMARC está configurado en el sistema de correo electrónico de su compañía y no forma parte de [!DNL Adobe Workfront]. Si recibe este correo electrónico, debe ponerse en contacto con el administrador del correo electrónico.

El administrador del correo electrónico debe configurar su sistema de correo electrónico para permitir/confiar en el correo electrónico de noreply@workfront.com o, preferiblemente, en todos los correos electrónicos de workfront.com.

Para obtener más información sobre DMARC, consulte [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
