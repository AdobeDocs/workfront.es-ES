---
product-area: documents
navigation-topic: manage-documents
title: Extraer documentos
description: Puede extraer un documento para evitar que otros usuarios lo eliminen o carguen una nueva versión. Solo un usuario puede extraer un documento a la vez. Puede extraer cualquier documento cargado en Adobe Workfront, así como documentos vinculados a proveedores de documentos de terceros (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint o cualquier otro proveedor personalizado).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 93%

---

# Extraer documentos

Puede extraer un documento para evitar que otros usuarios lo eliminen o carguen una nueva versión. Solo un usuario puede extraer un documento a la vez. Puede extraer cualquier documento cargado en Adobe Workfront, así como documentos vinculados a proveedores de documentos de terceros (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint o cualquier otro proveedor personalizado). 

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisión o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar el acceso al documento</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Acciones permitidas en los documentos extraídos

Los usuarios con acceso de administración al documento pueden hacer lo siguiente:

* Editar el documento (nombre del documento, descripción, datos personalizados)
* Mover el documento
* Compartir el documento
* Previsualizar el documento
* Descargar el documento

  >[!TIP]
  >
  >Aunque un usuario puede descargar un documento cuando lo haya extraído otro usuario, se recomienda que los usuarios esperen hasta que el documento se vuelva a insertar antes de descargarlo. Cuando se ha extraído un documento, a menudo indica que se está trabajando en él. Si se espera hasta que se vuelva a insertar un documento para descargarlo, se garantiza que el usuario tenga la versión más reciente.

* Aprobar un documento o aplicar una aprobación al documento.
* Revisar el documento en el visor de corrección

  Para obtener más información acerca de la revisión, consulte [Revisión](../../review-and-approve-work/proofing/proofing.md)

## Extraer un documento

Si tiene permisos de administración en un documento, puede extraerlo para prohibir determinadas acciones sobre el documento. 

1. Vaya al área donde está almacenado el documento y, a continuación, seleccione el documento. 

   Para obtener información sobre cómo añadir documentos, consulte [Añadir documentos a Adobe Workfront desde el sistema de archivos](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. Haga clic en el icono **Desproteger** ![Desproteger](assets/check-out-25x23.png).

1. Aparece un icono de candado ![Icono de candado](assets/lock-icon-locked-qs.png) a la derecha del nombre del documento. El documento permanece extraído después de cerrar la sesión de Workfront.
1. Solo el usuario que extrajo el documento o el administrador de Workfront pueden insertarlo.

## Administración de documentos extraídos

Tenga en cuenta lo siguiente sobre los documentos extraídos:

* Antes de poder eliminar un objeto en el que está almacenado un documento extraído, primero debe volver a insertarlo. 
* Si la persona con la función de administrador de Workfront elimina un usuario que ha desprotegido un documento que no era de su propiedad, Workfront protege automáticamente el documento.
* Si la persona con la función de administrador de Workfront elimina un usuario que ha desprotegido un documento de su propiedad y el documento se carga en un objeto, el documento permanece desprotegido. Solo una persona con la función de administrador de Workfront puede volver a protegerlo.
* Si la persona con la función de administrador de Workfront elimina un usuario que ha desprotegido un documento de su propiedad y el documento se carga solamente en el área Documentos (no en un objeto), el documento se elimina con el usuario.

  Para obtener información sobre la eliminación de usuarios, consulte [Eliminar usuarios](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Si la persona con la función de administrador de Workfront desactiva un usuario, todos los documentos que ha desprotegido permanecerán desprotegidos. Solo una persona con la función de administrador de Workfront puede volver a protegerlos. 

## Proteger un documento

Debe volver a proteger un documento para poder cargar una nueva versión o eliminarlo. 

Para proteger un documento:

1. Vaya al área donde está almacenado el documento y seleccione el documento. 

   Aparece un icono de candado ![Icono de candado](assets/lock-icon-locked-qs.png) a la derecha del nombre del documento.

1. Haga clic en el icono **Proteger** ![Proteger](assets/check-in-25x22.png).
