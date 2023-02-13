---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Comprender el estado de prueba en la prueba de Workfront
description: En [!DNL Workfront Proof], las pruebas existen en diferentes estados. Estos estados determinan qué acciones se pueden llevar a cabo en la prueba, como comentar o tomar decisiones.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Comprender el estado de prueba en la prueba de Workfront

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

En [!DNL Workfront Proof], las pruebas existen en diferentes estados. Estos estados determinan qué acciones se pueden llevar a cabo en la prueba, como comentar o tomar decisiones.

## Explicación del estado de prueba

Los cuatro estados son los siguientes:

* [Activo](#active)
* [Bloqueado](#locked)
* [Borrador (solo zona desplegable)](#draft-dropzone-only)
* [Enviado (sólo Dropzone)](#submitted-dropzone-only)

### Activo {#active}

Pruebas que se cargan en [!DNL Workfront Proof] a través de la página Nueva prueba o Dropzone aparecen como activos después de procesarlos. Cuando una prueba está activa, los usuarios pueden revisar, realizar comentarios y tomar decisiones sobre la prueba.

>[!NOTE]
>
>Las pruebas cargadas a través de Dropzone aparecen como Activas solo si la opción Activate proof on submit está activada. Si la opción no está activada, debe activar manualmente la prueba.

Para obtener más información sobre la configuración de Dropzone, consulte [Configure la zona de colocación en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### Bloqueado {#locked}

Puede bloquear una prueba cuando termine de revisarla. Bloquear una prueba significa que no se pueden realizar más comentarios o decisiones sobre la prueba, pero la prueba se puede abrir.

Cualquier usuario con derechos de edición en la prueba puede desbloquearlo.

Para obtener más información sobre derechos, consulte [Perfiles de permisos de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>Las notificaciones por correo electrónico ya no se envían cuando se bloquea una prueba. Por ejemplo, si una prueba está bloqueada antes de su fecha límite, no se envía un correo electrónico de notificación cuando se llega a la fecha límite.

### Borrador (solo zona desplegable) {#draft-dropzone-only}

Cuando envía una prueba a través de Dropzone, pasa al estado Borrador antes de que el administrador la active. Cuando se encuentra en la zona de borrador, no se puede realizar ninguna acción en la prueba.

### Enviado (sólo Dropzone) {#submitted-dropzone-only}

Después de que el administrador active un borrador, la prueba se muestra como Enviado en Dropzone. Una vez enviado, puede realizar acciones en la prueba.

## Visualización y cambio del estado de prueba

Para obtener información sobre la visualización de una lista de todas las pruebas de un estado específico, como la visualización de todas las pruebas activas o bloqueadas, consulte [Administrar elementos en la página Vistas de [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) en el artículo [Administrar elementos en la página Vistas de [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Acceda a su [!DNL Workfront Proof] Tablero.

   Para obtener más información, consulte [Acceso [!DNL Workfront Proof] de Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. En el **[!UICONTROL Panel]**, haga clic en **[!UICONTROL Expandir]** flecha junto a la prueba de la que desea ver o cambiar el estado.

   ![](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   La variable **[!UICONTROL Proceso de flujo de trabajo]** aparece.

   ![](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. Consulte la **[!UICONTROL Estado]** en el **[!UICONTROL Proceso de flujo de trabajo]**.

1. (Opcional) Para cambiar el estado, pase el ratón sobre el **[!UICONTROL Estado]** y haga clic en el menú desplegable y, a continuación, seleccione un nuevo estado.

   ![](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
