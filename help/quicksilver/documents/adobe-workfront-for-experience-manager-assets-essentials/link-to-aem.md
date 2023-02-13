---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Vincular recursos y carpetas desde Experience Manager Assets o Assets Essentials
description: Puede vincular un recurso o una carpeta de Experience Manager Assets o Assets Essentials a cualquier objeto de Adobe Workfront que admita documentos. Los recursos enviados desde Assets Essentials no se contabilizan en el almacenamiento general de documentos en Workfront. Los documentos cargados y enviados desde Workfront a Assets Essentials sí se contabilizan en el almacenamiento general.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Vincular recursos y carpetas desde Experience Manager Assets o Assets Essentials

Puede vincular un recurso o una carpeta de Experience Manager Assets o Assets Essentials a cualquier objeto de Adobe Workfront que admita documentos. Los recursos enviados desde Assets Essentials no se contabilizan en el almacenamiento general de documentos en Workfront. Los documentos cargados y enviados desde Workfront a Assets Essentials sí se contabilizan en el almacenamiento general.

Los campos de metadatos se asignan por primera vez al enviar un recurso de Workfront a Experience Manager Assets o Assets Essentials. Si el administrador de Workfront ha habilitado la sincronización de metadatos de objetos, los campos permanecen actualizados si se cambian en cualquiera de las aplicaciones.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Debe tener un Experience Manager as a Cloud Service o Assets Essentials, y debe agregarlo al producto como usuario en el Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Permisos de Experience Manager</td> 
    <td>Debe tener acceso de escritura a la carpeta .</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver acceso o superior</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de empezar,

* El administrador de Workfront debe configurar una integración de Experience Manager. Para obtener más información, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Vinculación de recursos desde Experience Manager Assets o Assets Essentials

Puede vincular un recurso de Experience Manager Assets o Assets Essentials a Workfront. Una vez que el recurso esté vinculado, puede

* [Prueba de un recurso vinculado para Experience Manager Assets o Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md)

1. Vaya a la **Documentos** en Workfront donde desee agregar el documento.
1. Select **Agregar nuevo** y, a continuación, seleccione la integración de Experience Manager que haya configurado el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que no puede mencionar específicamente Assets o Assets Essentials.

1. Seleccione los recursos que desee.

   ![](assets/select-an-asset.png)

1. Haga clic en **Select**.

## Vinculación de una carpeta desde Experience Manager Assets o Assets Essentials

Los permisos para ver recursos individuales dentro de una carpeta dependen de los permisos de Experience Manager Assets o Assets Essentials.

1. Vaya a la **Documentos** de Workfront donde desea la carpeta.
1. Select **Agregar nuevo** y, a continuación, seleccione la integración de Experience Manager que haya configurado el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que puede que no mencione específicamente Assets o Assets Essentials.

1. Seleccione las carpetas que desee.

   ![](assets/select-a-folder.png)

1. Haga clic en **Select**.

## Vinculación de una nueva versión desde Experience Manager Assets o Assets Essentials

Puede extraer un nuevo recurso de Assets Essentials y agregarlo a un recurso existente como una nueva versión. Si el documento ya está vinculado y se agrega una nueva versión en Assets Essentials, la nueva versión aparece automáticamente en Workfront.

Para vincular una nueva versión desde Assets Essentials:

1. Vaya a la **Documentos** en Workfront donde desee agregar el documento.
1. Seleccione el recurso que desea reemplazar con una nueva versión. No puede crear una nueva versión de un recurso en una carpeta vinculada.
1. Select **Agregar nuevo** > **Versión** y, a continuación, seleccione la integración de Experience Manager que haya configurado el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que puede que no mencione específicamente Assets o Assets Essentials.

1. Seleccione el recurso que desee.

   ![](assets/select-an-asset.png)

1. Haga clic en **Select**.

>[!TIP]
>
>Puede ver todas las versiones de un recurso si va a **Detalles del documento** > **Versiones**.
