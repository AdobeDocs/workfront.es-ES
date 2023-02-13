---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Compartir una prueba desde el visor de pruebas
description: Puede compartir una prueba desde el visualizador de pruebas si el propietario o el creador de la prueba han habilitado el uso compartido.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# Compartir una prueba desde el visor de pruebas

Puede compartir una prueba desde el visualizador de pruebas si el propietario o el creador de la prueba han habilitado el uso compartido.

>[!IMPORTANT]
>
>La configuración Permitir compartir prueba mediante URL pública o código incrustado debe estar habilitada.

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
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con el administrador de Workfront o Workfront Proof.

## Compartir la dirección URL

Puede compartir una prueba a través de una URL si el propietario ha configurado la prueba para compartir. Los propietarios de pruebas pueden actualizar la configuración de uso compartido en cualquier momento. Para obtener más información, consulte [Editar configuración de prueba](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. Si no se muestra el menú de icono de la izquierda, haga clic en el botón **Menú** en la esquina superior izquierda del visor de pruebas.

   ![](assets/menu-icon-in-proofing-viewer-350x188.png)

1. En el menú de icono de la izquierda del visualizador de pruebas, haga clic en el botón **Compartir** icono.

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. En el **Prueba de uso compartido** opciones que aparecen, asegúrese de **Obtener vínculo que se puede compartir** está seleccionado.

1.  Realice una de las siguientes acciones:

   * Para copiar el vínculo en el portapapeles, haga clic en **Copiar vínculo**.

      Ahora puede distribuir el vínculo a través de una herramienta de terceros, como un chat o una aplicación de correo electrónico.

   * Para enviar el vínculo directamente desde Adobe Workfront por correo electrónico, haga lo siguiente:

      1. En el **O enlace de correo electrónico a** , empiece a escribir y seleccione el nombre del destinatario. O especifique la dirección de correo electrónico de un usuario externo con el que desee compartir.

         >[!NOTE]
         >
         >Si ve un correo electrónico con alias al compartir una prueba, no cree un nuevo usuario invitado introduciendo el correo electrónico original si existe el correo electrónico con alias correspondiente.

      1. Seleccione entre las siguientes opciones:

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Enviar vínculo público</td>
            <td><p>Incluye un botón en la notificación por correo electrónico que dirige a los usuarios a la prueba dentro del visor de pruebas que están utilizando y concede acceso a la vista.</p><p>If <strong>Suscripción a la prueba mediante URL pública o código incrustado</strong> está desactivado para la prueba, los usuarios pueden iniciar sesión con sus credenciales de inicio de sesión de Workfront para agregar comentarios a la prueba. Si está activada, cualquier persona que proporcione su dirección de correo electrónico y su nombre (no se requiere contraseña) puede firmar y agregar comentarios a la prueba.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Enviar vínculo de descarga</td>
            <td>Incluye un botón en la notificación por correo electrónico que dirige a los usuarios a una página de descarga y que proporciona detalles del archivo, el nombre del archivo y el tamaño del archivo, y el archivo se muestra en línea. Los usuarios pueden hacer clic en el vínculo Descargar de la página de descarga para descargar el archivo.</td>
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

Para compartir una prueba mediante el código de incrustación:

1. En la barra de herramientas de la izquierda del visualizador de pruebas, haga clic en el botón **Compartir** icono.

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. En el **Prueba de uso compartido** opciones que aparecen, haga clic en **Obtener código incrustado** y haga clic en **Copiar**.

## Compartir una prueba agregándole usuarios

Puede agregar usuarios a una prueba mientras revisa una prueba si tiene cualquiera de los siguientes permisos:

* Permisos de supervisor o administrador
* Permisos de administrador y usted es el creador o propietario de la prueba
* Permisos de administrador con la función de prueba Autor o Moderador

Si la prueba tiene un flujo de trabajo automatizado, puede agregar el usuario a una etapa individual. Para obtener más información, consulte [Resumen del flujo de trabajo automatizado](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

De forma predeterminada, los usuarios que agregue a la prueba:

* Reciba una notificación por correo electrónico con un vínculo a la prueba.
* Puede tomar decisiones de aprobación en la prueba desde el área Inicio o Mi trabajo, tal como se describe en [Aprobación del trabajo](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* No es necesario tener las pruebas habilitadas para revisar la prueba.

Cuando Flujo de trabajo automatizado está habilitado y agrega un usuario a la prueba que no tiene la prueba habilitada en Workfront, se crea una nueva etapa en el Flujo de trabajo automatizado. El usuario que está agregando se agrega automáticamente a esta nueva etapa cuando ve la prueba por primera vez. Para obtener más información, consulte [Resumen del flujo de trabajo automatizado](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Para compartir una prueba con usuarios individuales:

1. En la barra de herramientas de la izquierda del visualizador de pruebas, haga clic en el botón **Compartir** icono.

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. Haga clic en **Añadir destinatarios** en la lista de la izquierda.
1. En **Nuevos destinatarios de prueba**, empiece a escribir el nombre de un usuario con el que desee compartir la prueba y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. (Opcional) Cambie las opciones del revisor a la derecha del nombre de la persona:

   * **Función de prueba**: Para obtener más información, consulte [Administrar funciones de prueba en la prueba de Workfront](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **Prueba**: (Disponible solo si la prueba tiene un flujo de trabajo automatizado). Para obtener más información, consulte  [Resumen de las etapas del flujo de trabajo automatizado](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **Alertas de correo electrónico**: seleccione una de las siguientes opciones para especificar cómo se notificará a la persona sobre la actividad en la prueba.

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Todas las actividades</td> 
        <td>Workfront envía un correo electrónico al revisor cada vez que hay alguna actividad en la prueba, como un nuevo comentario, respuesta o decisión. <p>Esta es una buena opción para la persona que está administrando el proceso de prueba porque les permite ver la actividad a medida que pasa. </p><p>Los usuarios no reciben una alerta por correo electrónico sobre su propia actividad.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Respuestas a mis comentarios</td> 
        <td>Solo se envía un correo electrónico al revisor si alguien responde explícitamente a su comentario (esto excluye sus propias respuestas en sus propios comentarios). Esto significa que si alguien de la prueba realiza un comentario nuevo, no se notifica al revisor.<p>Se recomienda este ajuste para los clientes en la prueba, de modo que no se les notifique de ningún otro comentario en la prueba y solo se les notifique de las respuestas a sus propios comentarios.</p><p>Aunque los revisores con esta configuración de alerta de correo electrónico no reciben notificaciones de otros comentarios nuevos, aún pueden ver todos los comentarios de la prueba en el visor de pruebas.</p><p>Para obtener información sobre los comentarios, consulte <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Ver y responder comentarios de prueba</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisiones</td> 
        <td>Workfront envía un correo electrónico al revisor solo cuando alguien toma una decisión.<p>Esto puede resultar útil para la persona que administra el proceso de aprobación (como un administrador de proyectos) y necesita monitorizar el progreso de la prueba y ver qué usuarios han tomado su decisión.</p><p>No se le notificará su propia decisión a menos que seleccione una opción de confirmación por correo electrónico al presentar su decisión.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisión final</td> 
        <td>Workfront envía un correo electrónico cuando el último aprobador de la prueba ha tomado una decisión.<p>Esta alerta la utiliza a menudo el diseñador, que no suele necesitar participar en la conversación de revisión real. Cuando se toma la decisión final, se notifica al diseñador y éste puede tomar las medidas necesarias.</p><p>Esta alerta también puede ser útil para un jefe de departamento al que solo se le debe notificar cuando haya terminado el proceso de revisión.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumen por hora</td> 
        <td>Workfront envía un correo electrónico al revisor cada hora con un resumen de todos los comentarios, respuestas y decisiones que se hayan producido en la hora.<p>El correo electrónico solo se envía cuando la actividad que no sea la suya tiene lugar en la última hora. </p><p>Esta alerta es una buena forma de ver una descripción general del proyecto.</p><p>Un caso de uso de ejemplo para este resumen es un revisor principal que necesita una descripción general del proyecto, pero no es necesario que se le notifique inmediatamente de toda la actividad de la prueba.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumen diario</td> 
        <td>Workfront envía un correo electrónico con todos los comentarios, respuestas y decisiones que aparecen solo en los días en que hay actividad además de la suya propia.<p>Esta alerta es una buena manera de ver un resumen del proyecto sin estar abrumado con múltiples actualizaciones a lo largo del día.</p><p>Un ejemplo de caso de uso para este resumen es un jefe de departamento que desea supervisar el progreso general del proyecto.</p><p>Para obtener más información, consulte <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Administrar notificaciones para comentarios y decisiones de prueba</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Sin correo electrónico</td> 
        <td>Workfront no envía ninguna alerta por correo electrónico.<br>Esto es útil para una persona que se agrega a una prueba solo con fines de referencia y no necesita que se le notifique de ningún cambio.<p>El sistema predeterminado es Resumen diario (también se ve como No establecido). Si usted o los revisores no realizan ningún otro cambio, todas las pruebas tendrán esta configuración.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (Opcional) Repita los dos pasos anteriores para agregar varios usuarios a la prueba. 
1. (Opcional) Configure un **Fecha límite** para los revisores (solo disponible si la prueba no tiene flujo de trabajo automatizado).
1. (Opcional) Seleccione **Enviar notificación por correo electrónico a nuevos destinatarios** para hacerles saber que los ha añadido a la prueba.
1. Cuando haya terminado de agregar usuarios a la prueba, haga clic en **Listo.**
