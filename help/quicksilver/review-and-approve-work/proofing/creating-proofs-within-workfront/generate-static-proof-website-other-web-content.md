---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creación de una prueba estática para un sitio web u otro contenido web
description: Puede generar una nueva prueba estática o una nueva versión de una prueba estática existente para el contenido web. El contenido web puede incluir elementos como anuncios con vídeo de streaming, animaciones de HTML o banners interactivos, pero se cortará en varias capturas de pantalla para permitir pruebas estáticas.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 35d76d3cb06c9e9b449844f304f1443e24a221d4
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---

# Creación de una prueba estática para un sitio web u otro contenido web

Puede generar una nueva prueba estática o una nueva versión de una prueba estática existente para el contenido web. El contenido web puede incluir elementos como anuncios con vídeo de streaming, animaciones de HTML o banners interactivos, pero se cortará en varias capturas de pantalla para permitir pruebas estáticas.

Tenga en cuenta lo siguiente al crear pruebas estáticas para un sitio web u otro contenido web:

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
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Responsable o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

## Creación de una prueba estática para un sitio web u otro contenido web

Para crear una revisión estática, el sitio web debe ser accesible públicamente (no detrás de un cortafuegos) o la lista de permitidos de su organización debe incluir el dominio de Workfront. Workfront no puede capturar un sitio web protegido por contraseña como una prueba estática.

>[!TIP]
>
>Se recomienda la revisión interactiva en lugar de la revisión estática para las páginas internas que requieren autorización y páginas protegidas con contraseña. Para obtener más información, consulte [Resumen de las pruebas de contenido interactivo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Vaya al proyecto, tarea o problema en el que desea crear una nueva revisión de sitio web o una nueva versión de una existente.
1. Haga clic en **Documentos** en el panel izquierdo
1. (Condicional) Si está creando una nueva prueba, haga clic en **Agregar nuevo** y, a continuación, haga clic en **Prueba** en el menú que aparece.
1. (Condicional) Si está creando una nueva versión de una revisión existente:

   1. Pase el cursor sobre la revisión de URL para la que desea crear una nueva versión y, a continuación, selecciónela haciendo clic en el fondo azul claro que la rodea.

      ![Seleccionar_revisión_por_seleccionar_fondo_azul_claro.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. Haga clic en **Agregar nuevo** > **Versión** > **Revisión**.

1. Escriba la dirección URL del sitio web que desea revisar en el área de **Agregar archivos** y, a continuación, presione **Entrar**.

   >[!NOTE]
   >
   > La dirección URL debe tener menos de 1000 caracteres.

1. Haga clic en la dirección URL que ha agregado.

   Aparecerán las opciones para configurar la revisión del sitio web.

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

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
   >Si agrega una nueva versión a una revisión de URL existente, todas las opciones configuradas en la revisión original o en la versión anterior se mantienen en esta versión.

1. Haga clic en **Crear revisión** para crear una revisión simple sin proceso de revisión.\
   o\
   Siga configurando una revisión avanzada:

   * [Creación de una prueba avanzada con un flujo de trabajo básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
