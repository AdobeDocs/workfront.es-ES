---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Enviar un documento con el conector mejorado
description: Puede enviar documentos desde Workfront a Experience Manager Assets. Los documentos cargados y enviados desde Workfront a Experience Manager Assets siguen contando en el almacenamiento general de documentos. Los Assets vinculados desde Experience Manager Assets no cuentan para el almacenamiento general.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 44%

---

# Enviar un documento con el conector mejorado

Puede enviar documentos desde Workfront a Experience Manager Assets. Los documentos cargados y enviados desde Workfront a Experience Manager Assets siguen contando en el almacenamiento general de documentos. Los Assets vinculados desde Experience Manager Assets no cuentan para el almacenamiento general.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior</p>
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Productos adicionales</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a documentos</p> s="MCXref xref"&gt;Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso de visualización o superior en Documentos</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Requisitos previos

Antes de empezar, debe

* Instale el conector mejorado de Workfront para Experience Manager.

## Enviar un documento a Experience Manager Assets

Cuando un usuario envía un documento desde Workfront a Experience Manager Assets, los metadatos asignados se transfieren a lo largo del documento. Si se configura, los metadatos se sincronizan continuamente cada vez que se realiza un cambio.

Para enviar documentos:

1. Vaya al área **Documentos** de Workfront y seleccione el documento que quiera enviar.
1. Haga clic en **Enviar a** y, a continuación, elija la integración de Experience Manager Assets que configuró el administrador.

   >[!NOTE]
   >
   >Se puede elegir cualquier nombre para esta integración, por lo que no se puede mencionar específicamente a Experience Manager Assets.

   ![Enviar a](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Elija dónde desea que vaya el recurso y haga clic en **Seleccionar carpeta**.
1. Al encontrar el destino deseado, haga clic en **Guardar**.

## Enviar una nueva versión a Experience Manager Assets

Es posible añadir una nueva versión a un documento que se haya cargado anteriormente en Workfront. Para obtener más información, consulte [Cargar una nueva versión de un documento](../../../documents/managing-documents/upload-new-document-version.md). Una vez cargada la versión más reciente, puede enviarla a Experience Manager Assets. Si un campo asignado en Workfront ha cambiado, la nueva versión actualiza los metadatos en Experience Manager Assets cuando envía.

Para enviar la versión más reciente:

1. Vaya al área de **Documentos** en Workfront y busque el documento.
1. Haga clic en **Enviar a** y, a continuación, elija la integración de Experience Manager Assets que configuró el administrador.

   >[!NOTE]
   >
   >Se puede elegir cualquier nombre para esta integración, por lo que no se puede mencionar específicamente a Experience Manager Assets.

   ![Enviar a](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Haga clic en **Guardar**. La nueva versión se guarda en la misma ubicación que la versión anterior.
