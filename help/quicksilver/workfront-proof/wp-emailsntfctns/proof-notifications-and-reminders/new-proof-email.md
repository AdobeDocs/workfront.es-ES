---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Correo electrónico de nueva prueba
description: Haga que este artículo funcione mejor para PiW.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
TQID: https://experienceleague.adobe.com/0HC5D2PBZQ7L7N5NI0Q2FbUg6qSjLK7M1OkRLrUj0kA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 806
ht-degree: 100%

---

# Correo electrónico de nueva prueba

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

Al crear una nueva prueba o versión de una prueba, añadir nuevas personas a una prueba o añadir un flujo de trabajo a una prueba, puede decidir si desea enviar un correo electrónico a los revisores, como se explica en estos artículos:

* [Crear una revisión avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Generar revisiones en  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

El correo electrónico que reciben los destinatarios se llama [!UICONTROL Nueva revisión]. Solo el creador de la prueba y los usuarios autorizados a añadir revisores a una prueba pueden controlar este correo electrónico. Los destinatarios no pueden deshabilitarlo.

El correo electrónico de nueva prueba contiene:

* Su mensaje personal (si decide incluir uno)
* Si siempre envía el mismo mensaje personalizado a sus revisores, podría ser recomendable guardarlo en su [!UICONTROL configuración personal], en la ficha [!UICONTROL Valores predeterminados de revisión]. Para obtener más información, consulte.
* Vínculo personal a la prueba
* **[!UICONTROL Ver detalles]** vínculo que le lleva al objeto de [!DNL Workfront] asociado (como un proyecto, tarea o problema)
* Miniatura de la imagen de la prueba
* Los siguientes detalles de la prueba:

   * Nombre de revisión
   * Número de versión
   * Lista de revisores y su progreso en la prueba
   * Un vínculo para compartir la prueba con otra persona

     Esto le permite compartir la URL de la prueba o el vínculo de descarga del archivo original. Esto no le permite añadir explícitamente revisores a la prueba, solo compartirá la URL pública de la prueba y el destinatario recibirá un acceso de solo lectura a la prueba.

     Consulte [Compartir una prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) para obtener más información.

     Si no desea que este enlace aparezca en el correo electrónico de su destinatario, puede deshabilitar la configuración de [!UICONTROL Uso compartido público] en la prueba

     (Descargar archivo original y URL pública). Consulte [Administrar detalles de la prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) para obtener más información.

## El registro de actividad

El envío de un correo electrónico [!UICONTROL Nueva prueba] a un revisor se registra en la sección [!UICONTROL Actividad] de la página [!UICONTROL Detalles de la prueba]. Consulte [Administrar[!UICONTROL  detalles de la revisión] en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) para obtener más información. Puede comprobar si el correo electrónico de [!UICONTROL nueva prueba] se habilitó en el momento de crear una prueba.

![New_Verison_email_-_acitivity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* Si el creador o propietario de la prueba tiene los correos electrónicos de las [!UICONTROL Pruebas realizadas] deshabilitados de forma predeterminada (en su configuración personal), no recibirá correos electrónicos de [!UICONTROL Pruebas realizadas] ni de [!UICONTROL Nuevas pruebas] aunque la casilla [!UICONTROL Notificar a las personas por correo electrónico] esté marcada en la página Nueva prueba. Para obtener más información, consulte.
>* Si las notificaciones por correo electrónico están deshabilitadas de forma predeterminada en la [!UICONTROL configuración de la cuenta], el creador/propietario de la prueba no recibirá ningún correo electrónico de [!UICONTROL Prueba realizada] o [!UICONTROL Nueva prueba] aunque esté habilitado en su configuración personal y la casilla de verificación [!UICONTROL Notificar] a las personas por correo electrónico esté marcada en la página Nueva prueba. Para obtener más información, consulte [El correo electrónico de [!UICONTROL Prueba realizada]](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) y vea .
>



## Habilite el correo electrónico de [!UICONTROL Nueva prueba] e incluya un mensaje personalizado

Puede especificar si desea enviar una alerta por correo electrónico a los revisores sobre una prueba cuando la cree o cuando añada a alguien a ella.

* [Al crear una prueba](#when-you-create-a-proof)
* [Cuando añade un revisor a una prueba](#when-you-add-a-reviewer-to-a-proof)

### Al crear una prueba {#when-you-create-a-proof}

Cuando esté creando una nueva prueba en la página [!UICONTROL Nueva prueba], en la sección **[!UICONTROL Compartir]**, puede seleccionar si desea enviar alertas por correo electrónico:

* Aquí puede decidir si desea [!UICONTROL Notificar a las personas por correo electrónico] (1). Si anula la selección de esta opción, ninguno de los revisores recibirá un correo electrónico para informarles de que la prueba está lista para su revisión.
* También puede incluir un mensaje personalizado en la notificación por correo electrónico (2).
* Si decide añadir su propio mensaje personalizado, podrá colocar una línea de asunto personalizada (3) y un mensaje en el cuerpo del correo electrónico (4).
* Para descartar el mensaje personalizado, simplemente haga clic en el vínculo (5).

  >[!NOTE]
  >
  >Si siempre envía el mismo mensaje personalizado a los revisores, sería aconsejable guardarlo en la configuración personal de la ficha [!UICONTROL Valores predeterminados de revisión]. Para obtener más información, consulte.

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### Cuando añade un revisor a una prueba {#when-you-add-a-reviewer-to-a-proof}

Puede seleccionar si un revisor nuevo añadido a una prueba existente recibirá una notificación de la prueba (similar a la anterior).

* Primero, añada nuevos revisores haciendo clic en el botón **[!UICONTROL Compartir esta versión]** en la página **[!UICONTROL Detalles de la prueba]** (1).

![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)

* Aparece un cuadro en el que puede añadir nuevos revisores. A continuación, puede decidir si desea que se les notifique por correo electrónico (2) y elegir añadir un mensaje personalizado al correo electrónico (3).

![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* Si decide añadir un mensaje personalizado, el cuadro se expande y podrá colocar una línea de asunto personalizada (4) y texto personalizado en el cuerpo del correo electrónico (5). También puede descartar el mensaje personalizado haciendo clic en el vínculo (6).

![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)
