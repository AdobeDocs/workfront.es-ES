---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Enviar un documento con el conector mejorado
description: Puede enviar documentos de Workfront a Experience Manager Assets. Los documentos cargados y enviados desde Workfront a Experience Manager Assets aún se cuentan en el almacenamiento general de documentos. Los recursos vinculados desde Experience Manager Assets no se contabilizan en el almacenamiento general.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 1%

---

# Enviar un documento con el conector mejorado

Puede enviar documentos de Workfront a Experience Manager Assets. Los documentos cargados y enviados desde Workfront a Experience Manager Assets aún se cuentan en el almacenamiento general de documentos. Los recursos vinculados desde Experience Manager Assets no se contabilizan en el almacenamiento general.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver acceso o superior en Documentos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de empezar, debe

* Instale Workfront para el conector mejorado del Experience Manager.

## Enviar un documento a Experience Manager Assets

Cuando un usuario envía un documento de Workfront a Experience Manager Assets, se asignan transferencias de metadatos a lo largo del documento. Si se configura, los metadatos se sincronizan continuamente cada vez que se realiza un cambio.

Para enviar un documento:

1. Vaya a la **Documentos** en Workfront y seleccione el documento que desea enviar.
1. Haga clic en **Enviar a** y, a continuación, elija la integración de Experience Manager Assets que configuró el administrador.

   >[!NOTE]
   >
   >Se puede elegir cualquier nombre para esta integración, por lo que no se puede mencionar específicamente Experience Manager Assets.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Elija dónde desea que se dirija el recurso y haga clic en **Seleccionar carpeta**.
1. Cuando encuentre el destino deseado, haga clic en **Guardar**.

## Enviar una nueva versión a Experience Manager Assets

Puede agregar una nueva versión a un documento que haya cargado previamente en Workfront. Para obtener más información, consulte [Cargar una nueva versión de un documento](../../../documents/managing-documents/upload-new-document-version.md). Una vez cargada la última versión, puede enviarla a Experience Manager Assets. Si un campo asignado en Workfront ha cambiado, la nueva versión actualiza los metadatos en Experience Manager Assets cuando se envían.

Para enviar la versión más reciente:

1. Vaya a la **Documentos** en Workfront y busque el documento.
1. Haga clic en **Enviar a** y, a continuación, elija la integración de Experience Manager Assets que configuró el administrador.

   >[!NOTE]
   >
   >Se puede elegir cualquier nombre para esta integración, por lo que no se puede mencionar específicamente Experience Manager Assets.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Haga clic en **Guardar**. La nueva versión se guarda en la misma ubicación que la versión anterior.
