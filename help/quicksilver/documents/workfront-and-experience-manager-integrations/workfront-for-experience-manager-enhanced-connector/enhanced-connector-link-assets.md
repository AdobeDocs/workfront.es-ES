---
title: Vinculación de recursos y carpetas con el conector mejorado
description: Puede vincular un recurso o una carpeta desde Experience Manager Assets a cualquier objeto de Workfront que admita documentos.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: dd8718b00a310bee6caa13db7644b86174b476f4
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---


# Vinculación de recursos y carpetas con el conector mejorado

Puede vincular un recurso o una carpeta desde Experience Manager Assets a cualquier objeto de Workfront que admita documentos. Assets enviado desde Experience Manager Assets no cuenta para el almacenamiento general de documentos en Workfront. Los documentos cargados y enviados desde Workfront a Experience Manager Assets no se contabilizan en el almacenamiento general.


>[!NOTE]
>
>Los archivos de Excel vinculados a través del conector mejorado no se pueden previsualizar en Workfront. Debe descargar el archivo para acceder a él.

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
   <td> <p>Actual: Solicitud o superior</p> 
   o
   <p>Nuevo: Colaborador o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver el acceso o superior en un documento</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.
+++

## Requisitos previos

Antes de empezar, debe

* Instalación del conector mejorado de Workfront para Experience Manager

## Vincular un recurso desde Experience Manager Assets

Puede vincular un recurso de Experience Manager Assets a Workfront. Una vez vinculado el recurso, puede

* [Probar un recurso vinculado para Experience Manager Assets](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [Cargar una nueva versión de un documento](../../../documents/managing-documents/upload-new-document-version.md)

Para vincular un recurso a Experience Manager Assets:

1. Vaya al área de **Documentos** de Workfront donde desea agregar el documento.
1. Haga clic en **Agregar nuevo** y, a continuación, elija la integración de Experience Manager Assets que configuró el administrador.

   >[!NOTE]
   >
   >Se puede elegir cualquier nombre para esta integración, por lo que no se puede mencionar específicamente a Experience Manager Assets.

1. Seleccione los recursos que desee.

   ![](assets/select-an-asset.png)

1. Haga clic en **Vínculo**.

## Vincular una carpeta desde Experience Manager Assets

Los permisos para ver recursos individuales dentro de una carpeta dependen de los permisos de Experience Manager Assets.

Para vincular una carpeta a Experience Manager Assets:

1. Vaya al área de **Documentos** de Workfront donde desea agregar el documento.
1. Haga clic en **Agregar nuevo** y, a continuación, elija la integración de Experience Manager Assets que configuró el administrador.

   >[!NOTE]
   >
   >Se puede elegir cualquier nombre para esta integración, por lo que no se puede mencionar específicamente a Experience Manager Assets.

1. Seleccione las carpetas que desee.

   ![](assets/select-a-folder.png)

1. Haga clic en **Vínculo**.

## Vincular una nueva versión desde Experience Manager Assets

Puede extraer un nuevo recurso de Experience Manager Assets y añadirlo a un recurso existente como una nueva versión en Workfront. Si el documento ya está vinculado y se agrega una nueva versión en Experience Manager Assets, la nueva versión aparece automáticamente en Workfront.

>[!TIP]
>
>Puede ver todas las versiones de un recurso si va a **Detalles del documento** > **Versiones**.

Para vincular una nueva versión desde Experience Manager Assets:

1. Vaya al área de **Documentos** de Workfront donde desea agregar el documento.
1. Seleccione el recurso que desea reemplazar con una nueva versión. No puede crear una nueva versión de un recurso en una carpeta vinculada.
1. Haga clic en **Agregar nuevo** y, a continuación, elija la integración de Experience Manager Assets que configuró el administrador.

   >[!NOTE]
   >
   >Se puede elegir cualquier nombre para esta integración, por lo que no se puede mencionar específicamente a Experience Manager Assets.

1. Seleccione el recurso que desee.

   ![](assets/select-an-asset.png)

1. Haga clic en **Vínculo**.
