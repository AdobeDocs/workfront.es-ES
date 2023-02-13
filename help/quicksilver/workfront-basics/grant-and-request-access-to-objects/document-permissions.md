---
title: Compartir un documento
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar documentos cuando asignen niveles de acceso, tal como se explica en Conceder acceso a documentos.
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 4%

---

# Compartir un documento

El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar documentos cuando asignen niveles de acceso, tal como se explica en [Concesión de acceso a documentos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

El nivel de acceso que el administrador de Workfront concede a los usuarios les permite ver o editar documentos. Además de esto, otros usuarios también pueden conceder a otros permisos para ver o administrar documentos específicos que ellos mismos cargaron o que tienen acceso a compartir.

Los permisos son específicos para un elemento de Workfront y definen qué acciones se pueden realizar en ese elemento. Para obtener información sobre los permisos de objetos, consulte [Información general sobre cómo compartir permisos en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

De forma predeterminada, el usuario que carga un documento en Workfront tiene permisos de administración.

Para obtener información sobre cómo compartir una carpeta de documento completa, consulte [Compartir una carpeta de documento](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Consideraciones sobre el uso compartido de documentos

Además de las consideraciones siguientes, consulte [Información general sobre cómo compartir permisos en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Un administrador de Workfront puede agregar o quitar permisos para cualquier elemento del sistema, para todos los usuarios, sin ser el propietario de esos elementos.

* Compartir un documento es similar a compartir cualquier otro objeto en Workfront. Para obtener información sobre cómo compartir documentos en Workfront, consulte [Compartir un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Puede conceder los siguientes permisos a los documentos:

   * Vista
   * Administrar

* También puede compartir un documento de forma pública o en todo el sistema.

   >[!CAUTION]
   >
   >Se recomienda tener cuidado al compartir un objeto que contenga información confidencial con usuarios externos. Esto les permite ver información sin ser usuarios de Workfront ni formar parte de su organización.

* Puede compartir un documento con alguien que no tenga una cuenta de Workfront agregando su dirección de correo electrónico al campo Dar acceso al documento .
* Cuando comparte un documento, los usuarios tienen el mismo acceso a todas las versiones del documento y a todas las pruebas del documento.\
   Para obtener más información sobre las pruebas en Workfront, consulte la [Prueba](../../review-and-approve-work/proofing/proofing.md) para obtener más información.

* Puede heredar permisos para documentos de los objetos a los que están asociados. El administrador de Workfront puede restringir la herencia de permisos para documentos en el nivel de acceso.

   Para obtener más información sobre la restricción de permisos heredados en documentos, consulte [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

   Puede quitar manualmente los permisos heredados de los documentos. Para obtener más información, consulte [Eliminación de permisos de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Un documento adjunto hereda los permisos únicamente del objeto al que estaba adjunto. Si crea una carpeta en el objeto y mueve el documento a la carpeta, heredará los permisos de la carpeta. Sin embargo, si crea una carpeta en un objeto principal o principal y mueve el documento a esa carpeta, no heredará los permisos de esa carpeta.

## Permisos del documento

La tabla siguiente muestra los permisos que puede conceder a los usuarios cuando les permite ver o administrar documentos:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Acción</strong> </p> </th> 
   <th> <p><strong>Administrar</strong> </p> </th> 
   <th> <p><strong>Vista</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Crear</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Editar detalles del documento</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Eliminar*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Descargar</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Cierre de compra</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Agregar aprobadores</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aprobar documento</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Adjuntar formulario personalizado</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Editar campos personalizados</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Mover a (objeto)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Enviar a (integración)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Actualizaciones/ Comentarios</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Cargar nueva versión</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Eliminar versión</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ver documentos</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Vista previa</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Proof**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Generar revisión**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Eliminar revisión**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Compartir*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Compartir en todo el sistema*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Compartir documentos públicamente*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Compartir con una dirección de correo electrónico externa</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Agregar o quitar</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Cambiar nombre</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Vínculo (con integración)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Desvincular (con integración)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; La acción la comparten tanto Documents como Document Folders.

&#42;&#42; Debe tener una licencia de prueba independiente asociada a su cuenta de Workfront para poder probar los documentos. Póngase en contacto con el administrador de cuentas para obtener una licencia de prueba. Para obtener más información sobre las pruebas en Workfront, consulte [Prueba](../../review-and-approve-work/proofing/proofing.md).
