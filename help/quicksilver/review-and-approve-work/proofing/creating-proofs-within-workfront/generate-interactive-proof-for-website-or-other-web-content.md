---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creación de pruebas interactivas para sitios web u otro contenido web
description: Es posible generar una nueva prueba interactiva o una nueva versión de una prueba interactiva existente del contenido web. Puede tratarse de sitios web u otro tipo de contenido interactivo, como anuncios con streaming de vídeo o audio, animaciones con HTML y titulares interactivos.
author: Courtney
feature: Digital Content and Documents
exl-id: 56e5eeea-1ab9-43c8-bc84-d10638171871
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 99%

---

# Creación de pruebas interactivas para sitios web u otro contenido web

Es posible generar una nueva prueba interactiva o una nueva versión de una prueba interactiva existente del contenido web. Puede tratarse de sitios web u otro tipo de contenido interactivo, como anuncios con streaming de vídeo o audio, animaciones con HTML y titulares interactivos.

En una prueba interactiva, los revisores pueden navegar e interactuar como lo harían normalmente con el sitio web u otro contenido web.

>[!IMPORTANT]
>
>Asegúrese de que las personas que vayan a revisarlos puedan acceder al sitio web o contenido interactivo. Podrán acceder a el en el proceso de revisión solo si también pueden acceder a el en Internet.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: pro o superior</p> <p>o</p> <p>Plan heredado: Premium</p> <p>Para obtener más información sobre el acceso de revisión en los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: trabajo o plan</p> <p>Plan heredado: cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de prueba </td> 
   <td>Administrador o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creación o modificación de niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Creación de pruebas interactivas para sitios web u otro contenido web

1. Vaya al proyecto, tarea o problema del que quiera crear una nueva revisión de sitio web o una nueva versión de una existente.
1. Haga clic en **Documentos**, en el panel izquierdo.
1. (Condicional) Si está creando una nueva prueba, haga clic en **Añadir nuevo** y, a continuación, haga clic en **Prueba** en el menú que aparezca.

1. (Condicional) En la página **Nueva prueba** aparecerá, si está creando una nueva versión de una prueba existente:

   1. Pase el puntero por encima de la prueba de la URL para la que quiera crear una nueva versión y, a continuación, selecciónela haciendo clic en el fondo azul claro que la rodea.

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)


   1. En el menú desplegable **Añadir nuevo**, haga clic en **Versión** > **Prueba**.

1. En la sección **Añadir archivos**, escriba la dirección URL del sitio web que quiera revisar y, a continuación, presione **Entrar**.  Se puede repetir este proceso para añadir varios sitios web para revisarlos.

   ![proof_website.png](assets/proof-website-350x65.png)


   >[!NOTE]
   >
   > La URL debe contener menos de 1000 caracteres.

1. Haga clic en la dirección URL añadida.

   ![Haga clic en la URL](assets/click-url-350x137.png)

1. (Opcional) Si desea cambiar el nombre de la prueba de la URL del sitio web a algo distinto, escriba un **Nombre de la revisión**.
1. Seleccione **Interactivo** y, a continuación, haga clic en **Listo**.

   >[!NOTE]
   >
   >Si se añadiera una nueva versión a una prueba de URL existente, todas las opciones configuradas en la prueba original o en la versión anterior se mantendrán en esta versión.

1. Haga clic en **Crear prueba** para crear una prueba simple sin proceso de revisión.\
   o\
   Seguir configurando una prueba avanzada:

   * [Creación de una prueba avanzada con un flujo de trabajo básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Crear una revisión avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
