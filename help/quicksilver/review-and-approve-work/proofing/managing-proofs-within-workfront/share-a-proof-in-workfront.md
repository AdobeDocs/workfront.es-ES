---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Compartir una revisión en Adobe Workfront
description: Puede compartir un documento revisado en Adobe Workfront compartiéndolo o agregando usuarios a la revisión.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 5c0cd18074cffdf0a4fe15affaf61add7314a83a
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# Compartir una revisión en Adobe Workfront

Puede compartir un documento revisado en Adobe Workfront compartiéndolo o agregando usuarios a la revisión.

Si comparte la prueba, como se explica en este artículo, su destinatario tiene el mismo acceso al documento y a la prueba. Además, puede solicitar la aprobación de la prueba al destinatario.

>[!TIP]
>
>También puede compartir una prueba desde el visualizador de pruebas. Para obtener instrucciones, vea [Compartir una revisión del visor de revisión](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

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
   <td role="rowheader">Función de prueba</td> 
   <td>Autor o moderador</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

## Compartir un vínculo de prueba

Al compartir un vínculo de prueba, los usuarios de Workfront pueden ver el acceso. Los usuarios pueden realizar comentarios sobre la prueba y suscribirse a las notificaciones por correo electrónico de la prueba con sus credenciales de inicio de sesión de Workfront. Los usuarios que no son revisores pueden realizar comentarios y suscribirse mediante una dirección de correo electrónico y un nombre para mostrar.

>[!IMPORTANT]
>
>Debe habilitarse la configuración Permitir el uso compartido de la revisión mediante una URL pública o un código incrustado.

1. Seleccione el documento que contiene la prueba que desea compartir con los usuarios.

   Solo puede seleccionar un documento. No se puede compartir el vínculo para varios documentos al mismo tiempo.

1. Haga clic en **Compartir** > **Vínculo de revisión**.
1. En el cuadro **Vínculo de prueba** que aparece, realice una de las acciones siguientes:

   * Para copiar el vínculo en el portapapeles, haga clic en **Copiar vínculo**.

     Ahora puede distribuir el vínculo mediante una herramienta de terceros, como un chat o una aplicación de correo electrónico.

   * Para enviar por correo electrónico el vínculo directamente desde Adobe Workfront, haga lo siguiente:

      1. En el campo **O enviar un vínculo por correo electrónico a**, empiece a escribir y seleccione el nombre del destinatario. O especifique la dirección de correo electrónico de un usuario externo con el que desee compartir.

         >[!NOTE]
         >
         >Si ve un correo electrónico de alias al compartir una prueba, no cree un nuevo usuario invitado introduciendo el correo electrónico original si existe un correo electrónico de alias correspondiente.

      1. Seleccione entre las siguientes opciones:

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Enviar vínculo público</td>
            <td><p>Incluye un botón en la notificación por correo electrónico que dirige a los usuarios a la prueba dentro del visor de pruebas que están utilizando y concede acceso de visualización.</p><p>Si <strong>Suscribirse a la revisión mediante una dirección URL pública o código incrustado</strong> está desactivado para la revisión, los usuarios podrán iniciar sesión con sus credenciales de inicio de sesión de Workfront para agregar comentarios a la revisión. Si está activada, cualquier persona que proporcione su dirección de correo electrónico y nombre (sin contraseña) puede firmar y agregar comentarios a la prueba.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Enviar vínculo de descarga</td>
            <td>Incluye un botón en la notificación por correo electrónico que dirige a los usuarios a una página de descarga, que proporciona detalles del archivo, su nombre y tamaño, y que muestra el archivo en línea. Los usuarios pueden hacer clic en el vínculo Descargar de la página de descarga para descargar el archivo.</td>
           </tr>
           <tr>
            <td role="rowheader">Añadir mensaje personalizado</td>
            <td>Permite especificar un asunto y un cuerpo personalizados para la notificación por correo electrónico.</td>
           </tr>
          </tbody>
         </table>

      1. Haga clic en **Enviar**.

         Los destinatarios reciben una notificación por correo electrónico que contiene información sobre la prueba y los botones que ha elegido incluir.

         ![](assets/proof-share-email-350x87.png)

## Adición de usuarios a una prueba

Puede añadir cualquier usuario de Workfront a la prueba si tiene derechos de edición sobre la prueba. Si la prueba tiene varias fases, agregue el usuario a una fase individual

>[!WARNING]
>
>Además de los métodos enumerados en este artículo, es posible agregar usuarios a una prueba al etiquetarlos en un comentario desde la pestaña Actualizaciones de una prueba existente. Sin embargo, los usuarios añadidos a una prueba de esta manera no recibirán una notificación por correo electrónico a menos que se les vuelva a etiquetar después de que se les haya agregado al flujo de trabajo de la prueba.
>
>Por lo tanto, recomendamos añadir usuarios a una prueba mediante uno de los métodos enumerados a continuación y no etiquetándolos en un comentario.
>

>[!NOTE]
>
>Tenga en cuenta lo siguiente si utiliza un plan de Workfront heredado en el que las pruebas se puedan habilitar y deshabilitar para un usuario:
>
>* Los destinatarios no necesitan tener la revisión habilitada para poder revisar la revisión.
>* Cuando el flujo de trabajo automatizado está habilitado y agrega un usuario a la revisión que no tiene la revisión habilitada en Workfront, se crea una nueva etapa dentro del flujo de trabajo automatizado. El usuario que está agregando se agrega automáticamente a esta nueva etapa cuando ve la prueba por primera vez. (Para obtener más información, consulte [Resumen del flujo de trabajo automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>

### Añada usuarios a una revisión existente desde la pestaña Documentos

1. Seleccione el documento que contiene la prueba a la que desea agregar usuarios.
1. Si la revisión no tiene un flujo de trabajo automatizado (fases), haga clic en el icono **Más** en la esquina superior derecha de la sección Fase 1 y, a continuación, haga clic en **Compartir** en el menú desplegable.

   O

   Si la revisión no tiene un flujo de trabajo automatizado, haga clic en el icono **Más** en la esquina superior derecha del escenario donde desea agregar al revisor y, a continuación, haga clic en **Compartir** en el menú desplegable.

1. En el cuadro **Compartir esta versión** que aparece, en **Compartir**, empiece a escribir el nombre o la dirección de correo electrónico del usuario con el que desea compartir la prueba y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

1. (Opcional) Repita este paso para agregar varios usuarios a la prueba.
1. (Opcional) Establezca una fecha límite para los revisores.
1. (Opcional) Asegúrese de que **Notificar a las personas por correo electrónico** esté seleccionado si desea que los revisores sepan que las ha agregado a la prueba.
1. (Opcional) **Agregue un mensaje personalizado** al correo electrónico.
1. Cuando haya agregado todos los revisores, haga clic en **Compartir**.

### Agregar usuarios a una prueba existente desde el visor de pruebas

Puede agregar usuarios a una prueba mientras la revisa en el Visor de pruebas web y en el Visor de pruebas de escritorio.

Para obtener más información, consulte [Compartir una prueba agregándole usuarios](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) en el artículo [Compartir una prueba desde el visor de pruebas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## Informar sobre aprobaciones de revisión

Puede crear un informe que informe sobre las aprobaciones de revisión compartidas en Workfront. Este informe proporciona la siguiente información de aprobación de pruebas en el sistema:

* Documento enviado para su aprobación
* Nombre del aprobador
* Versión de revisión
* Identificador de revisión
* Fecha de creación de revisión

Puede obtener acceso a esta aprobación al crear un informe basado en un objeto, como se describe en [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obtener más información sobre el informe de objetos de aprobaciones de pruebas, consulte la sección [Informe sobre objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) en [Comprender los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## Aprobar una revisión compartida

Cuando un usuario le añade a una prueba y concede la función Aprobador o la función Revisor y aprobador mediante un flujo de trabajo automatizado, la solicitud de aprobación se muestra en la pestaña Aprobaciones del área de Inicio o Mi trabajo. A continuación, puede ver la prueba y tomar una decisión de aprobación directamente desde Workfront.

Para obtener información sobre cómo tomar decisiones de aprobación en el área de Mi trabajo, vea [Aprobar trabajo del área de inicio](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) o [Aprobar trabajo](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) en [Aprobar trabajo](../../../review-and-approve-work/manage-approvals/approving-work.md).
