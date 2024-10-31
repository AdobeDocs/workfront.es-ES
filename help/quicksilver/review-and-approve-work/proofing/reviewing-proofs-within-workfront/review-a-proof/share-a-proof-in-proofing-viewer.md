---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Compartir una prueba desde el visor de pruebas
description: Puede compartir una prueba desde el visor de pruebas si el propietario o el creador de la prueba habilita el uso compartido.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: aaf5beb8692b2fdbb797ba908796d78b4ee8866c
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# Compartir una prueba desde el visor de pruebas

Puede compartir una prueba desde el visor de pruebas si el propietario o el creador de la prueba habilita el uso compartido.

>[!IMPORTANT]
>
>Debe habilitarse la configuración Permitir el uso compartido de la revisión mediante una URL pública o un código incrustado.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Compartir la URL

Puede compartir una prueba a través de una dirección URL si el propietario ha configurado la prueba para compartir. Los propietarios de pruebas pueden actualizar la configuración de uso compartido en cualquier momento. Para obtener más información, consulte [Editar configuración de revisión](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. Si no se muestra el menú del icono izquierdo, haga clic en el icono **Menú** en la esquina superior izquierda del visor de revisión.

   ![](assets/menu-icon-in-proofing-viewer-350x188.png)

1. En el menú del icono izquierdo del visor de revisión, haga clic en el icono **Compartir**.

   ![Compartir_btn_en_visor.png](assets/share-btn-in-viewer.png)

1. En las opciones de **Compartir revisión** que aparecen, asegúrese de que **Obtener vínculo para compartir** esté seleccionado.

1.  Realice una de las acciones siguientes:

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

## Uso compartido del código incrustado

Puede compartir una prueba mediante el código incrustado si el propietario de la prueba la ha configurado para esto.

Para compartir una prueba mediante el código incrustado:

1. En la barra de herramientas de la izquierda del visor de revisión, haga clic en el icono **Compartir**.

   ![Compartir_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. En las opciones de **Compartir revisión** que aparecen, haz clic en **Obtener código incrustado** y luego haz clic en **Copiar**.

## Compartir una prueba agregándole usuarios

Puede añadir usuarios a una prueba mientras revisa una prueba si tiene cualquiera de los siguientes permisos:

* Permisos de supervisor o administrador
* Permisos de responsable y usted es el creador o propietario de la prueba
* Permisos de responsable con la función de prueba de autor o moderador

Si la prueba tiene un flujo de trabajo automatizado, puede añadir al usuario a una fase individual. Para obtener más información, consulte [Resumen del flujo de trabajo automatizado](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

De forma predeterminada, los usuarios que agregue a la prueba:

* Reciba una notificación por correo electrónico con un vínculo a la prueba.
* Puede tomar decisiones de aprobación sobre la revisión desde el área de Inicio, tal como se describe en [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* No es necesario tener la revisión habilitada para poder revisarla.

Cuando el flujo de trabajo automatizado está habilitado y agrega un usuario a la revisión que no tiene la revisión habilitada en Workfront, se crea una nueva etapa dentro del flujo de trabajo automatizado. El usuario que está agregando se agrega automáticamente a esta nueva etapa cuando ve la prueba por primera vez. Para obtener más información, consulte [Resumen del flujo de trabajo automatizado](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Para compartir una prueba con usuarios individuales:

1. En la barra de herramientas de la izquierda del visor de revisión, haga clic en el icono **Compartir**.

   ![Compartir_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. Haga clic en **Agregar destinatarios** en la lista de la izquierda.
1. En **Nuevos destinatarios de prueba**, empiece a escribir el nombre del usuario con el que desea compartir la prueba y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. (Opcional) Cambie las opciones de cualquier revisor a la derecha del nombre de la persona:

   * **Función de revisión**: para obtener más información, consulte [Administrar funciones de revisión en Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **Fase**: (disponible solo si la prueba tiene un flujo de trabajo automatizado). Para obtener más información, consulte  [Resumen de fases del flujo de trabajo automatizado](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **Alertas por correo electrónico**: seleccione una de las siguientes opciones para especificar cómo se notificará a la persona sobre la actividad de la prueba.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Toda la actividad</td> 
        <td>Workfront envía un correo electrónico al revisor cada vez que se produce alguna actividad en la prueba, como un nuevo comentario, una respuesta o una decisión. <p>Esta es una buena opción para la persona que administra el proceso de revisión porque le permite ver la actividad a medida que se produce. </p><p>Los usuarios no reciben una alerta por correo electrónico sobre su propia actividad.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Respuestas a mis comentarios</td> 
        <td>Se envía un correo electrónico al revisor únicamente si alguien responde explícitamente a su comentario (esto excluye sus propias respuestas a sus propios comentarios). Esto significa que si alguien en la prueba hace un nuevo comentario, no se notifica al revisor.<p>Se recomienda esta configuración para los clientes de la prueba, de modo que no se les notifique ningún otro comentario sobre la prueba y solo se les notifique de las respuestas a sus propios comentarios.</p><p>Aunque no se notifica a los revisores con esta configuración de alerta por correo electrónico de otros comentarios nuevos, pueden ver todos los comentarios de la prueba en el visor de revisión.</p><p>Para obtener información acerca de los comentarios, vea <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Ver y responder a los comentarios de revisión</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisiones</td> 
        <td>Workfront envía un correo electrónico al revisor únicamente cuando alguien toma una decisión.<p>Esto puede resultar útil para la persona que administra el proceso de aprobación (como un administrador de proyectos) y necesita supervisar el progreso de la prueba y ver qué usuarios han tomado su decisión.</p><p>No se le notificará su propia decisión a menos que seleccione una opción de confirmación por correo electrónico al enviar su decisión.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisión final</td> 
        <td>Workfront envía un mensaje de correo electrónico cuando el último aprobador de la prueba ha tomado una decisión.<p>Esta alerta la suele utilizar el diseñador, que no suele tener que participar en la discusión de revisión real. Cuando se toma la decisión final, se notifica al diseñador y luego se puede tomar medidas sobre los cambios necesarios.</p><p>Esta alerta también puede ser útil para un jefe de departamento al que sólo se debe notificar cuando haya finalizado el proceso de revisión.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumen por hora</td> 
        <td>Workfront envía un correo electrónico al revisor cada hora con un resumen de todos los comentarios, respuestas y decisiones que se han producido en la hora.<p>El correo electrónico se envía únicamente cuando se produce una actividad distinta de la suya en las últimas horas. </p><p>Esta alerta es una buena manera de ver una descripción general del proyecto.</p><p>Un ejemplo de uso de este resumen es un revisor sénior que necesita una visión general del proyecto, pero no necesita que se le notifique inmediatamente de toda la actividad de la prueba.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumen diario</td> 
        <td>Workfront envía un correo electrónico con todos los comentarios, respuestas y decisiones enumerados solo los días en que hay actividad aparte de la suya propia.<p>Esta alerta es una buena manera de ver un resumen del proyecto sin verse abrumado por múltiples actualizaciones a lo largo del día.</p><p>Un ejemplo de uso de este resumen es un jefe de departamento que desea supervisar el progreso general del proyecto.</p><p>Para obtener más información, consulte <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Administrar notificaciones para comentarios y decisiones sobre pruebas</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Sin correo electrónico</td> 
        <td>Workfront no envía alertas por correo electrónico.<br>Esto es útil para una persona que se agrega a una prueba solamente con fines de referencia y no necesita ser notificada de ningún cambio.<p>El valor predeterminado del sistema es Resumen diario (también se ve como No configurado). Si usted o los revisores no realizan ningún otro cambio, todas las pruebas tienen esta configuración.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (Opcional) Repita los dos pasos anteriores para agregar varios usuarios a la prueba. 
1. (Opcional) Establezca un **Plazo** para los revisores (disponible solo si la prueba no tiene un flujo de trabajo automatizado).
1. (Opcional) Seleccione **Enviar notificación por correo electrónico a los nuevos destinatarios** para que sepan que los ha agregado a la prueba.
1. Cuando termine de agregar usuarios a la prueba, haga clic en **Listo.**
