---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creación de una prueba de varias páginas
description: Puede combinar varios archivos en una sola prueba de varias páginas. Los revisores pueden utilizar las herramientas de navegación del visor de pruebas para navegar por las páginas en una prueba de varias páginas.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# Creación de una prueba de varias páginas

Puede combinar varios archivos en una sola prueba de varias páginas. Los revisores pueden utilizar las herramientas de navegación del visor de pruebas para navegar por las páginas en una prueba de varias páginas.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o Superior</p> <p>o</p> <p>Plan heredado: Select o Premium</p> <p>Para obtener más información sobre cómo revisar el acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o Plan</p> <p>Plan heredado: Cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Responsable o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, licencia o perfil de permiso de revisión tiene, comuníquese con el administrador de Workfront o de Workfront Proof.

## Creación de una prueba de varias páginas

Cuando esta opción está habilitada, los archivos estáticos y los sitios web están disponibles en una sola prueba. Cuando esta opción está desactivada, todos los documentos y sitios web se generan como pruebas individuales y se pueden cargar hasta 100 archivos a la vez.

Para crear una prueba de varias páginas:

1. Vaya al proyecto, tarea o problema donde desee la prueba y, a continuación, haga clic en la sección **Documentos**.
1. Haga clic en **Agregar nuevo** > **Revisión** .
1. Arrastre y suelte los archivos o examine y selecciónelos en el explorador de archivos. Puede cargar hasta 50 archivos a la vez. Para obtener información sobre los límites de archivos, consulte la sección [Consideraciones](#considerations) en este artículo.

   >[!NOTE]
   >
   >Los archivos interactivos, incluidos los vídeos y los sitios web interactivos, no se pueden combinar en una sola prueba.

1. En **Una sola revisión**, habilite la opción **Combinar todos los archivos compatibles en una sola revisión**.
1. En el campo **Nombre de revisión**, especifique un nombre nuevo para la revisión combinada.
1. (Opcional) En la lista de archivos que ha cargado, reordene los archivos arrastrándolos. El orden de los archivos es el orden de páginas de la prueba combinada.
1. (Opcional) Para eliminar un solo archivo de la página Nueva prueba, pase el ratón sobre el archivo y haga clic en el icono **Papelera** que aparece a la derecha.

   O

   Para eliminar todos los archivos cargados a la vez, haga clic en **Eliminar todo** en la esquina superior derecha de la lista.

1. Una vez cargados todos los archivos, debe decidir si desea configurar una prueba básica o automatizada:

   * Con una prueba básica, puede agregar tantos revisores como desee a una prueba, pero no están organizados en fases. Todos los revisores que agregue podrán acceder a la prueba inmediatamente después de crearla. Para configurar una revisión básica, consulte [Crear una revisión avanzada con un flujo de trabajo básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * Con una revisión automatizada, la revisión pasa de una fase a otra y Adobe Workfront notifica a cada usuario cuándo es su turno de revisarla. para configurar una revisión automatizada, consulte [Crear una revisión avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Consideraciones {#considerations}

Tenga en cuenta lo siguiente al combinar archivos en una sola prueba:

* Puede cargar hasta 500 archivos independientes.
* Puede combinar archivos estáticos de diferentes tipos (por ejemplo, PDF, JPG, DOCUMENTO, PPT, EXC), hasta un total de 2000 páginas.
* Puede combinar capturas web estáticas.
* Puede combinar archivos de GIF; sin embargo, los GIF animados se procesan como archivos estáticos.
* No se pueden combinar archivos AV con capturas Web interactivas.
* La imagen en miniatura de la revisión se toma de la primera página (vea [Administrar detalles de revisión en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* Puede comprobar los nombres de los archivos combinados para crear la prueba en la página Detalles de la prueba. Para obtener más información, consulte [Administrar detalles de revisión en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* Si la opción para descargar los archivos originales está activada en la prueba, puede descargar todos los archivos que se hayan combinado para crear la prueba como archivo .zip. Para obtener más información, consulte  [Descargar archivos almacenados en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
