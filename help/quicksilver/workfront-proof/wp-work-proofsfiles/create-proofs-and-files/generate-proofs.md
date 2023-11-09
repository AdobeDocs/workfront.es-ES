---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Generación de pruebas en [!DNL Workfront Proof]
description: Workfront Proof permite crear pruebas a partir de documentos o sitios web, así como compartirlas con otros usuarios.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '2254'
ht-degree: 0%

---

# Generación de pruebas en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] permite crear pruebas a partir de documentos o sitios web, y compartirlas con otros. Los pasos siguientes describen las distintas opciones de configuración disponibles:

## Generación de una prueba para un documento

1. Realice una de las siguientes acciones para empezar a crear una nueva prueba y mostrar el [!UICONTROL Nueva revisión] página:

   * Haga clic en el icono verde **[!UICONTROL Nueva revisión]** en la esquina superior izquierda de cualquier página.
   * En el **[!UICONTROL Tablero]** , en el **[!UICONTROL Información general]** , haga clic en **[!UICONTROL Nueva revisión]** vínculo.

   * Enviar mediante Dropzone (función de empresa).
   * El **[!UICONTROL Nueva revisión]** página muestra.

1. Para revisar uno o varios documentos, agregue los documentos que desee revisar de cualquiera de las siguientes maneras (repita este proceso para agregar varios documentos que desee revisar):

   * Arrastre un documento desde el sistema de archivos al área de arrastrar y soltar de la **[!UICONTROL Agregar archivos]** área.
   * Haga clic en el área de arrastrar y soltar de la **[!UICONTROL Agregar archivos]** , a continuación busque y seleccione el documento que desea cargar desde el sistema de archivos de su estación de trabajo.

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. Para revisar uno o varios sitios web, especifique la dirección URL del sitio web que desea revisar en la **[!UICONTROL Agregar archivos]** y, a continuación, pulse **[!UICONTROL Entrar]**.

1. (Opcional) Repita este proceso para agregar varios sitios web a la prueba.

   Para obtener más información sobre la revisión de sitios web, consulte [Generación de una prueba para una dirección URL](#generate-a-proof-for-a-url).

   ![](assets/proof-website-350x65.png)

1. (Opcional) Modifique los nombres de archivo de los archivos cargados:

   1. Pase el cursor sobre el nombre del documento que desee modificar en la lista de documentos de **[!UICONTROL Agregar archivos]** y luego haga clic en el **[!UICONTROL Editar]** icono.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. En el **[!UICONTROL Nombre de revisión]** , especifique un nuevo nombre y haga clic en **[!UICONTROL Listo]**.

   1. (Opcional) Para eliminar cualquier archivo de la carga, pase el ratón sobre el documento que desea eliminar en la lista de documentos de **[!UICONTROL Agregar archivos]** y luego haga clic en el **[!UICONTROL Eliminar]** icono.

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Opcional) Habilite la opción, **[!UICONTROL Combinar todos los archivos compatibles en una sola prueba]**.

      **Cuando esta opción está habilitada:** Todos los archivos estáticos y sitios web están disponibles en una sola prueba, y puede cargar hasta 50 archivos a la vez.

      >[!NOTE]
      >
      >Los archivos interactivos, incluidos los vídeos y los sitios web interactivos, no se pueden combinar en una sola prueba.

      **Cuando esta opción está desactivada:** Todos los documentos y sitios web se generan como pruebas individuales y puede cargar hasta 20 archivos a la vez.

      Para combinar todos los archivos y sitios web cargados en una sola prueba:

      1. Habilite la opción, **[!UICONTROL Combinar todos los archivos compatibles en una sola prueba]**.
      1. En el **[!UICONTROL Nombre de revisión]** , especifique un nuevo nombre para la prueba combinada.
      1. En el **[!UICONTROL Agregar archivos]** , reordene los archivos incluidos arrastrando un archivo al orden deseado. El orden de los archivos es el orden de páginas de la prueba combinada. Para obtener más información sobre la creación de pruebas combinadas, consulte [Creación de una prueba de varias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Opcional) Si desea utilizar un flujo de trabajo automatizado que incluya varias fases, en la variable **[!UICONTROL Flujo de trabajo]** , seleccione entre las siguientes opciones:

   * **Básico:** Seleccione esta opción para designar a los usuarios a los que desea que tengan acceso a la prueba inmediatamente después de crearla. Puede compartir la prueba con varios usuarios.

     Para obtener más información sobre cómo compartir una prueba, consulte &quot;Añadir usuarios a una prueba&quot; en [Compartir una prueba en [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automatizado:** Seleccione esta opción para administrar la revisión y aprobación de contenido cuando tenga procesos de revisión complejos o si envía contenido para su revisión a los mismos grupos de personas con regularidad. Con el flujo de trabajo automatizado, la prueba se desplaza de una fase a otra hasta la aprobación final. Se notifica a los usuarios correspondientes cada vez que se les requiere que realicen una aprobación.

     Para obtener más información sobre la creación de un flujo de trabajo automatizado, consulte [Configuración de una prueba con un flujo de trabajo automatizado en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Seleccione si desea enviar notificaciones por correo electrónico y un mensaje personalizado a los usuarios seleccionados en el paso anterior:

   * **Notificar a los destinatarios sobre esta prueba:** Seleccione esta opción para enviar una notificación por correo electrónico a los usuarios. Cuándo **[!UICONTROL Uso compartido básico]** está seleccionado en la **[!UICONTROL Flujo de trabajo]** , una notificación por correo electrónico envía cuando se crea la prueba. Cuándo **[!UICONTROL Flujo de trabajo automatizado]** está seleccionado en la **[!UICONTROL Flujo de trabajo]** , una notificación por correo electrónico envía cuando la prueba entra en la fase del flujo de trabajo automatizado a la que está asociado el usuario.

   * **Añadir mensaje personalizado:** Seleccione esta opción para incluir un mensaje personalizado en la notificación. Puede especificar el asunto y el cuerpo del mensaje. El cuerpo del mensaje puede incluir formato de texto enriquecido, como negrita, viñetas e hipervínculos.

1. Seleccione cualquiera de las siguientes opciones de configuración de prueba:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Requerir inicio de sesión: la prueba solo se puede compartir con otros usuarios</td> 
      <td> <p><strong>Requerir inicio de sesión: la prueba solo se puede compartir con otros usuarios:</strong> Cuando se selecciona esta opción, solo [!DNL Workfront Proof] Los usuarios de pueden ver la prueba.</p> <p>Esta opción está desactivada de forma predeterminada; cualquier persona con la URL puede ver la prueba.</p> <p>Cuando se selecciona esta opción:</p> 
       <ul> 
        <li>Los usuarios no pueden iniciar sesión en la prueba a menos que se les haya agregado a la prueba.</li> 
        <li>No se pueden activar las suscripciones.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Solo se requiere una decisión para esta prueba</td> 
      <td> <p>Cuando se selecciona esta opción, la revisión se completa después de que uno de los responsables de la toma de decisiones tome su decisión.</p> <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requerir que las decisiones se firmen electrónicamente</td> 
      <td>Los usuarios deben especificar su nombre de usuario y contraseña en el momento en que toman una decisión sobre una prueba.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear la revisión cuando se tomen todas las decisiones necesarias</td> 
      <td> <p><strong></strong> Cuando esta configuración está habilitada, el estado de prueba se bloquea después de que se hayan tomado todas las decisiones. El estado cambia automáticamente de desbloqueado a bloqueado cuando el aprobador final toma su decisión.</p> <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descargar archivo original</td> 
      <td> <p><strong></strong> Cuando se selecciona esta opción, los revisores pueden descargar el archivo original desde el que se creó la prueba.</p> <p>Cuando esta opción no está seleccionada, el icono Descargar ya no está visible.<br>Esta opción está habilitada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartir la revisión mediante una URL pública o código para insertar</td> 
      <td>Cuando se selecciona esta opción, la prueba se puede compartir mediante una URL pública o un código incrustado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suscribirse a la revisión mediante una URL pública o un código para insertar</td> 
      <td> <p>Si se selecciona esta opción, las personas que no se hayan añadido explícitamente a la prueba podrán suscribirse a ella. A la persona que se suscribe a la prueba se le concede la función y el correo electrónico que defina en la siguiente configuración:</p> 
       <ul> 
        <li><strong>Función de suscriptor</strong>: La función de prueba predeterminada asignada a todos los revisores que se suscriben a la prueba.</li> 
        <li><strong>Configuración de alertas de correo electrónico para suscriptores</strong>: Alerta de correo electrónico predeterminada asignada a todos los revisores que se suscriben a la prueba.</li> 
        <li> <p><strong>Se requiere acceso de revisión por correo electrónico para</strong>: Configure si el suscriptor recibe un correo electrónico con un vínculo a la prueba. Puede seleccionar <strong>Sin correo electrónico</strong> (no se requiere un enlace de correo electrónico para acceder a la prueba), <strong>Solo correo electrónico de notificación de revisión</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico sin ninguna verificación), o <strong>Correos electrónicos de validación y notificación de prueba</strong> (El suscriptor recibe un vínculo a la prueba por correo electrónico y debe hacer clic en el vínculo para acceder a una prueba; el propósito de esta opción es garantizar que la persona haya introducido una dirección de correo electrónico correcta a la que tenga acceso).</p> <p>Nota: Si las pruebas tienen un flujo de trabajo automatizado adjunto, todas las suscripciones generarán correos electrónicos de confirmación al propietario de la prueba para que pueda decidir a qué fase se debe agregar a la persona.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Crear revisión]**.

   Workfront comienza a generar una prueba de los documentos o sitios web seleccionados. Según el tamaño y el tipo de archivo, el tiempo de posposición de la carga de un documento varía. Tenga paciencia, ya que los archivos más grandes tardan más en generarse. Puede salir de la página y Workfront seguirá generando el archivo. El tamaño máximo de carga de archivo es de 4 GB.

   Una vez generada la prueba, haga clic en **[!UICONTROL Ir a la revisión]** para iniciar la herramienta de corrección.

   ![Screenshot_2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-350x134.png)

   El documento aparecerá en la herramienta de corrección.

   Los usuarios que no tengan la revisión habilitada en su cuenta aún pueden ver el documento y realizar comentarios en la revisión.

## Generación de una prueba para una dirección URL {#generate-a-proof-for-a-url}

Puede generar una prueba para una URL por primera vez. O bien, puede generar una nueva versión de una revisión de URL en la que se haya generado una revisión anteriormente.

>[!NOTE]
>
>Solo puede generar una prueba interactiva para una dirección URL si su [!DNL Workfront] El entorno de está integrado con un [!DNL Workfront Proof] Cuenta Premium. Si no puede utilizar la revisión como se describe en esta sección, póngase en contacto con el administrador del sistema.

Para generar una prueba para una URL:

1. Realice una de las siguientes acciones para empezar a crear una nueva prueba y mostrar el [!UICONTROL Nueva revisión] página:

   * Haga clic en el icono verde **[!UICONTROL Nueva revisión]** en la esquina superior izquierda de cualquier página.
   * En el **[!UICONTROL Tablero]** , en el **[!UICONTROL Información general]** , haga clic en **[!UICONTROL Nueva revisión]** vínculo.

   * Enviar mediante Dropzone (función de empresa).

1. (Condicional) En el **[!UICONTROL Nueva revisión]** página que aparece, para crear una nueva versión de una revisión existente:

   1. Seleccione la revisión de URL donde desee añadir una nueva versión.
   1. Haga clic en **[!UICONTROL Nueva versión]** en la parte superior de la página.

      ![Screenshot_2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56-350x80.png)

1. En la página Nueva versión de prueba que aparece, especifique la dirección URL del sitio web que desea revisar en la **[!UICONTROL Agregar archivos]** y, a continuación, pulse **[!UICONTROL Entrar]**.

1. (Opcional) Repita este proceso para agregar varios sitios web a la prueba.

   ![proof_website.png](assets/proof-website-350x65.png)

1. Haga clic en el sitio web en la lista de documentos de **[!UICONTROL Agregar archivos]** área.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Especifique un **[!UICONTROL Nombre de revisión]** para la prueba.

   De forma predeterminada, el nombre de la prueba es el mismo que la dirección URL del sitio.

1. Seleccionar **[!UICONTROL Administrar contenido del sitio]** opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Captura de pantalla</td> 
      <td>Crea una prueba de una imagen estática de la página principal de la dirección URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Interactiva</td> 
      <td> <p>Crea una revisión que permite a los revisores navegar por el sitio, ver imágenes de HTML5, elementos de Flash, etc.</p> <p>Para crear una prueba interactiva, el sitio web debe alojarse con un protocolo seguro (https). Además, los sitios web que no se puedan incrustar en un iframe no se pueden generar como una prueba interactiva (las restricciones de incrustación de iframes las controla el sitio web que intenta incrustar).</p> <p>Una vez creada la prueba inicial, esta configuración no se puede cambiar al crear versiones posteriores.</p> <p>Para obtener más información sobre las pruebas interactivas, consulte <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Generación de una prueba para contenido interactivo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resolución de captura de pantalla</td> 
      <td> <p>(Esta opción no está disponible para pruebas interactivas). Puede ajustar la resolución en la que se muestra el contenido o seleccionar varias resoluciones.</p> <p>Esto permite a los usuarios que revisan la prueba ver cómo aparecerá el contenido en diferentes dispositivos, como varios tamaños de teléfono, tabletas y monitores.</p> <p>Si selecciona varias resoluciones, se crea una prueba independiente para cada resolución que seleccione.</p> <p>Cuando los usuarios realizan comentarios sobre la prueba, la resolución de pantalla actual se muestra automáticamente en el comentario para garantizar que los demás usuarios sepan con qué resolución está asociado el comentario.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Buscar subpáginas</td> 
      <td>(Esta opción no está disponible para pruebas interactivas). Seleccione esta opción para navegar por las páginas del sitio web. Puede ampliar el sitio web hasta 2 niveles de profundidad desde la página principal. Pase el ratón sobre una página para ver la dirección URL de la página. Seleccione solo las páginas que desee revisar. Cada página que seleccione se creará como una prueba individual de forma predeterminada; o bien, habilite la opción <strong>Combinar en una sola prueba</strong> para combinar todas las páginas seleccionadas en una sola prueba.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Configure cualquier opción de revisión avanzada, como compartir la prueba, agregar un flujo de trabajo automatizado o configurar el acceso y la suscripción. Para obtener más información sobre estas opciones, consulte los siguientes artículos:

   * [Compartir una prueba en [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configuración de una prueba con un flujo de trabajo automatizado en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Configuración de acceso y suscripción para una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Clic **[!UICONTROL Listo]**.

   Si agrega una nueva versión a una revisión de URL existente, todas las opciones configuradas en la revisión original o en la versión anterior se mantienen en esta versión. Si agrega una nueva versión a una revisión de URL existente, todas las opciones configuradas en la revisión original o en la versión anterior se mantienen en esta versión.

1. Clic **[!UICONTROL Crear revisión]**.

## Generación de una prueba para contenido interactivo {#generate-a-proof-for-interactive-content}

Se requiere un plan Pro Workfront o superior para utilizar esta función. Para obtener más información sobre los distintos planes disponibles, consulte [Planes de Workfront](https://www.workfront.com/plans).

Para obtener más información sobre el contenido interactivo, consulte [Resumen de pruebas de contenido interactivo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Añadir contenido interactivo como URL](#add-interactive-content-as-a-url)
* [Añadir contenido interactivo como archivo ZIP](#add-interactive-content-as-a-zip-file)

### Añadir contenido interactivo como URL {#add-interactive-content-as-a-url}

Para obtener información sobre cómo añadir una prueba de URL interactiva, consulte  [Generación de una prueba para una dirección URL](#generate-a-proof-for-a-url).

### Añadir contenido interactivo como archivo ZIP {#add-interactive-content-as-a-zip-file}

1. Prepare el contenido creando un archivo agrupado .zip.

   Para obtener información sobre las especificaciones de los archivos agrupados .zip, consulte [Preparar contenido interactivo en un archivo ZIP para la revisión](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) en el artículo [Resumen de pruebas de contenido interactivo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Realice una de las siguientes acciones para empezar a crear una nueva prueba y mostrar el [!UICONTROL Nueva revisión] página:

   * Haga clic en el icono verde **[!UICONTROL Nueva revisión]** en la esquina superior izquierda de cualquier página.
   * En el **[!UICONTROL Tablero]** , en el **[!UICONTROL Información general]** , haga clic en **[!UICONTROL Nueva revisión]** vínculo.

   * Enviar mediante Dropzone (función de empresa).

1. En el **[!UICONTROL Nueva revisión]** Cuando aparezca, arrastre y suelte el paquete .zip interactivo en el **[!UICONTROL Añadir archivos]** área.

1. (Opcional) Configure cualquier opción de revisión avanzada, como compartir la prueba, añadir un flujo de trabajo automatizado o configurar el acceso y la configuración de suscripción. Para obtener más información sobre estas opciones, consulte los siguientes artículos:

   * [Compartir una prueba en [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * en el artículo
   * [Configuración de acceso y suscripción para una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Clic **[!UICONTROL Crear revisión]**.

   Workfront comienza a generar una prueba del paquete .zip. Según el tamaño del paquete, el tiempo de posposición de la carga de un documento varía. Los archivos más grandes tardan más en generarse. Puede salir de la página y Workfront seguirá generando el archivo. El tamaño máximo de carga de archivo es de 4 GB.

   Una vez generada la prueba, puede hacer clic en **[!UICONTROL Ir a la revisión]** que aparece para abrir la prueba.
