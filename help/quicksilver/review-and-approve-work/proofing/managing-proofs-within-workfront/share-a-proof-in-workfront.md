---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Compartir una prueba en Adobe Workfront
description: Comparta documentos revisados en Adobe Workfront mediante el uso compartido o añadiendo usuarios a la prueba.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 94%

---

# Compartir una prueba en Adobe Workfront

Comparta documentos revisados en Adobe Workfront mediante el uso compartido o añadiendo usuarios a la prueba.

Como se explica en este artículo, al compartir la prueba el destinatario tendrá el mismo acceso al documento y a la prueba. Además, es posible solicitar la aprobación de la prueba al destinatario.

>[!TIP]
>
>También es posible compartir pruebas desde el visualizador de revisión. Para obtener instrucciones, consulte [Compartir pruebas desde el visualizador de revisión](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Estándar</p>
   <p>Trabajo o plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de prueba </td> 
   <td>Administrador o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Función de prueba</td> 
   <td>Autor o moderador</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a documentos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Compartir un vínculo de prueba

Al compartir un vínculo de prueba, los usuarios de Workfront podrán ver el acceso. Los usuarios pueden realizar comentarios sobre la prueba y suscribirse a las notificaciones por correo electrónico de la prueba con sus credenciales de inicio de sesión de Workfront. Los usuarios que no sean revisores podrán realizar comentarios y suscribirse mediante una dirección de correo electrónico y un nombre para mostrar.

>[!IMPORTANT]
>
>Debe habilitarse la configuración Permitir el uso compartido de pruebas mediante una URL pública o código incrustado.

1. Seleccione el documento que contenga la prueba que quiera compartir con los usuarios.

   Solo es posible seleccionar un documento. No se puede compartir el vínculo para varios documentos al mismo tiempo.

1. Haga clic en **Compartir** > **Vínculo de prueba**.
1. En el cuadro **Vínculo de prueba** que aparezca, realice una de las acciones siguientes:

   * Para copiar el vínculo en el portapapeles, haga clic en **Copiar vínculo**.

     Ahora puede distribuir el vínculo mediante una herramienta de terceros, como un chat o una aplicación de correo electrónico.

   * Para enviar por correo electrónico el vínculo directamente desde Adobe Workfront, haga lo siguiente:

      1. En el campo **O enviar un vínculo por correo electrónico a**, empiece a escribir y seleccione el nombre del destinatario. O bien especifique la dirección de correo electrónico de un usuario externo con el que desea compartir.

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
            <td><p>Incluye un botón en la notificación por correo electrónico que dirige a los usuarios a la prueba dentro del visor de corrección que están utilizando y concede acceso de visualización.</p><p>Si la opción <strong>Suscribirse a la prueba mediante una dirección URL pública o código incrustado</strong> está desactivada para la prueba, los usuarios podrán iniciar sesión con sus credenciales de inicio de sesión de Workfront para añadir comentarios a ella. Si está activada, cualquier persona que facilite su dirección de correo electrónico y nombre (no se necesita contraseña) puede firmar y añadir comentarios a la prueba.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Enviar vínculo de descarga</td>
            <td>Incluye un botón en la notificación por correo electrónico que dirige a los usuarios a una página de descarga, que proporciona detalles del archivo, su nombre y tamaño, y que muestra el archivo en línea. Los usuarios pueden hacer clic en el vínculo Descargar de la página de descarga para descargar el archivo.</td>
           </tr>
           <tr>
            <td role="rowheader">Añadir mensaje personalizado</td>
            <td>Le permite especificar un asunto y un cuerpo personalizados para la notificación por correo electrónico.</td>
           </tr>
          </tbody>
         </table>

      1. Haga clic en **Enviar**.

         Los destinatarios reciben una notificación por correo electrónico que contiene información sobre la prueba y los botones que ha elegido incluir.

         ![](assets/proof-share-email-350x87.png)

## Adición de usuarios a una prueba

Añada a cualquier usuario de Workfront a la prueba en caso de disponer de derechos de edición sobre la misma. Si la prueba tuviera varias fases, añada al usuario a una fase individual

>[!WARNING]
>
>Además de los métodos enumerados en este artículo, es posible añadir usuarios a una prueba al etiquetarlos en comentarios desde la pestaña Actualizaciones de una prueba existente. Sin embargo, los usuarios añadidos a una prueba de esta manera no recibirán una notificación por correo electrónico a menos que se les vuelva a etiquetar después de que se les haya añadido al flujo de trabajo de la prueba.
>
>Por lo tanto, se recomienda añadir usuarios a pruebas mediante uno de los métodos enumerados a continuación y no etiquetándolos en comentarios.
>

>[!NOTE]
>
>Tenga en cuenta lo siguiente al usar un plan de Workfront heredado en el que las pruebas se puedan habilitar y deshabilitar para un usuario:
>
>* Los destinatarios no necesitan tener la revisión habilitada para poder revisar pruebas.
>* Cuando el flujo de trabajo automatizado está habilitado y añade un usuario a la prueba que no tiene la revisión habilitada en Workfront, se crea una nueva fase dentro del flujo de trabajo automatizado. El usuario que está añadiendo se añade automáticamente a esta nueva fase cuando ve la prueba por primera vez. (Para obtener más información, consulte [Información general sobre flujos de trabajo automatizados](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)).
>

### Añada usuarios a pruebas existentes desde la pestaña Documentos

1. Seleccione el documento que contenga la prueba a la que quiera añadir usuarios.
1. Si la prueba no tuviera un flujo de trabajo automatizado (fases), haga clic en el icono **Más** de la esquina superior derecha de la sección Fase 1 y, a continuación, haga clic en **Compartir**, en el menú desplegable.

   O

   Si la prueba no tuviera un flujo de trabajo automatizado, haga clic en el icono **Más** de la esquina superior derecha del escenario del que quiera añadir el revisor y, a continuación, haga clic en **Compartir**, en el menú desplegable.

1. En el cuadro **Compartir esta versión** que aparezca, en **Compartir**, empiece a escribir el nombre o la dirección de correo electrónico del usuario con el que quiera compartir la prueba y, a continuación, haga clic en el nombre cuando aparezca de la lista desplegable.

1. (Opcional) Repita este paso para añadir varios usuarios a la prueba.
1. (Opcional) Establezca una fecha límite para los revisores.
1. (Opcional) Asegúrese de que **Notificar a los usuarios por correo electrónico** esté seleccionado en caso de querer que los revisores sepan que se les añadió a la prueba.
1. (Opcional) **Añada un mensaje personalizado** al correo electrónico.
1. Cuando haya añadido a todos los revisores, haga clic en **Compartir**.

### Añadir usuarios a pruebas existentes desde el visualizador de revisión

Es posible añadir usuarios a pruebas mientras se revisan en el Visualizador de revisión web y en el Visualizador de revisión de escritorio.

Para obtener más información, consulte [Compartir una prueba añadiéndole usuarios](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) en el artículo [Compartir una prueba desde el visualizador de pruebas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## Informar sobre aprobaciones de revisión

Es posible crear un informe que muestre las aprobaciones de revisión compartidas en Workfront. Este informe proporcionará la siguiente información de aprobación de pruebas en el sistema:

* Documento enviado para su aprobación
* Nombre del aprobador
* Versión de la prueba
* Identificador de revisión
* Fecha de creación de la prueba

Se accede a esta aprobación al crear un informe basado en un objeto, tal y como se describe en [Creación de informes personalizados](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obtener más información sobre el informe de objetos de aprobaciones de pruebas, consulte la sección [Informes sobre objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects), en [Comprender los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## Aprobación de pruebas compartidas

Cuando un usuario le añade a una prueba y concede la función Aprobador o la función Revisor y aprobador mediante un flujo de trabajo automatizado, la solicitud de aprobación se muestra en el widget Mis aprobaciones del área de Inicio. A continuación, será posible consultar la prueba y tomar una decisión de aprobación directamente desde Workfront.

Para obtener información sobre cómo tomar decisiones de aprobación desde el widget Mis aprobaciones, consulte [Aprobar trabajo desde el área de inicio](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) o [Aprobar trabajo](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) en [Aprobar trabajo](../../../review-and-approve-work/manage-approvals/approving-work.md).
