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
source-git-commit: db6d682b43caf1d28779599495b931da5c80d126
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 3%
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

## Guardar un nuevo documento en Workfront desde una aplicación de Creative Cloud

Puede guardar un archivo nuevo en Workfront o puede guardar una copia nueva de un archivo existente en Workfront desde Photoshop, Illustrator o InDesign.

Para guardar un nuevo documento en Workfront:

1. Abra Photoshop, Illustrator o InDesign y cree un nuevo archivo.
1. Si estás guardando un nuevo archivo, haz clic en **Guardar** en el menú superior.
O
Si está guardando una copia nueva de un archivo existente, haga clic en **Guardar como** en el menú superior.
1. En el cuadro de diálogo **Guardar como**, seleccione **Guardar en documentos de la nube** y, a continuación, elija el proyecto de Workfront que necesite.

   >[!NOTE]
   >
   >Al guardar un documento que ya se encuentra en el proyecto de Workfront, el cuadro de diálogo Guardar como no se abre. Puede seleccionar un proyecto de Workfront, guardarlo en una carpeta diferente o elegir un proyecto de Workfront diferente.


   ![guardar nuevo documento en workfront](assets/save-new-to-wf.png)

1. Elija una carpeta de documentos y haga clic en **Guardar**. Si no elige una carpeta, el documento se guarda en la carpeta raíz del proyecto.

   ![elija una carpeta para guardar el nuevo documento en workfront](assets/save-to-folder.png)

## Solicitar una aprobación de un documento

Puede agregar una aprobación de documento en Workfront a cualquier documento que haya cargado desde Photoshop, Illustrator o InDesign, o desde Adobe Cloud Drive, igual que cualquier otro documento. Para obtener más información, consulte [Crear un flujo de trabajo de aprobación de documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).



## Administrar versiones de un documento en Workfront desde una aplicación de Creative Cloud

Al guardar un documento de Photoshop, Illustrator o InDesign en Workfront, los cambios que guarde aparecerán en el archivo Actual en la pestaña Versiones y se marcarán con el distintivo &quot;Nuevos cambios&quot;.

Puede solicitar una aprobación sobre el archivo actual en lugar de cargar una nueva versión del documento. Para obtener más información, consulte [Solicitar aprobación para el archivo actual](#request-approval-on-the-current-file).

![archivo actual con nuevo distintivo de cambios](assets/current-file.png)

### Solicitar aprobación para el archivo actual

Para solicitar una aprobación sobre el archivo actual de un documento en Workfront:

1. Vaya al proyecto de Workfront que contiene el documento sobre el que desea solicitar una aprobación.
1. Abra el documento y vaya a la ficha **Versiones**.
1. En el archivo Actual, haga clic en el menú **Más** y, a continuación, en **Solicitar aprobación**.
1. En el cuadro de diálogo **Solicitar aprobación**, siga los pasos de [Crear un flujo de trabajo de aprobación de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) para crear la aprobación.

   ![solicitar aprobación para el archivo actual](assets/request-update-on-current-file.png)

