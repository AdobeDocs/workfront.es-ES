---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Administración de notificaciones para comentarios y decisiones sobre pruebas
description: Al trabajar en una prueba, tanto si es un usuario de Adobe Workfront como si es un colaborador externo, puede especificar qué notificaciones de correo electrónico desea recibir sobre los comentarios y las decisiones tomadas al respecto. Para obtener más información, consulte la información general sobre notificaciones para comentarios y decisiones sobre pruebas.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: b3fe63f7a332f50c7bac3bedee5db3bbbabd2b42
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 28%

---

# Administración de notificaciones para comentarios y decisiones sobre pruebas

Al trabajar en una prueba, tanto si es un usuario de Adobe Workfront como si es un colaborador externo, puede especificar qué notificaciones de correo electrónico desea recibir sobre los comentarios y las decisiones tomadas al respecto. Para obtener más información, consulte [Información general sobre notificaciones para comentarios y decisiones sobre pruebas.](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Estas notificaciones son diferentes a las alertas por correo electrónico que puede recibir sobre el flujo de una prueba entre los revisores, así como a la configuración de las alertas por correo electrónico que puede configurar en Workfront.

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
   <td> <p>Acceso de edición a documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Administración de notificaciones para comentarios y decisiones sobre pruebas

1. Abra la prueba para la que desee configurar las notificaciones.
1. Si no se muestra la barra de herramientas izquierda, haga clic en el icono **Menú** en la esquina superior izquierda del Visor de revisión web.

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. En la barra de herramientas izquierda, haga clic en el icono **Configuración** ![Icono_Configuración.png](assets/settings-icon.png) .

1. En la sección **Enviarme notificaciones por correo electrónico sobre**, seleccione la configuración de notificación para esta revisión.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toda la actividad</td> 
      <td>Se envía un correo electrónico al revisor cada vez que se produce alguna actividad en la prueba, como un nuevo comentario, una respuesta o una decisión.<br><p>Esta configuración se recomienda para la persona que administra el proceso de revisión, ya que le permite ver la actividad a medida que se produce. Los usuarios no reciben una alerta por correo electrónico sobre su propia actividad (por ejemplo, comentarios, respuestas o decisiones tomadas).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Respuestas a mis comentarios</td> 
      <td>Se envía un correo electrónico al revisor únicamente si alguien responde directamente a su comentario (excluyendo las respuestas de otros usuarios sobre sus propios comentarios).<p>Se recomienda esta configuración para los clientes, de modo que solo se les notifiquen las respuestas a sus propios comentarios y no los demás comentarios realizados en la prueba, aunque aún pueden ver todos los comentarios en el visor de pruebas.</p>
      <p>Para obtener más información, vea <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Ver y responder a los comentarios de revisión</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisiones</td> 
      <td>Solo se envía un correo electrónico al revisor cuando alguien toma una decisión.<br><p>Esta alerta de correo electrónico puede ser útil para la persona que administra el proceso de aprobación porque permite a la persona que administra el proceso de aprobación monitorizar el progreso de la prueba y ver qué usuarios han tomado su decisión.<br></p><p>No se le notificará su propia decisión a menos que seleccione una opción de confirmación por correo electrónico al enviar su decisión.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisión final</td> 
      <td>Se envía un correo electrónico cuando se toma la decisión final sobre la prueba.<br><p>El diseñador suele utilizar esta alerta porque no es necesario que participe en la discusión de revisión real. Cuando se toma la decisión final, se notifica al diseñador y luego se puede tomar medidas sobre los cambios necesarios.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resumen por horas</td> 
      <td>Se envía un correo electrónico al revisor cada hora con un resumen de todos los comentarios, respuestas y decisiones que se han producido en la última hora.<br><p>El correo electrónico se envía únicamente cuando se produce una actividad distinta de la suya en las últimas horas. Si no hay actividad de otros usuarios, no se envía ningún correo electrónico.<br></p><p>Esta alerta es una buena manera de ver una descripción general del proyecto a medida que avanza.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resumen diario</td> 
      <td>(Configuración predeterminada): Se envía un correo electrónico todos los días con todos los comentarios, respuestas y decisiones enumerados. Se envía solo los días en los que hay actividad aparte de la suya propia.<br><p>Esta alerta es una buena manera de ver un resumen del proyecto sin verse abrumado por múltiples actualizaciones a lo largo del día.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">No hay correo electrónico</td> 
      <td>No se envían alertas por correo electrónico.<br><p>Esta configuración es útil para una persona que se agrega a una prueba solo con fines de referencia y no necesita recibir notificaciones de ningún cambio.</p><p>Nota: <p>Esta opción solo desactiva las alertas de correo electrónico sobre comentarios y decisiones sobre pruebas; no desactiva las alertas de correo electrónico que puede recibir sobre el flujo de una prueba, como el correo electrónico Nueva prueba o Prueba tardía. Para obtener más información, consulte los siguientes artículos: </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">Correo electrónico de nueva prueba</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">Correo electrónico de Nueva versión</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">Correo electrónico de prueba atrasada</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">Correo electrónico de la prueba realizada</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
