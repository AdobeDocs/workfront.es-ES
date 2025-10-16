---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Crear una prueba de varias páginas
description: Puede combinar varios archivos en una sola prueba de varias páginas. Los revisores pueden utilizar las herramientas de navegación del visor de pruebas para navegar por las páginas en una prueba de varias páginas.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 99%

---

# Crear una prueba de varias páginas

Puede combinar varios archivos en una sola prueba de varias páginas. Los revisores pueden utilizar las herramientas de navegación del visor de pruebas para navegar por las páginas en una prueba de varias páginas.

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
    <p>Trabajo o plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de prueba </td> 
   <td>Administrador o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a documentos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una prueba de varias páginas

Cuando esta opción está habilitada, los archivos estáticos y los sitios web están disponibles en una sola prueba. Cuando esta opción está desactivada, todos los documentos y sitios web se generan como pruebas individuales y se pueden cargar hasta 100 archivos a la vez.

Para crear una prueba de varias páginas:

1. Vaya al proyecto, tarea o problema donde desee la prueba y, a continuación, haga clic en la sección **Documentos**.
1. Haga clic en **Añadir nuevo** > **Revisión** .
1. Arrastre y suelte los archivos o examine y selecciónelos en el explorador de archivos. Puedes cargar hasta 50 archivos a la vez. Para obtener información sobre los límites de archivos, consulte la sección [Consideraciones](#considerations) en este artículo.

   >[!NOTE]
   >
   >Los archivos interactivos, incluidos los vídeos y los sitios web interactivos, no se pueden combinar en una sola prueba.

1. En **Una sola revisión**, habilite la opción **Combinar todos los archivos compatibles en una sola revisión**.
1. En el campo **Nombre de revisión**, especifique un nombre nuevo para la revisión combinada.
1. (Opcional) En la lista de archivos que ha cargado, reordene los archivos arrastrándolos. El orden de los archivos es el orden de páginas de la prueba combinada.
1. (Opcional) Para eliminar un solo archivo de la página de Nueva prueba, pase el puntero por encima del archivo y haga clic en el icono de **Papelera** que aparece a la derecha.

   O

   Para eliminar todos los archivos cargados a la vez, haga clic en **Eliminar todo** en la esquina superior derecha de la lista.

1. Una vez cargados todos los archivos, debe decidir si desea configurar una prueba básica o automatizada:

   * Con una prueba básica, puede añadir tantos revisores como desee a una prueba, pero no están organizados en fases. Todos los revisores que añada podrán acceder a la prueba inmediatamente después de crearla. Para configurar una revisión básica, consulte [Crear una revisión avanzada con un flujo de trabajo básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * Con una revisión automatizada, la revisión pasa de una fase a otra y Adobe Workfront notifica a cada usuario cuándo es su turno de revisarla. para configurar una revisión automatizada, consulte [Crear una revisión avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Consideraciones {#considerations}

Tenga en cuenta lo siguiente al combinar archivos en una sola prueba:

* Puede cargar hasta 500 archivos independientes.
* Puede combinar archivos estáticos de diferentes tipos (por ejemplo, PDF, JPG, DOC, PPT, EXC), hasta un total de 2000 páginas.
* Puede combinar capturas web estáticas.
* Puede combinar archivos de GIF; sin embargo, los GIF animados se procesan como archivos estáticos.
* No se pueden combinar archivos AV con capturas Web interactivas.
* La imagen en miniatura de la revisión se toma de la primera página (vea [Administrar detalles de revisión en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* Puede comprobar los nombres de los archivos combinados para crear la prueba en la página Detalles de revisión. Para obtener más información, consulte [Administrar detalles de revisión en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* Si la opción para descargar los archivos originales está habilitada en la prueba, puedes descargar todos los archivos que se han combinado para crear la prueba en un archivo .zip. Para obtener más información, consulte  [Descargar archivos almacenados en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
