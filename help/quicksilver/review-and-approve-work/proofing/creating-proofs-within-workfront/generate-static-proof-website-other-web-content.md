---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creación de una prueba estática para un sitio web u otro contenido web
description: Puede generar una nueva prueba estática o una nueva versión de una prueba estática existente para el contenido web. El contenido web puede incluir elementos como anuncios con vídeo de streaming, animaciones de HTML o banners interactivos, pero se cortará en varias capturas de pantalla para permitir pruebas estáticas.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 35%

---

# Creación de una prueba estática para un sitio web u otro contenido web

Puede generar una nueva prueba estática o una nueva versión de una prueba estática existente para el contenido web. El contenido web puede incluir elementos como anuncios con vídeo de streaming, animaciones de HTML o banners interactivos, pero se cortará en varias capturas de pantalla para permitir pruebas estáticas.

Tenga en cuenta lo siguiente al crear pruebas estáticas para un sitio web u otro contenido web:

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
   <td role="rowheader">Perfil de permiso de prueba </td> 
   <td>Administrador o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creación o modificación de niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Creación de una prueba estática para un sitio web u otro contenido web

Para crear una revisión estática, el sitio web debe ser accesible públicamente (no detrás de un cortafuegos) o la lista de permitidos de su organización debe incluir el dominio de Workfront. Workfront no puede capturar un sitio web protegido por contraseña como una prueba estática.

>[!TIP]
>
>Se recomienda la revisión interactiva en lugar de la revisión estática para las páginas internas que requieren autorización y páginas protegidas con contraseña. Para obtener más información, consulte [Resumen de las pruebas de contenido interactivo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Vaya al proyecto, tarea o problema del que quiera crear una nueva revisión de sitio web o una nueva versión de una existente.
1. Haga clic en **Documentos** en el panel izquierdo
1. (Condicional) Si está creando una nueva prueba, haga clic en **Agregar nuevo** y, a continuación, haga clic en **Prueba** en el menú que aparece.
1. (Condicional) Si está creando una nueva versión de una revisión existente:

   1. Pase el cursor sobre la revisión de URL para la que desea crear una nueva versión y, a continuación, selecciónela haciendo clic en el fondo azul claro que la rodea.

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. Haga clic en **Agregar nuevo** > **Versión** > **Revisión**.

1. Escriba la dirección URL del sitio web que desea revisar en el área de **Agregar archivos** y, a continuación, presione **Entrar**.

   >[!NOTE]
   >
   > La URL debe contener menos de 2.000 caracteres.

1. Haga clic en la dirección URL añadida.

   Aparecerán las opciones para configurar la revisión del sitio web.

   ![revisión interactiva](assets/interactive-proof-radio-btn-area-350x199.png)

1. (Opcional) Si desea cambiar el nombre de la revisión de la URL del sitio web a otra cosa, escriba un **Nombre de revisión.**
1. Asegúrese de que **Capturar captura de pantalla** está seleccionada y use cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Resolución de captura de pantalla</strong> </td> 
      <td> <p>Ajuste la resolución del contenido cuando los revisores vean la prueba, lo que les permite ver cómo aparece en dispositivos de distintos tamaños, como teléfonos, tabletas y monitores.</p> <p>Si selecciona varias resoluciones, se crea una prueba independiente para cada resolución que seleccione.</p> <p>Nota: Cuando un revisor realiza un comentario sobre la prueba, el comentario incluye la resolución que muestra cuándo se realizó el comentario para que otros revisores sepan qué resolución está asociada con el comentario. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Buscar subpáginas</strong> </td> 
      <td> <p>Capturar las subpáginas del sitio web así como sus páginas principales. Puede hacer clic en Seleccionar todo para incluir todas las páginas o puede hacer clic solo en determinadas páginas que desee incluir. Los botones más y menos permiten expandir y cerrar las áreas de subpágina del sitio web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >No puede cambiar la configuración de Captura de pantalla para ninguna versión posterior de la prueba que cree.

1. Haga clic en **Listo**.

   Si seleccionó varias resoluciones de captura de pantalla en el paso 8, la lista incluye un conjunto de capturas de pantalla para cada resolución. Puede generar estas capturas de pantalla como pruebas independientes o combinarlas en una sola prueba (consulte  en .). Le recomendamos que los combine, especialmente si está creando una prueba de sitio web estática.

   >[!NOTE]
   >
   >Si se añadiera una nueva versión a una prueba de URL existente, todas las opciones configuradas en la prueba original o en la versión anterior se mantendrán en esta versión.

1. Haga clic en **Crear prueba** para crear una prueba simple sin proceso de revisión.\
   o\
   Seguir configurando una prueba avanzada:

   * [Creación de una prueba avanzada con un flujo de trabajo básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Crear una revisión avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
