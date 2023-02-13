---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Administrar notificaciones para comentarios y decisiones de prueba
description: Cuando trabaje en una prueba, ya sea usuario de Adobe Workfront o colaborador externo, puede especificar qué notificaciones por correo electrónico desea recibir sobre los comentarios y las decisiones que se han tomado en la prueba. Para obtener más información, consulte Información general sobre notificaciones para comentarios de prueba y decisiones.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '983'
ht-degree: 0%

---

# Administrar notificaciones para comentarios y decisiones de prueba

Cuando trabaje en una prueba, ya sea usuario de Adobe Workfront o colaborador externo, puede especificar qué notificaciones por correo electrónico desea recibir sobre los comentarios y las decisiones que se han tomado en la prueba. Para obtener más información, consulte [Resumen de notificaciones para comentarios y decisiones de prueba](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Estas notificaciones son diferentes de las alertas de correo electrónico que puede recibir sobre el flujo de una prueba entre los revisores. También son diferentes de las opciones de alerta de correo electrónico que se pueden configurar en Workfront. 

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
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con el administrador de Workfront o Workfront Proof.

## Administrar notificaciones para comentarios y decisiones de prueba

1. Abra la prueba para la que desee configurar las notificaciones que recibirá.
1. Si no se muestra la barra de herramientas izquierda, haga clic en el botón **Menú** , situado en la esquina superior izquierda del visor de pruebas web.

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. En la barra de herramientas de la izquierda, haga clic en el botón **Configuración** icono. ![Settings_icon.png](assets/settings-icon.png)

1. En **Enviarme notificaciones por correo electrónico acerca de**, haga clic en la configuración que desee para la prueba.

   La configuración que seleccione solo se mantiene en vigor para la prueba que haya abierto.

   El valor predeterminado del sistema es **Resumen diario**. Si usted o los revisores no realizan ningún otro cambio, todas las pruebas tendrán esta configuración.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Todas las actividades</td> 
      <td>Se envía un correo electrónico al revisor cada vez que hay alguna actividad en la prueba, como un nuevo comentario, respuesta o decisión.<br><p>Esta es una buena opción para la persona que está administrando el proceso de prueba porque les permite ver la actividad a medida que pasa. Los usuarios no reciben una alerta por correo electrónico sobre su propia actividad (por ejemplo, comentarios, respuestas y decisiones tomadas).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Respuestas a mis comentarios</td> 
      <td>Solo se envía un correo electrónico al revisor si alguien responde explícitamente a su comentario (esto excluye sus propias respuestas en sus propios comentarios). Esto significa que si alguien de la prueba realiza un comentario nuevo, no se notifica al revisor.<p>Se recomienda este ajuste para los clientes en la prueba, de modo que no se les notifique de ningún otro comentario en la prueba y solo se les notifique de las respuestas a sus propios comentarios.</p><p>Aunque los revisores con esta configuración de alerta de correo electrónico no reciben notificaciones de otros comentarios nuevos, aún pueden ver todos los comentarios de la prueba en el visor de pruebas.<br></p><p>Para obtener información, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Ver y responder comentarios de prueba</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisiones</td> 
      <td>Un correo electrónico se envía al revisor solo cuando alguien toma una decisión.<br><p>Esta alerta por correo electrónico puede resultar útil para la persona que administra el proceso de aprobación (como un administrador de proyectos) porque permite a la persona que administra el proceso de aprobación controlar el progreso de la prueba y ver qué usuarios han tomado una decisión.<br></p><p>No se le notificará su propia decisión a menos que seleccione una opción de confirmación por correo electrónico al presentar su decisión.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisión final</td> 
      <td>Se envía un correo electrónico cuando se toma la decisión final sobre la prueba (cuando el último aprobador de la prueba ha tomado su decisión).<br><p>Esta alerta suele ser utilizada por el diseñador porque este no necesita participar en la conversación de revisión real. Cuando se toma la decisión final, se notifica al diseñador y éste puede tomar las medidas necesarias.<br></p><p>Esta alerta también puede ser útil para un jefe de departamento al que solo se le debe notificar cuando haya terminado el proceso de revisión.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resumen por hora</td> 
      <td>Cada hora se envía un correo electrónico al revisor con un resumen de todos los comentarios, respuestas y decisiones que se hayan producido en la última hora.<br><p>El correo electrónico solo se envía cuando la actividad que no sea la suya tiene lugar en la última hora. Si no hay actividad de otros usuarios, no se envía ningún correo electrónico.<br></p><p>Esta alerta es una buena forma de ver una descripción general del proyecto.<br></p><p>Un caso de uso de ejemplo para este resumen es un revisor principal que necesita una descripción general del proyecto, pero no es necesario que se le notifique inmediatamente de toda la actividad de la prueba.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resumen diario</td> 
      <td>(Configuración predeterminada): Se envía un correo electrónico todos los días con todos los comentarios, respuestas y decisiones enumerados. Un correo electrónico se envía solo en los días en que hay actividad además de la suya propia.<br><p>Esta alerta es una buena manera de ver un resumen del proyecto sin estar abrumado con múltiples actualizaciones a lo largo del día.<br></p><p>Un ejemplo de caso de uso para este resumen es un jefe de departamento que desea supervisar el progreso general del proyecto.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sin correo electrónico</td> 
      <td>No se envían alertas por correo electrónico.<br><p>Esta configuración es útil para una persona que se agrega a una prueba solo con fines de referencia y no necesita que se le notifique de ningún cambio.</p><p>Nota: <p>Esta opción desactiva solo las alertas de correo electrónico que puede recibir sobre comentarios y decisiones de prueba. No desactiva las alertas de correo electrónico que puede recibir sobre el flujo de una prueba, como el correo electrónico de prueba nueva o prueba tardía. Para obtener más información sobre las alertas de correo electrónico relativas al flujo de una prueba, consulte los siguientes artículos: </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">Nuevo correo electrónico de prueba</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">El correo electrónico de la nueva versión</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">Correo electrónico de prueba atrasada</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">El correo electrónico de prueba realizada</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
