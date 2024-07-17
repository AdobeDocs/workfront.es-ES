---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Cuando no se acepta un correo electrónico autenticado debido a la política DMARC del dominio
description: Si un correo electrónico enviado desde el sistema  [!DNL Workfront] no se acepta debido a la directiva DMARC del dominio, el administrador de correo electrónico puede solucionar el problema configurando el sistema de correo electrónico para permitir todos los correos electrónicos de workfront.com.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# No se aceptan correos electrónicos no autenticados debido a la política DMARC del dominio

## Problema

[Prueba] He recibido el siguiente correo electrónico de devolución:

550-5.7.1 El correo electrónico no autenticado de &quot;customer domain.com&quot; no se acepta debido a\
Directiva DMARC del dominio 550-5.7.1. Póngase en contacto con el administrador de &quot;customer domain.com&quot;\
Dominio 550-5.7.1 si se trata de un correo legítimo. Visite\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) para obtener más información sobre DMARC\
550 5.7.1 iniciativa.

## Solución

DMARC está configurado en el sistema de correo electrónico de su compañía y no forma parte de [!DNL Adobe Workfront]. Si recibe este correo electrónico, debe ponerse en contacto con el administrador de correo electrónico.

El administrador de correo electrónico debe configurar su sistema de correo electrónico para permitir/confiar en el correo electrónico de noreply@workfront.com o, preferiblemente, en todos los correos electrónicos de workfront.com.

Para obtener más información acerca de DMARC, consulte [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
