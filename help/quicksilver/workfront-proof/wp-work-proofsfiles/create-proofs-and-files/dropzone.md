---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: create-proofs-and-files
title: Dropzone
description: Si tiene el plan de Enterprise, puede utilizar Dropzone para enviar nuevas pruebas y nuevas versiones de pruebas a su cuenta sin tener que iniciar sesión en su cuenta.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e66142fa-3b0d-4821-9aa5-040c62f00d62
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 0%

---

# Dropzone

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Si tiene el plan de Enterprise, puede utilizar Dropzone para enviar nuevas pruebas y nuevas versiones de pruebas a su cuenta sin tener que iniciar sesión en su cuenta.

Cuando envía una prueba a través de Dropzone, esta aparece en la página Dropzone del [!DNL Workfront Proof] cuenta. Desde allí, puede enrutarlo al flujo de trabajo.

## Envío de una nueva prueba a través de la URL de Dropzone

1. En el explorador, vaya a la URL de zona de colocación única, tal como se describe en [Configure la zona de colocación en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. Escriba su dirección de correo electrónico.
1. Haga clic en **[!UICONTROL Seleccionar un archivo]** o **[!UICONTROL Capturar una página web]** y elija el archivo o la página web que desea cargar.

1. Introduzca el código de seguridad y haga clic en **[!UICONTROL Siguiente]**.\
   Una barra de progreso muestra el progreso de la carga.\
   En la siguiente pantalla, podrá añadir detalles de prueba.\
   Tenga en cuenta que esta sección solo aparece si se ha habilitado en la configuración de zona de colocación.

1. Una vez rellenados los detalles, haga clic en **[!UICONTROL Siguiente]**.
1. Los revisores añadidos a la prueba solo recibirán un correo electrónico de notificación tras la activación de la prueba (consulte a continuación).
1. La prueba pasa a los siguientes estados después de enviarla a Dropzone:

   * Cuando se carga por primera vez un archivo en la zona de colocación, la prueba se muestra como borrador.
   * Una vez que complete el envío, la prueba se muestra en su Dropzone como Enviado.
   * Una vez que la prueba se ha activado y desbloqueado, se muestra en Dropzone como Activa.
   * Si la prueba está bloqueada, se muestra en la zona de colocación como Bloqueada.

## Envío de una nueva versión de una prueba existente mediante la URL de Dropzone

1. En el explorador, vaya a la URL de zona de colocación única, tal como se describe en [Configure la zona de colocación en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. Escriba su dirección de correo electrónico.
1. Seleccione la casilla de verificación para indicar que está cargando una nueva versión de una prueba existente.\
   Para obtener información sobre la creación de una nueva versión de una prueba, consulte .
1. Haga clic en **[!UICONTROL Seleccionar un archivo]** o **[!UICONTROL Capturar una página web]** y elija el archivo o la página web que desea cargar.

1. Introduzca el código de seguridad y haga clic en **[!UICONTROL Siguiente]**.\
   Una barra de progreso muestra el progreso de la carga.\
   Workfront Proof le envía un correo electrónico de validación.

1. Haga clic en el vínculo del correo electrónico.\
   El correo electrónico abre la ventana Zona de colocación en el explorador. El vínculo de la notificación por correo electrónico es válido durante 24 horas.
1. Seleccione la versión anterior de la prueba (solo se mostrarán las pruebas que haya creado o enviado).\
   En la siguiente pantalla podrá añadir detalles de prueba.\
   Esta sección aparece únicamente si está habilitada en la configuración de Dropzone.

1. Escriba los detalles, haga clic en **[!UICONTROL Siguiente]**.

   >[!NOTE]
   >
   >Los revisores añadidos a la prueba solo recibirán un correo electrónico de notificación tras la activación de la prueba (consulte a continuación).

   La prueba pasa a los siguientes estados después de enviarla a Dropzone:

   * Cuando se carga por primera vez un archivo en la zona de colocación, la prueba se muestra como borrador.
   * Una vez que complete el envío, la prueba se muestra en su Dropzone como Enviado.
   * Una vez que la prueba se ha activado y desbloqueado, se muestra en Dropzone como Activa.
   * Si la prueba está bloqueada, se muestra en la zona de colocación como Bloqueada.

## Envío por correo electrónico de una prueba a Dropzone

>[!NOTE]
>
>Ya no se puede enviar por correo electrónico una prueba a la zona de colocación.


## Finalización del envío

Workfront le envía (al remitente) un correo electrónico de envío completo en el que se le solicita que confirme si el archivo es una prueba nueva o una versión nueva. El vínculo de la notificación por correo electrónico es válido durante 24 horas.

1. Haga clic en el vínculo y siga los pasos anteriores, en función de si es una prueba nueva o una versión nueva de una prueba existente.

## Activación de la prueba

El propietario de Dropzone recibe un mensaje de correo electrónico de notificación para informarle de que se ha enviado una nueva prueba a Dropzone:

* La prueba aparece en la página Zona de colocación de la cuenta (para acceder a la página Zona de colocación, haga clic en el vínculo de la barra lateral de navegación izquierda).
* El propietario de Dropzone (o un usuario que tenga al menos un perfil de Supervisor) puede acceder a la prueba. El propietario se puede cambiar en la configuración de Dropzone (solo un administrador de facturación o un administrador pueden hacerlo).
* Antes de poder trabajar en la prueba, debe activarla o desbloquearla el propietario de Dropzone (un usuario con al menos un perfil de Supervisor también puede hacerlo). El estado de la prueba se muestra como Enviado hasta que se ha activado/desbloqueado.

Para activar la prueba:

1. Vaya al menú desplegable a la derecha de la prueba y haga clic en **[!UICONTROL Activar]**.
1. Una vez activada o desbloqueada la prueba:

   * El estado de prueba cambia a Activo.
   * Cualquier persona que se haya agregado a la prueba recibirá un correo electrónico de notificación para avisarle de que tiene una nueva prueba que revisar. (No se envía ningún correo electrónico hasta que se haya activado o desbloqueado la prueba).
   * La prueba se puede trabajar con normalidad
   * Si el remitente también se agrega explícitamente a la prueba, no recibirá un correo electrónico de prueba nueva. Para obtener más información, consulte [Nuevo correo electrónico de prueba](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

## Administración de la zona de colocación

La página Dropzone facilita la administración de los envíos a su Dropzone. La página Zona de colocación incluye las siguientes opciones y funcionalidades:

* Diseño de página (1)
* Elija incluir/excluir pruebas archivadas en la vista (2)
* Botones de acción (3)
* Ordenar (4)
* Filtro (5)
* Menú de acciones de prueba (6)
* Desarchivar la prueba (7)
* Resumen de la prueba de expansión/contracción (8)
* Seleccionar una prueba (9)

Las opciones de diseño de página y clasificación y filtrado son las mismas que en la [!DNL Views] listas. Consulte [Administrar elementos en la página Vistas de [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) para obtener más información.

![New_Dropzone_design__Feb_2013_.jpg](assets/new-dropzone-design--feb-2013--350x224.jpg)
