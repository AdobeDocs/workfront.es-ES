---
product-area: documents
navigation-topic: manage-documents
title: Ver documentos
description: Puede extraer un documento para evitar que otros usuarios lo eliminen o carguen una nueva versión de él. Solo un usuario puede extraer un documento a la vez. Puede consultar cualquier documento cargado en Adobe Workfront, así como documentos vinculados a proveedores de documentos de terceros (Caja, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint o cualquier otro proveedor personalizado).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Ver documentos

Puede extraer un documento para evitar que otros usuarios lo eliminen o carguen una nueva versión de él. Solo un usuario puede extraer un documento a la vez. Puede consultar cualquier documento cargado en Adobe Workfront, así como documentos vinculados a proveedores de documentos de terceros (Caja, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint o cualquier otro proveedor personalizado). 

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar el acceso al documento</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Acciones permitidas en documentos retirados

Los usuarios con acceso de administración al documento pueden hacer lo siguiente:

* Editar el documento (nombre del documento, descripción, datos personalizados)
* Mover el documento
* Compartir el documento
* Vista previa del documento
* Descargar el documento

   >[!TIP]
   >
   > Aunque un usuario puede descargar un documento cuando otro usuario lo desprotege, se recomienda que los usuarios esperen hasta que el documento se haya recuperado antes de descargarlo. Cuando se retira un documento, a menudo indica que aún se está trabajando en él. Esperar hasta que se vuelva a proteger un documento para descargarlo garantiza que el usuario tenga la versión más reciente.

* Aprobar un documento o aplicar una aprobación al documento.
* Revise el documento en el visor de pruebas

   Para obtener más información sobre pruebas, consulte [Prueba](../../review-and-approve-work/proofing/proofing.md)

## Extracción de un documento

Si tiene permisos de gestión para un documento, puede comprobarlo para prohibir ciertas acciones en el documento. 

1. Vaya al área donde está almacenado el documento y seleccione el documento. 

   Para obtener información sobre cómo agregar documentos, consulte [Agregar documentos a Adobe Workfront desde el sistema de archivos](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. Haga clic en el **Comprobar** icono ![](assets/check-out-25x23.png).

1. Icono de candado ![](assets/lock-icon-locked-qs.png) se muestra a la derecha del nombre del documento. El documento permanece desprotegido después de cerrar la sesión de Workfront.
1. Solo el usuario que ha extraído el documento o el administrador de Workfront pueden proteger el documento.

## Administrar documentos retirados

Tenga en cuenta lo siguiente sobre los documentos desprotegidos:

* Para poder eliminar un objeto en el que está almacenado un documento desprotegido, primero debe volver a proteger el documento. 
* Si el administrador de Workfront elimina un usuario que ha retirado un documento que no era de su propiedad, Workfront comprueba automáticamente el documento.
* Si el administrador de Workfront elimina a un usuario que ha extraído un documento que posee y el documento se carga en un objeto, el documento permanece desprotegido. Solo los administradores de Workfront pueden volver a comprobarlo.
* Si el administrador de Workfront elimina a un usuario que ha extraído un documento que posee y el documento solo se carga en el área Documentos (no en un objeto), el documento se elimina con el usuario.

   Para obtener información sobre la eliminación de usuarios, consulte [Eliminar usuarios](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Si el administrador de Workfront desactiva un usuario, los documentos que haya extraído permanecerán desprotegidos. Solo los administradores de Workfront pueden volver a iniciarlos. 

## Comprobar un documento en

Debe volver a proteger un documento antes de poder cargar una nueva versión o eliminarla. 

Para proteger un documento:

1. Vaya al área donde está almacenado el documento y seleccione el documento. 

   Icono de candado ![](assets/lock-icon-locked-qs.png) se muestra a la derecha del nombre del documento.

1. Haga clic en el **Proteger** icono ![](assets/check-in-25x22.png).
