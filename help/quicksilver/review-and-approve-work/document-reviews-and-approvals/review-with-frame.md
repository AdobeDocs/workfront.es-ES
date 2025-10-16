---
product-area: documents
navigation-topic: approvals
title: Revisión y aprobación con el visor Frame.io
description: Obtenga información sobre cómo revisar y aprobar documentos con el visor Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 3190ad18-180e-42e5-aa10-bdad74303d3d
source-git-commit: a5041aecad22d3e576d7f0e9a4388a3e5bc69565
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Revisión y aprobación con el visor Frame.io

Puede revisar y aprobar documentos en Workfront mediante el visor Frame.io.

La revisión de documentos de Workfront con el visor Frame.io le permite dejar comentarios o marcar secciones específicas de un documento, imagen o vídeo para colaborar eficazmente con su equipo y garantizar que los comentarios sean claros y procesables.

Para obtener más información sobre la integración de Frame.io con Workfront, consulte [Información general sobre la integración de Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md).


<!--## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses</td> 
   <td> <p>Request or higher</p>
   <p>Contributor or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Documents</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit access to the object associated with the document</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ -->

## Requisitos previos

* Debe tener la integración de Workfront y Frame.io configurada en la instancia de Workfront. Para obtener más información, consulte [Resumen de la integración de Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md#integration-requirements).

## Revisar un documento

Como revisor, puede agregar comentarios a y marcar recursos. Una vez finalizada, puede marcar su revisión como completada en Workfront. No es necesario marcar la revisión como completada para que el recurso avance en el proceso de aprobación.

1. Vaya a la notificación de correo electrónico de revisión y haga clic en **Ir a revisión**.
o
Vaya a la página de inicio de Workfront, busque el widget Mis aprobaciones y haga clic en **Abrir revisión**.

   >[!NOTE]
   > 
   >Es posible que tenga que agregar el widget Mis aprobaciones a la página de inicio. Para obtener más información, consulte [Agregar, editar o quitar widgets en Inicio](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md).

1. En Frame.io, utilice las herramientas de comentarios para dejar comentarios o hacer preguntas.
Los comentarios y el marcado de recursos solo son visibles en el visor de Frame.io. Los comentarios no se muestran en Workfront. Para obtener más información sobre el uso del visor Frame.io, consulte [Comentarios sobre el contenido](https://help.frame.io/en/articles/9105251-commenting-on-your-media).
1. Una vez que esté satisfecho con el documento, vuelva a la página de detalles del documento en Workfront y marque la revisión como completada.

   ![Marcar revisión como completada](assets/mark-review-complete.png)

## Aprobar un documento

Como aprobador, puede agregar comentarios y marcar como recursos. Debe tomar la decisión de adelantar el proceso de aprobación.

El documento no pasa a un estado aprobado hasta que todos los aprobadores asignados eligen &quot;aprobado&quot;.

Para tomar una decisión sobre un documento:

1. Vaya a la notificación de correo electrónico de revisión y haga clic en **Ir a revisión**.
o
Vaya a la página de inicio de Workfront, busque el widget Mis aprobaciones y haga clic en **Abrir revisión**.

   >[!NOTE]
   > 
   >Es posible que tenga que agregar el widget Mis aprobaciones a la página de inicio. Para obtener más información, consulte [Agregar, editar o quitar widgets en Inicio](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md).


1. En Frame.io, utilice las herramientas de comentarios para dejar comentarios o hacer preguntas. Los comentarios y el marcado de recursos solo son visibles en el visor de Frame.io. Para obtener más información sobre el uso del visor Frame.io, consulte [Comentarios sobre el contenido](https://help.frame.io/en/articles/9105251-commenting-on-your-media).
1. Una vez que esté satisfecho con el documento, puede elegir una de las siguientes decisiones en el visor de Frame.io:

   * **Aprobar**: el recurso no necesita cambios y está listo para usarse.
   * **Necesita trabajo**: el recurso necesita cambios y no está listo para usarse. Una vez realizados los cambios especificados, el recurso debe cargarse como una nueva versión y pasar por otra ronda de aprobaciones. Para obtener más información, vea [Cargar una nueva versión del documento y solicitar la aprobación](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md). <!--do they need to tell someone it was uploaded via comment tagging?-->

   Una vez que tome una decisión, se notifica al propietario del documento por correo electrónico.

   Para obtener más información sobre las decisiones en Workfront, consulte [Resumen del estado de decisión del documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

   ![Visor de fotogramas y decisión](assets/make-decision-frame.png)



<!--is document owner the correct term?-->
