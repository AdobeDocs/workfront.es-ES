---
product-area: documents
navigation-topic: manage-documents
title: Comprobar límites de almacenamiento de documentos
description: Como administrador de Adobe Workfront, puede ver el uso y la cuota de almacenamiento de documentos en la página Información del cliente. La forma en que aparece el almacenamiento depende de si su organización utiliza el almacenamiento heredado de Workfront o el almacenamiento empresarial de Adobe.
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7b6d24d6a5b7fd052a3e7c97034e920e771022a6
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 19%

---

# Comprobar límites de almacenamiento de documentos

{{highlighted-preview}}

Aunque no hay restricciones en los tipos y tamaños de archivos individuales que los usuarios pueden cargar en la instancia de Workfront, su plan de Workfront incluye una cuota de almacenamiento total. Como administrador de Workfront, supervisa el uso y la cuota desde el área de Configuración en la página Información del cliente.

La forma en que aparece el almacenamiento depende de si su organización utiliza el almacenamiento heredado de Workfront o el almacenamiento empresarial de Adobe:

* Si usa almacenamiento heredado de Workfront, consulte [Almacenamiento heredado de Workfront](#legacy-workfront-storage) en este artículo.
* Si usa el almacenamiento empresarial de Adobe, consulte [almacenamiento empresarial de Adobe](#adobe-enterprise-storage) en este artículo.

  Para obtener más información acerca del almacenamiento empresarial, consulte [Descripción general del almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Plan de Workfront</td> 
   <td> <p>Cualquier paquete de Workfront para administrar documentos mediante el almacenamiento heredado</p>
      <p>Cualquier paquete de flujo de trabajo para administrar documentos mediante el almacenamiento empresarial de Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Almacenamiento de Workfront heredado

Si su organización utiliza almacenamiento de Workfront heredado, la página Información del cliente muestra una única cuota de almacenamiento para los documentos cargados directamente en Workfront.

Para comprobar el almacenamiento de documentos heredado de Workfront:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Sistema** > **Información del cliente**.
1. En la sección **Información básica**, busque **Cuota de almacenamiento**. Aquí puede ver la cantidad de almacenamiento que está utilizando actualmente, así como la cantidad total de almacenamiento que incluye su plan de Workfront.

La cuota de almacenamiento se actualiza diariamente para mostrar el recuento más actualizado.

>[!NOTE]
>
>Este límite no se aplica a los documentos que vincule a Workfront desde cualquier otro proveedor de servicios de terceros (SharePoint, Google Drive, Webdam, Box, Dropbox o cualquier otro proveedor de administración de recursos de documentos).

<div class="preview">

## almacenamiento empresarial de Adobe

<!--
If your organization uses Adobe enterprise storage, your storage quota is reported as a single pooled allocation that combines storage provisioned through your V2 Workfront SKU and any storage provisioned through a Frame.io Enterprise SKU or add-on. There's no hard cap on storage usage; users can continue uploading documents even when usage exceeds your quota.

Beginning with the May 2026 release, you can view your pooled storage quota and a usage breakdown on the Customer Info page.

-->

### Ver el uso del almacenamiento en Información del cliente

Para comprobar el almacenamiento de documentos empresariales de Adobe:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Sistema** > **Información del cliente**.
1. Vaya a la sección **Información general sobre almacenamiento**.
1. Revise su uso. La Información general de almacenamiento muestra la cuota de almacenamiento agrupada y desglosa el uso en:

   * Los proyectos heredados de Workfront y los proyectos de Adobe enterprise storage se muestran en la barra azul.
   * Los proyectos independientes de marco se muestran en la barra verde. Estos proyectos son independientes de Workfront y solo están disponibles si tiene una licencia de Frame.io Enterprise.


![Uso de almacenamiento empresarial de Adobe en la información del cliente](assets/storage-usage.png)

Las cifras de uso se actualizan regularmente para que vea un recuento actualizado.

### Notificaciones por correo electrónico para administradores

Cuando el uso supera el 75 %, el 90 % o el 100 % de la cuota de almacenamiento, Workfront envía una notificación por correo electrónico a los administradores del sistema.

</div>