---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: disable,public,sharing,proof,public,url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Deshabilitar el uso compartido de prueba mediante una URL pública o código incrustado
description: Puede desactivar la capacidad de compartir una prueba con una URL pública o incrustar código en una prueba mediante pruebas o para usuarios individuales.
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Deshabilitar el uso compartido de prueba mediante una URL pública o código incrustado

Puede desactivar la capacidad de compartir una prueba con una URL pública o incrustar código en una prueba mediante pruebas o para usuarios individuales.

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
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con el administrador de Workfront o Workfront Proof.

## Deshabilitar por prueba

Debe ser el propietario de la prueba o el creador, o tener la función de prueba Autor o Moderador .

1. En el proyecto que contiene la prueba, haga clic en **Documentos** en el panel izquierdo.
1. Pase el ratón sobre la prueba y seleccione **Detalles del documento** .
1. En el panel izquierdo, haga clic en **Configuración del visor de pruebas** y, a continuación, deshabilite el **Permitir el uso compartido de pruebas mediante una URL pública o código incrustado** casilla de verificación.

   ![](assets/proofing-viewer-settings-350x200.png)

1. Haga clic en **Guardar**.

## Deshabilitar por usuario

Puede deshabilitar la configuración de prueba pública para usuarios individuales en la instancia de Workfront. Debe tener un perfil de permisos de prueba de administrador para realizar este cambio.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Prueba**.
1. Haga clic en **Configuración de la cuenta** cerca de la esquina superior derecha.
1. Haga clic en el **Usuarios** y, a continuación, haga clic en el nombre de un usuario.
1. En el **Configuración de prueba predeterminada** , desactive la **Uso compartido público** casilla de verificación.

   ![](assets/default-proof-settings--public-sharing-350x210.png)
