---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Administración de notificaciones para comentarios y decisiones de prueba
description: Al trabajar en una prueba, tanto si es un usuario de Adobe Workfront como si es un colaborador externo, puede especificar qué notificaciones de correo electrónico desea recibir sobre los comentarios y las decisiones tomadas al respecto. Para obtener más información, consulte Notificaciones para comentarios de prueba e información general sobre decisiones.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '978'
ht-degree: 1%

---

# Administración de notificaciones para comentarios y decisiones de prueba

Al trabajar en una prueba, tanto si es un usuario de Adobe Workfront como si es un colaborador externo, puede especificar qué notificaciones de correo electrónico desea recibir sobre los comentarios y las decisiones tomadas al respecto. Para obtener más información, consulte [Notificaciones para comentarios de prueba y descripción general de decisiones](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Estas notificaciones son diferentes a las alertas por correo electrónico que puede recibir sobre el flujo de una prueba entre los revisores. También son diferentes de las opciones de configuración de alertas de correo electrónico que se pueden configurar en Workfront. 

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
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

## Administración de notificaciones para comentarios y decisiones de prueba

1. Abra la prueba para la que desea configurar las notificaciones que recibirá.
1. Si no aparece la barra de herramientas izquierda, haga clic en el icono **Menú**, que se encuentra en la esquina superior izquierda del Visor de revisión web.

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. En la barra de herramientas izquierda, haga clic en el icono **Configuración**. ![icono_configuración.png](assets/settings-icon.png)

1. En **Enviarme notificaciones por correo electrónico sobre**, haga clic en la configuración que desee para la revisión.

   La configuración que seleccione permanecerá vigente únicamente para la prueba que haya abierto.

   El valor predeterminado del sistema es **Resumen diario**. Si usted o los revisores no realizan ningún otro cambio, todas las pruebas tienen esta configuración.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toda la actividad</td> 
      <td>Se envía un correo electrónico al revisor cada vez que se produce alguna actividad en la prueba, como un nuevo comentario, una respuesta o una decisión.<br><p>Esta es una buena opción para la persona que administra el proceso de revisión porque le permite ver la actividad a medida que se produce. Los usuarios no reciben una alerta por correo electrónico sobre su propia actividad (por ejemplo, comentarios, respuestas y decisiones tomadas).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Respuestas a mis comentarios</td> 
      <td>Se envía un correo electrónico al revisor únicamente si alguien responde explícitamente a su comentario (esto excluye sus propias respuestas a sus propios comentarios). Esto significa que si alguien en la prueba hace un nuevo comentario, no se notifica al revisor.<p>Se recomienda esta configuración para los clientes de la prueba, de modo que no se les notifique ningún otro comentario sobre la prueba y solo se les notifique de las respuestas a sus propios comentarios.</p><p>Aunque no se notifica a los revisores con esta configuración de alerta por correo electrónico de otros comentarios nuevos, pueden ver todos los comentarios de la prueba en el visor de revisión.<br></p><p>Para obtener información, vea <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Ver y responder a los comentarios de revisión</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisiones</td> 
      <td>Solo se envía un correo electrónico al revisor cuando alguien toma una decisión.<br><p>Esta alerta de correo electrónico puede ser útil para la persona que administra el proceso de aprobación (como un administrador de proyectos), ya que permite a la persona que administra el proceso de aprobación monitorizar el progreso de la prueba y ver qué usuarios han tomado su decisión.<br></p><p>No se le notificará su propia decisión a menos que seleccione una opción de confirmación por correo electrónico al enviar su decisión.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisión final</td> 
      <td>Se envía un correo electrónico cuando se toma la decisión final sobre la prueba (cuando el último aprobador de la prueba ha tomado su decisión).<br><p>El diseñador suele utilizar esta alerta porque no es necesario que participe en la discusión de revisión real. Cuando se toma la decisión final, se notifica al diseñador y luego se puede tomar medidas sobre los cambios necesarios.<br></p><p>Esta alerta también puede ser útil para un jefe de departamento al que sólo se debe notificar cuando haya finalizado el proceso de revisión.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resumen horario</td> 
      <td>Se envía un correo electrónico al revisor cada hora con un resumen de todos los comentarios, respuestas y decisiones que se han producido en la última hora.<br><p>El correo electrónico se envía únicamente cuando se produce una actividad distinta de la suya en las últimas horas. Si no hay actividad de otros usuarios, no se envía ningún correo electrónico.<br></p><p>Esta alerta es una buena manera de ver una descripción general del proyecto.<br></p><p>Un ejemplo de uso de este resumen es un revisor sénior que necesita una visión general del proyecto, pero no necesita que se le notifique inmediatamente de toda la actividad de la prueba.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resumen diario</td> 
      <td>(Configuración predeterminada): Se envía un correo electrónico todos los días con todos los comentarios, respuestas y decisiones enumerados. Un correo electrónico se envía solo los días en que hay actividad aparte de la suya propia.<br><p>Esta alerta es una buena manera de ver un resumen del proyecto sin verse abrumado por múltiples actualizaciones a lo largo del día.<br></p><p>Un ejemplo de uso de este resumen es un jefe de departamento que desea supervisar el progreso general del proyecto.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sin correo electrónico</td> 
      <td>No se envían alertas por correo electrónico.<br><p>Esta configuración es útil para una persona que se agrega a una prueba solo con fines de referencia y no necesita recibir notificaciones de ningún cambio.</p><p>Nota: <p>Esta opción desactiva únicamente las alertas de correo electrónico que puede recibir acerca de los comentarios y decisiones sobre las pruebas. No desactiva las alertas de correo electrónico que puede recibir sobre el flujo de una prueba, como el correo electrónico Nueva prueba o Prueba tardía. Para obtener más información sobre las alertas de correo electrónico relacionadas con el flujo de una prueba, consulte los siguientes artículos: </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">Nuevo correo electrónico de prueba</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">Correo electrónico sobre la nueva versión</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">Correo electrónico de prueba tardía</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">Correo electrónico de la prueba realizada</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
