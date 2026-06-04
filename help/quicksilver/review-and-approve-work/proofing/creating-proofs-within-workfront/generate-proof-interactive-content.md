---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Crear una revisión de un contenido interactivo en un archivo ZIP
description: Puede generar una prueba para el contenido interactivo que no sea de un sitio web y que se almacene en un archivo ZIP. Algunos ejemplos de este tipo de contenido web son los anuncios con flujo de vídeo o audio, las animaciones de HTML y los titulares interactivos.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
TQID: https://experienceleague.adobe.com/wJNC4pCRhTpOfoiB1X6-6vKrYvWA2EaR-x2HfhwcDaY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 350
ht-degree: 35%

---

# Crear una revisión de un contenido interactivo en un archivo ZIP

Puede generar una prueba para el contenido interactivo que no sea de un sitio web y que se almacene en un archivo ZIP. Algunos ejemplos de este tipo de contenido web son los anuncios con flujo de vídeo o audio, las animaciones de HTML y los titulares interactivos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Estándar</p>
   <p>Trabajo o plan</p> 
   </td> 
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

## Crear una revisión de un contenido interactivo en un archivo ZIP

Una vez que se añade contenido interactivo en un archivo ZIP a una prueba, Adobe Workfront crea una prueba de los documentos comprimidos. Según el tamaño del archivo, el tiempo de carga puede variar. La creación de archivos más grandes tarda más. Puede salir de la página y Workfront seguirá creando el archivo. El tamaño máximo de carga de archivo es de 4 GB. 

1. Prepare el contenido creando un archivo agrupado ZIP.

   El archivo ZIP debe cumplir los siguientes requisitos:

   * Todos los recursos, como CSS, JavaScript, vídeos, sonidos e imágenes, deben incluirse en el archivo del paquete.
   * Asegúrese de que el archivo principal (como index.html, index.htm) se encuentra en la carpeta raíz y que es el único archivo .html/.htm almacenado allí.

     Si el archivo principal no se coloca en la carpeta raíz, Workfront busca en la carpeta para encontrar el archivo principal.

   * El tamaño máximo del paquete es 500 MB.
   * En el caso de los archivos ZIP creados en iOS, la herramienta identifica automáticamente la carpeta correcta en la que se coloca el contenido.

1. Vaya al proyecto, tarea o problema en el que desea cargar el archivo ZIP.
1. Haga clic en **Documentos** en el panel izquierdo
1. Haga clic en **Agregar nuevo** y, a continuación, haga clic en **Revisión** en el menú que aparece.
1. En la sección **Agregar archivos**, arrastre y suelte o busque el archivo ZIP que necesite.
1. Haga clic en **Crear prueba** para crear una prueba simple sin proceso de revisión.\
   o\
   Seguir configurando una prueba avanzada:

   * [Creación de una prueba avanzada con un flujo de trabajo básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Crear una revisión avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
