---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Probar un recurso vinculado con el conector mejorado
description: Una vez que haya vinculado un recurso desde Experience Manager Assets, puede crear una prueba y asignar usuarios para que revisen y agreguen comentarios al recurso.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d72ac84f-1865-4122-bc77-d8200a4d0f69
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Probar un recurso vinculado con el conector mejorado

Una vez que haya vinculado un recurso desde Experience Manager Assets, puede crear una prueba y asignar usuarios para que revisen y agreguen comentarios al recurso. Las pruebas creadas a partir de recursos vinculados se contabilizan en la cuota de almacenamiento de pruebas.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Debe tener Experience Manager Assets Essentials.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver acceso o superior</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de empezar, debe

* Instalación del conector mejorado de Workfront para Experience Manager

## Creación de una prueba

Puede crear pruebas estáticas, de vídeo o interactivas.

Para crear una prueba:

1. Vaya al proyecto, tarea o problema donde desee la prueba y, a continuación, haga clic en la sección **Documentos**.
1. Pase el ratón sobre el documento y luego haga clic en el vínculo **Crear revisión** que aparece debajo del nombre del documento.

   >[!NOTE]
   >
   >Si tiene **Generar revisiones automáticamente al cargar documentos** habilitados en su perfil de usuario, el sistema crea automáticamente una revisión simple.

1. Elija una de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Corrección simple</td> 
      <td>Esta opción crea una prueba sin flujo de trabajo adjunto y aplica la configuración de prueba predeterminada. Puede actualizar la configuración de revisión predeterminada o agregar un flujo de trabajo después de crear la revisión. Para obtener más información sobre la configuración de prueba, consulte <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Editar configuración de prueba</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Corrección avanzada</td> 
      <td> <p>Esta opción le permite configurar un flujo de trabajo Básico o Avanzado y modificar la configuración de prueba de la prueba que cree. Para obtener más información, consulte </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Crear una revisión avanzada con un flujo de trabajo básico</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Crear una revisión avanzada con un flujo de trabajo automatizado</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Administrar una revisión existente

Una vez creada una prueba, puede hacer cosas como

* Ver actividad de fase actual
* Actualizar revisores y plazos
* Edición del flujo de trabajo

Para obtener más información sobre cómo administrar una revisión existente, consulte [Administrar revisiones en Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Revisión de una prueba

Los revisores asignados pueden hacer cosas como

* Ver el recurso y hacer comentarios
* Agregar acciones a comentarios
* Comparar versiones
* Aprobar o rechazar la prueba

Para obtener más información acerca de lo que puede hacer con la herramienta de revisión, vea [Revisar pruebas en Adobe Workfront](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
