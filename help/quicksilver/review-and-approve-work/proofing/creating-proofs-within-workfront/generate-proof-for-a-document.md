---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Crear una prueba para un documento
description: Puede generar una prueba para un documento en el momento en que lo está cargando en Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Crear una prueba para un documento

Puede generar una prueba para un documento en el momento en que lo está cargando en Workfront.

También puede generar una prueba para un documento ya cargado en Adobe Workfront o para una nueva versión de una prueba que ya esté en Workfront.

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o superior</p> <p>o</p> <p>Plan heredado: Select o Premium</p> <p>Para obtener más información sobre la prueba de acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de pruebas en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o plan</p> <p>Plan heredado: Cualquiera (debe tener las pruebas habilitadas para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Administrador o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con el administrador de Workfront o Workfront Proof.

## Cargar un documento y crear una prueba

1. Vaya al proyecto, la tarea o el problema en el que desea crear una prueba nueva.
1. Haga clic en el **Documentos** pestaña .
1. Haga clic en Documentos ![](assets/document-icon.png) en el panel izquierdo.
1. Haga clic en **Agregar nuevo** y haga clic en **Prueba** en el menú que aparece.

   >[!TIP]
   >
   >Puede habilitar la variable **Generar pruebas automáticamente al cargar documentos** en su perfil de usuario para automatizar este proceso. Para obtener más información, consulte [Configurar mis ajustes](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) .

1. En el **Nueva prueba** que aparece, puede

   * [Creación de una prueba avanzada con un flujo de trabajo Básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Cargar un documento y crear una nueva versión de una prueba

1. Vaya al proyecto, la tarea o el problema en el que desea crear una nueva versión de una prueba existente.
1. Haga clic en el **Documentos** pestaña .
1. Seleccione el documento en el que desea agregar una versión nueva.
1. Haga clic en **Agregar nuevo** > **Versión** > **Prueba**.
1. En el **Nueva versión de prueba** que aparece, puede

   * [Creación de una prueba avanzada con un flujo de trabajo Básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Utilice la función de arrastrar y soltar para generar una prueba sencilla de una nueva versión

Puede arrastrar y soltar un documento desde el sistema de archivos (como el escritorio) para crear una nueva prueba o una nueva versión de una prueba existente. La prueba contiene la siguiente configuración, en función de si está creando una prueba nueva o una versión nueva:

* **Nueva prueba:** Crea una prueba sencilla que solo se comparte con usted. Puede modificar la configuración de uso compartido después de crear la prueba como se describe en [Editar configuración de prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* **Nueva versión de la prueba existente:** Crea una nueva versión con la misma configuración de prueba que la versión anterior.

Para usar arrastrar y soltar para generar una nueva prueba o una nueva versión de prueba:

1. Asegúrese de que las pruebas estén configuradas para que se generen automáticamente, como se describe en .
1. Continuar con  [Agregar documentos a Adobe Workfront desde el sistema de archivos](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md), que explica el método de arrastrar y soltar para agregar documentos. 

## Crear una prueba para un documento existente

1. Vaya al proyecto, la tarea o el problema en el que desea la prueba y, a continuación, haga clic en el botón **Documentos** para obtener más información.
1. Pase el ratón sobre el documento y haga clic en la **Crear prueba** vínculo que aparece debajo del nombre del documento.

   >[!NOTE]
   >
   >Si tiene **Generar pruebas automáticamente al cargar documentos** activado en el perfil de usuario, el sistema crea automáticamente una prueba sencilla.

1. Elija una de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prueba simple</td> 
      <td>Esta opción crea una prueba sin flujo de trabajo adjunto y aplica la configuración de prueba predeterminada. Puede actualizar la configuración de pruebas predeterminada o agregar un flujo de trabajo después de crear la prueba. Para obtener más información sobre la configuración de prueba, consulte <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Editar configuración de prueba</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prueba avanzada</td> 
      <td> <p>Esta opción le permite configurar un flujo de trabajo Básico o Avanzado y modificar la configuración de prueba para la prueba que cree. Para obtener más información, consulte </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Creación de una prueba avanzada con un flujo de trabajo Básico</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Creación de una prueba avanzada con un flujo de trabajo automatizado</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
