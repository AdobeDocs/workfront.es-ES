---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Compartir una prueba desde el visor de corrección
description: Puede compartir una prueba desde el visor de corrección si el propietario o el creador de la prueba habilita el uso compartido.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 98%

---

# Compartir una prueba desde el visor de corrección

Puede compartir una prueba desde el visor de corrección si el propietario o el creador de la prueba habilita el uso compartido.

>[!IMPORTANT]
>
>Debe habilitarse la configuración Permitir el uso compartido de pruebas mediante una URL pública o código incrustado.

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
   <td> <p>Acceso de edición a documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Compartir la URL

Puede compartir una prueba a través de una URL si el propietario ha configurado la prueba para su uso compartido. Los propietarios de pruebas pueden actualizar la configuración de uso compartido en cualquier momento. Para obtener más información, consulte [Editar configuración de prueba](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. Si no se muestra el menú del icono izquierdo, haga clic en el icono del **Menú** en la esquina superior izquierda del visor de corrección.

   ![Icono de menú](assets/menu-icon-in-proofing-viewer-350x188.png)

1. En el menú del icono izquierdo del visor de corrección, haga clic en el icono **Compartir**.

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. En las opciones de **Compartir prueba** que aparecen, asegúrese de que **Obtener vínculo para compartir** esté seleccionado.

1. Realice una de las siguientes acciones:

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

## Compartir el código incrustado

Puede compartir una prueba mediante el código incrustado si el propietario de la prueba la ha configurado para ello.

Para compartir una prueba mediante el código incrustado:

1. En la barra de herramientas de la izquierda del visor de corrección, haga clic en el icono **Compartir**.

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. En las opciones de **Compartir prueba** que aparecen, haz clic en **Obtener código incrustado** y luego haz clic en **Copiar**.

## Compartir una prueba añadiéndole usuarios

Puede añadir usuarios a una prueba mientras la revisa si tiene cualquiera de los siguientes permisos:

* Permisos de supervisor o administrador
* Permisos de administrador y usted es el creador o propietario de la prueba
* Permisos de administrador con la función de prueba de autor o moderador

Si la prueba tiene un flujo de trabajo automatizado, puede añadir al usuario a una fase individual. Para obtener más información, consulte [Información general de flujo de trabajo automatizado](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

De forma predeterminada, los usuarios que añada a la prueba:

* Reciben una notificación por correo electrónico con un vínculo a la prueba.
* Puede tomar decisiones de aprobación sobre la revisión desde el área de Inicio, tal como se describe en [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* No es necesario tener la revisión habilitada para poder revisar la prueba.

Cuando el flujo de trabajo automatizado está habilitado y añade un usuario a la prueba que no tiene la revisión habilitada en Workfront, se crea una nueva fase dentro del flujo de trabajo automatizado. El usuario que está añadiendo se añade automáticamente a esta nueva fase cuando ve la prueba por primera vez. Para obtener más información, consulte [Información general de flujo de trabajo automatizado](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Para compartir una prueba con usuarios individuales:

1. En la barra de herramientas de la izquierda del visor de revisión, haga clic en el icono **Compartir**.

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. Haga clic en **Añadir destinatarios** en la lista de la izquierda.
1. En **Nuevos destinatarios de prueba**, empiece a escribir el nombre del usuario con el que desea compartir la prueba y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. (Opcional) Cambie las opciones de cualquier revisor a la derecha del nombre de la persona:

   * **Función de prueba**: para obtener más información, consulte [Administrar funciones de prueba en Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **Fase**: (disponible solo si la prueba tiene un flujo de trabajo automatizado). Para obtener más información, consulte [Visión general de fases del flujo de trabajo automatizado](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **Alertas por correo electrónico**: seleccione una de las siguientes opciones para especificar cómo se notificará a la persona sobre la actividad de la prueba.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Toda la actividad</td> 
        <td>Workfront envía un correo electrónico al revisor cada vez que se produce alguna actividad en la prueba, como un nuevo comentario, una respuesta o una decisión. <p>Es una buena opción para la persona que administra el proceso de revisión porque le permite ver la actividad a medida que ocurre. </p><p>Los usuarios no reciben una alerta por correo electrónico sobre su propia actividad.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Respuestas a mis comentarios</td> 
        <td>Se envía un correo electrónico al revisor únicamente si una persona responde explícitamente a su comentario (esto excluye sus propias respuestas a sus propios comentarios). Esto significa que si una persona en la prueba hace un nuevo comentario, no se le notifica al revisor.<p>Se recomienda esta configuración para los clientes de la prueba, para que no se les notifique ningún otro comentario en la prueba y solo se les notifique las respuestas a sus propios comentarios.</p><p>Aunque no se notifica a los revisores con esta configuración de alerta por correo electrónico de otros comentarios nuevos, pueden seguir viendo todos los comentarios de la prueba en el visor de corrección.</p><p>Para obtener información acerca de los comentarios, consulte <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Ver y responder a los comentarios de revisión</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisiones</td> 
        <td>Workfront envía un correo electrónico al revisor únicamente cuando alguien toma una decisión.<p>Esto puede resultar útil para la persona que administra el proceso de aprobación (como un administrador de proyecto) y necesita supervisar el progreso de la prueba y ver qué usuarios han tomado su decisión.</p><p>No se le notificará su propia decisión a menos que seleccione una opción de confirmación por correo electrónico al enviar su decisión.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisión final</td> 
        <td>Workfront envía un mensaje de correo electrónico cuando el último aprobador de la prueba ha tomado una decisión.<p>Esta alerta la suele utilizar el diseñador, que no suele tener que participar en la discusión de revisión real. Cuando se toma la decisión final, se notifica al diseñador y, a continuación se pueden tomar medidas sobre los cambios necesarios.</p><p>Esta alerta también puede ser útil para un jefe de departamento al que solo se debe notificar cuando haya finalizado el proceso de revisión.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumen por horas</td> 
        <td>Workfront envía un correo electrónico al revisor cada hora con un resumen de todos los comentarios, respuestas y decisiones que se han producido en la hora.<p>El correo electrónico se envía únicamente cuando se produce una actividad distinta de la suya en la última hora. </p><p>Esta alerta es una buena manera de ver una descripción general del proyecto.</p><p>Un ejemplo de uso de este resumen es un revisor sénior que necesita una visión general del proyecto, pero no necesita que se le notifique inmediatamente de toda la actividad de la prueba.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumen diario</td> 
        <td>Workfront envía un correo electrónico con todos los comentarios, respuestas y decisiones enumerados solo los días en que hay actividad aparte de la suya propia.<p>Esta alerta es una buena manera de ver un resumen del proyecto sin verse abrumado por múltiples actualizaciones a lo largo del día.</p><p>Un ejemplo de uso de este resumen es un jefe de departamento que desea supervisar el progreso general del proyecto.</p><p>Para obtener más información, consulte <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Administrar notificaciones para comentarios y decisiones de la prueba</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">No hay correo electrónico</td> 
        <td>Workfront no envía alertas por correo electrónico.<br>Esto es útil para una persona que se añade a una prueba solamente como referencia y no necesita que se le notifique de ningún cambio.<p>El valor predeterminado del sistema es Resumen diario (también se visualiza como no configurado). Si usted o los revisores no realizan ningún otro cambio, todas las pruebas tienen esta configuración.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (Opcional) Repita los dos pasos anteriores para añadir varios usuarios a la prueba. 
1. (Opcional) Establezca una **Fecha límite** para los revisores (disponible solo si la prueba no tiene un flujo de trabajo automatizado).
1. (Opcional) Seleccione **Enviar notificación por correo electrónico a los nuevos destinatarios** para que sepan que los ha añadido a la prueba.
1. Cuando termine de añadir usuarios a la prueba, haga clic en **Listo.**
