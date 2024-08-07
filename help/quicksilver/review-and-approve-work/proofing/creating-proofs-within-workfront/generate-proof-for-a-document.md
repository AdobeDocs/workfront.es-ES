---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creación de una prueba para un documento
description: Puede generar una prueba para un documento en el momento en que lo esté cargando en Workfront. También puede generar una prueba para un documento ya cargado en Adobe Workfront o para una nueva versión de una prueba ya cargada en Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---

# Creación de una prueba para un documento

<!-- Audited: 1/2024 -->

Puede generar una prueba para un documento en el momento en que lo esté cargando en Workfront.

También puede generar una prueba para un documento ya cargado en Adobe Workfront o para una nueva versión de una prueba ya cargada en Workfront.

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> 
   <p>Nuevo: Cualquiera </p>
   <p>Actual: Pro o Superior</p> <p>Plan heredado: Select o Premium</p> <p>Para obtener más información sobre cómo revisar el acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Nuevo: estándar</p>
   <p>Actual : Trabajo o Plan</p> <p>Plan heredado: Cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Responsable o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cargar un documento y crear una prueba

1. Vaya al proyecto, tarea o problema en el que desea crear una nueva prueba.
1. Haga clic en la ficha **Documentos**.
1. Haga clic en Documentos ![](assets/document-icon.png) en el panel izquierdo.
1. Haga clic en **Agregar nuevo** y, a continuación, haga clic en **Revisión** en el menú que aparece.

   >[!TIP]
   >
   >Puede habilitar la configuración **Generar revisiones automáticamente al cargar documentos** en su perfil de usuario para automatizar este proceso. Para obtener más información, consulte [Configurar mis opciones](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) .

1. En la página **Nueva revisión** que aparece, puede

   * [Crear una revisión avanzada con un flujo de trabajo básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Cargar un documento y crear una nueva versión de una prueba

1. Vaya al proyecto, tarea o problema en el que desea crear una nueva versión de una revisión existente.
1. Haga clic en la ficha **Documentos**.
1. Seleccione el documento en el que desea agregar una nueva versión.
1. Haga clic en **Agregar nuevo** > **Versión** > **Revisión**.
1. En la página **Nueva versión de revisión** que aparece, puede

   * [Crear una revisión avanzada con un flujo de trabajo básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Utilice arrastrar y soltar para generar una prueba sencilla para una nueva versión

Puede arrastrar y soltar un documento desde el sistema de archivos (como el escritorio) para crear una nueva prueba o una nueva versión de una prueba existente. La prueba contiene la siguiente configuración, en función de si va a crear una nueva prueba o una nueva versión:

* **Nueva revisión:** Crea una revisión simple que se comparte solamente con usted. Puede modificar la configuración del recurso compartido una vez que se haya creado la revisión tal como se describe en [Editar la configuración de la revisión](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* **Nueva versión de revisión existente:** Crea una nueva versión con la misma configuración de revisión que la versión anterior.

Para usar arrastrar y soltar para generar una nueva prueba o versión:

1. Asegúrese de que las pruebas estén configuradas para generarse automáticamente, tal como se describe en
1. Continuar con  [Agregue documentos a Adobe Workfront desde su sistema de archivos](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md), lo que explica el método de arrastrar y soltar para agregar documentos. 

## Crear una prueba para un documento existente

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
