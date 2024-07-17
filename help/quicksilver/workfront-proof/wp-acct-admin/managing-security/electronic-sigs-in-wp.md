---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Explicación de las firmas electrónicas en  [!DNL Workfront Proof]
description: Las firmas electrónicas le permiten mejorar la seguridad de sus pruebas y cumplir con los estándares del sector, como ISO.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: caff2a03-cccc-4779-9dcc-3362c527dcb9
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Explicación de las firmas electrónicas en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Las firmas electrónicas le permiten mejorar la seguridad de sus pruebas y cumplir con los estándares del sector, como ISO.

Esta configuración puede hacerse obligatoria o no obligatoria en el nivel de cuenta. Si es obligatorio de forma predeterminada, está habilitado en todas las pruebas creadas en su cuenta y no se puede deshabilitar en el nivel de prueba. Si esta configuración no es obligatoria de forma predeterminada, podrá habilitarla o deshabilitarla en el nivel de prueba.

Para obtener más información, consulte .

Cuando la configuración de firma electrónica está habilitada en una prueba, un cuadro de firma electrónica solicita a cualquier revisor que tome una decisión sobre la prueba que proporcione su correo electrónico y contraseña.

![Electronic_sig_required_box.png](assets/electronic-sig-required-box.png)

## Firmas electrónicas en la página [!UICONTROL Detalles de revisión]

Si un revisor toma su decisión al seleccionar su decisión en la página [!UICONTROL Detalles de la prueba] (1), aparecerá un cuadro emergente de [!UICONTROL Firma electrónica] en el que se le pedirá que introduzca sus detalles (2) y que confirme su decisión (3).

La ventana emergente mostrará el conjunto de mensajes predeterminado (si lo hay) y el revisor deberá introducir su correo electrónico y contraseña.

La ventana emergente [!UICONTROL Firma electrónica] aparecerá en el visor de revisiones y también en la página [!UICONTROL Detalles de la revisión] si el revisor decide tomar su decisión a partir de ese nivel.

![Firma_electrónica_-_Proof_Details.png](assets/electronic-signature---proof-details-350x146.png)

![Firma electrónica_-_Proof_Details_2.png](assets/electronic-signature---proof-details-2-350x148.png)

Si la opción [!UICONTROL Inicio de sesión único] está habilitada en la revisión, los detalles del correo electrónico y la contraseña no se mostrarán en la ventana emergente [!UICONTROL Firma electrónica] al tomar una decisión.

En su lugar, después de hacer clic en el botón [!UICONTROL Confirmar] (4) de esta ventana emergente, el revisor será redirigido a la página [!UICONTROL Inicio de sesión único].

Después de escribir sus credenciales de SSO, el revisor se redirigirá automáticamente a la página [!UICONTROL Detalles de la prueba] (o a [!UICONTROL Visor de pruebas] si la decisión se toma desde allí).

![Firma electrónica_SSO_-_Proof_Details_3.png](assets/electronic-signature-sso---proof-details-3-350x146.png)

>[!NOTE]
>
> Si la decisión está firmada electrónicamente, el **[!UICONTROL icono de firma]** (5) aparece junto a la decisión en la sección [!UICONTROL Flujo de trabajo] de la página [!UICONTROL Detalles de la prueba]. Si la decisión no es modificada por el revisor, sino por otra persona que tiene derechos de edición en la prueba, a esa persona no se le pedirá que firme electrónicamente la decisión y no habrá ningún icono de firma junto a la decisión (6).

![Electronic_Signature_icon.png](assets/electronic-signature-icon-350x52.png)Para obtener más información sobre el inicio de sesión único, consulte [Inicio de sesión único en Workfront Proof](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

Para obtener información sobre la página de detalles de revisión, consulte [Administrar detalles de revisión en [!DNL Workfront] Revisión](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
