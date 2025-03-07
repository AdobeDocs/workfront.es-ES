---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Configurar configuración de prueba en [!DNL Workfront Proof]
description: Puede configurar una prueba que esté creando o editando en pruebas.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ca379054-4737-4796-a812-f2ec38b437ba
source-git-commit: 5635906462cf838c3ca162cb47b16f157e6a66f6
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 94%

---

# Configurar configuración de prueba en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Puede configurar una prueba que esté creando o editando de cualquiera de las siguientes maneras:

>[!NOTE]
>
>Puede configurar estos ajustes para todas las pruebas nuevas que cree. Para obtener más información, consulte.

## Bloquear la prueba cuando se tome la última decisión

Puede establecer que un estado de revisión se bloquee cuando el aprobador final tome su decisión. Esto resulta útil si desea asegurarse de que los revisores no puedan volver a la revisión y añadir comentarios adicionales o cambiar sus decisiones.

1. Cree una nueva prueba, tal como se describe en [Generar revisiones en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   O\
   Abra la página de detalles de prueba de una prueba existente, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para una nueva prueba, en **[!UICONTROL Configuración de prueba]**, seleccione **[!UICONTROL Bloquear prueba cuando se tomen todas las decisiones necesarias]**.\
   O\
   Para una prueba existente, en **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Bloquear la prueba cuando se tomen todas las decisiones]**.

Para obtener información acerca de las decisiones, consulte [Tomar una decisión sobre una prueba en el visor de pruebas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

## Requerir inicio de sesión para todos los usuarios que revisan la prueba

Una de las mejores cosas de [!DNL Workfront Proof] es que cualquiera puede revisar una prueba; no necesita tener su propio [!DNL Workfront Proof] para hacerlo. Los destinatarios reciben un correo electrónico con una URL personal que los lleva directamente a la página de prueba, sin que tengan que iniciar sesión en [!DNL Workfront Proof].

Sin embargo, si necesita niveles más altos de seguridad para el proceso de revisión y aprobación, puede utilizar requerir el inicio de sesión en la prueba. Esto significa que solamente se pueden añadir [!DNL Workfront Proof] usuarios a la prueba. Y deben introducir su correo electrónico y contraseña antes de poder acceder a él.

>[!NOTE]
>
>* *Para que alguien inicie sesión en la prueba (cuando el inicio de sesión requerido se ha habilitado), debe haber sido añadido a la prueba.*
>* *Si el inicio de sesión necesario está habilitado, las suscripciones no se pueden habilitar.*

Para requerir el inicio de sesión para todos los usuarios que revisen la prueba:

1. Cree una nueva prueba, tal como se describe en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   O\
   Abra la página de detalles de una prueba existente, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para una nueva prueba, en **[!UICONTROL Configuración de prueba]**, seleccione **[!UICONTROL Requerir inicio de sesión]**.\
   O\
   Para una prueba existente, en **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Se requiere inicio de sesión]**.

## Requerir solo una decisión para la prueba

Esta configuración es útil en casos en los que solo necesita una persona de un grupo, departamento o compañía para tomar una decisión sobre la prueba.

Incluso si asigna la función de aprobador o revisor y aprobador a varias personas, una vez que una persona tome una decisión sobre una prueba, el estado de la prueba se actualizará (según la decisión tomada). Para obtener más información sobre el estado de prueba, consulte [Ver el progreso y el estado de una prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)

1. Cree una nueva prueba, tal como se describe en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   O\
   Abra la página de detalles de una prueba existente, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para una nueva prueba, en **[!UICONTROL Flujo de trabajo]**, seleccione **[!UICONTROL Requerir solo una decisión para esta fase]**.\
   O\
   Para una prueba existente, en **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Solo se requiere una decisión]**.

Para obtener información acerca de las decisiones, consulte [Tomar una decisión sobre una prueba en el visor de pruebas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

## Requerir que las decisiones se firmen electrónicamente

Puede requerir una firma electrónica de cualquier revisor que tome la decisión sobre la prueba de proporcionar su correo electrónico y contraseña. Cuando un revisor toma una decisión, aparece una indicación pidiéndole que introduzca su correo electrónico y contraseña, y que confirme su decisión. Para obtener más información, consulte [Comprender las firmas electrónicas en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)

1. Cree una nueva prueba, tal como se describe en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   O\
   Abra la página de detalles de prueba de una prueba existente, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para una nueva prueba, en **[!UICONTROL Configuración de prueba]**, seleccione **[!UICONTROL Requerir que las decisiones se firmen electrónicamente]**.\
   O\
   Para una prueba existente, en **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Requerir que las decisiones se firmen electrónicamente]**.

Para obtener información acerca de las decisiones, consulte [Configurar las opciones de decisión de aprobación en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## Impedir que los usuarios descarguen el archivo original

Puede impedir que los revisores de una prueba descarguen el archivo original a partir del cual se creó la prueba.

1. Cree una nueva prueba, tal como se describe en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   O\
   Abra la página de detalles de prueba de una prueba existente, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para una nueva prueba, en **[!UICONTROL Configuración de prueba]**, anule la selección **[!UICONTROL Descargar archivo original]**.\
   O\
   Para una prueba existente, en **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Descargar archivo original]**.

## Permitir que otros usuarios se suscriban a la prueba

La suscripción es una configuración avanzada que funciona con la URL de prueba y la prueba mínima.

De forma predeterminada, las personas que no se hayan añadido específicamente a la prueba y estén utilizando la URL de prueba o la prueba mínima para acceder a ella solo pueden ver la prueba en modo de solo lectura. Las personas que ya son revisoras de la prueba pueden iniciar sesión con su dirección de correo electrónico. Para obtener más información, consulte [Administrar funciones de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)

Al habilitar la suscripción en la revisión, los usuarios que no se hayan añadido explícitamente a la revisión pueden suscribirse a ella (es decir, añadirse a la revisión). A continuación, se les asignará la función y la alerta de correo electrónico que seleccione para ellos en la Configuración de suscripción.

Si se ha habilitado la suscripción en una revisión, los campos siguientes se activarán:

* **[!UICONTROL Función de suscriptor]**: esta es la función de prueba predeterminada que se asignará a todos los revisores que se suscriban a la prueba.
* **[!UICONTROL Configuración de alertas de correo electrónico para suscriptores]**: esta es la alerta de correo electrónico predeterminada que se asignará a todos los revisores que se suscriban a la revisión.
* **[!UICONTROL Se requiere acceso a la revisión por correo electrónico para]** - El suscriptor debe hacer clic en un enlace de un mensaje de correo electrónico para acceder a una revisión\
   Si selecciona esta opción, la persona suscrita no tendrá acceso inmediato a la prueba, pero recibirá un vínculo a la prueba en un correo electrónico. El propósito de la validación del suscriptor es garantizar que la persona haya introducido una dirección de correo electrónico correcta a la que tenga acceso.



Ver también [Suscribirse a una prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)

Para permitir que otros usuarios se suscriban a una prueba:

1. Cree una nueva prueba, tal como se describe en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   O\
   Abra la página de detalles de prueba de una prueba existente, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para una nueva prueba, en **[!UICONTROL Configuración de prueba]**, anule la selección **[!UICONTROL Suscribirse a la prueba mediante una URL pública o un código incrustado]**.\
   O\
   Para una prueba existente, en **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Suscripción]**.
