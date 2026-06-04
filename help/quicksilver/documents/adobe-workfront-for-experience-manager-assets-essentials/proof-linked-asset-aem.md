---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Probar un recurso vinculado para Experience Manager Assets o Assets Essentials
description: Después de haber vinculado un recurso desde Experience Manager Assets Essentials, puede crear una prueba y asignar usuarios para que revisen y añadan comentarios al recurso.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
TQID: https://experienceleague.adobe.com/adxs5pYRdr8p6SSjnGCXnHwSNKcJl3qGZjkbp764NfM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 452
ht-degree: 79%

---

# Probar un recurso vinculado para Experience Manager Assets o Assets Essentials

Después de haber vinculado un recurso desde Experience Manager Assets Essentials, puede crear una prueba y asignar usuarios para que revisen y añadan comentarios al recurso.

>[!NOTE]
>
>Esta funcionalidad no está disponible en el área de documentos nuevos.<br>
>Si su organización utiliza el almacenamiento en la nube de Adobe, verá el área de Documentos nuevos cuando acceda a documentos en Workfront. Desde allí, puede añadir recursos de Experience Manager Assets y revisarlos y aprobarlos con el visor de Frame.io. Para obtener más información, consulte [Usar Adobe Experience Manager con la integración de Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

## Requisitos de acceso

<!-- Audited: 4/2025 -->

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront</td> 
   <td> 
   <p>Estándar</p>
   <p>Trabajo o superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Productos adicionales</td> 
   <td>Debe tener Experience Manager as a Cloud Service o Assets Essentials, además de estar añadido al producto como usuario en Admin Console. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso de visualización o superior</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de empezar:

* El administrador de Workfront debe configurar una integración de Experience Manager. Para obtener más información, consulte [Configuración de la integración Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Crear una prueba

Puede crear pruebas estáticas, de vídeo o interactivas.

Para crear una prueba:

1. Vaya al proyecto, tarea o problema donde desee la prueba y, a continuación, haga clic en la sección **Documentos**.
1. Pase el puntero por encima del documento y luego haga clic en el vínculo **Crear prueba** que aparece debajo del nombre del documento.

   >[!NOTE]
   >
   >Si tiene la opción **Generar pruebas automáticamente al cargar documentos** habilitada en su perfil de usuario, el sistema crea automáticamente una prueba simple.

1. Elija una de las siguientes opciones de la lista desplegable:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Prueba sencilla</strong></td> 
      <td>Esta opción crea una prueba sin flujo de trabajo adjunto y aplica la configuración de prueba predeterminada. Puede actualizar la configuración de prueba predeterminada o agregar un flujo de trabajo después de crear la prueba. Para obtener más información sobre la configuración de la prueba, consulte <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Editar configuración de prueba</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prueba avanzada</strong></td> 
      <td> <p>Esta opción le permite configurar un flujo de trabajo Básico o Avanzado y modificar la configuración de prueba de la prueba que cree. Para obtener más información, consulte lo siguiente: </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Crear una prueba avanzada con un flujo de trabajo básico</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Crear una prueba avanzada con un flujo de trabajo automatizado</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Administrar una prueba existente

Una vez creada una prueba, puede hacer lo siguiente:

* Ver actividad de fase actual
* Actualizar revisores y plazos
* Editar el flujo de trabajo

Para obtener más información sobre cómo administrar una revisión existente, consulte [Administrar revisiones en Adobe Workfront: índice de artículos](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Revisión de una prueba

Los revisores asignados pueden hacer lo siguiente:

* Ver el recurso y hacer comentarios
* Añadir acciones a comentarios
* Comparar versiones
* Aprobar o rechazar la prueba

Para obtener más información acerca de lo que puede hacer con la herramienta de revisión, vea [Revisar pruebas en Adobe Workfront: índice de artículos](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
