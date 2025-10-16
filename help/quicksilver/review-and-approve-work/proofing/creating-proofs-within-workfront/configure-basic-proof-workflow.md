---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Creación de una prueba avanzada con un flujo de trabajo básico
description: Con un flujo de trabajo básico, puede asignar varios revisores a una prueba, pero no están organizados en fases. Todos los revisores que agregue podrán acceder a la prueba inmediatamente después de crearla.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '1793'
ht-degree: 72%

---

# Creación de una prueba avanzada con un flujo de trabajo básico

<!-- Audited: 1/2024 -->

Con un flujo de trabajo básico, puede asignar varios revisores a una prueba, pero no están organizados en fases. Todos los revisores que agregue podrán acceder a la prueba inmediatamente después de crearla.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td>
   <p>Cualquiera</p>
    </td> 
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
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a documentos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de una prueba avanzada con un flujo de trabajo básico

1. Vaya al proyecto, tarea o problema donde desee la revisión y, a continuación, haga clic en la pestaña **Documentos**.
1. Haga clic en **Añadir nuevo** > Revisión, cargue el contenido y trabaje en las secciones que se indican a continuación.

   o

   Pase el puntero por encima de un documento existente, haga clic en **Crear revisión** > **Revisión avanzada** y trabaje en las secciones que se indican a continuación.

## Configuración del flujo de trabajo y adición de revisores

1. En la sección Tipo de flujo de trabajo, elija **Básico**.
1. Especifique los usuarios que desea agregar y, a continuación, elija una Función de prueba.

   ![Nuevas funciones de revisión](assets/new-proof---roles-350x213.png)

1. En la tabla siguiente se enumera cada función y los derechos asociados a ella.

   <table border="1" cellspacing="15" cellpadding="1"> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p> </p> </th> 
      <th> <p><strong>Ver una prueba</strong> </p> </th> 
      <th> <p><strong>Añadir marcas</strong> </p> </th> 
      <th> <p><strong>Añadir comentarios</strong> </p> </th> 
      <th> <p><strong>Editar comentarios propios si no hay respuestas</strong> </p> </th> 
      <th> <p><strong>Tomar una decisión</strong> </p> </th> 
      <th> <p><strong>Eliminar los comentarios de otros</strong> </p> </th> 
      <th>Resolver comentarios</th> 
      <th>Aplicar acciones a los comentarios</th> 
      <th> <p><strong>Editar la prueba</strong> </p> </th> 
      <th>Compartir la prueba con otros usuarios</th> 
      <th>Crear nueva versión</th> 
      <th> <p><strong>Ver solicitudes de aprobación en el área de inicio</strong> </p> </th> 
      <th>Añadir nuevos revisores</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>Solo lectura</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Revisor</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Aprobador</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Revisor y aprobador</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Autor</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> </td> 
      <td>✓</td> 
     </tr> 
     <tr> 
      <td> <p><strong>Moderador</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p><strong>✓</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
     </tr> 
    </tbody> 
   </table>

1. Los usuarios de los nuevos planes de Workfront pueden otorgar funciones de autor o moderador a cualquier usuario del sistema. Los usuarios de los planes heredados pueden conceder funciones de autor o moderador a cualquier usuario con una licencia de prueba en el sistema.
1. (Opcional) Con el menú desplegable aún abierto, seleccione los permisos adicionales disponibles en la parte inferior del menú:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Resolver comentarios y aplicar acciones </td> 
      <td> <p>Permite al usuario de Workfront hacer lo siguiente:</p> 
       <ul> 
        <li>Resuelva un comentario una vez que se haya dirigido, tal como se explica en <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">Resolver comentarios de prueba</a>.</li> 
        <li>Aplicar acciones a comentarios, como se explica en <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">Usar acciones en comentarios de revisión</a>. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartir la revisión mediante etiquetado</td> 
      <td> <p>Permite que el revisor agregue cualquier usuario de Workfront a la revisión, tal como se explica en <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">Etiquete a los usuarios para que compartan una revisión</a>.</p> <p>Nota:  <p>Si estas dos opciones no están disponibles (atenuadas), el usuario ya tiene un perfil de permisos que permite resolver comentarios, aplicar acciones a los comentarios y etiquetar a cualquier usuario. </p> <p>Si no aparecen las opciones, la persona que ha añadido no es titular de una licencia de Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Repita los pasos del 1 al 3 con los demás usuarios que haya agregado a la prueba.
1. Para cada usuario con el que comparta, en la lista desplegable **Alertas de correo electrónico**, seleccione el tipo de alertas de correo electrónico que este usuario recibe cuando las personas realizan comentarios y toman decisiones sobre la prueba:

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
      <td>Se envía un correo electrónico al revisor únicamente si una persona responde explícitamente a su comentario (esto excluye sus propias respuestas a sus propios comentarios). Esto significa que si una persona en la prueba hace un nuevo comentario, no se le notifica al revisor.<p>Se recomienda esta configuración para los clientes de la prueba, para que no se les notifique ningún otro comentario en la prueba y solo se les notifique las respuestas a sus propios comentarios.</p><p>Aunque no se notifica a los revisores con esta configuración de alerta por correo electrónico de otros comentarios nuevos, pueden seguir viendo todos los comentarios de la prueba en el visor de corrección.</p><p>Para obtener información acerca de los comentarios, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Ver y responder a los comentarios de revisión</a>.</p></td> 
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
      <td>Workfront envía un correo electrónico con todos los comentarios, respuestas y decisiones enumerados solo los días en que hay actividad aparte de la suya propia.<p>Esta alerta es una buena manera de ver un resumen del proyecto sin verse abrumado por múltiples actualizaciones a lo largo del día.</p><p>Un ejemplo de uso de este resumen es un jefe de departamento que desea supervisar el progreso general del proyecto.</p><p>Para obtener más información, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Administrar notificaciones para comentarios y decisiones de la prueba</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">No hay correo electrónico</td> 
      <td>Workfront no envía alertas por correo electrónico.<br>Esto es útil para una persona que se añade a una prueba solamente como referencia y no necesita que se le notifique de ningún cambio.<p>El valor predeterminado del sistema es Resumen diario (también se visualiza como no configurado). Si usted o los revisores no realizan ningún otro cambio, todas las pruebas tienen esta configuración.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continúe con [Configurar opciones de correo electrónico para la revisión](#configure-email-settings-for-the-proof) que se muestra a continuación.

## Configurar opciones de correo electrónico para la revisión {#configure-email-settings-for-the-proof}

1. En la sección **Notificación por correo electrónico**, seleccione si desea enviar notificaciones por correo electrónico y un mensaje personalizado a los usuarios seleccionados en [Crear una prueba avanzada con un flujo de trabajo básico](#workflow), anteriormente en este artículo:

   <table>
   <tbody>
   <tr>
   <td>Notificar a los destinatarios sobre esta prueba</td>
   <td>Seleccione esta opción para enviar una notificación por correo electrónico a los usuarios. Cuando se selecciona <strong>Uso compartido básico</strong> en la sección <strong>Flujo de trabajo</strong>, se envía una notificación por correo electrónico cuando se crea la prueba. Cuando se selecciona <strong>Flujo de trabajo automatizado</strong> en la sección <strong>Flujo de trabajo</strong>, se envía una notificación por correo electrónico cuando la prueba entra en la fase del flujo de trabajo automatizado con el que se asocia el usuario.</td>
   </tr>
   <tr>
   <td>Añadir mensaje personalizado</td>
   <td>Seleccione esta opción para incluir un mensaje personalizado en la notificación. Puede especificar el asunto y el cuerpo del mensaje. El cuerpo del mensaje puede incluir formato de texto enriquecido, como negrita, viñetas e hipervínculos.</td>
   </tr>
   </tbody>
   </table>


1. Continúe con [Configurar opciones de prueba](#configure-proof-settings) que se muestra a continuación.

## Configurar opciones de prueba {#configure-proof-settings}

1. En la sección **Configuración de prueba**, seleccione cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Inicio de sesión obligatorio: la prueba solo se puede compartir con otros usuarios</td> 
      <td>Cuando esta opción está deshabilitada (predeterminada), cualquier persona con la URL puede ver la prueba. <br>Cuando se selecciona esta opción:
       <ul>
        <li>Solo los usuarios de Workfront Proof pueden ver la revisión.</li>
        <li>Los usuarios no pueden iniciar sesión en la prueba a menos que se les haya añadido a la prueba.</li>
        <li>No se pueden habilitar las suscripciones.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Solo se requiere una decisión para esta prueba</td> 
      <td>Cuando se selecciona esta opción, la prueba se completa después de que uno de los responsables de la toma de decisiones tome su decisión.<br>Esta opción está desactivada de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requerir que las decisiones se firmen electrónicamente</td> 
      <td>Los usuarios deben especificar su nombre de usuario y contraseña en el momento en el que toman una decisión sobre una prueba.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear prueba cuando se toman todas las decisiones necesarias</td> 
      <td>Cuando esta configuración está habilitada, el estado de prueba se bloquea después de que se hayan tomado todas las decisiones. El estado cambia automáticamente de desbloqueado a bloqueado cuando el aprobador final toma su decisión.<br>Esta opción está desactivada de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descargar archivo original</td> 
      <td>Cuando se selecciona esta opción, los revisores pueden descargar el archivo original desde el que se creó la prueba.<br>Cuando esta opción no está seleccionada, el icono Descargar ya no es visible.<br>Esta opción está deshabilitada de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que se comparta la prueba mediante una dirección URL pública o código incrustado</td> 
      <td>Cuando se selecciona esta opción, la prueba se puede compartir mediante una URL pública o un código incrustado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suscribirse a la prueba mediante una dirección URL pública o código incrustado</td> 
      <td>Si se selecciona esta opción, las personas que no se hayan añadido explícitamente a la prueba podrán suscribirse a ella. A la persona que se suscribe a la prueba se le concede la función y el correo electrónico que defina en la siguiente configuración:
       <ul>
        <li><strong>Rol de suscriptor:</strong> El rol de prueba predeterminado que se asigna a todos los revisores que se suscriben a la prueba. </li>
        <li><strong>Configuración de alertas de correo electrónico para suscriptores:</strong> La alerta de correo electrónico predeterminada asignada a todos los revisores que se suscriben a la revisión.</li>
       </ul><p>
        <ul>
         <li><strong>Se requiere acceso a la prueba mediante un vínculo de correo electrónico para:</strong> Configure si el suscriptor recibe un correo electrónico con un vínculo a la prueba. Puede seleccionar <strong>Sin correo electrónico</strong> (el vínculo de correo electrónico no es necesario para acceder a la prueba), <strong>Solo correo electrónico de notificación de prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico sin ninguna verificación) o <strong>Correos electrónicos de notificación de validación y prueba</strong> (el suscriptor recibe un vínculo a la prueba por correo electrónico y debe hacer clic en el vínculo para acceder a una prueba, el propósito de esta opción es garantizar que la persona haya escrito una dirección de correo electrónico correcta a la que tenga acceso).</li>
        </ul><p>Nota:  Si las pruebas tienen un flujo de trabajo automatizado adjunto, todas las suscripciones generarán correos electrónicos de confirmación a los propietarios de la prueba para que puedan decidir a qué fase se debe agregar a la persona.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Crear prueba**.

   Workfront comienza a generar una prueba de los documentos o sitios web seleccionados. Según el tamaño y el tipo de archivo, el tiempo de posposición de la carga de un documento puede variar. Tenga en cuenta que los archivos grandes tardan más en generarse. Puede salir de la página y Workfront seguirá generando el archivo. El tamaño máximo de carga de archivo es de 4 GB.

1. Una vez generada la revisión, haga clic en **Abrir revisión** para iniciar el visor de revisiones.

   ![Abrir revisión](assets/open-proof-350x132.png)

   Los usuarios que no tengan la revisión habilitada en su cuenta aún pueden ver el documento y realizar comentarios en la revisión.
