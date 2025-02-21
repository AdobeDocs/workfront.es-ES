---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: disable,public,sharing,proof,public,url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Deshabilitar el uso compartido de la prueba mediante una dirección URL pública o código incrustado
description: Puede desactivar la capacidad de compartir una prueba con una URL pública o código incrustado para cada prueba o para usuarios individuales.
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 93%

---

# Deshabilitar el uso compartido de la prueba mediante una dirección URL pública o código incrustado

Puede desactivar la capacidad de compartir una prueba con una URL pública o código incrustado para cada prueba o para usuarios individuales.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: pro o superior</p> <p>o</p> <p>Plan heredado: select o premium</p> <p>Para obtener más información sobre el acceso de revisión con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: trabajo o plan</p> <p>Plan heredado: cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Deshabilitar por prueba

Debe ser el propietario o creador de la prueba o tener la función de autor o moderador de la prueba.

1. En el proyecto que contiene la prueba, haga clic en **Documentos** en el panel izquierdo.
1. Pase el puntero por encima de la prueba y seleccione **Detalles del documento** .
1. En el panel izquierdo, haga clic en **Configuración del visualizador de revisión** y, a continuación, deshabilite la casilla de verificación **Permitir el uso compartido de la prueba mediante una dirección URL pública o un código incrustado**.

   ![Configuración del visor de revisiones](assets/proofing-viewer-settings-350x200.png)

1. Haga clic en **Guardar**.

## Deshabilitar por usuario

Puede deshabilitar la configuración de prueba pública para usuarios individuales de la instancia de Workfront. Debe tener un perfil de permiso de prueba de administrador para realizar este cambio.

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Revisión**.
1. Haga clic en **Configuración de la cuenta** cerca de la esquina superior derecha.
1. Haga clic en la ficha **Usuarios** y luego haga clic en el nombre de un usuario.
1. En la sección **Configuración de prueba predeterminada**, deshabilite la casilla de verificación **Uso compartido público**.

   ![Uso compartido público](assets/default-proof-settings--public-sharing-350x210.png)
