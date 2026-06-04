---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Correo electrónico de prueba atrasada
description: El correo electrónico de prueba atrasada se envía a los destinatarios cuando una prueba está cerca del plazo o alcanza este. No es posible desactivar este tipo de correos electrónicos a nivel de prueba, pero se pueden configurar a nivel de cuenta y en la configuración personal del usuario.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
TQID: https://experienceleague.adobe.com/7mN20lz57PSto-MAK1EqBg19RdMwIjnEUnzEIEpNxvU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 403
ht-degree: 100%

---

# Correo electrónico de [!UICONTROL prueba atrasada]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

El correo electrónico de la [!UICONTROL Prueba atrasada] se envía a los destinatarios cuando una prueba está cerca de la fecha límite o llega a ella. No es posible desactivar este tipo de correos electrónicos a nivel de prueba, pero se pueden configurar a nivel de cuenta y en la configuración personal del usuario.

* [!UICONTROL Los mensajes de correo electrónico de prueba atrasada] se envían automáticamente a los revisores cuando una prueba alcanza su fecha límite y no se han tomado todas las revisiones o decisiones.

  Estos correos electrónicos están habilitados de forma predeterminada y no se pueden ajustar para todas las cuentas, pero los usuarios pueden deshabilitarlos en sus valores predeterminados de revisión.

* Los correos electrónicos en riesgo se envían a los revisores cuando una prueba está cerca del plazo. Están deshabilitadas de manera predeterminada y se pueden habilitar en [!UICONTROL Configuración de la cuenta]. Una vez habilitados, también se pueden ajustar en [!UICONTROL Valores predeterminados de revisión].

Estas notificaciones no se pueden personalizar.

Las personas a las que se notificará son:

* El Propietario, solo cuando la alerta [!UICONTROL Correo electrónico] cuando las pruebas están atrasadas se comprueba en los [!UICONTROL Valores predeterminados de revisión del propietario].
* Cualquier aprobador que aún no haya tomado una decisión sobre la prueba. Para obtener información acerca de las decisiones, consulte [Tomar una decisión sobre una prueba en el visor de revisión](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>Si las notificaciones por correo electrónico están deshabilitadas de forma predeterminada en la [!UICONTROL configuración de la cuenta], no se enviarán correos electrónicos de [!UICONTROL prueba atrasada], incluso si los revisores y aprobadores no han enviado aún sus comentarios y decisiones. También puede deshabilitar [!UICONTROL revisión atrasada] correos electrónicos en los valores predeterminados de revisiones.

Tenga en cuenta lo siguiente sobre las notificaciones de prueba:

* Su [!DNL Workfront] administrador o [!DNL Workfront Proof] administrador puede incluir el logotipo de su organización en las notificaciones por correo electrónico, como se explica en [Personalizar el [!DNL Workfront Proof] sitio](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).
* Si necesita compartir varias pruebas con los mismos revisores y no desea que reciban varios correos electrónicos, puede cargarlas al mismo tiempo. Todos los revisores reciben un correo electrónico que detalla todas las pruebas e incluye una URL personal para cada prueba.

  >[!NOTE]
  >
  >El creador de las pruebas recibe un correo electrónico [!UICONTROL Prueba realizada] independiente para cada una de las pruebas creadas. Para obtener más información, consulte [El correo electrónico de [!UICONTROL prueba realizada]](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md).

* Si usted o sus revisores no reciben una notificación por correo electrónico esperada, consulte [Configurar [!DNL Workfront Proof] correos electrónicos para evitar filtros de spam](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
