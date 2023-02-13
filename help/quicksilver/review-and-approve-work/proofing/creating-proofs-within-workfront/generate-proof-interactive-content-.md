---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Crear una prueba de contenido interactivo en un archivo ZIP
description: Puede generar una prueba del contenido interactivo que no sea del sitio web y que esté almacenado en un archivo ZIP. Algunos ejemplos de este tipo de contenido web son los anuncios con vídeo o audio de flujo continuo, las animaciones del HTML y los banners interactivos.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# Crear una prueba de contenido interactivo en un archivo ZIP

Puede generar una prueba del contenido interactivo que no sea del sitio web y que esté almacenado en un archivo ZIP. Algunos ejemplos de este tipo de contenido web son los anuncios con vídeo o audio de flujo continuo, las animaciones del HTML y los banners interactivos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o superior</p> <p>o</p> <p>Plan heredado: Premium</p> <p>Para obtener más información sobre la prueba de acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de pruebas en Workfront</a>.</p> </td> 
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

## Crear una prueba de contenido interactivo en un archivo ZIP

Una vez que se añade contenido interactivo en un archivo ZIP a una prueba, Adobe Workfront crea una prueba de los documentos comprimidos. El tiempo de carga puede variar en función del tamaño del archivo. Los archivos más grandes tardan más en crearse. Puede salir de la página y Workfront seguirá creando el archivo. El tamaño máximo de carga de archivos es de 4 GB. 

1. Prepare su contenido creando un archivo ZIP empaquetado.

   El archivo ZIP debe cumplir los siguientes requisitos:

   * Todos los recursos, como CSS, JavaScript, vídeos, sonidos e imágenes, deben incluirse en el archivo del paquete.
   * Asegúrese de que el archivo principal (como index.html, index.htm) se encuentra en la carpeta raíz y que es el único archivo .html/.htm que se almacena allí.

      Si el archivo principal no se coloca en la carpeta raíz, Workfront busca en la carpeta para encontrar el archivo principal.

   * El tamaño máximo del paquete es de 500 MB.
   * En el caso de los archivos ZIP creados en iOS, la herramienta identifica automáticamente la carpeta correcta donde se coloca el contenido.

1. Vaya al proyecto, la tarea o el problema en el que desea cargar el archivo ZIP.
1. Haga clic en **Documentos** en el panel izquierdo .
1. Haga clic en **Agregar nuevo** y haga clic en **Prueba** en el menú que aparece.
1. En el **Agregar archivos** , arrastre y suelte o busque el archivo ZIP que necesite.
1. Haga clic en **Crear prueba** para crear una prueba sencilla sin proceso de revisión.\
   o\
   A continuación, configure una prueba avanzada:

   * [Creación de una prueba avanzada con un flujo de trabajo Básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
