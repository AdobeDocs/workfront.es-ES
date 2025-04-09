---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Generar pruebas en  [!DNL Workfront Proof]
description: Workfront Proof le permite crear pruebas a partir de documentos o sitios web y compartirlas con otros.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: 1443551b605dac6e53531c5d445b89517384fe11
workflow-type: tm+mt
source-wordcount: '1889'
ht-degree: 53%

---

# Generar pruebas en [!DNL Workfront Proof]

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] le permite crear pruebas a partir de documentos o sitios web, así como compartirlas con otros usuarios. Los pasos siguientes describen las distintas opciones de configuración disponibles:

## Generación de una prueba a partir de un documento

1. Realice una de las siguientes acciones para abrir la página **[!UICONTROL Nueva revisión]**:

   * Haga clic en el botón **[!UICONTROL Nueva revisión]** en la esquina superior izquierda de cualquier página.
   * Envíe a través de Dropzone (función de empresa).

1. Para probar uno o varios documentos, agregue los documentos que desea revisar de cualquiera de las siguientes maneras (repita este proceso para agregar varios documentos):

   * Arrastre un documento del sistema de archivos al área de arrastrar y soltar del área **[!UICONTROL Agregar archivos]**.
   * En el área **[!UICONTROL Agregar archivos]**, haga clic en el vínculo **examinar** para buscar y seleccionar el documento que desea cargar desde el sistema de archivos de su estación de trabajo.

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. Para revisar un sitio web, ingresa la URL del sitio web en el área **[!UICONTROL Agregar archivos]** y luego oprime **[!UICONTROL Entrar]**. Repita este paso para agregar varios sitios web a la prueba.

   Para obtener más información sobre la revisión de sitios web, consulte [Generar una prueba para una URL](#generate-a-proof-for-a-url).

   ![Sitio web de revisión](assets/proof-website-350x65.png)

1. (Opcional) Modifique los nombres de archivo de los archivos cargados:

   1. En la lista de documentos, pase el ratón sobre el nombre del documento que quiera modificar y luego haga clic en el icono **[!UICONTROL Editar]**.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. En el campo **[!UICONTROL Nombre de la revisión]**, especifique un nombre nuevo y luego haga clic en **[!UICONTROL Listo]**.

   1. (Opcional) Para eliminar cualquier archivo que se vaya a cargar, pase el ratón sobre el documento que quiera eliminar en la lista de documentos y, a continuación, haga clic en el icono **[!UICONTROL Eliminar]**.

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Opcional) Habilite la opción **[!UICONTROL Combinar todos los archivos compatibles en una sola prueba]**.

      **Cuando esta opción está habilitada:** todos los archivos estáticos y sitios web están disponibles en una sola prueba y puede cargar hasta 50 archivos al mismo tiempo.

      >[!NOTE]
      >
      >Los archivos interactivos, incluidos los vídeos y los sitios web interactivos, no se pueden combinar en una sola prueba.

      **Cuando esta opción está deshabilitada:** todos los documentos y sitios web se generan como pruebas individuales y puede cargar hasta 20 archivos al mismo tiempo.

      Para combinar todos los archivos y sitios web cargados en una sola prueba:

      1. Habilite la opción **[!UICONTROL Combinar todos los archivos compatibles en una sola revisión]**.
      1. En el campo **[!UICONTROL Nombre de revisión]**, escriba un nombre nuevo para la revisión combinada.
      1. En el área **[!UICONTROL Añadir archivos]**, reordene los archivos incluidos arrastrando un archivo al orden deseado. El orden de los archivos es el orden de páginas de la prueba combinada. Para obtener más información sobre la creación de pruebas combinadas, consulte [Crear una prueba de varias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Opcional) Si desea utilizar un flujo de trabajo automatizado que incluya varias fases, seleccione una de las siguientes opciones en la sección **[!UICONTROL Flujo de trabajo]**:

   * **Básico:** seleccione esta opción para designar a los usuarios a los que desea que tengan acceso a la prueba inmediatamente después de crearla. También puede compartir la prueba con varios usuarios.

     Para obtener más información acerca de cómo compartir una prueba, vea [Compartir una prueba en [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automatizado:** seleccione esta opción para administrar la prueba y aprobación de contenido cuando tenga procesos de prueba complejos o si envía contenido para su prueba a los mismos grupos de personas con regularidad. Con un flujo de trabajo automatizado, la prueba pasa de una fase a otra hasta la aprobación final. Se notifica a los usuarios correspondientes cada vez que es necesario realizar una aprobación.

     Para obtener más información acerca de cómo crear un flujo de trabajo automatizado, consulte [Configurar una prueba con un flujo de trabajo automatizado en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Seleccione si desea enviar notificaciones por correo electrónico y un mensaje personalizado a los usuarios seleccionados en el paso anterior:

   * **Notificar a los destinatarios sobre esta prueba:** seleccione esta opción para enviar una notificación por correo electrónico a los usuarios. Cuando se selecciona **[!UICONTROL Uso compartido básico]** en la sección **[!UICONTROL Flujo de trabajo]**, se envía una notificación por correo electrónico cuando se crea la prueba. Cuando se selecciona **[!UICONTROL Flujo de trabajo automatizado]** en la sección **[!UICONTROL Flujo de trabajo]**, se envía una notificación por correo electrónico cuando la prueba entra en la fase del flujo de trabajo automatizado con el que está asociado el usuario.

   * **Añadir mensaje personalizado:** seleccione esta opción para incluir un mensaje personalizado en la notificación. Puede especificar el asunto y el cuerpo del mensaje. El cuerpo del mensaje puede incluir formato de texto enriquecido, como negrita, viñetas e hipervínculos.

1. Seleccione cualquiera de las siguientes opciones de configuración de prueba:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Requerir inicio de sesión. Esta revisión no se puede compartir con otros usuarios</td> 
      <td> <p>Cuando se selecciona esta opción:</p> 
       <ul> 
        <li>Los usuarios no pueden iniciar sesión en la prueba para verla a menos que se les haya agregado.</li> 
        <li>No se pueden habilitar las suscripciones.</li> 
       </ul> 
       <p>Esta opción está desactivada de forma predeterminada.</p> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requerir que las decisiones se firmen electrónicamente</td> 
      <td><p>Cuando se selecciona esta opción, se requiere que los usuarios especifiquen su nombre de usuario y contraseña en el momento en que tomen una decisión sobre una prueba.</p>
      <p>Esta opción está desactivada de forma predeterminada.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear prueba cuando se toman todas las decisiones necesarias</td> 
      <td> <p>Cuando esta configuración está habilitada, el estado de prueba se bloquea después de que se hayan tomado todas las decisiones. El estado cambia automáticamente de desbloqueado a bloqueado cuando el aprobador final toma su decisión.</p> 
      <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir la descarga del archivo original</td> 
      <td> <p><strong></strong> Cuando se selecciona esta opción, los revisores pueden descargar el archivo original desde el que se creó la prueba.</p> <p>Cuando esta opción no está seleccionada, el icono Descargar ya no está visible.</p>
      <p>Esta opción está habilitada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que se comparta la revisión mediante una dirección URL pública o código para insertar</td> 
      <td><p>Cuando se selecciona esta opción, la prueba se puede compartir mediante una URL pública o un código incrustado.</p>
       <p>Esta opción está habilitada de forma predeterminada.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir la suscripción a la revisión mediante una dirección URL pública o código para insertar</td> 
      <td> <p>Si se selecciona esta opción, las personas que no se hayan añadido a la prueba podrán suscribirse a ella. A la persona que se suscribe a la prueba se le concede la función y el correo electrónico que defina en la siguiente configuración:</p> 
       <ul> 
        <li><strong>Función de suscriptor</strong>: la función de prueba predeterminada que se asigna a todos los revisores que se suscriben a la prueba.</li> 
        <li><strong>Configuración de alertas de correo electrónico para suscriptores</strong>: la alerta de correo electrónico predeterminada asignada a todos los revisores que se suscriben a la prueba.</li> 
        <li> <p><strong>Se requiere acceso a la prueba mediante vínculo de correo electrónico para</strong>: configura si el suscriptor recibe un correo electrónico con un vínculo a la prueba. Puede seleccionar <strong>Sin correo electrónico</strong> (el vínculo de correo electrónico no es necesario para acceder a la prueba), <strong>Solo correo electrónico de notificación de prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico sin ninguna verificación) o <strong>Correos electrónicos de notificación de validación y prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico y debe hacer clic en el vínculo para acceder a una prueba. El propósito de esta opción es garantizar que la persona ha introducido una dirección de correo electrónico correcta a la que tiene acceso).</p> <p>Nota: Si las pruebas tienen un flujo de trabajo automatizado adjunto, todas las suscripciones generarán correos electrónicos de confirmación al propietario de la prueba para que pueda decidir a qué fase se debe agregar a la persona.</p> </li> 
       </ul> 
        <p>Esta opción está desactivada de forma predeterminada.</p>
       </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Crear revisión]**. Workfront genera una prueba de los documentos o sitios web seleccionados.

   El tiempo de retardo en la carga de un documento varía según el tamaño y el tipo del archivo. Los archivos más grandes tardarán más en generarse. Puede salir de la página mientras Workfront continúa generando el archivo. El tamaño máximo de carga del archivo es de 4 GB.

## Generación de una prueba estática con una dirección URL {#generate-a-proof-for-a-url}

Puede generar una prueba estática mediante la dirección URL de un sitio web.

>[!NOTE]
>
>Solo puede generar una prueba interactiva para una URL si su entorno de [!DNL Workfront] está integrado en una cuenta de [!DNL Workfront Proof] Premium. Si no puede utilizar la revisión como se describe en esta sección, póngase en contacto con su administrador de Workfront.

1. Realice una de las siguientes acciones para abrir la página **[!UICONTROL Nueva revisión]**:

   * Haga clic en el botón **[!UICONTROL Nueva revisión]** en la esquina superior izquierda de cualquier página.
   * Envíe a través de Dropzone (función de empresa).

1. En la página **Nueva revisión**, escribe la dirección URL del sitio web desde el que deseas crear la revisión en el área **[!UICONTROL Agregar archivos]** y, a continuación, presiona **[!UICONTROL Intro]** o **[!UICONTROL Retorno]** en el teclado.

1. (Opcional) Repita este proceso para agregar varios sitios web a la prueba.

   ![proof_website.png](assets/proof-website-350x65.png)

1. En el área **[!UICONTROL Agregar archivos]**, haga clic en el icono **Editar** a la derecha de la dirección URL para abrir los detalles de revisión del sitio web.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Escriba un **[!UICONTROL Nombre de revisión]**. De forma predeterminada, el nombre de la prueba es el mismo que la dirección URL del sitio.

1. Seleccione cualquiera de las siguientes opciones **[!UICONTROL Administrar contenido del sitio]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Hacer captura de pantalla</td> 
      <td>Crea una prueba de una imagen estática de la página principal de la dirección URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Interactiva</td> 
      <td> <p>Crea una prueba que permite a los revisores navegar por el sitio, ver imágenes de HTML5, elementos de Flash, etc.</p> <p>Para crear una prueba interactiva, el sitio web debe alojarse con un protocolo seguro (https). Además, los sitios web que no se pueden incrustar en un iframe no se pueden generar como una prueba interactiva (las restricciones de incrustación de iframes las controla el sitio web que intenta incrustar).</p> <p>Una vez creada la prueba inicial, esta configuración no se puede cambiar al crear versiones posteriores.</p> <p>Para obtener más información acerca de las pruebas interactivas, consulte <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Generar una prueba para contenido interactivo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resolución de captura de pantalla</td> 
      <td> <p>(Esta opción no está disponible para pruebas interactivas). Puede ajustar la resolución en la que se muestra el contenido o seleccionar varias resoluciones.</p> <p>Esto permite a los usuarios que revisan la prueba ver cómo aparecerá el contenido en diferentes dispositivos, como varios tamaños de teléfono, tabletas y monitores.</p> <p>Si selecciona varias resoluciones, se crea una prueba independiente para cada resolución que seleccione.</p> <p>Cuando los usuarios realizan comentarios sobre la prueba, la resolución de pantalla actual se muestra automáticamente en el comentario para garantizar que los demás usuarios sepan con qué resolución está asociado el comentario.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Buscar subpáginas</td> 
      <td>(Esta opción no está disponible para pruebas interactivas). Seleccione esta opción para navegar por las páginas del sitio web. Puede ampliar el sitio web hasta 2 niveles de profundidad desde la página principal. Pase el ratón sobre una página para ver la dirección URL de la página y seleccione solo las páginas que quiera revisar. Cada página que seleccione se creará como una prueba individual de forma predeterminada. También puede habilitar la opción <strong>Combinar todos los archivos compatibles en una sola revisión</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Configure cualquier opción de prueba avanzada, como compartir la prueba, añadir un flujo de trabajo automatizado o configurar el acceso y la suscripción. Para obtener más información sobre estas opciones, consulte los siguientes artículos:

   * [Compartir una prueba en  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configurar una prueba con un flujo de trabajo automatizado en  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Configuración de acceso y suscripción para una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Haga clic en **[!UICONTROL Listo]**.

1. Haga clic en **[!UICONTROL Crear revisión]**.

## Generación de una prueba para contenido interactivo {#generate-a-proof-for-interactive-content}

<!--A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).-->

Para obtener más información sobre el contenido interactivo, consulte [Resumen de las pruebas de contenido interactivo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Añadir contenido interactivo como URL](#add-interactive-content-as-a-url)
* [Añadir contenido interactivo como archivo ZIP](#add-interactive-content-as-a-zip-file)

### Añadir contenido interactivo como URL {#add-interactive-content-as-a-url}

Para obtener información sobre cómo agregar una revisión de URL interactiva, consulte [Generar una revisión para una URL](#generate-a-proof-for-a-url).

### Añadir contenido interactivo como archivo ZIP {#add-interactive-content-as-a-zip-file}

1. Prepare el contenido creando un archivo agrupado .zip.

   Para obtener información sobre las especificaciones de los archivos empaquetados .zip, consulte [descripción general de las pruebas de contenido interactivo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Realice una de las siguientes acciones para abrir la página **[!UICONTROL Nueva revisión]**:

   * Haga clic en el botón **[!UICONTROL Nueva revisión]** en la esquina superior izquierda de cualquier página.
   * Envíe a través de Dropzone (función de empresa).

1. En la página **[!UICONTROL Nueva prueba]**, arrastre y suelte el paquete .zip interactivo en el área **[!UICONTROL Agregar archivos]**.

1. (Opcional) Configure cualquier opción de prueba avanzada, como compartir la prueba, añadir un flujo de trabajo automatizado o configurar el acceso y la suscripción. Para obtener más información sobre estas opciones, consulte los siguientes artículos:

   * [Compartir una prueba en  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configuración de acceso y suscripción para una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Haga clic en **[!UICONTROL Crear revisión]**. Workfront genera una prueba del archivo zip.

   El tiempo de retardo en la carga de un documento varía según el tamaño del archivo zip. Puede salir de la página mientras Workfront continúa generando el archivo. El tamaño máximo de carga del archivo es de 4 GB.
