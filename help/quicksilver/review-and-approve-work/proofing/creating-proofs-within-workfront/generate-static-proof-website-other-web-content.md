---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creación de una prueba estática para un sitio web u otro contenido web
description: Puede generar una nueva prueba estática o una nueva versión de una prueba estática existente para el contenido web. El contenido web puede incluir anuncios con vídeo de flujo continuo, animaciones de HTML o banners interactivos, pero se cortará en varias capturas de pantalla para permitir pruebas estáticas.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# Creación de una prueba estática para un sitio web u otro contenido web

Puede generar una nueva prueba estática o una nueva versión de una prueba estática existente para el contenido web. El contenido web puede incluir anuncios con vídeo de flujo continuo, animaciones de HTML o banners interactivos, pero se cortará en varias capturas de pantalla para permitir pruebas estáticas.

Tenga en cuenta lo siguiente al crear pruebas estáticas para un sitio web u otro contenido web:

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

## Creación de una prueba estática para un sitio web u otro contenido web

Para crear una prueba estática, el sitio web debe ser de acceso público (no estar detrás de un servidor de seguridad) o la lista de permitidos de la organización debe incluir el dominio de Workfront. Workfront no puede capturar un sitio web protegido mediante contraseña como prueba estática.

>[!TIP]
>
>Recomendamos las pruebas interactivas en lugar de las estáticas para las páginas internas que requieran autorización y páginas protegidas con contraseña. Para obtener más información, consulte [Información general sobre pruebas de contenido interactivo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Vaya al proyecto, la tarea o el problema en el que desea crear una prueba de sitio web nueva o una versión nueva de una existente.
1. Haga clic en **Documentos** en el panel izquierdo .
1. (Condicional) Si está creando una prueba nueva, haga clic en **Agregar nuevo** y haga clic en **Prueba** en el menú que aparece.
1. (Condicional) Si está creando una nueva versión de una prueba existente:

   1. Pase el cursor sobre la prueba de URL para la que desea crear una nueva versión y, a continuación, selecciónela haciendo clic en el fondo azul claro que la rodea.

      ![Select_proof_by_select_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. Haga clic en **Agregar nuevo** > **Versión** > **Prueba**.

1. Escriba la dirección URL del sitio web que desee probar en la **Agregar archivos** área y, a continuación, pulse **Entrar**.

   La dirección URL aparece debajo del cuadro donde la escribió.

   ![](assets/url-name-appears-below-350x142.png)

1. Haga clic en la dirección URL que ha agregado.

   Aparecerán las opciones para configurar la prueba del sitio web.

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. (Opcional) Si desea cambiar el nombre de la prueba de la dirección URL del sitio web a otra cosa, escriba un **Nombre de la prueba.**
1. Asegúrese de **Captura de pantalla** está seleccionado y utilice cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Resolución de la captura de pantalla</strong> </td> 
      <td> <p>Ajuste la resolución del contenido cuando los revisores vean la prueba, lo que les permite ver cómo aparece en dispositivos de distintos tamaños, como teléfonos, tabletas y monitores.</p> <p>Si selecciona varias resoluciones, se crea una prueba independiente para cada resolución seleccionada.</p> <p>Nota: Cuando un revisor comenta sobre la prueba, el comentario incluye la resolución que muestra cuándo se hizo el comentario para que otros revisores sepan qué resolución está asociada al comentario. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Buscar subpáginas</strong> </td> 
      <td> <p>Capture las subpáginas del sitio web así como sus páginas principales. Puede hacer clic en Seleccionar todo para incluir todas las páginas o puede hacer clic únicamente en las páginas que desee incluir. Los botones más y menos permiten expandir y cerrar las áreas de subpágina del sitio web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >No se puede cambiar la configuración Captura de captura de captura para ninguna versión posterior de la prueba que se haya creado.

1. Haga clic en **Listo**.

   Si ha seleccionado varias resoluciones de captura de pantalla en el paso 8, la lista incluye un conjunto de capturas de pantalla para cada resolución. Puede generar estas capturas de pantalla como pruebas independientes o combinarlas en una sola prueba (consulte en ). Se recomienda combinarlas, especialmente si se está creando una prueba de sitio web estática.

   >[!NOTE]
   >
   >Si agrega una versión nueva a una prueba de URL existente, todas las opciones configuradas en la prueba original o en la versión anterior se mantendrán en esta versión.

1. Haga clic en **Crear prueba** para crear una prueba sencilla sin proceso de revisión.\
   o\
   A continuación, configure una prueba avanzada:

   * [Creación de una prueba avanzada con un flujo de trabajo Básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
