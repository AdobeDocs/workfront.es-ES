---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Configurar las notificaciones por correo electrónico en  [!DNL Workfront Proof]
description: Las notificaciones por correo electrónico generadas desde Workfront Proof informan a los colaboradores sobre la actividad reciente en las pruebas, como comentarios, respuestas o decisiones.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '2049'
ht-degree: 0%

---

# Configurar las notificaciones por correo electrónico en [!DNL Workfront Proof]

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Las notificaciones por correo electrónico informan a los colaboradores sobre la actividad reciente en las pruebas, como comentarios, respuestas o decisiones.

Puede establecer notificaciones por correo electrónico para los revisores en las siguientes áreas:

Las notificaciones por correo electrónico para los revisores se pueden establecer en la página Nueva prueba, [!UICONTROL Nueva versión] y administrar en la sección [!UICONTROL Flujo de trabajo] de la página [!UICONTROL Detalles de la prueba]. Para obtener más información, consulte [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* La página Nueva prueba
* La página [!UICONTROL Nueva versión]
* La sección [!UICONTROL Flujo de trabajo] de la página [!UICONTROL Detalles de la prueba].

Para obtener más información, consulte [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)


* [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Administrar detalles de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).


Cada usuario también puede definir su propia configuración de alertas por correo electrónico que se aplica automáticamente cuando se comparte una prueba con él si los colaboradores tienen sus preferencias o si los administradores de cuenta tienen su recomendación sobre la frecuencia de las alertas. Esto puede establecerse como prueba predeterminada en las páginas de detalles de los usuarios.

Cada usuario también puede establecer su propia configuración de alertas por correo electrónico que se aplicará automáticamente cuando se comparta una prueba con él. <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>Estos ajustes se sugieren cuando los usuarios crean las pruebas y agregan estos colaboradores. Sin embargo, solo son sugerencias, por lo que se pueden ajustar en cualquier momento durante el proceso de revisión y los cambios se aplican a toda la actividad realizada después del cambio. La configuración predeterminada de la prueba se anula en el nivel de prueba.

Los usuarios con perfiles de [!UICONTROL Administrador] o [!UICONTROL Administrador de facturación] también pueden establecer los valores predeterminados de prueba para otros usuarios de su cuenta desde Configuración de la cuenta.

Para obtener información acerca de los perfiles, vea [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
<tr> 
   <td role="rowheader">Product</td> 
   <td>Workfront Proof independiente</td> 
  </tr> 
</table>

+++

## Configurar valores predeterminados de revisión en la configuración personal ([!DNL Workfront Proof] usuarios solamente)

Puede configurar los ajustes de prueba para las pruebas que cree.

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración personal]**.

1. Haga clic en la ficha **[!UICONTROL Valores predeterminados de revisión]**.
1. Haga clic en **[!UICONTROL Configuración predeterminada de notificaciones por correo electrónico]** para expandirla.
1. En la lista desplegable a la derecha de las dos configuraciones siguientes, seleccione una de las opciones explicadas en la tabla siguiente.

   * **[!UICONTROL Alerta de correo electrónico predeterminada]**: Afecta a todas las revisiones compartidas con usted. Esta configuración se puede sobrescribir en el nivel de prueba.
   * **[!UICONTROL Alerta de correo electrónico predeterminada para nuevos revisores invitados]**: afecta a los revisores que no existían anteriormente como contactos de su cuenta.

   >[!NOTE]
   >
   >Si no elige una de las siguientes opciones, [!DNL Workfront Proof] le envía un resumen diario sobre la actividad de las pruebas.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Toda la actividad]</td> 
      <td>[!UICONTROL Workfront] envía un mensaje de correo electrónico al revisor cada vez que hay alguna actividad en la revisión, como un nuevo comentario, una respuesta o una decisión. <p>Esta es una buena opción para la persona que administra el proceso de revisión porque le permite ver la actividad a medida que se produce. </p><p>Los usuarios no reciben una alerta por correo electrónico sobre su propia actividad.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Respuestas a mis comentarios]</td> 
      <td>Se envía un correo electrónico al revisor únicamente si alguien responde explícitamente a su comentario (esto excluye sus propias respuestas a sus propios comentarios). Esto significa que si alguien en la prueba hace un nuevo comentario, no se notifica al revisor.<p>Se recomienda esta configuración para los clientes de la prueba, de modo que no se les notifique ningún otro comentario sobre la prueba y solo se les notifique de las respuestas a sus propios comentarios.</p><p>Aunque no se notifica a los revisores con esta configuración de alerta por correo electrónico de otros comentarios nuevos, pueden ver todos los comentarios de la prueba en el visor de revisión.</p><p>Para obtener información acerca de los comentarios, vea <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Ver y responder a los comentarios de revisión</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisiones]</td> 
      <td>[!DNL Workfront] envía un correo electrónico al revisor únicamente cuando alguien toma una decisión.<p>Esto puede resultar útil para la persona que administra el proceso de aprobación (como un administrador de proyectos) y necesita supervisar el progreso de la prueba y ver qué usuarios han tomado su decisión.</p><p>No se le notificará su propia decisión a menos que seleccione una opción de confirmación por correo electrónico al enviar su decisión.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisión final]</td> 
      <td>[!DNL Workfront] envía un correo electrónico cuando el último aprobador de la prueba ha tomado una decisión.<p>Esta alerta la suele utilizar el diseñador, que no suele tener que participar en la discusión de revisión real. Cuando se toma la decisión final, se notifica al diseñador y luego se puede tomar medidas sobre los cambios necesarios.</p><p>Esta alerta también puede ser útil para un jefe de departamento al que sólo se debe notificar cuando haya finalizado el proceso de revisión.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Resumen por hora]</td> 
      <td>[!DNL Workfront] envía un correo electrónico al revisor cada hora con un resumen de todos los comentarios, respuestas y decisiones que se han producido en la hora.<p>El correo electrónico se envía únicamente cuando se produce una actividad distinta de la suya en las últimas horas. </p><p>Esta alerta es una buena manera de ver una descripción general del proyecto.</p><p>Un ejemplo de uso de este resumen es un revisor sénior que necesita una visión general del proyecto, pero no necesita que se le notifique inmediatamente de toda la actividad de la prueba.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Resumen diario]</td> 
      <td>[!DNL Workfront] envía un correo electrónico con todos los comentarios, respuestas y decisiones enumerados solo los días en que hay actividad aparte de la suya propia.<p>Esta alerta es una buena manera de ver un resumen del proyecto sin verse abrumado por múltiples actualizaciones a lo largo del día.</p><p>Un ejemplo de uso de este resumen es un jefe de departamento que desea supervisar el progreso general del proyecto.</p><p>Para obtener más información, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Administrar notificaciones para comentarios y decisiones sobre pruebas</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Sin correo electrónico]</td> 
      <td>[!DNL Workfront] no envía ninguna alerta por correo electrónico.<br>Esto es útil para una persona que se agrega a una prueba solamente con fines de referencia y no necesita ser notificada de ningún cambio.<p>El valor predeterminado del sistema es [!UICONTROL Daily summary] (también se ve como [!UICONTROL Not Set]). Si usted o los revisores no realizan ningún otro cambio, todas las pruebas tienen esta configuración.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cambie cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Confirmación por correo electrónico cuando las pruebas estén listas]</td> 
      <td>Especifique si desea recibir un correo electrónico de [!UICONTROL Proof made] al crear una prueba. Para obtener más información, vea <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">El correo electrónico de [!UICONTROL Proof Made]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Formato de correos electrónicos enviados a mí] </td> 
      <td> <p>Elija entre correos electrónicos con estilo HTML y de texto sin formato. </p> <p><b>NOTA</b></p>
      <p>La configuración predeterminada de revisión se anula en el nivel de prueba. Sin embargo, si las notificaciones de prueba por correo electrónico están desactivadas para toda la cuenta en la configuración de [!UICONTROL Account], no se enviarán alertas por correo electrónico a los colaboradores aunque la [!UICONTROL Deshabilitado alerta por correo electrónico] no esté seleccionada en las pruebas.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. En **[!UICONTROL Configuración del mensaje]**, cambie cualquiera de las siguientes opciones:

   | Plantilla de prueba | Descripción |
   |---|---|
   | **[!UICONTROL Plantilla de asunto de revisión]** | Se muestra en las páginas Nueva prueba, Nueva versión, Mensaje y Recordatorio. Se puede editar antes de enviarlo. |
   | **[!UICONTROL Plantilla de mensaje de revisión]** | Se muestra en las páginas Nueva prueba, Nueva versión, Mensaje y Recordatorio. Se puede editar antes de enviarlo. |

## Cambiar las alertas de correo electrónico de un destinatario

Puede cambiar las alertas de correo electrónico de un destinatario determinado en una acción por lotes.

1. Haga clic en **[!UICONTROL Contactos]** en el panel de navegación izquierdo.
1. Haga clic en el menú **[!UICONTROL Más]** ![](assets/more-button-small.png) del destinatario y, a continuación, haga clic en **[!UICONTROL Ver detalles del miembro]** en el menú desplegable.

1. Abra la sección **[!UICONTROL Elementos compartidos]**.
1. Seleccione la casilla a la izquierda de cada elemento para el que desee cambiar la alerta de correo electrónico.
1. Haga clic en **[!UICONTROL Más]** sobre la lista de elementos compartidos y luego haga clic en **[!UICONTROL Cambiar alerta de correo electrónico]** en el menú desplegable.

1. Cambie la alerta por correo electrónico y haga clic en **[!UICONTROL Enviar]**.

## Configurar valores predeterminados de prueba para un usuario

Si es administrador de [!DNL Workfront Proof], puede establecer valores predeterminados de revisión para los usuarios de su cuenta.

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la cuenta]**.

1. Abra la ficha **[!UICONTROL Usuarios]**.
1. Abra el menú **[!UICONTROL Más]** ![More_button_small.png](assets/more-button-small.png) a la derecha del nombre del usuario.

1. Haga clic en **[!UICONTROL Ver detalles de los usuarios]** en el menú desplegable.
1. En **[!UICONTROL Configuración]**, haga clic en **[!UICONTROL Configuración predeterminada de alertas de correo electrónico]** para expandirla.

1. En la lista desplegable a la derecha de las dos configuraciones siguientes, seleccione una de las opciones explicadas en la tabla siguiente:

   * **[!UICONTROL Alerta de correo electrónico predeterminada]**: Afecta a todas las revisiones compartidas con usted. Esta configuración se puede sobrescribir en el nivel de prueba.
   * **[!UICONTROL Alerta de correo electrónico predeterminada para nuevos revisores invitados]**: afecta a los revisores que no existían anteriormente como contactos de su cuenta.

   >[!NOTE]
   >
   >Si no elige una de las siguientes opciones para un usuario, [!DNL Workfront Proof] envía a los usuarios un resumen diario de la actividad en sus pruebas.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL Toda la actividad]</td>
      <td>[!DNL Workfront] envía un correo electrónico al revisor cada vez que se produce alguna actividad en la prueba, como un nuevo comentario, una respuesta o una decisión. <p>Esta es una buena opción para la persona que administra el proceso de revisión porque le permite ver la actividad a medida que se produce. </p><p>Los usuarios no reciben una alerta por correo electrónico sobre su propia actividad.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Respuestas a mis comentarios]</td>
      <td>Se envía un correo electrónico al revisor únicamente si alguien responde explícitamente a su comentario (esto excluye sus propias respuestas a sus propios comentarios). Esto significa que si alguien en la prueba hace un nuevo comentario, no se notifica al revisor.<p>Se recomienda esta configuración para los clientes de la prueba, de modo que no se les notifique ningún otro comentario sobre la prueba y solo se les notifique de las respuestas a sus propios comentarios.</p><p>Aunque no se notifica a los revisores con esta configuración de alerta por correo electrónico de otros comentarios nuevos, pueden ver todos los comentarios de la prueba en el visor de revisión.</p><p>Para obtener información acerca de los comentarios, vea <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Ver y responder a los comentarios de revisión</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisiones]</td>
      <td>[!DNL Workfront] envía un correo electrónico al revisor únicamente cuando alguien toma una decisión.<p>Esto puede resultar útil para la persona que administra el proceso de aprobación (como un administrador de proyectos) y necesita supervisar el progreso de la prueba y ver qué usuarios han tomado su decisión.</p><p>No se le notificará su propia decisión a menos que seleccione una opción de confirmación por correo electrónico al enviar su decisión.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisión final]</td>
      <td>[!DNL Workfront] envía un correo electrónico cuando el último aprobador de la prueba ha tomado una decisión.<p>Esta alerta la suele utilizar el diseñador, que no suele tener que participar en la discusión de revisión real. Cuando se toma la decisión final, se notifica al diseñador y luego se puede tomar medidas sobre los cambios necesarios.</p><p>Esta alerta también puede ser útil para un jefe de departamento al que sólo se debe notificar cuando haya finalizado el proceso de revisión.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Resumen por hora]</td>
      <td>[!DNL Workfront] envía un correo electrónico al revisor cada hora con un resumen de todos los comentarios, respuestas y decisiones que se han producido en la hora.<p>El correo electrónico se envía únicamente cuando se produce una actividad distinta de la suya en las últimas horas. </p><p>Esta alerta es una buena manera de ver una descripción general del proyecto.</p><p>Un ejemplo de uso de este resumen es un revisor sénior que necesita una visión general del proyecto, pero no necesita que se le notifique inmediatamente de toda la actividad de la prueba.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Resumen diario]</td>
      <td>[!DNL Workfront] envía un correo electrónico con todos los comentarios, respuestas y decisiones enumerados solo los días en que hay actividad aparte de la suya propia.<p>Esta alerta es una buena manera de ver un resumen del proyecto sin verse abrumado por múltiples actualizaciones a lo largo del día.</p><p>Un ejemplo de uso de este resumen es un jefe de departamento que desea supervisar el progreso general del proyecto.</p><p>Para obtener más información, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Administrar notificaciones para comentarios y decisiones sobre pruebas</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL Sin correo electrónico]</td>
      <td>[!DNL Workfront] no envía ninguna alerta por correo electrónico.<br>Esto es útil para una persona que se agrega a una prueba solamente con fines de referencia y no necesita ser notificada de ningún cambio.<p>El valor predeterminado del sistema es [!UICONTROL Daily summary] (también se ve como [!UICONTROL Not Set]). Si usted o los revisores no realizan ningún otro cambio, todas las pruebas tienen esta configuración.</p></td>
     </tr>
    </tbody>
   </table>

1. En los restantes **[!UICONTROL valores predeterminados de alertas de correo electrónico]**, cambie cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Confirmación por correo electrónico cuando las pruebas estén listas]</td> 
      <td>Especifique si desea recibir un correo electrónico de [!UICONTROL Proof made] al crear una prueba. Para obtener más información, vea <a href="https://support.workfront.com/hc/en-us/article">El correo electrónico de [!UICONTROL Proof Made].</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Formato de correos electrónicos enviados a mí] </td> 
      <td> <p>Elija entre correos electrónicos con estilo HTML y de texto sin formato. </p> <p><b>NOTA</b></p> <p>La configuración predeterminada de revisión se anula en el nivel de prueba. Sin embargo, si las notificaciones de prueba por correo electrónico están desactivadas para toda la cuenta en la configuración de [!UICONTROL Account], no se enviarán alertas por correo electrónico a los colaboradores aunque la [!UICONTROL Deshabilitado alerta por correo electrónico] no esté seleccionada en las pruebas.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
