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
source-wordcount: '689'
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

&#42;Para averiguar qué plan, licencia o perfil de permiso de prueba tiene, póngase en contacto con el administrador de Workfront o Workfront Proof.

## Creación de una prueba de varias páginas

Cuando esta opción está habilitada, los archivos estáticos y los sitios web están disponibles en una sola prueba. Cuando esta opción está desactivada, todos los documentos y sitios web se generan como pruebas individuales y puede cargar hasta 100 archivos a la vez.

Para crear una prueba de varias páginas:

1. Vaya al proyecto, la tarea o el problema en el que desea la prueba y, a continuación, haga clic en el botón **Documentos** para obtener más información.
1. Haga clic en **Agregar nuevo** > **Prueba** .
1. Arrastre y suelte los archivos o navegue y selecciónelos en el explorador de archivos. Puede cargar hasta 50 archivos a la vez. Para obtener información sobre los límites de archivos, consulte la [Consideraciones](#considerations) en este artículo.

   >[!NOTE]
   >
   >Los archivos interactivos, incluidos los vídeos y los sitios web interactivos, no se pueden combinar en una sola prueba.

1. En **Prueba única**, habilite la opción , **Combinar todos los archivos compatibles en una sola prueba**.
1. En el **Nombre de la prueba** especifique un nuevo nombre para la prueba combinada.
1. (Opcional) En la lista de archivos que ha cargado, reordene los archivos arrastrándolos. El orden de los archivos es el orden de página de la prueba combinada.
1. (Opcional) Para eliminar un solo archivo de la página New proof , pase el ratón sobre el archivo y haga clic en el botón **Papelera** que aparece a la derecha.

   O

   Para eliminar todos los archivos cargados a la vez, haga clic en **Eliminar todo** en la esquina superior derecha de la lista.

1. Una vez cargados todos los archivos, debe decidir si desea configurar una prueba básica o una prueba automatizada:

   * Con una prueba básica, puede agregar tantos revisores como desee a una prueba, pero no están organizados en etapas. Todos los revisores que agregue pueden acceder a la prueba inmediatamente después de crearla. Para configurar una prueba básica, consulte [Creación de una prueba avanzada con un flujo de trabajo Básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * Con una prueba automatizada, la prueba pasa de un escenario a otro y Adobe Workfront notifica a cada usuario cuando le toca revisarla. para configurar una prueba automatizada, consulte [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Consideraciones {#considerations}

Tenga en cuenta lo siguiente cuando combine archivos en una sola prueba:

* Puede cargar hasta 500 archivos independientes.
* Puede combinar archivos estáticos de diferentes tipos (por ejemplo, PDF, JPG, DOC, PPT, EXC), hasta un total de 2000 páginas.
* Puede combinar capturas web estáticas.
* Puede combinar archivos GIF; sin embargo, los GIF animados se procesan como archivos estáticos.
* No se pueden combinar archivos AV y capturas web interactivas.
* La imagen en miniatura de la prueba se toma de la primera página de la prueba (consulte [Administrar detalles de prueba en la prueba de Workfront](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* Puede comprobar los nombres de los archivos combinados para crear la prueba en la página Detalles de la prueba . Para obtener más información, consulte [Administrar detalles de prueba en la prueba de Workfront](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* Si la opción para descargar los archivos originales está habilitada en la prueba, puede descargar todos los archivos combinados para crear la prueba como un archivo .zip. Para obtener más información, consulte  [Descargar archivos almacenados en la prueba de Workfront](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
