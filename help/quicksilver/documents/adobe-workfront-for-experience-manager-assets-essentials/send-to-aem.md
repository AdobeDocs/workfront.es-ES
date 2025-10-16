---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Enviar documentos a Experience Manager Assets o Assets Essentials
description: Es posible enviar documentos desde Workfront a Experience Manager Assets o Assets Essentials. Los documentos cargados y enviados desde Workfront a Assets Essentials siguen contando en el almacenamiento general de documentos. Los recursos vinculados de Assets Essentials no se contabilizan en el almacenamiento general.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '868'
ht-degree: 98%

---

# Enviar documentos a Experience Manager Assets o Assets Essentials

Es posible enviar documentos desde Workfront a Experience Manager Assets o Assets Essentials. Los documentos cargados y enviados desde Workfront a Assets Essentials siguen contando en el almacenamiento general de documentos. Los recursos vinculados de Assets Essentials no se contabilizan en el almacenamiento general.

Los recursos que se envíen a Experience Manager mediante esta integración tendrán un límite de tamaño de **5 GB**.

En el entorno de vista previa, los recursos enviados a Experience Manager mediante esta integración tendrán un límite de tamaño de **30 GB**.

Los campos de metadatos se asignan por primera vez al enviar un recurso desde Workfront a Experience Manager Assets o a Assets Essentials. También se envían los metadatos configurados para asignar a objetos principales. Para obtener más información sobre la configuración de la asignación de metadatos, consulte [Configuración de la integración de Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Ejemplo**: cuando se envía por primera vez un recurso adjunto a una tarea, los metadatos de esta se asignan a Experience Manager Assets o Assets Essentials, así como cualquier metadato asignado de objetos principales, como proyectos, portafolios y programas.

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


## Enviar documentos desde Workfront

Cuando un usuario envía un documento desde Workfront a Experience Manager Assets o a Assets Essentials, los metadatos asignados se transfieren a lo largo del documento. Una vez enviado el documento, los cambios realizados en los metadatos del documento en Workfront no se reflejarán en Assets ni en Assets Essentials. Al cambiar campos asignados en Workfront, es necesario enviar una nueva versión del documento con los metadatos actualizados a Assets o a Assets Essentials. Para configurar o editar metadatos, consulte [Configuración de la integración de Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Para enviar documentos:

1. Vaya al área **Documentos** de Workfront y seleccione el documento que quiera enviar.
1. Haga clic en **Enviar a** y, a continuación, elija la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente los recursos ni a Assets Essentials.

   ![Enviar a](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Elija dónde desea que vaya el recurso y haga clic en **Seleccionar carpeta**.
1. Al encontrar el destino deseado, haga clic en **Guardar**.

## Enviar una nueva versión

Es posible añadir una nueva versión a un documento que se haya cargado anteriormente en Workfront. Para obtener más información, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md). Una vez cargada la versión más reciente, puede enviarla a Assets Essentials. Si un campo asignado en Workfront ha cambiado, la nueva versión actualiza los metadatos en Assets Essentials cuando los envía.

>[!IMPORTANT]
>
>Antes de cargar una nueva versión en Workfront, le recomendamos que cambie el nombre del archivo. Si carga una nueva versión con el mismo nombre de archivo que una versión anterior, solo se puede descargar la versión más reciente desde Workfront. Todas las versiones se pueden descargar desde Experience Manager Assets o Assets Essentials, independientemente del nombre del archivo.

Para enviar la versión más reciente:

1. Vaya al área de **Documentos** en Workfront y busque el documento.
1. Seleccione **Enviar a** y, a continuación, elija la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente los recursos ni a Assets Essentials.

   ![Enviar a](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Haga clic en **Guardar**. La nueva versión se guarda en la misma ubicación que la versión anterior.

## Mover un documento a una carpeta vinculada en Experience Manager Assets

>[!NOTE]
>
>Esta funcionalidad solo está disponible para Experience Manager Assets as a Cloud Service. No está disponible para Experience Manager Assets Essentials.

Puede mover un documento a una carpeta vinculada en Experience Manager Assets si el documento y la carpeta vinculada están en la misma lista de documentos (como el área de documento de un proyecto).

1. Busque el documento que desea mover.
1. Arrastre y suelte el documento en la carpeta de Experience Manager Assets vinculada a la que desea moverlo.

Las opciones de documento no están disponibles mientras el documento está en proceso de traslado. Una vez que el documento se ha movido a Experience Manager Assets, ya no estará visible en la lista de documentos de Workfront.

>[!NOTE]
>
> Las acciones o ediciones que realice en el documento mientras se mueve no aparecerán en el documento en Experience Manager Assets y, por lo tanto, se perderán.

