---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Crear una carpeta vinculada a Experience Manager Assets o Assets Essentials
description: Puede crear una carpeta vinculada a Experience Manager Assets o Assets Essentials en Workfront.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Crear una carpeta vinculada a Experience Manager Assets o Assets Essentials

Puede crear una carpeta vinculada a Experience Manager Assets o Assets Essentials en Workfront. Dado que la carpeta está vinculada, cualquier recurso añadido a ella se mostrará automáticamente tanto en Workfront como en Experience Manager. No es necesario que envíe manualmente el recurso si se encuentra en una carpeta vinculada.


## Requisitos de acceso

Debe tener lo siguiente:

<table>
  <tr>
   <td><strong>plan de Adobe Workfront*</strong>
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
   <td>Debe tener Experience Manager Assets as a Cloud Service o Assets Essentials, y debe agregarlo al producto como usuario.
   </td>
  </tr>
  <tr>
   <td><strong>Permisos del Experience Manager</strong>
   </td>
   <td>Debe tener acceso de escritura a la carpeta de destino en la integración de Experience Manager.
   </td>
  </tr>
  <tr>
   <td><strong>Configuraciones de nivel de acceso</strong>
   </td>
   <td>Debe ser administrador de Workfront. Para obtener información sobre los administradores de Workfront, consulte <strong>Conceder a un usuario acceso administrativo completo</strong>.
   </td>
  </tr>
</table>


*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.


## Requisitos previos

Antes de empezar,

* El administrador de Workfront debe configurar una integración de Experience Manager. Para obtener más información, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Crear una carpeta vinculada

La carpeta vinculada se crea en la ubicación especificada por el administrador de Workfront cuando configura la integración. Cada integración solo puede tener una ubicación de carpeta para las carpetas vinculadas.

El nombre de la carpeta vinculada se crea automáticamente en función del Portfolio, Programa, Proyecto asociado a y no se puede cambiar. Si el proyecto no está asociado a un Portfolio o Programa, la carpeta vinculada mostrará el nombre del proyecto y la fecha de creación.

Para crear una carpeta vinculada:



1. Vaya al proyecto en el que desea la carpeta.
1. Select **Agregar nuevo** y, a continuación, vaya a la integración de Experience Manager configurada por su administrador.
   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente Experience Manager Assets o Assets Essentials.

1. Select **Crear carpeta vinculada**. El sistema crea automáticamente una carpeta en el Experience Manager en función de la ubicación especificada cuando se configuró la integración.
   ![crear una carpeta vinculada](assets/linked-folder.png)
