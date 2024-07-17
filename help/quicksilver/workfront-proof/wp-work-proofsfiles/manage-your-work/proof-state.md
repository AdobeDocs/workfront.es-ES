---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Comprender el estado de prueba en Workfront Proof
description: En  [!DNL Workfront Proof], las pruebas existen en diferentes estados. Estos estados determinan qué acciones puede realizar en la prueba, como comentar o tomar decisiones.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Comprender el estado de prueba en Workfront Proof

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

En [!DNL Workfront Proof], las pruebas existen en diferentes estados. Estos estados determinan qué acciones puede realizar en la prueba, como comentar o tomar decisiones.

## Explicación del estado de prueba

Los cuatro estados son los siguientes:

* [Activo](#active)
* [Bloqueado](#locked)
* [Borrador (solo Dropzone)](#draft-dropzone-only)
* [Enviado (solo Dropzone)](#submitted-dropzone-only)

### Activo {#active}

Las pruebas que se cargan en [!DNL Workfront Proof] a través de la página Nueva prueba o la Dropzone aparecen como Activas una vez que se procesan. Cuando una prueba está activa, los usuarios pueden revisarla, realizar comentarios y tomar decisiones al respecto.

>[!NOTE]
>
>Las pruebas que se cargan a través de la Dropzone aparecen como Activas solo si la opción Activar prueba al enviar está activada. Si la opción no está activada, debe activar manualmente la prueba.

Para obtener más información acerca de la configuración de Dropzone, consulte [Configurar la Dropzone en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### Bloqueado {#locked}

Puede bloquear una prueba cuando termine de revisarla. Bloquear una prueba significa que no se pueden realizar más comentarios ni tomar más decisiones sobre la prueba, pero aún se puede abrir la prueba.

Cualquier usuario con derechos de edición en la prueba puede desbloquearla.

Para obtener más información acerca de los derechos, vea [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>Las notificaciones por correo electrónico ya no se envían cuando se bloquea una prueba. Por ejemplo, si una prueba está bloqueada antes de su fecha límite, no se envía un mensaje de correo electrónico de notificación cuando se llega a la fecha límite.

### Borrador (solo Dropzone) {#draft-dropzone-only}

Cuando envía una prueba a través de la Dropzone, pasa al estado de Borrador antes de que el administrador la active. Cuando se encuentra en la zona de borrador, no puede realizar ninguna acción en la prueba.

### Enviado (solo Dropzone) {#submitted-dropzone-only}

Una vez que el administrador activa un borrador, la prueba se muestra como Enviada en la Dropzone. Una vez enviada, puede realizar acciones en la prueba.

## Visualización y cambio del estado de prueba

Para obtener información sobre cómo ver una lista de todas las pruebas en un estado específico, como ver todas las pruebas activas o bloqueadas, consulte [Administrar elementos en la página de vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) en el artículo [Administrar elementos en la página de vistas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Acceda a su tablero [!DNL Workfront Proof].

   Para obtener más información, consulte [Acceso [!DNL Workfront Proof] desde Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. En el **[!UICONTROL panel]**, haga clic en la flecha de **[!UICONTROL Expandir]** que se encuentra junto a la revisión cuyo estado desea ver o modificar.

   ![](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   Aparece la sección **[!UICONTROL Proceso de flujo de trabajo]**.

   ![](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. Ver **[!UICONTROL estado]** en **[!UICONTROL proceso de flujo de trabajo]**.

1. (Opcional) Para cambiar el estado, pase el ratón sobre el **[!UICONTROL estado]** actual, haga clic en el menú desplegable y, a continuación, seleccione un nuevo estado.

   ![](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
