---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Nuevo correo electrónico de prueba
description: Haga que este artículo funcione mejor para PiW.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Nuevo correo electrónico de prueba

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

Cuando crea una prueba nueva o una versión nueva de una prueba, agrega personas nuevas a una prueba o agrega un flujo de trabajo a una prueba, puede decidir si desea enviar un correo electrónico a los revisores, como se explica en estos artículos:

* [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

El correo electrónico que reciben los destinatarios se denomina [!UICONTROL Nueva prueba] correo electrónico. Solo el creador de pruebas y los usuarios autorizados para agregar revisores a una prueba pueden controlar este correo electrónico. Los destinatarios no pueden deshabilitarlo.

El correo electrónico de prueba nueva contiene:

* Su mensaje personal (si decide incluir uno)
* Si siempre envía el mismo mensaje personalizado a los revisores, puede que sea recomendable guardarlo en su [!UICONTROL Ajustes personales] en el [!UICONTROL Valores predeterminados de prueba] pestaña . Para obtener más información, consulte .
* Enlace personal a la prueba
* **[!UICONTROL Ver detalles]** vínculo que lo lleva a la [!DNL Workfront] (como un proyecto, una tarea o un problema)
* Miniatura de la imagen de prueba
* Los siguientes detalles de la prueba:

   * Nombre de revisión
   * Número de versión

      Para obtener más información, consulte .

   * Lista de los revisores y su progreso en la prueba
   * Un vínculo para compartir la prueba con otra persona

      Esto le permite compartir la URL de prueba o el vínculo de descarga del archivo original. Esto no le permite añadir explícitamente revisores a la prueba, solo compartirá la URL de prueba pública y el destinatario recibirá acceso de solo lectura a la prueba.

      Consulte [Compartir una prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) para obtener más información.

      Si no desea que este vínculo aparezca en el correo electrónico del destinatario, puede desactivar la variable [!UICONTROL Uso compartido público] configuración de la prueba

      (Descargue el archivo original y la URL pública). Consulte [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) para obtener más información.

## El registro de actividades

Envío de un [!UICONTROL Nueva prueba] El correo electrónico a un revisor se registra en la [!UICONTROL Actividad] sección de [!UICONTROL Detalles de la prueba] página. Consulte  [Administrar[!UICONTROL  Detalles de la prueba] en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) para obtener más información. Puede comprobar si la variable [!UICONTROL Nueva prueba] El correo electrónico se habilitó en el momento de crear una prueba.

![New_Version_email_-_acitivity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* Si el Creador o el Propietario de la prueba tiene [!UICONTROL Prueba realizada] los correos electrónicos desactivados de forma predeterminada (en su configuración personal) no reciben ningún [!UICONTROL Prueba realizada] o [!UICONTROL Nueva prueba] los correos electrónicos incluso si la variable [!UICONTROL Notificar a las personas por correo electrónico] se marca en la página New proof . Para obtener más información, consulte .
>* Si las notificaciones por correo electrónico están deshabilitadas de forma predeterminada en la variable [!UICONTROL Configuración de la cuenta] el Creador/Propietario de la prueba no recibirá ninguna [!UICONTROL Prueba realizada] o [!UICONTROL Nueva prueba] los correos electrónicos, incluso si están activados en su configuración personal y la variable [!UICONTROL Notificar] la casilla personas por correo electrónico está marcada en la página Nueva prueba . Para obtener más información, [La variable [!UICONTROL Prueba realizada] email](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) y consulte .
>




## Active la variable [!UICONTROL Nueva prueba] correo electrónico e incluir un mensaje personalizado

Puede especificar si desea enviar una alerta por correo electrónico a los revisores en una prueba cuando la cree o cuando añada alguien a ella.

* [Al crear una prueba](#when-you-create-a-proof)
* [Al añadir un revisor a una prueba](#when-you-add-a-reviewer-to-a-proof)

### Al crear una prueba {#when-you-create-a-proof}

Cuando esté creando una prueba nueva en la [!UICONTROL Nueva prueba] en el **[!UICONTROL Compartir]** , puede seleccionar si desea enviar alertas por correo electrónico:

* Aquí puede decidir si desea [!UICONTROL Notificar a las personas por correo electrónico] (1) Si anula la selección de esta opción, ninguno de los revisores recibe un mensaje de correo electrónico para informarles de que la prueba está lista para su revisión.
* También puede incluir un mensaje personalizado en la notificación por correo electrónico (2).
* Si decide añadir su propio mensaje personalizado, podrá colocar un asunto personalizado (3) y un mensaje en el cuerpo del mensaje de correo electrónico (4).
* Para descartar el mensaje personalizado simplemente haga clic en el vínculo (5).

   >[!NOTE]
   >
   >Si siempre envía el mismo mensaje personalizado a los revisores, puede que sea aconsejable guardarlo en la configuración personal de [!UICONTROL Valores predeterminados de prueba] pestaña . Para obtener más información, consulte .

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### Al añadir un revisor a una prueba {#when-you-add-a-reviewer-to-a-proof}

Puede seleccionar si se notificará de la prueba a un nuevo revisor añadido a una prueba existente (similar a lo anterior).

* En primer lugar, agregue nuevos revisores haciendo clic en el botón **[!UICONTROL Compartir esta versión]** en el **[!UICONTROL Detalles de la prueba]** página (1).

![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)

* Aparece un cuadro en el que puede agregar nuevos revisores. A continuación, puede decidir si desea que se les notifique por correo electrónico (2) y elegir añadir un mensaje personalizado al correo electrónico (3).

![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* Si decide añadir un mensaje personalizado, el cuadro se expande y podrá colocar una línea de asunto personalizada (4) y texto personalizado en el cuerpo del correo electrónico (5). También puede descartar el mensaje personalizado haciendo clic en el vínculo (6).

![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)
