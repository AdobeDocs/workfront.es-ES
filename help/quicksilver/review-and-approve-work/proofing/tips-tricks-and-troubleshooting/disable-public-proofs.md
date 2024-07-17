---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: disable,public,sharing,proof,public,url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Deshabilitar el uso compartido de la revisión mediante una URL pública o código para insertar
description: Puede desactivar la capacidad de compartir una prueba con una URL pública o incrustar código para cada prueba o para usuarios individuales.
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Deshabilitar el uso compartido de la revisión mediante una URL pública o código para insertar

Puede desactivar la capacidad de compartir una prueba con una URL pública o incrustar código para cada prueba o para usuarios individuales.

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
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

## Deshabilitar por revisión

Debe ser el propietario o creador de la prueba o tener la función de autor o moderador de la prueba.

1. En el proyecto que contiene la revisión, haga clic en **Documentos** en el panel izquierdo.
1. Pase el ratón sobre la revisión y seleccione **Detalles del documento** .
1. En el panel izquierdo, haga clic en **Configuración del visor de pruebas** y, a continuación, deshabilite la casilla de verificación **Permitir el uso compartido de la prueba mediante una dirección URL pública o un código incrustado**.

   ![](assets/proofing-viewer-settings-350x200.png)

1. Haga clic en **Guardar**.

## Deshabilitar por usuario

Puede deshabilitar la configuración de Public proof para usuarios individuales de la instancia de Workfront. Debe tener un perfil de permiso de prueba de administrador para realizar este cambio.

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y luego haga clic en **Revisión**.
1. Haga clic en **Configuración de la cuenta** cerca de la esquina superior derecha.
1. Haga clic en la ficha **Usuarios** y luego haga clic en el nombre de un usuario.
1. En la sección **Configuración de prueba predeterminada**, deshabilite la casilla de verificación **Uso compartido público**.

   ![](assets/default-proof-settings--public-sharing-350x210.png)
