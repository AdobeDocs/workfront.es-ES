---
product-area: documents
navigation-topic: manage-documents
title: Mover documentos
description: Un usuario con derechos para administrar un documento puede mover el documento a otro objeto.
author: Courtney
feature: Digital Content and Documents
exl-id: 46039017-58b3-4e9d-8dcd-6e1f52d98d27
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/cltbYOyyPJM9NIkrHZqE3JqvIF94tvQXjatzAhcw1Es
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 434
ht-degree: 61%

---

# Mover documentos

Un usuario con derechos para administrar un documento puede mover el documento a otro objeto.

El usuario también debe tener permisos para añadir documentos al nuevo objeto para completar esta acción. 

Al mover un documento, cualquiera de los siguientes elementos también se moverá con el documento:

* Versiones de documento
* Pruebas de documentos
* Aprobaciones de documentos

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td><p>Cualquier paquete de Workfront para administrar documentos mediante el almacenamiento heredado de Workfront</p>
<p>Cualquier paquete de flujo de trabajo para administrar documentos mediante Adobe Cloud Storage.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior</p>
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar el acceso al documento</p> <p>Permiso para añadir documentos al nuevo objeto</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mover un documento al área de documentos heredados

Si su organización utiliza un almacenamiento de Workfront heredado, verá el área de documentos heredados al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento de Workfront, consulte [Diferencias entre el almacenamiento en la nube de Adobe y el almacenamiento de Workfront heredado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Para mover un documento:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.
1. Busque el documento que necesita.

1. Haga clic en el icono **Mover** ![Mover icono](assets/move-document--25x19.png).
   ![Mover ubicación del icono en la página](assets/move-doc-legacy.png)

1. En el menú desplegable del cuadro que aparece, haga clic en **Problema**, **Proyecto** o **Tarea** para indicar el tipo de objeto al que desea mover el documento. 

1. Escriba el nombre del **Problema**, **Proyecto** o **Tarea** en el cuadro de texto.

   >[!NOTE]
   >
   >Solo puede pasar a otro proyecto, tarea o problema mediante el almacenamiento heredado de Workfront.

1. Haga clic en **Finalizar**.

También puede mover un documento desde la página Detalles del documento.

## Mover un documento al área de Documentos nueva

Si su organización utiliza el almacenamiento en la nube de Adobe, verá la nueva área Documentos al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento en la nube de Adobe, consulte [Información general sobre el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Para mover un documento:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.
1. Busque el documento que necesita.
1. Haga clic en **Mover** en la parte inferior de la página.

![Mover ubicación del icono en la página](assets/move-new-doc.png)

1. En el menú desplegable del cuadro que aparece, haga clic en **Problema**, **Proyecto** o **Tarea** para indicar el tipo de objeto al que desea mover el documento.

1. Escriba el nombre del **Problema**, **Proyecto** o **Tarea** en el cuadro de texto.

   >[!NOTE]
   >
   >Solo puede pasar a otro proyecto, tarea o problema mediante Adobe Cloud Storage.

1. Haga clic en **Mover**.