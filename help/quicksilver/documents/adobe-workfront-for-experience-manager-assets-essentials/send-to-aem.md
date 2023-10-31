---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Enviar un documento a Experience Manager Assets o a los Assets Essentials
description: Puede enviar documentos desde Workfront a Experience Manager Assets o a Assets Essentials. Los documentos cargados y enviados desde Workfront a los Assets Essentials siguen contando en el almacenamiento general de documentos. Los recursos vinculados desde Assets Essentials no se contabilizan en el almacenamiento general.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 24ffde1850a005428a3f619fc00842a8779bbc6d
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 0%

---

# Enviar un documento a Experience Manager Assets o a los Assets Essentials

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>

Puede enviar documentos desde Workfront a Experience Manager Assets o a Assets Essentials. Los documentos cargados y enviados desde Workfront a los Assets Essentials siguen contando en el almacenamiento general de documentos. Los recursos vinculados desde Assets Essentials no se contabilizan en el almacenamiento general.

Los campos de metadatos se asignan por primera vez al enviar un recurso desde Workfront a Experience Manager Assets o a los Assets Essentials. También se envían los metadatos configurados para asignar a objetos principales. Para obtener más información sobre la configuración de la asignación de metadatos, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Ejemplo** Cuando envía por primera vez un recurso adjunto a una tarea, los metadatos de la tarea se asignan a Experience Manager Assets o a Assets Essentials, así como cualquier metadato asignado de objetos principales como un proyecto, portafolio y programa.

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
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Resumen de licencias heredadas</a>*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Debe tener Experience Manager as a Cloud Service o Assets Essentials, y se le debe añadir al producto como usuario en el Admin Console.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver acceso o superior en Documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Requisitos previos

Antes de empezar,

* El administrador de Workfront debe configurar una integración de Experience Manager. Para obtener más información, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Enviar un documento desde Workfront

Cuando un usuario envía un documento desde Workfront a Experience Manager Assets o a Assets Essentials, los metadatos asignados se transfieren a lo largo del documento. Una vez enviado el documento, los cambios realizados en los metadatos del documento en Workfront no se reflejarán en Assets ni en Assets Essentials. Si se cambia un campo asignado en Workfront, se debe enviar una nueva versión del documento con los metadatos actualizados a Assets o a Assets Essentials. Para configurar o editar metadatos, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Para enviar un documento:

1. Vaya a la **Documentos** en Workfront y seleccione el documento que desee enviar.
1. Clic **Enviar a** y, a continuación, elija la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente Recursos o Assets Essentials.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Elija a dónde desea que vaya el recurso y haga clic en **Seleccionar carpeta**.
1. Cuando encuentre el destino deseado, haga clic en **Guardar**.

## Enviar una nueva versión

Puede agregar una nueva versión a un documento que haya cargado anteriormente en Workfront. Para obtener más información, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md). Una vez cargada la versión más reciente, puede enviarla a los Assets Essentials. Si un campo asignado en Workfront ha cambiado, la nueva versión actualiza los metadatos en los Assets Essentials cuando envía.

>[!IMPORTANT]
>
>Antes de cargar una nueva versión en Workfront, le recomendamos que cambie el nombre del archivo. Si carga una nueva versión con el mismo nombre de archivo que una versión anterior, solo se puede descargar la versión más reciente desde Workfront. Todas las versiones se pueden descargar desde Experience Manager Assets o Assets Essentials independientemente del nombre del archivo.

Para enviar la versión más reciente:

1. Vaya a la **Documentos** en Workfront y busque el documento.
1. Seleccionar **Enviar a** y, a continuación, elija la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente Recursos o Assets Essentials.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Haga clic en **Guardar**. La nueva versión se guarda en la misma ubicación que la versión anterior.

## Mover un documento a una carpeta vinculada en Experience Manager Assets

>[!NOTE]
>
>Esta funcionalidad solo está disponible para Experience Manager Assets as a Cloud Service. No está disponible para Experience Manager Assets Essentials.

Puede mover un documento a una carpeta vinculada en Experience Manager Assets si el documento y la carpeta vinculada están en la misma lista de documentos (como el área de documento de un proyecto).

1. Busque el documento que desea mover.
1. Arrastre y suelte el documento en la carpeta de Experience Manager Assets vinculada a la que desea moverlo.

<div class="preview">Las opciones de documento no están disponibles mientras el documento se está moviendo. Una vez que el documento se ha movido a Experience Manager Assets, ya no estará visible en la lista de documentos de Workfront.

>[!NOTE]
>
> Las acciones o ediciones que realice en el documento mientras se mueve no aparecerán en el documento en Experience Manager Assets y, por lo tanto, se perderán.
</div>
