---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Vincular recursos y carpetas desde Experience Manager Assets o Assets Essentials
description: Puede vincular un recurso o una carpeta desde Experience Manager Assets o Assets Essentials a cualquier objeto de Adobe Workfront que admita documentos. Los recursos enviados desde Assets Essentials no cuentan para el almacenamiento general de documentos en Workfront. Los documentos cargados y enviados desde Workfront a Assets Essentials no se contabilizan en el almacenamiento general.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 97%

---

# Vincular recursos y carpetas desde Experience Manager Assets o Assets Essentials

Puede vincular un recurso o una carpeta desde Experience Manager Assets o Assets Essentials a cualquier objeto de Adobe Workfront que admita documentos. Los recursos enviados desde Assets Essentials no cuentan para el almacenamiento general de documentos en Workfront. Los documentos cargados y enviados desde Workfront a Assets Essentials no se contabilizan en el almacenamiento general.

Los campos de metadatos se asignan por primera vez al enviar un recurso desde Workfront a Experience Manager Assets o a Assets Essentials. Si el administrador de Workfront ha habilitado la sincronización de metadatos de objetos, los campos permanecen actualizados si se modifican en alguna de las aplicaciones.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior</p> 
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Productos adicionales</td> 
   <td>Debe tener Experience Manager as a Cloud Service o Assets Essentials, además de estar añadido al producto como usuario en Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Permisos de Experience Manager</td> 
    <td>Debe tener acceso de escritura a la carpeta.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso de visualización o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de comenzar,

* El administrador de Workfront debe configurar una integración de Experience Manager. Para obtener más información, consulte [Configuración de la integración de Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Vincular un recurso desde Experience Manager Assets o Assets Essentials

Puede vincular un recurso desde Experience Manager Assets o desde Assets Essentials a Workfront. Una vez vinculado el recurso, puede

* [Probar un recurso vinculado para Experience Manager Assets o Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md)

1. Vaya al área de **Documentos** de Workfront donde desea añadir el documento.
1. Seleccione **Añadir nuevo** y luego, la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente los recursos ni a Assets Essentials.

1. Seleccione los recursos que desee.

   ![Seleccionar un recurso](assets/select-an-asset.png)

1. Haga clic en **Seleccionar**.

## Vincular una carpeta desde Experience Manager Assets o Assets Essentials

Los permisos para ver recursos individuales dentro de una carpeta dependen de los permisos de Experience Manager Assets o de Assets Essentials.

1. Vaya al área de **Documentos** de Workfront donde desee colocar la carpeta.
1. Seleccione **Añadir nuevo** y luego seleccione la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente los recursos ni a Assets Essentials.

1. Seleccione las carpetas que desee.

   ![Seleccionar una carpeta](assets/select-a-folder.png)

1. Haga clic en **Seleccionar**.

## Vincular una nueva versión desde Experience Manager Assets o Assets Essentials

Puede extraer un nuevo recurso de Assets Essentials y añadirlo a un recurso existente como una nueva versión. Si el documento ya está vinculado y se añade una nueva versión en Assets Essentials, la nueva versión aparecerá automáticamente en Workfront.

Para vincular una nueva versión desde Assets Essentials:

1. Vaya al área de **Documentos** de Workfront donde desea añadir el documento.
1. Seleccione el recurso que desea reemplazar con una nueva versión. No puede crear una nueva versión de un recurso en una carpeta vinculada.
1. Seleccione **Añadir nuevo**> **Versión** y, a continuación, seleccione la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente los recursos ni a Assets Essentials.

1. Seleccione el recurso que desee.

   ![Seleccionar un recurso](assets/select-an-asset.png)

1. Haga clic en **Seleccionar**.

>[!TIP]
>
>Puede ver todas las versiones de un recurso si va a **Detalles del documento**> **Versiones**.
