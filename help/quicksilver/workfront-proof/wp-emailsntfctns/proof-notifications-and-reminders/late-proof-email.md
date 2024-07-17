---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Correo electrónico de prueba tardía
description: El correo electrónico de prueba tardía se envía a los destinatarios cuando una prueba está cerca del plazo o alcanza este. Estos tipos de correos electrónicos no se pueden deshabilitar en un nivel de prueba, pero se pueden configurar en la cuenta y en el nivel de configuración personal del usuario.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!UICONTROL Correo electrónico de revisión tardía]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

El correo electrónico [!UICONTROL Prueba tardía] se envía a los destinatarios cuando una prueba está cerca del plazo o llega a este. Estos tipos de correos electrónicos no se pueden deshabilitar en un nivel de prueba, pero se pueden configurar en la cuenta y en el nivel de configuración personal del usuario.

* [!UICONTROL Los mensajes de correo electrónico de prueba tardía] se envían automáticamente a los revisores cuando una prueba alcanza su fecha límite y no se han tomado todas las revisiones o decisiones.

  Estos correos electrónicos están habilitados de forma predeterminada y no se pueden ajustar para todas las cuentas, pero los usuarios pueden deshabilitarlos en sus Valores predeterminados de revisión.

* Los correos electrónicos en riesgo se envían a los revisores cuando una prueba está cerca del plazo. Están deshabilitadas de manera predeterminada y se pueden habilitar en [!UICONTROL Configuración de la cuenta]. Una vez activados, también se pueden ajustar en [!UICONTROL Valores predeterminados de revisión].

Estas notificaciones no se pueden personalizar.

Las personas a las que se notificará son:

* El Propietario, solo cuando la alerta [!UICONTROL Correo electrónico] cuando las pruebas están atrasadas se comprueba en los [!UICONTROL Valores predeterminados de revisión del propietario].
* Cualquier aprobador que aún no haya tomado una decisión sobre la prueba. Para obtener información acerca de las decisiones, vea [Tomar una decisión sobre una prueba en el visor de revisión](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>Si las notificaciones por correo electrónico están deshabilitadas como predeterminadas en [!UICONTROL Configuración de la cuenta], no se enviarán correos electrónicos de [!UICONTROL prueba tardía] aunque los revisores y aprobadores aún no hayan enviado sus comentarios y decisiones. También puede deshabilitar [!UICONTROL revisiones tardías] correos electrónicos en los valores predeterminados de revisiones.

Tenga en cuenta lo siguiente sobre las notificaciones de prueba:

* Su administrador de [!DNL Workfront] o [!DNL Workfront Proof] puede incluir el logotipo de su organización en sus notificaciones por correo electrónico, tal como se explica en [Marca el [!DNL Workfront Proof] sitio](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).
* Si necesita compartir varias pruebas con los mismos revisores y no desea que reciban varios correos electrónicos, puede cargarlas al mismo tiempo. Todos los revisores reciben un correo electrónico que detalla todas las pruebas e incluye una URL personal para cada prueba.

  >[!NOTE]
  >
  >El creador de las pruebas recibe un correo electrónico [!UICONTROL Prueba realizada] independiente para cada una de las pruebas creadas. Para obtener más información, consulte [El [!UICONTROL correo electrónico que se hizo la revisión]](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md).

* Si usted o los revisores no reciben la notificación por correo electrónico esperada, consulte [Configurar [!DNL Workfront Proof] correos electrónicos para evitar filtros de correo no deseado](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
