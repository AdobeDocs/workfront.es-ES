---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Generar pruebas en  [!DNL Workfront Proof]
description: Workfront Proof le permite crear pruebas a partir de documentos o sitios web y compartirlas con otros.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '2259'
ht-degree: 92%

---

# Generar pruebas en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] le permite crear pruebas a partir de documentos o sitios web, así como compartirlas con otros usuarios. Los pasos siguientes describen las distintas opciones de configuración disponibles:

## Crear una prueba para este documento

1. Realice una de las siguientes acciones para empezar a crear una nueva prueba y mostrar la página [!UICONTROL Nueva prueba]:

   * Haga clic en el botón verde **[!UICONTROL Nueva prueba]** en la esquina superior izquierda de cualquier página.
   * En el área **[!UICONTROL Panel de control]**, en la ficha **[!UICONTROL Información general]**, haga clic en el vínculo **[!UICONTROL Nueva prueba]**.

   * Envíe a través de Dropzone (función de empresa).
   * Se muestra la página **[!UICONTROL Nueva prueba]**.

1. Para probar uno o varios documentos, añada los documentos que desea probar de cualquiera de las siguientes maneras (repita este proceso para añadir varios documentos que desee probar):

   * Arrastre un documento del sistema de archivos al área de arrastrar y soltar del área **[!UICONTROL Agregar archivos]**.
   * Haga clic en el área de arrastrar y soltar en el área **[!UICONTROL Añadir archivos]** y, a continuación, busque y seleccione el documento que desea cargar desde el sistema de archivos de la estación de trabajo.

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. Para probar uno o más sitios web, especifique la dirección URL del sitio web que desea probar en el área **[!UICONTROL Añadir archivos]** y luego presione **[!UICONTROL entrar]**.

1. (Opcional) Repita este proceso para añadir varios sitios web a la prueba.

   Para obtener más información sobre la revisión de sitios web, consulte [Generar una prueba para una URL](#generate-a-proof-for-a-url).

   ![Sitio web de revisión](assets/proof-website-350x65.png)

1. (Opcional) Modifique los nombres de archivo de los archivos cargados:

   1. Pase el cursor sobre el nombre del documento que quiera modificar en la lista de documentos del área **[!UICONTROL Añadir archivos]** y luego haga clic en el icono **[!UICONTROL Editar]**.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. En el campo **[!UICONTROL Nombre de la revisión]**, especifique un nombre nuevo y luego haga clic en **[!UICONTROL Listo]**.

   1. (Opcional) Para eliminar cualquier archivo que se vaya a cargar, pase el ratón sobre el documento que quiera eliminar en la lista de documentos del área **[!UICONTROL Añadir archivos]** y, a continuación, haga clic en el icono **[!UICONTROL Eliminar]**.

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Opcional) Habilite la opción para **[!UICONTROL Combinar todos los archivos compatibles en una sola prueba]**.

      **Cuando esta opción está habilitada:** todos los archivos estáticos y sitios web están disponibles en una sola prueba y puede cargar hasta 50 archivos al mismo tiempo.

      >[!NOTE]
      >
      >Los archivos interactivos, incluidos los vídeos y los sitios web interactivos, no se pueden combinar en una sola prueba.

      **Cuando esta opción está deshabilitada:** todos los documentos y sitios web se generan como pruebas individuales y puede cargar hasta 20 archivos al mismo tiempo.

      Para combinar todos los archivos y sitios web cargados en una sola prueba:

      1. Habilite la opción para **[!UICONTROL Combinar todos los archivos compatibles en una sola prueba]**.
      1. En el campo **[!UICONTROL Nombre de la revisión]**, especifique un nombre nuevo para la prueba combinada.
      1. En el área **[!UICONTROL Añadir archivos]**, reordene los archivos incluidos arrastrando un archivo al orden deseado. El orden de los archivos es el orden de páginas de la prueba combinada. Para obtener más información sobre la creación de pruebas combinadas, consulte [Crear una prueba de varias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Opcional) Si desea utilizar un flujo de trabajo automatizado que incluya varias fases, en la sección **[!UICONTROL Flujo de trabajo]**, seleccione una de las siguientes opciones:

   * **Básico:** seleccione esta opción para designar a los usuarios a los que desea que tengan acceso a la prueba inmediatamente después de crearla. También puede compartir la prueba con varios usuarios.

     Para obtener más información sobre cómo compartir una prueba, consulte “Añadir usuarios a una prueba” en [Compartir una prueba en [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

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
      <td role="rowheader">Inicio de sesión obligatorio: la prueba solo se puede compartir con otros usuarios</td> 
      <td> <p><strong>Inicio de sesión obligatorio: la prueba solo se puede compartir con otros usuarios:</strong> al seleccionar esta opción, solo los usuarios de [!DNL Workfront Proof] pueden ver la prueba.</p> <p>Esta opción está desactivada de forma predeterminada; cualquier persona con la URL puede ver la prueba.</p> <p>Cuando se selecciona esta opción:</p> 
       <ul> 
        <li>Los usuarios no pueden iniciar sesión en la prueba a menos que se les haya añadido a la prueba.</li> 
        <li>No se pueden habilitar las suscripciones.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Solo se requiere una decisión para esta prueba</td> 
      <td> <p>Cuando se selecciona esta opción, la prueba se completa después de que uno de los responsables de la toma de decisiones tome su decisión.</p> <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requerir que las decisiones se firmen electrónicamente</td> 
      <td>Los usuarios deben especificar su nombre de usuario y contraseña en el momento en el que toman una decisión sobre una prueba.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear prueba cuando se toman todas las decisiones necesarias</td> 
      <td> <p><strong></strong> Cuando esta configuración está habilitada, el estado de prueba se bloquea después de que se hayan tomado todas las decisiones. El estado cambia automáticamente de desbloqueado a bloqueado cuando el aprobador final toma su decisión.</p> <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descargar archivo original</td> 
      <td> <p><strong></strong> Cuando se selecciona esta opción, los revisores pueden descargar el archivo original desde el que se creó la prueba.</p> <p>Cuando esta opción no está seleccionada, el icono Descargar ya no está visible.<br>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartir la revisión mediante una URL pública o código para insertar</td> 
      <td>Cuando se selecciona esta opción, la prueba se puede compartir mediante una URL pública o un código incrustado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suscribirse a la revisión a través de una URL pública o código para insertar</td> 
      <td> <p>Si se selecciona esta opción, las personas que no se hayan añadido explícitamente a la prueba podrán suscribirse a ella. A la persona que se suscribe a la prueba se le concede la función y el correo electrónico que defina en la siguiente configuración:</p> 
       <ul> 
        <li><strong>Función de suscriptor</strong>: la función de prueba predeterminada que se asigna a todos los revisores que se suscriben a la prueba.</li> 
        <li><strong>Configuración de alertas de correo electrónico para suscriptores</strong>: la alerta de correo electrónico predeterminada asignada a todos los revisores que se suscriben a la prueba.</li> 
        <li> <p><strong>Se requiere acceso a la prueba mediante vínculo de correo electrónico para</strong>: configura si el suscriptor recibe un correo electrónico con un vínculo a la prueba. Puede seleccionar <strong>Sin correo electrónico</strong> (el vínculo de correo electrónico no es necesario para acceder a la prueba), <strong>Solo correo electrónico de notificación de prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico sin ninguna verificación) o <strong>Correos electrónicos de validación y notificación de prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico y debe hacer clic en el vínculo para acceder a esta; el propósito de esta opción es garantizar que la persona haya entrado una dirección de correo electrónico correcta a la que tenga acceso).</p> <p>Nota: Si las pruebas tienen un flujo de trabajo automatizado adjunto, todas las suscripciones generarán correos electrónicos de confirmación al propietario de la prueba para que pueda decidir a qué fase se debe añadir a la persona.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Crear prueba]**.

   Workfront comienza a generar una prueba de los documentos o sitios web seleccionados. El tiempo de retardo de carga de un documento varía según el tamaño y el tipo de archivo. Tenga en cuenta que los archivos grandes tardan más en generarse. Puede salir de la página y Workfront seguirá generando el archivo. El tamaño máximo de carga del archivo es de 4 GB.

   Una vez generada la prueba, haga clic en **[!UICONTROL Ir a la prueba]** para iniciar la herramienta de revisión.

   ![Screenshot_2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-350x134.png)

   El documento aparece en la herramienta de revisión.

   Los usuarios que no tengan la revisión habilitada en su cuenta aún pueden ver el documento y realizar comentarios en la prueba.

## Generación de una prueba para una URL {#generate-a-proof-for-a-url}

Puede generar una prueba para una URL por primera vez. O bien, puede generar una nueva versión de una prueba de URL en la que se haya generado una prueba anteriormente.

>[!NOTE]
>
>Solo puede generar una prueba interactiva para una URL si su entorno de [!DNL Workfront] está integrado en una cuenta de [!DNL Workfront Proof] Premium. Si no puede utilizar la revisión como se describe en esta sección, póngase en contacto con el administrador del sistema.

Para generar una prueba para una URL:

1. Realice una de las siguientes acciones para crear una nueva prueba y mostrar la página [!UICONTROL Nueva prueba]:

   * Haga clic en el botón verde **[!UICONTROL Nueva prueba]** en la esquina superior izquierda de cualquier página.
   * En el área **[!UICONTROL Panel de control]**, en la ficha **[!UICONTROL Información general]**, haga clic en el vínculo **[!UICONTROL Nueva prueba]**.

   * Envíe a través de Dropzone (función de empresa).

1. (Condicional) En la página **[!UICONTROL Nueva prueba]** que aparece, para crear una nueva versión de una prueba existente:

   1. Seleccione la prueba de URL donde desee añadir una nueva versión.
   1. Haga clic en el botón **[!UICONTROL Nueva versión]** en la parte superior de la página.

      ![Captura de pantalla_2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56-350x80.png)

1. En la página Nueva versión de prueba que se muestra, especifique la dirección URL del sitio web que quiera revisar en el área **[!UICONTROL Agregar archivos]** y luego pulse **[!UICONTROL Intro]**.

1. (Opcional) Repita este proceso para añadir varios sitios web a la prueba.

   ![proof_website.png](assets/proof-website-350x65.png)

1. Haga clic en el sitio web en la lista de documentos en el área **[!UICONTROL Añadir archivos]**.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Especifique un **[!UICONTROL Nombre de prueba]** para la prueba.

   De forma predeterminada, el nombre de la prueba es el mismo que la dirección URL del sitio.

1. Seleccione las opciones **[!UICONTROL Administrar contenido del sitio]**:

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
      <td> <p>Crea una prueba que permite a los revisores navegar por el sitio, ver imágenes de HTML5, elementos de Flash, etc.</p> <p>Para crear una prueba interactiva, el sitio web debe alojarse con un protocolo seguro (https). Además, los sitios web que no se puedan incrustar en un iframe no se pueden generar como una prueba interactiva (las restricciones de incrustación de iframe las controla el sitio web que intenta incrustar).</p> <p>Una vez creada la prueba inicial, esta configuración no se puede cambiar al crear versiones posteriores.</p> <p>Para obtener más información acerca de las pruebas interactivas, consulte <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Generar una prueba para contenido interactivo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resolución de captura de pantalla</td> 
      <td> <p>(Esta opción no está disponible para pruebas interactivas). Puede ajustar la resolución en la que se muestra el contenido o seleccionar varias resoluciones.</p> <p>Esto permite a los usuarios que revisan la prueba ver cómo aparecerá el contenido en diferentes dispositivos, como varios tamaños de teléfono, tabletas y monitores.</p> <p>Si selecciona varias resoluciones, se crea una prueba independiente para cada resolución que seleccione.</p> <p>Cuando los usuarios realizan comentarios sobre la prueba, la resolución de pantalla actual se muestra automáticamente en el comentario para garantizar que los demás usuarios sepan con qué resolución está asociado el comentario.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Buscar subpáginas</td> 
      <td>(Esta opción no está disponible para pruebas interactivas). Seleccione esta opción para navegar por las páginas del sitio web. Puede ampliar el sitio web hasta 2 niveles de profundidad desde la página principal. Pase el ratón sobre una página para ver la dirección URL de la página. Seleccione solo las páginas que desee revisar. Cada página que seleccione se crea como una prueba individual de forma predeterminada. También, se puede habilitar la opción <strong>Combinar en una sola prueba</strong> para combinar todas las páginas seleccionadas en una sola prueba.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Configure cualquier opción de prueba avanzada, como compartir la prueba, añadir un flujo de trabajo automatizado o configurar el acceso y la suscripción. Para obtener más información sobre estas opciones, consulte los siguientes artículos:

   * [Compartir una prueba en  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configurar una prueba con un flujo de trabajo automatizado en  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Configuración de acceso y suscripción para una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Haga clic en **[!UICONTROL Listo]**.

   Si agrega una nueva versión a una revisión de URL existente, todas las opciones configuradas en la revisión original o en la versión anterior se mantienen en esta versión. Si se añadiera una nueva versión a una prueba de URL existente, todas las opciones configuradas en la prueba original o en la versión anterior se mantendrán en esta versión.

1. Haga clic en **[!UICONTROL Crear revisión]**.

## Generación de una prueba para contenido interactivo {#generate-a-proof-for-interactive-content}

Se requiere un plan Pro Workfront o superior para utilizar esta función. Para obtener más información sobre los diversos planes disponibles, consulte [Planes de Workfront](https://www.workfront.com/plans).

Para obtener más información sobre el contenido interactivo, consulte [Resumen de las pruebas de contenido interactivo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Añadir contenido interactivo como URL](#add-interactive-content-as-a-url)
* [Añadir contenido interactivo como archivo ZIP](#add-interactive-content-as-a-zip-file)

### Añadir contenido interactivo como URL {#add-interactive-content-as-a-url}

Para obtener información sobre cómo agregar una revisión de URL interactiva, consulte [Generar una revisión para una URL](#generate-a-proof-for-a-url).

### Añadir contenido interactivo como archivo ZIP {#add-interactive-content-as-a-zip-file}

1. Prepare el contenido creando un archivo agrupado .zip.

   Para obtener información sobre las especificaciones de los archivos .zip agrupados, consulte [Acerca de la preparación de contenido interactivo en un archivo ZIP para la prueba](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) en el artículo [Resumen de las pruebas de contenido interactivo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Realice una de las siguientes acciones para empezar a crear una nueva prueba y mostrar la página [!UICONTROL Nueva prueba]:

   * Haga clic en el botón verde **[!UICONTROL Nueva prueba]** en la esquina superior izquierda de cualquier página.
   * En el área **[!UICONTROL Panel de control]**, en la ficha **[!UICONTROL Información general]**, haga clic en el vínculo **[!UICONTROL Nueva prueba]**.

   * Envíe a través de Dropzone (función de empresa).

1. En la página **[!UICONTROL Nueva prueba]** que aparece, arrastre y suelte el paquete .zip interactivo en el área **[!UICONTROL Añadir archivos]**.

1. (Opcional) Configure cualquier opción de prueba avanzada, como compartir la prueba, añadir un flujo de trabajo automatizado o configurar el acceso y la suscripción. Para obtener más información sobre estas opciones, consulte los siguientes artículos:

   * [Compartir una prueba en  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * en el artículo
   * [Configuración de acceso y suscripción para una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Haga clic en **[!UICONTROL Crear prueba]**.

   Workfront comienza a generar una prueba del paquete .zip. Según el tamaño del paquete, el tiempo de retraso en la carga de un documento varía. Los archivos más grandes tardan más en generarse. Puede salir de la página y Workfront seguirá generando el archivo. El tamaño máximo de carga del archivo es de 4 GB.

   Una vez generada la prueba, puede hacer clic en el botón **[!UICONTROL Ir a la prueba]** que aparece para abrirla.
