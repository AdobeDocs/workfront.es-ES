---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Creación de una prueba avanzada con un flujo de trabajo básico
description: Con un flujo de trabajo básico, puede asignar varios revisores a una prueba, pero no están organizados en fases. Todos los revisores que agregue podrán acceder a la prueba inmediatamente después de crearla.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1853'
ht-degree: 1%

---

# Creación de una prueba avanzada con un flujo de trabajo básico

<!-- Audited: 1/2024 -->

Con un flujo de trabajo básico, puede asignar varios revisores a una prueba, pero no están organizados en fases. Todos los revisores que agregue podrán acceder a la prueba inmediatamente después de crearla.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td>
   <p>Nuevo: Cualquiera</p>
    <p>Plan actual: Pro o Superior</p>
   <p>Plan heredado: Select o Superior</p> <p>Para obtener más información sobre cómo revisar el acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
    <p>Actual: Trabajo o Plan</p> <p>Plan heredado: Cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Responsable o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a documentos</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Creación de una prueba avanzada con un flujo de trabajo básico

1. Vaya al proyecto, tarea o problema donde desee la prueba y, a continuación, haga clic en la ficha **Documentos**.
1. Haga clic en **Agregar nuevo** > Prueba, cargue el contenido y luego revise las secciones que se indican a continuación.

   o

   Pase el ratón sobre un documento existente y luego haga clic en **Crear revisión** > **Revisión avanzada**, y revise las secciones que se indican a continuación.

## Configuración del flujo de trabajo y adición de revisores

1. En la sección Tipo de flujo de trabajo, elija **Básico**.
1. Especifique los usuarios que desea agregar y, a continuación, elija una Función de prueba.

   ![](assets/new-proof---roles-350x213.png)

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
      <th> <p><strong>Ver una revisión</strong> </p> </th> 
      <th> <p><strong>Agregar marcas</strong> </p> </th> 
      <th> <p><strong>Agregar comentarios</strong> </p> </th> 
      <th> <p><strong>Editar sus propios comentarios si no hay respuestas</strong> </p> </th> 
      <th> <p><strong>Tomar una decisión</strong> </p> </th> 
      <th> <p><strong>Eliminar comentarios de otros</strong> </p> </th> 
      <th>Resolver comentarios</th> 
      <th>Aplicar acciones a comentarios</th> 
      <th> <p><strong>Editar la revisión</strong> </p> </th> 
      <th>Compartir la prueba con otros usuarios</th> 
      <th>Crear nueva versión</th> 
      <th> <p><strong>Ver solicitudes de aprobación en el área de inicio</strong> </p> </th> 
      <th>Añadir nuevos revisores</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>Sólo lectura</strong> </p> </td> 
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
      <td> <p>✓ <strong></strong> </p> </td> 
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

1. Los usuarios con nuevos planes de Workfront pueden otorgar funciones de autor o moderador a cualquier usuario del sistema. Los usuarios con planes heredados pueden conceder funciones de autor o moderador a cualquier usuario con una licencia de revisión en el sistema.
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
      <td>Workfront envía un correo electrónico al revisor cada vez que se produce alguna actividad en la prueba, como un nuevo comentario, una respuesta o una decisión. <p>Esta es una buena opción para la persona que administra el proceso de revisión porque le permite ver la actividad a medida que se produce. </p><p>Los usuarios no reciben una alerta por correo electrónico sobre su propia actividad.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Respuestas a mis comentarios</td> 
      <td>Se envía un correo electrónico al revisor únicamente si alguien responde explícitamente a su comentario (esto excluye sus propias respuestas a sus propios comentarios). Esto significa que si alguien en la prueba hace un nuevo comentario, no se notifica al revisor.<p>Se recomienda esta configuración para los clientes de la prueba, de modo que no se les notifique ningún otro comentario sobre la prueba y solo se les notifique de las respuestas a sus propios comentarios.</p><p>Aunque no se notifica a los revisores con esta configuración de alerta por correo electrónico de otros comentarios nuevos, pueden ver todos los comentarios de la prueba en el visor de revisión.</p><p>Para obtener información acerca de los comentarios, vea <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Ver y responder a los comentarios de revisión</a>.</p></td> 
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
      <td>Workfront envía un correo electrónico con todos los comentarios, respuestas y decisiones enumerados solo los días en que hay actividad aparte de la suya propia.<p>Esta alerta es una buena manera de ver un resumen del proyecto sin verse abrumado por múltiples actualizaciones a lo largo del día.</p><p>Un ejemplo de uso de este resumen es un jefe de departamento que desea supervisar el progreso general del proyecto.</p><p>Para obtener más información, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Administrar notificaciones para comentarios y decisiones sobre pruebas</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Sin correo electrónico</td> 
      <td>Workfront no envía alertas por correo electrónico.<br>Esto es útil para una persona que se agrega a una prueba solamente con fines de referencia y no necesita ser notificada de ningún cambio.<p>El valor predeterminado del sistema es Resumen diario (también se ve como No configurado). Si usted o los revisores no realizan ningún otro cambio, todas las pruebas tienen esta configuración.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continúe con [Configurar correo electrónico para la revisión](#configure-email-settings-for-the-proof) a continuación.

## Configuración de correo electrónico para la prueba {#configure-email-settings-for-the-proof}

1. En la sección **Notificación por correo electrónico**, seleccione si desea enviar notificaciones por correo electrónico y un mensaje personalizado a los usuarios seleccionados en [Crear una prueba avanzada con un flujo de trabajo básico](#workflow), anteriormente en este artículo:

   <table>
   <tbody>
   <tr>
   <td>Notificar a los destinatarios sobre esta revisión</td>
   <td>Seleccione esta opción para enviar una notificación por correo electrónico a los usuarios. Cuando se selecciona <strong>Uso compartido básico</strong> en la sección <strong>Flujo de trabajo</strong>, se envía una notificación por correo electrónico cuando se crea la prueba. Cuando se selecciona <strong>Flujo de trabajo automatizado</strong> en la sección <strong>Flujo de trabajo</strong>, se envía una notificación por correo electrónico cuando la prueba entra en la fase del flujo de trabajo automatizado con el que está asociado el usuario.</td>
   </tr>
   <tr>
   <td>Añadir mensaje personalizado</td>
   <td>Seleccione esta opción para incluir un mensaje personalizado en la notificación. Puede especificar el asunto y el cuerpo del mensaje. El cuerpo del mensaje puede incluir formato de texto enriquecido, como negrita, viñetas e hipervínculos.</td>
   </tr>
   </tbody>
   </table>


1. Continúe con [Configurar opciones de revisión](#configure-proof-settings) a continuación.

## Configurar ajustes de prueba {#configure-proof-settings}

1. En la sección **Configuración de prueba**, seleccione cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Requerir inicio de sesión: la prueba solo se puede compartir con otros usuarios</td> 
      <td>Cuando esta opción está deshabilitada (predeterminada), cualquier persona con la URL puede ver la revisión. <br>Cuando se selecciona esta opción:
       <ul>
        <li>Solo los usuarios de Workfront Proof pueden ver la revisión.</li>
        <li>Los usuarios no pueden iniciar sesión en la prueba a menos que se les haya agregado a la prueba.</li>
        <li>No se pueden activar las suscripciones.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Solo se requiere una decisión para esta prueba</td> 
      <td>Cuando se selecciona esta opción, la revisión se completa después de que uno de los responsables de la toma de decisiones tome su decisión.<br>Esta opción está deshabilitada de manera predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requerir que las decisiones se firmen electrónicamente</td> 
      <td>Los usuarios deben especificar su nombre de usuario y contraseña en el momento en que toman una decisión sobre una prueba.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear la revisión cuando se tomen todas las decisiones necesarias</td> 
      <td>Cuando esta configuración está habilitada, el estado de prueba se bloquea después de que se hayan tomado todas las decisiones. El estado cambia automáticamente de desbloqueado a bloqueado cuando el aprobador final toma su decisión.<br>Esta opción está deshabilitada de manera predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descargar archivo original</td> 
      <td>Cuando se selecciona esta opción, los revisores pueden descargar el archivo original desde el que se creó la prueba.<br>Cuando esta opción no está seleccionada, el icono Descargar ya no está visible.<br>Esta opción está habilitada de manera predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartir la revisión mediante una URL pública o código para insertar</td> 
      <td>Cuando se selecciona esta opción, la prueba se puede compartir mediante una URL pública o un código incrustado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suscribirse a la revisión mediante una URL pública o un código para insertar</td> 
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

1. Haga clic en **Crear revisión**.

   Workfront comienza a generar una prueba de los documentos o sitios web seleccionados. Según el tamaño y el tipo de archivo, el tiempo de posposición de la carga de un documento puede variar. Tenga paciencia, ya que los archivos más grandes tardan más en generarse. Puede salir de la página y Workfront seguirá generando el archivo. El tamaño máximo de carga de archivo es de 4 GB.

1. Una vez generada la revisión, haga clic en **Abrir revisión** para iniciar el visor de revisiones.

   ![](assets/open-proof-350x132.png)

   Los usuarios que no tengan la revisión habilitada en su cuenta aún pueden ver el documento y realizar comentarios en la revisión.