---
product-area: documents
navigation-topic: manage-documents
title: Desproteger documentos
description: Puede retirar un documento para evitar que otros usuarios lo eliminen o carguen una nueva versión. Sólo un usuario puede desproteger un documento a la vez. Puede retirar cualquier documento cargado en Adobe Workfront, así como documentos vinculados a proveedores de documentos de terceros (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint o cualquier otro proveedor personalizado).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: 9aa6822c9c1ecade776d4c71b113c1afd997f40c
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Desproteger documentos

Puede retirar un documento para evitar que otros usuarios lo eliminen o carguen una nueva versión. Sólo un usuario puede desproteger un documento a la vez. Puede retirar cualquier documento cargado en Adobe Workfront, así como documentos vinculados a proveedores de documentos de terceros (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint o cualquier otro proveedor personalizado). 

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar el acceso al documento</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Acciones permitidas en los documentos retirados

Los usuarios con acceso de administración al documento pueden hacer lo siguiente:

* Editar el documento (nombre del documento, descripción, datos personalizados)
* Mover el documento
* Compartir el documento
* Previsualizar el documento
* Descargar el documento

  >[!TIP]
  >
  > Aunque un usuario puede descargar un documento cuando está desprotegido por otro usuario, se recomienda que los usuarios esperen hasta que el documento se vuelva a proteger antes de descargarlo. Cuando un documento está desprotegido, a menudo indica que se está trabajando en él. Si se espera hasta que se vuelva a registrar un documento para descargarlo, se garantiza que el usuario tenga la versión más reciente.

* Aprobar un documento o aplicar una aprobación al documento.
* Revisar el documento en el visor de revisión

  Para obtener más información acerca de la revisión, vea [Revisión](../../review-and-approve-work/proofing/proofing.md)

## Extraer un documento

Si tiene permisos de administración en un documento, puede desprotegerlo para prohibir ciertas acciones en el documento. 

1. Vaya al área donde está almacenado el documento y, a continuación, seleccione el documento. 

   Para obtener información sobre cómo agregar documentos, consulte [Agregar documentos a Adobe Workfront desde el sistema de archivos](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. Haga clic en el icono **Desproteger** ![](assets/check-out-25x23.png).

1. Aparece un icono de candado ![](assets/lock-icon-locked-qs.png) a la derecha del nombre del documento. El documento permanece desprotegido después de cerrar la sesión de Workfront.
1. Sólo el usuario que desprotegió el documento o el administrador de Workfront pueden proteger el documento.

## Administrar documentos retirados

Tenga en cuenta lo siguiente sobre los documentos desprotegidos:

* Antes de poder eliminar un objeto en el que está almacenado un documento extraído, primero debe volver a archivar el documento. 
* Si el administrador de Workfront elimina un usuario que ha retirado un documento que no era de su propiedad, Workfront registra automáticamente el documento.
* Si el administrador de Workfront elimina un usuario que ha extraído un documento de su propiedad y el documento se carga en un objeto, el documento permanece extraído. Solo un administrador de Workfront puede volver a protegerlo.
* Si el administrador de Workfront elimina un usuario que ha retirado un documento de su propiedad y el documento se carga solamente en el área Documentos (no en un objeto), el documento se elimina con el usuario.

  Para obtener información sobre cómo eliminar usuarios, consulte [Eliminar usuarios](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Si el administrador de Workfront desactiva un usuario, todos los documentos que haya retirado permanecerán desprotegidos. Solo un administrador de Workfront puede volver a registrarlos. 

## Proteger un documento

Debe volver a proteger un documento para poder cargar una nueva versión o eliminarlo. 

Para registrar un documento:

1. Vaya al área donde está almacenado el documento y seleccione el documento. 

   Aparece un icono de candado ![](assets/lock-icon-locked-qs.png) a la derecha del nombre del documento.

1. Haga clic en el icono **Proteger** ![](assets/check-in-25x22.png).
