---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Ver metadatos asignados para Experience Manager Assets o Assets Essentials
description: Puede ver una vista en tiempo real de los metadatos asignados en el panel Detalles del documento y Resumen de los documentos.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: cfad5855-033c-4a15-b5a2-7ff32ed65fe9
TQID: 'https://experienceleague.adobe.com/qLz7SnubnOZKoh1J66yIHui8fessEmy80fdrGKq2t4k'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 97%
---
# Ver metadatos asignados para Experience Manager Assets o Assets Essentials

Puede ver una vista en tiempo real de los metadatos asignados en el panel Detalles del documento y Resumen de los documentos. Los campos de metadatos se asignan por primera vez al enviar un recurso desde Workfront a Experience Manager Assets o a Assets Essentials. Si el administrador de Workfront ha habilitado la sincronización de metadatos de objetos, los campos permanecen actualizados si se modifican en alguna de las aplicaciones.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table>
  <tr>
   <td><strong>paquete de Adobe Workfront</strong>
   </td>
   <td>Cualquiera
   </td>
  </tr>
  <tr>
   <td><strong>licencias de Adobe Workfront</strong>
   </td>
   <td>
   <p>Colaborador o superior</p>
   <p>Solicitud o superior</p>
   </td>
  </tr>
  <tr>
   <td><strong>Productos adicionales</strong>
   </td>
   <td>Debe tener Experience Manager Assets as a Cloud Service o Assets Essentials, y debe estar añadido al producto como usuario en la Admin Console.
   </td>
  </tr>
  <tr>
   <td><strong>Configuraciones de nivel de acceso</strong>
   </td>
   <td><p>Acceso de edición a documentos</p>
   </td>
  </tr>
  <tr>
   <td><strong>Permisos de objeto</strong>
   </td>
   <td>Acceso de visualización o superior
   </td>
  </tr>
</table>


Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de comenzar,

* El administrador de Workfront debe configurar una integración de Experience Manager. Para obtener más información, consulte [Configuración de la integración de Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Detalles del documento

Para abrir el panel Metadatos en Detalles del documento:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.
1. Pase el puntero por encima del documento que necesita y luego seleccione **Detalles del documento**.
1. Busque y expanda la sección **Metadatos**.

   >[!NOTE]
   >
   >No puede editar campos en esta sección. Son de solo lectura.

![panel de detalles del documento](assets/metadata-panel-doc-details.png)


## Resumen de los documentos

Para abrir el panel Metadatos en el panel Resumen:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.
1. Busque el documento que necesita.
1. Haga clic en el **Icono de resumen** ![Icono de resumen](assets/summary-panel-icon.png) y, a continuación, expanda la sección **Metadatos**.

   >[!NOTE]
   >
   >No puede editar campos en esta sección. Son de solo lectura.

![resumen de documentos](assets/metadata-panel-summary.png)
