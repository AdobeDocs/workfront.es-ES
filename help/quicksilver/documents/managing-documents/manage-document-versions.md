---
product-area: documents
navigation-topic: manage-documents
title: Administrar versiones de documentos
description: Puede administrar varias versiones de un documento en Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
TQID: https://experienceleague.adobe.com/rCnj3Gx1SB3-UziuppQfifv2hJ6q3OjepNO9FcEEHEk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 634
ht-degree: 10%

---

# Administrar versiones de documentos

<!-- Audited: 5/2025 -->

Puede administrar varias versiones de un documento en Workfront.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquier paquete de Workfront para administrar documentos mediante el almacenamiento heredado de Workfront</p>
<p>Cualquier paquete de flujo de trabajo para administrar documentos mediante Adobe Cloud Storage.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior</p>
   <p>Solicitud o superior </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Ver acceso a los documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver acceso al documento</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

* Este artículo supone que el documento tiene varias versiones.

  Si necesita información sobre cómo cargar nuevas versiones de un documento en Workfront, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md).

## Ver una lista de todas las versiones de un documento

{{step1-to-documents}}

1. En la página **Documentos**, seleccione un documento de la lista.

1. En la esquina superior derecha de la página, haga clic en el icono **Abrir resumen** ![Abrir resumen](assets/qs-summary-in-new-toolbar-small.png). Se abre el panel lateral **Resumen del documento**.

1. Desplácese hacia abajo hasta la sección **Versiones** para ver todas las versiones del documento.

## Ver y administrar detalles de una versión anterior del documento

{{step1-to-documents}}

1. Pase el puntero por encima del documento y haga clic en **Detalles del documento**.

1. Cerca de la parte superior de la página **Detalles del documento**, haga clic en el menú desplegable situado junto al nombre y, a continuación, haga clic en el nombre de la versión que desee ver y administrar.

   ![Menú desplegable Versión en la página Detalles del documento](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Además de ver los detalles de la versión, puede realizar cambios en la misma, como el nombre, los metadatos y la configuración de revisión (si se trata de una revisión de documento).

## Descargar una sola versión del documento

{{step1-to-documents}}

1. En la página **Documentos**, seleccione un documento de la lista.

1. En la esquina superior derecha de la página, haga clic en el icono **Abrir resumen** ![Abrir resumen](assets/qs-summary-in-new-toolbar-small.png). Se abre el panel lateral **Resumen del documento**.

1. En la sección **Versiones**, haga clic en el menú **Más** ![Menú más](assets/more-icon.png) que se encuentra a la derecha de la versión y, a continuación, haga clic en **Descargar** en la lista desplegable que aparece.

   ![Descargar un solo documento](assets/more-versions-350x143.png)

## Descargar todas las versiones de un documento

{{step1-to-documents}}

1. En la página **Documentos**, seleccione un documento de la lista.

1. En la esquina superior derecha de la página, haga clic en el icono **Abrir resumen** ![Abrir resumen](assets/qs-summary-in-new-toolbar-small.png). Se abre el panel lateral **Resumen del documento**.

1. Desplácese hacia abajo hasta la sección **Versiones** y, a continuación, haga clic en **Descargar todo**.

## Eliminar una versión de documento

Si carga una versión de un documento por error o ya no es necesaria, puede eliminar la versión y mantener el documento original.

>[!IMPORTANT]
>
>No puede recuperar una versión de documento que elimine individualmente.

Tenga en cuenta lo siguiente cuando considere la posibilidad de eliminar una versión de documento:

* Solo se puede eliminar una versión a la vez. Si se elimina una versión, esta acción aparece en la sección Actualizaciones del documento.
* Si carga una nueva versión después de eliminarla, esta recibirá el siguiente número secuencial. Por ejemplo, si hay tres versiones de un documento y elimina la versión 3, el siguiente documento cargado será la versión 4.
* Las actualizaciones del sistema y los comentarios realizados sobre una versión se conservan en Workfront después de eliminarse la versión.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Para eliminar una versión de documento:

{{step1-to-documents}}

1. En la página **Documentos**, seleccione el documento de la lista.

1. En la esquina superior derecha de la página, haga clic en el icono **Abrir resumen** ![Abrir resumen](assets/qs-summary-in-new-toolbar-small.png). Se abre el panel lateral **Resumen del documento**.

1. Desplácese hacia abajo hasta la sección **Versiones** para ver todas las versiones del documento.
1. En la sección **Versiones**, haga clic en el menú **Más** ![Menú más](assets/more-icon.png) que se encuentra a la derecha de la versión y, a continuación, haga clic en **Eliminar** en la lista desplegable que aparece.

   >[!NOTE]
   >
   >* La opción **Delete** solo está visible si hay al menos 2 versiones.
   >* Si el documento está vinculado a una fuente externa, ese vínculo se elimina y el documento ya no es accesible a través de Workfront.

   ![Eliminar la versión del documento](assets/more-versions-350x143.png)
