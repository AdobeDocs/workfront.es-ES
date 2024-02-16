---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creación de una prueba para contenido interactivo en un archivo ZIP
description: Puede generar una prueba para el contenido interactivo que no sea de un sitio web y que se almacene en un archivo ZIP. Algunos ejemplos de este tipo de contenido web son los anuncios con flujo de vídeo o audio, las animaciones de HTML y los titulares interactivos.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# Creación de una prueba para contenido interactivo en un archivo ZIP

Puede generar una prueba para el contenido interactivo que no sea de un sitio web y que se almacene en un archivo ZIP. Algunos ejemplos de este tipo de contenido web son los anuncios con flujo de vídeo o audio, las animaciones de HTML y los titulares interactivos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o Superior</p> <p>o</p> <p>Plan heredado: Premium</p> <p>Para obtener más información sobre la revisión del acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
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
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de pruebas tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

## Creación de una prueba para contenido interactivo en un archivo ZIP

Una vez que se añade contenido interactivo en un archivo ZIP a una prueba, Adobe Workfront crea una prueba de los documentos comprimidos. Según el tamaño del archivo, el tiempo de carga puede variar. La creación de archivos más grandes tarda más. Puede salir de la página y Workfront seguirá creando el archivo. El tamaño máximo de carga de archivo es de 4 GB. 

1. Prepare el contenido creando un archivo agrupado ZIP.

   El archivo ZIP debe cumplir los siguientes requisitos:

   * Todos los recursos, como CSS, JavaScript, vídeos, sonidos e imágenes, deben incluirse en el archivo del paquete.
   * Asegúrese de que el archivo principal (como index.html, index.htm) se encuentra en la carpeta raíz y que es el único archivo .html/.htm almacenado allí.

     Si el archivo principal no se coloca en la carpeta raíz, Workfront busca en la carpeta para encontrar el archivo principal.

   * El tamaño máximo del paquete es 500 MB.
   * En el caso de los archivos ZIP creados en iOS, la herramienta identifica automáticamente la carpeta correcta en la que se coloca el contenido.

1. Vaya al proyecto, tarea o problema en el que desea cargar el archivo ZIP.
1. Clic **Documentos** en el panel izquierdo
1. Clic **Añadir nuevo**, luego haga clic en **Proof** en el menú que aparece.
1. En el **Agregar archivos** , arrastre y suelte o busque el archivo ZIP que necesite.
1. Clic **Crear revisión** para crear una prueba simple sin proceso de revisión.\
   o\
   Siga configurando una revisión avanzada:

   * [Creación de una prueba avanzada con un flujo de trabajo básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
