---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Configure la configuración de prueba en [!DNL Workfront Proof]
description: 'Puede configurar una prueba que esté creando o editando de cualquiera de las siguientes maneras: EDITE ME.'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ca379054-4737-4796-a812-f2ec38b437ba
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 1%

---

# Configure la configuración de prueba en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Puede configurar una prueba que esté creando o editando de cualquiera de estas formas:

>[!NOTE]
>
>Puede configurar estos ajustes para todas las pruebas nuevas que cree. Para obtener más información, consulte .

## Bloquear la prueba cuando se tome la última decisión

Puede establecer un estado de prueba para que se bloquee cuando el Aprobador final tome su decisión. Esto resulta útil si desea asegurarse de que los revisores no puedan volver a la prueba y agregar comentarios adicionales o cambiar sus decisiones.

1. Cree una nueva prueba, tal como se describe en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   O\
   Abra la página Detalles de la prueba para una prueba existente, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para obtener una prueba nueva, en **[!UICONTROL Configuración de prueba]**, seleccione **[!UICONTROL Bloquear la prueba cuando se toman todas las decisiones necesarias]**.\
   O\
   Para una prueba existente, en **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Bloquear la prueba cuando se tomen todas las decisiones]**.

Para obtener información sobre las decisiones, consulte [Tome una decisión sobre una prueba en el visor de pruebas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

## Requerir inicio de sesión para todos los usuarios que revisen la prueba

Una de las buenas cosas de [!DNL Workfront Proof] es que cualquiera puede revisar una prueba, no necesitas tener la tuya propia [!DNL Workfront Proof] para ello. Los destinatarios reciben un correo electrónico con una URL personal que los lleva directamente a la página de prueba, sin que tengan que iniciar sesión [!DNL Workfront Proof].

Sin embargo, si necesita niveles de seguridad más altos para el proceso de revisión y aprobación, puede usar requerir inicio de sesión en la prueba. Esto significa que solo [!DNL Workfront Proof] los usuarios se pueden agregar a la prueba. Y deben introducir su correo electrónico y contraseña para poder acceder a él.

>[!NOTE]
>
>* *Para que alguien pueda iniciar sesión en la prueba (cuando el Inicio de sesión requerido se ha habilitado), debe haberse añadido a la prueba.*
>* *Si el Inicio de sesión requerido está habilitado, las suscripciones no se pueden habilitar.*


Para requerir inicio de sesión para todos los usuarios que revisen la prueba:

1. Cree una nueva prueba, tal como se describe en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   O\
   Abra la página Detalles de la prueba para una prueba existente, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para obtener una prueba nueva, en **[!UICONTROL Configuración de prueba]**, seleccione **[!UICONTROL Requerir inicio de sesión]**.\
   O\
   Para una prueba existente, en **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Inicio de sesión requerido]**.

## Exigir una única decisión para la prueba

Esta configuración es útil en casos en los que solo necesita una persona de un grupo, departamento o empresa para tomar una decisión sobre la prueba.

Aunque asigne la función de Aprobador o Revisor y Aprobador a varias personas, una vez que una persona tome una decisión sobre una prueba, el estado de la prueba se actualizará (según la decisión tomada). Para obtener más información sobre el estado de prueba, consulte [Ver el progreso y estado de una prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)

1. Cree una nueva prueba, tal como se describe en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   O\
   Abra la página Detalles de la prueba para una prueba existente, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para obtener una prueba nueva, en **[!UICONTROL Flujo de trabajo]**, seleccione **[!UICONTROL Requerir solo una decisión para esta fase]**.\
   O\
   Para una prueba existente, en **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Solo se requiere una decisión]**.

Para obtener información sobre las decisiones, consulte [Tome una decisión sobre una prueba en el visor de pruebas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

## Requiere que las decisiones se firmen electrónicamente

Puede requerir una firma electrónica de cualquier revisor que tome una decisión sobre la prueba para proporcionar su correo electrónico y contraseña. Cuando un revisor toma una decisión, aparece un mensaje pidiendo que introduzca su correo electrónico y contraseña y que confirme su decisión. Para obtener más información, consulte [Explicación de las firmas electrónicas en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)

1. Cree una nueva prueba, tal como se describe en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   O\
   Abra la página Detalles de la prueba para una prueba existente, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para obtener una prueba nueva, en **[!UICONTROL Configuración de prueba]**, seleccione **[!UICONTROL Requiere que las decisiones se firmen electrónicamente]**.\
   O\
   Para una prueba existente, en **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Requiere que las decisiones se firmen electrónicamente]**.

Para obtener información sobre las decisiones, consulte [Configure las opciones de decisión de aprobación en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## No permitir que los usuarios descarguen el archivo original

Puede evitar que los revisores descarguen el archivo original desde el que se creó la prueba.

1. Cree una nueva prueba, tal como se describe en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   O\
   Abra la página Detalles de la prueba para una prueba existente, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para obtener una prueba nueva, en **[!UICONTROL Configuración de prueba]**, deseleccionar **[!UICONTROL Descargar archivo original]**.\
   O\
   Para una prueba existente, en **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Descarga del archivo original]**.

## Permitir que otros usuarios se suscriban a la prueba

La suscripción es una configuración avanzada que funciona con la prueba de la URL de prueba y la prueba Mini.

De forma predeterminada, las personas que no se hayan agregado específicamente a la prueba y que estén utilizando la URL de prueba o la prueba Mini para acceder a ella solo pueden ver la prueba en modo de solo lectura. Las personas que ya sean revisores en la prueba pueden iniciar sesión con su dirección de correo electrónico. Para obtener más información, consulte [Administrar funciones de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)

La activación de la suscripción en la prueba permite que las personas que no se hayan añadido explícitamente a la prueba se suscriban a la prueba (es decir, se añadan a la prueba). A continuación, se les asignará la función y la alerta de correo electrónico que seleccione para ellos en la configuración de suscripción.

Si la suscripción se ha habilitado en una prueba, los campos siguientes se activarán:

* **[!UICONTROL Se requiere la validación del suscriptor]** - El suscriptor debe hacer clic en un vínculo de un correo electrónico para acceder a una prueba\
   Si selecciona esta opción, la persona que se suscriba no obtendrá acceso inmediato a la prueba, pero obtendrá un vínculo a la prueba en un mensaje de correo electrónico. El propósito de la validación del suscriptor es garantizar que la persona ha introducido una dirección de correo electrónico correcta a la que tiene acceso.

* **[!UICONTROL Función predeterminada para nuevos suscriptores]** : Esta es la función de prueba predeterminada que se asigna a todos los revisores que se suscriben a la prueba.
* **[!UICONTROL Alerta de correo electrónico predeterminada para nuevos suscriptores]** : Esta es la alerta de correo electrónico predeterminada que se asigna a todos los revisores que se suscriben a la prueba.

Consulte también [Suscripción a una prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)

Para permitir que otros usuarios se suscriban a una prueba:

1. Cree una nueva prueba, tal como se describe en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   O\
   Abra la página Detalles de la prueba para una prueba existente, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. Para obtener una prueba nueva, en **[!UICONTROL Configuración de prueba]**, deseleccionar **[!UICONTROL Suscripción a la prueba mediante URL pública o código incrustado]**.\
   O\
   Para una prueba existente, en **[!UICONTROL Configuración]**, seleccione **[!UICONTROL Suscripción]**.
