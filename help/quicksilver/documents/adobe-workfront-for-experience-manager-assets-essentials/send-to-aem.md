---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Enviar un documento a Experience Manager Assets o Assets Essentials
description: Puede enviar documentos de Workfront a Experience Manager Assets o Assets Essentials. Los documentos cargados y enviados desde Workfront a Assets Essentials aún se cuentan en el almacenamiento general de documentos. Los recursos vinculados desde Assets Essentials no se contabilizan en el almacenamiento general.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 6bedca2f3394fadc6d6ffbb34654fd1f0194a5d6
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Enviar un documento a Experience Manager Assets o Assets Essentials


Puede enviar documentos de Workfront a Experience Manager Assets o Assets Essentials. Los documentos cargados y enviados desde Workfront a Assets Essentials aún se cuentan en el almacenamiento general de documentos. Los recursos vinculados desde Assets Essentials no se contabilizan en el almacenamiento general.

Los campos de metadatos se asignan por primera vez al enviar un recurso de Workfront a Experience Manager Assets o Assets Essentials. También se envían los metadatos configurados para asignar objetos principales. Para obtener más información sobre la configuración de la asignación de metadatos, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Ejemplo** Cuando envía por primera vez un recurso adjunto a una tarea, los metadatos de la tarea se asignan a Experience Manager Assets o Assets Essentials, así como los metadatos asignados de objetos principales como un proyecto, un portafolio y un programa.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plan de Adobe Workfront</a>*</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre las licencias de Adobe Workfront</a>*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Debe tener un Experience Manager as a Cloud Service o Assets Essentials, y debe agregarlo al producto como usuario en el Admin Console.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver acceso o superior en Documentos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de empezar,

* El administrador de Workfront debe configurar una integración de Experience Manager. Para obtener más información, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Enviar un documento desde Workfront

Cuando un usuario envía un documento de Workfront a Experience Manager Assets o Assets Essentials, se asignan transferencias de metadatos a lo largo del documento. Una vez enviado el documento, los cambios realizados en los metadatos del documento en Workfront no se reflejan en Assets ni en Assets Essentials. Si se cambia un campo asignado en Workfront, debe enviar una nueva versión del documento con los metadatos actualizados a Assets o Assets Essentials. Para configurar o editar metadatos, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Para enviar un documento:

1. Vaya a la **Documentos** en Workfront y seleccione el documento que desea enviar.
1. Haga clic en **Enviar a** y, a continuación, elija la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que no puede mencionar específicamente Assets o Assets Essentials.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Elija dónde desea que se dirija el recurso y haga clic en **Seleccionar carpeta**.
1. Cuando encuentre el destino deseado, haga clic en **Guardar**.

## Enviar una nueva versión

Puede agregar una nueva versión a un documento que haya cargado previamente en Workfront. Para obtener más información, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md). Una vez cargada la última versión, puede enviarla a Assets Essentials. Si un campo asignado en Workfront ha cambiado, la nueva versión actualiza los metadatos en Assets Essentials cuando se envían.

>[!IMPORTANT]
>
>Antes de cargar una nueva versión en Workfront, se recomienda cambiar el nombre del archivo. Si carga una versión nueva con el mismo nombre de archivo que una versión anterior, solo se puede descargar la versión más reciente de Workfront. Todas las versiones se pueden descargar desde Experience Manager Assets o Assets Essentials independientemente del nombre del archivo.

Para enviar la versión más reciente:

1. Vaya a la **Documentos** en Workfront y busque el documento.
1. Select **Enviar a** y, a continuación, elija la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que puede que no mencione específicamente Assets o Assets Essentials.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Haga clic en **Guardar**. La nueva versión se guarda en la misma ubicación que la versión anterior.
