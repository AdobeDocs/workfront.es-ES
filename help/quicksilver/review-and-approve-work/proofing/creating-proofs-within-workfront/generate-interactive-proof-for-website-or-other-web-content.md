---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Crear una prueba interactiva para un sitio web u otro contenido web
description: Puede generar una nueva prueba interactiva o una nueva versión de una prueba interactiva existente para el contenido web. Puede ser un sitio web u otro tipo de contenido interactivo, como anuncios con vídeo o audio de flujo continuo, animaciones de HTML y banners interactivos.
author: Courtney
feature: Digital Content and Documents
exl-id: 56e5eeea-1ab9-43c8-bc84-d10638171871
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Crear una prueba interactiva para un sitio web u otro contenido web

Puede generar una nueva prueba interactiva o una nueva versión de una prueba interactiva existente para el contenido web. Puede ser un sitio web u otro tipo de contenido interactivo, como anuncios con vídeo o audio de flujo continuo, animaciones de HTML y banners interactivos.

En una prueba interactiva, los revisores pueden navegar e interactuar como lo harían normalmente con el sitio web u otro contenido web.

>[!IMPORTANT]
>
>Asegúrese de que el sitio web o el contenido interactivo sean accesibles para las personas que lo van a revisar. Solo pueden acceder a él en el proceso de pruebas si también pueden acceder a él a través de Internet.

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

## Crear una prueba interactiva para un sitio web u otro contenido web

1. Vaya al proyecto, la tarea o el problema en el que desea crear una prueba de sitio web nueva o una versión nueva de una existente.
1. Haga clic en **Documentos** en el panel izquierdo.
1. (Condicional) Si está creando una prueba nueva, haga clic en **Agregar nuevo** y haga clic en **Prueba** en el menú que aparece.

1. (Condicional) En el **Nueva prueba** si está creando una nueva versión de una prueba existente:

   1. Pase el ratón sobre la prueba de URL para la que desea crear una nueva versión y, a continuación, selecciónela haciendo clic en el fondo azul claro que la rodea.

      ![Select_proof_by_select_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. En el **Agregar nuevo** desplegable, haga clic en **Versión** > **Prueba**.

1. En el **Añadir archivos** , escriba la dirección URL del sitio web que desea probar y, a continuación, presione **Entrar**.

   ![proof_website.png](assets/proof-website-350x65.png)

   Puede repetir este proceso para agregar varios sitios web que desee probar.

1. Haga clic en la dirección URL que ha agregado.

   ![](assets/click-url-350x137.png)

1. (Opcional) Si desea cambiar el nombre de la prueba de la dirección URL del sitio web a otra cosa, escriba un **Nombre de la prueba**.
1. Select **Interactivo** y haga clic en **Listo**.

   >[!NOTE]
   >
   >Si agrega una versión nueva a una prueba de URL existente, todas las opciones configuradas en la prueba original o en la versión anterior se mantendrán en esta versión.

1. Haga clic en **Crear prueba** para crear una prueba sencilla sin proceso de revisión.\
   o\
   A continuación, configure una prueba avanzada:

   * [Creación de una prueba avanzada con un flujo de trabajo Básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
