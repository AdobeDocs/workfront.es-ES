---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Vincular recursos y carpetas desde Experience Manager Assets o Assets Essentials
description: Puede vincular un recurso o una carpeta desde Experience Manager Assets o Assets Essentials a cualquier objeto de Adobe Workfront que admita documentos. Assets enviado por los Assets Essentials no cuenta para el almacenamiento general de documentos en Workfront. Los documentos cargados y enviados desde Workfront a los Assets Essentials no se contabilizan en el almacenamiento general.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: b87839d6c6dbfe978a3e14ef4b448560742f95c3
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---

# Vincular recursos y carpetas desde Experience Manager Assets o Assets Essentials

Puede vincular un recurso o una carpeta desde Experience Manager Assets o Assets Essentials a cualquier objeto de Adobe Workfront que admita documentos. Assets enviado por los Assets Essentials no cuenta para el almacenamiento general de documentos en Workfront. Los documentos cargados y enviados desde Workfront a los Assets Essentials no se contabilizan en el almacenamiento general.

Los campos de metadatos se asignan por primera vez al enviar un recurso desde Workfront a Experience Manager Assets o a los Assets Essentials. Si el administrador de Workfront ha activado la sincronización de metadatos de objeto, los campos permanecen actualizados si se cambian en alguna de las aplicaciones.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Debe tener Assets Essentials as a Cloud Service Experience Manager y se le debe agregar al producto como usuario en el Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Permisos de Experience Manager</td> 
    <td>Debe tener acceso de escritura a la carpeta.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver acceso o superior</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Requisitos previos

Antes de empezar,

* El administrador de Workfront debe configurar una integración de Experience Manager. Para obtener más información, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Vincular un recurso desde Experience Manager Assets o Assets Essentials

Puede vincular un recurso de Experience Manager Assets o de Assets Essentials a Workfront. Una vez vinculado el recurso, puede

* [Probar un recurso vinculado para Experience Manager Assets o Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md)

1. Vaya al área de **Documentos** de Workfront donde desea agregar el documento.
1. Seleccione **Agregar nuevo** y luego seleccione la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente a Assets ni a los Assets Essentials.

1. Seleccione los recursos que desee.

   ![](assets/select-an-asset.png)

1. Haga clic en **Seleccionar**.

## Vincular una carpeta desde Experience Manager Assets o Assets Essentials

Los permisos para ver recursos individuales dentro de una carpeta dependen de los permisos de Experience Manager Assets o de los Assets Essentials.

1. Vaya al área de **Documentos** de Workfront donde desee colocar la carpeta.
1. Seleccione **Agregar nuevo** y luego seleccione la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente a Assets ni a los Assets Essentials.

1. Seleccione las carpetas que desee.

   ![](assets/select-a-folder.png)

1. Haga clic en **Seleccionar**.

## Vincular una nueva versión desde Experience Manager Assets o Assets Essentials

Puede extraer un nuevo recurso de los Assets Essentials y añadirlo a un recurso existente como una nueva versión. Si el documento ya está vinculado y se agrega una nueva versión en los Assets Essentials, la nueva versión aparece automáticamente en Workfront.

Para vincular una nueva versión desde Assets Essentials:

1. Vaya al área de **Documentos** de Workfront donde desea agregar el documento.
1. Seleccione el recurso que desea reemplazar con una nueva versión. No puede crear una nueva versión de un recurso en una carpeta vinculada.
1. Seleccione **Agregar nuevo** > **Versión** y, a continuación, seleccione la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente a Assets ni a los Assets Essentials.

1. Seleccione el recurso que desee.

   ![](assets/select-an-asset.png)

1. Haga clic en **Seleccionar**.

>[!TIP]
>
>Puede ver todas las versiones de un recurso si va a **Detalles del documento** > **Versiones**.
