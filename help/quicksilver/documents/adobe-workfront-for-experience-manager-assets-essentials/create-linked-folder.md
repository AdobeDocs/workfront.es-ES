---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Cree una carpeta vinculada a Experience Manager Assets o a Assets Essentials
description: Puede crear una carpeta vinculada a Experience Manager Assets o a Assets Essentials en Workfront.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 1744e6f2b78c64ba2fa4856d9c6a0611404e4458
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# Cree una carpeta vinculada a Experience Manager Assets o a Assets Essentials

Puede crear una carpeta vinculada a Experience Manager Assets o a Assets Essentials en Workfront. Como la carpeta está vinculada, cualquier recurso agregado a la carpeta se mostrará automáticamente en Workfront y Experience Manager. No es necesario que envíe manualmente el recurso si está en una carpeta vinculada.


## Requisitos de acceso

Debe tener lo siguiente:

<table>
  <tr>
   <td><strong>plan Adobe Workfront*</strong>
   </td>
   <td>Cualquiera
   </td>
  </tr>
  <tr>
   <td><strong>Licencias de Adobe Workfront*</strong>
   </td>
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong>Product</strong>
   </td>
   <td>Debe tener Experience Manager Assets as a Cloud Service o Assets Essentials y se le debe añadir al producto como usuario.
   </td>
  </tr>
  <tr>
   <td><strong>Permisos de Experience Manager</strong>
   </td>
   <td>Debe tener acceso de escritura a la carpeta de destino en la integración de Experience Manager.
   </td>
  </tr>
  <tr>
   <td><strong>Configuraciones de nivel de acceso</strong>
   </td>
   <td>Debe ser administrador de Workfront para configurar una integración de Experience Manager. Una vez configurada, los usuarios con una licencia de planificación pueden configurar carpetas vinculadas en proyectos individuales.
   </td>
  </tr>
</table>


*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.


## Requisitos previos

Antes de empezar,

* El administrador de Workfront debe configurar una integración de Experience Manager. Para obtener más información, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Crear una carpeta vinculada

La carpeta vinculada se crea en la ubicación especificada por el administrador de Workfront cuando configura la integración. Cada integración solo puede tener una ubicación de carpeta para las carpetas vinculadas.

El nombre de la carpeta vinculada se crea automáticamente en función del Portfolio, el programa o el proyecto con el que esté asociado y no se puede cambiar. Si el proyecto no está asociado a un Portfolio o a un programa, la carpeta vinculada mostrará el nombre del proyecto y la fecha de creación.

Para crear una carpeta vinculada:



1. Vaya al proyecto donde desee colocar la carpeta.
1. Seleccionar **Añadir nuevo** y, a continuación, vaya a la integración de Experience Manager que configuró su administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente a Experience Manager Assets ni a los Assets Essentials.

1. Seleccionar **Crear carpeta vinculada**. El sistema crea automáticamente una carpeta en Experience Manager en función de la ubicación especificada cuando se configuró la integración.
   ![crear una carpeta vinculada](assets/linked-folder.png)
