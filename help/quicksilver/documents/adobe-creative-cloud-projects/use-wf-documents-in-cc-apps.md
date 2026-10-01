---
product-area: documents;workfront-integrations
navigation-topic: adobe-creative-cloud-projects
title: Uso de documentos de Workfront en aplicaciones de Creative Cloud
description: Abra, edite y guarde documentos de Workfront de Photoshop, Illustrator y InDesign, y solicite las aprobaciones correspondientes.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: deeb63ceccc28b8f376713d4a6fb6c103ab4e06b
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 7%
---
# Uso de documentos de Workfront en aplicaciones de Creative Cloud

Una vez que un proyecto de Workfront está disponible en el panel Proyectos de Creative Cloud, puede trabajar con sus documentos directamente desde Photoshop, Illustrator o InDesign.

## Requisitos previos

* Su organización debe contar con una versión de Workfront que admita el almacenamiento en la nube de Adobe.
* Workfront y Photoshop, Illustrator o InDesign deben tener derechos en la misma organización de Adobe Identity Management System (IMS).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versión de Adobe Workfront</td> 
   <td>Flujo de trabajo de Ultimate, con Adobe Cloud Storage habilitado</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>
      <p>Ver el acceso a un proyecto para verlo en el panel Proyectos Creative Cloud</p>
      <p>Editar el acceso a un proyecto para agregarlo, editarlo o eliminarlo</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Acceso a un proyecto de Workfront

La estructura de carpetas Documentos de un proyecto de Workfront se refleja en el panel Proyectos. Cuando abra un documento desde una carpeta de proyecto, lo edite y lo guarde, los cambios aparecerán en Workfront.

>[!NOTE]
>
>Los proyectos de almacenamiento de Workfront heredados no son compatibles con el panel Proyectos: solo con proyectos de almacenamiento de Adobe en la nube.


Para acceder a un proyecto de Workfront en Photoshop, Illustrator o InDesign:

1. Abra Photoshop, Illustrator o InDesign.
1. En el panel **Proyectos** que se encuentra en la parte izquierda de la aplicación, seleccione el proyecto de Workfront que desee abrir.

   ![Proyectos Workfront enumerados en el panel Proyectos](assets/cc-projects.png)

1. Abra un documento del proyecto para editarlo. Una vez guardados los cambios, se vuelven a guardar automáticamente en el proyecto de Workfront.


>[!TIP]
>
>Para editar un tipo de archivo que Photoshop, Illustrator o InDesign no puedan abrir, como un documento de Word o Excel, use Adobe Cloud Drive en su lugar. Para obtener más información, consulte [Información general sobre Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md).

## Solicitar una aprobación de un documento

Puede agregar una aprobación de documento en Workfront a cualquier documento que haya cargado desde Photoshop, Illustrator o InDesign, o desde Adobe Cloud Drive, igual que cualquier otro documento. Para obtener más información, consulte [Crear un flujo de trabajo de aprobación de documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

<!--
need to verify
Creating an approval on a Creative Cloud document also creates a new version of the document. For more information, see [Manage document versions](/help/quicksilver/documents/managing-documents/manage-document-versions.md#view-the-current-file-during-an-approval).
-->