---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Probar un recurso vinculado con el conector mejorado
description: Una vez que haya vinculado un recurso desde Experience Manager Assets, puede crear una prueba y asignar usuarios para que revisen y añadan comentarios al recurso.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d72ac84f-1865-4122-bc77-d8200a4d0f69
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 98%

---

# Probar un recurso vinculado con el conector mejorado

Una vez que haya vinculado un recurso desde Experience Manager Assets, puede crear una prueba y asignar usuarios para que revisen y añadan comentarios al recurso. Las pruebas creadas a partir de recursos vinculados se contabilizan en la cuota de almacenamiento de pruebas.

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
   <p>Estándar</p>
   <p>Trabajo o superior</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Productos adicionales</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a documentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver el acceso o superior en un documento</p> </td> 
  </tr> 
 </tbody> 
</table>


Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de empezar, debe

* Instalar el conector mejorado de Workfront para Experience Manager

## Crear una prueba

Puede crear pruebas estáticas, de vídeo o interactivas.

Para crear una prueba:

1. Vaya al proyecto, tarea o problema donde desee la prueba y, a continuación, haga clic en la sección **Documentos**.
1. Pase el puntero por encima del documento y luego haga clic en el vínculo **Crear prueba** que aparece debajo del nombre del documento.

   >[!NOTE]
   >
   >Si tiene la opción **Generar pruebas automáticamente al cargar documentos** habilitada en su perfil de usuario, el sistema crea automáticamente una prueba simple.

1. Seleccione una de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prueba sencilla</td> 
      <td>Esta opción crea una prueba sin flujo de trabajo adjunto y aplica la configuración de prueba predeterminada. Puede actualizar la configuración de prueba predeterminada o añadir un flujo de trabajo después de crear la prueba. Para obtener más información sobre la configuración de la prueba, consulte <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Editar configuración de prueba</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prueba avanzada</td> 
      <td> <p>Esta opción le permite configurar un flujo de trabajo Básico o Avanzado y modificar la configuración de prueba de la prueba que cree. Para obtener más información, consulte </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Crear una prueba avanzada con un flujo de trabajo básico</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Crear una prueba avanzada con un flujo de trabajo automatizado</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Administrar una prueba existente

Una vez creada una prueba, puede hacer cosas como

* Ver actividad de fase actual
* Actualizar revisores y plazos
* Editar el flujo de trabajo

Para obtener más información sobre cómo administrar una prueba existente, consulte [Administrar pruebas en Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Revisión de una prueba

Los revisores asignados pueden hacer cosas como

* Ver el recurso y hacer comentarios
* Añadir acciones a comentarios
* Comparar versiones
* Aprobar o rechazar la prueba

Para obtener más información sobre lo que se puede hacer con la herramienta de revisión, consulte [Revisar pruebas en Adobe Workfront](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
