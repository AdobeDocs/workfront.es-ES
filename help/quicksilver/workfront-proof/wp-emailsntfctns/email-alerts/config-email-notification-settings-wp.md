---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Configure las opciones de notificación por correo electrónico en [!DNL Workfront Proof]
description: Las notificaciones por correo electrónico informan a los colaboradores sobre la actividad reciente de las pruebas, como comentarios, respuestas y decisiones.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '1998'
ht-degree: 0%

---

# Configure las opciones de notificación por correo electrónico en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Las notificaciones por correo electrónico informan a los colaboradores sobre la actividad reciente de las pruebas, como comentarios, respuestas y decisiones.

Las notificaciones por correo electrónico para los revisores se pueden configurar en la página New proof , [!UICONTROL Nueva versión] y se administran en la variable [!UICONTROL Flujo de trabajo] de la sección [!UICONTROL Detalles de la prueba] página. Para obtener más información, consulte [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

Todos los usuarios también pueden establecer su propia configuración de alerta de correo electrónico que se aplicará automáticamente cuando se comparta una prueba con ellos. Si los colaboradores tienen sus preferencias o si los administradores de la cuenta tienen sus recomendaciones sobre la frecuencia de las alertas. Esto se puede establecer como una prueba predeterminada en las páginas de detalles del usuario.

>[!NOTE]
>
>Estos ajustes se sugieren cuando los usuarios crean las pruebas y añaden estos colaboradores. Sin embargo, estas son sugerencias únicamente, por lo que se pueden ajustar en cualquier momento durante el proceso de revisión y los cambios se aplican a toda la actividad realizada después del cambio. La configuración predeterminada de la prueba se anula con la configuración en el nivel de prueba.

Usuarios con [!UICONTROL Administrador] o [!UICONTROL Administrador de facturación] Los perfiles también pueden establecer los valores predeterminados de prueba para otros usuarios de su cuenta desde la configuración de la cuenta.

Para obtener información sobre los perfiles, consulte [Perfiles de permisos de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [Configure los valores predeterminados de prueba en la configuración personal ([!DNL Workfront Proof] solo usuarios)](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [Cambiar alertas de correo electrónico para un destinatario](#change-email-alerts-for-a-recipient)
* [Configuración de los valores predeterminados de prueba para un usuario](#configure-proof-defaults-for-a-user)

## Configure los valores predeterminados de prueba en la configuración personal ([!DNL Workfront Proof] solo usuarios)

Puede configurar la configuración de la prueba para las pruebas que cree.

Para obtener información sobre la configuración de prueba, la variable [!DNL Workfront] administrador o [!DNL Workfront Proof] puede configurar, consulte .

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes personales]**.

1. Haga clic en el **[!UICONTROL Valores predeterminados de prueba]** pestaña .
1. Haga clic en **[!UICONTROL Configuración predeterminada de notificaciones por correo electrónico]** para expandirla.
1. En la lista desplegable situada a la derecha de las dos configuraciones siguientes, seleccione una de las opciones que se explican en la tabla siguiente.

   * **[!UICONTROL Alerta de correo electrónico predeterminada]**: Afecta a todas las pruebas que se comparten con usted. Esta configuración se puede sobrescribir en el nivel de prueba.
   * **[!UICONTROL Alerta de correo electrónico predeterminada para nuevos revisores invitados]**: Afecta a los revisores que no existían anteriormente como contactos en la cuenta.

   >[!NOTE]
   >
   >Si no elige una de las siguientes opciones, [!DNL Workfront Proof] le envía un resumen diario de la actividad en sus pruebas.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Toda actividad]</td> 
      <td>[!UICONTROL Workfront] envía un correo electrónico al revisor cada vez que hay actividad en la prueba, como un nuevo comentario, respuesta o decisión. <p>Esta es una buena opción para la persona que está administrando el proceso de prueba porque les permite ver la actividad a medida que pasa. </p><p>Los usuarios no reciben una alerta por correo electrónico sobre su propia actividad.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Respuestas a mis comentarios]</td> 
      <td>Solo se envía un correo electrónico al revisor si alguien responde explícitamente a su comentario (esto excluye sus propias respuestas en sus propios comentarios). Esto significa que si alguien de la prueba realiza un comentario nuevo, no se notifica al revisor.<p>Se recomienda este ajuste para los clientes en la prueba, de modo que no se les notifique de ningún otro comentario en la prueba y solo se les notifique de las respuestas a sus propios comentarios.</p><p>Aunque los revisores con esta configuración de alerta de correo electrónico no reciben notificaciones de otros comentarios nuevos, aún pueden ver todos los comentarios de la prueba en el visor de pruebas.</p><p>Para obtener información sobre los comentarios, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Ver y responder comentarios de prueba</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisiones]</td> 
      <td>[!DNL Workfront] envía un correo electrónico al revisor solo cuando alguien toma una decisión.<p>Esto puede resultar útil para la persona que administra el proceso de aprobación (como un administrador de proyectos) y necesita monitorizar el progreso de la prueba y ver qué usuarios han tomado su decisión.</p><p>No se le notificará su propia decisión a menos que seleccione una opción de confirmación por correo electrónico al presentar su decisión.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisión final]</td> 
      <td>[!DNL Workfront] envía un correo electrónico cuando el último aprobador de la prueba ha tomado una decisión.<p>Esta alerta la utiliza a menudo el diseñador, que no suele necesitar participar en la conversación de revisión real. Cuando se toma la decisión final, se notifica al diseñador y éste puede tomar las medidas necesarias.</p><p>Esta alerta también puede ser útil para un jefe de departamento al que solo se le debe notificar cuando haya terminado el proceso de revisión.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Resumen por hora]</td> 
      <td>[!DNL Workfront] envía un correo electrónico al revisor cada hora con un resumen de todos los comentarios, respuestas y decisiones que se hayan producido en la hora.<p>El correo electrónico solo se envía cuando la actividad que no sea la suya tiene lugar en la última hora. </p><p>Esta alerta es una buena forma de ver una descripción general del proyecto.</p><p>Un caso de uso de ejemplo para este resumen es un revisor principal que necesita una descripción general del proyecto, pero no es necesario que se le notifique inmediatamente de toda la actividad de la prueba.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Resumen diario]</td> 
      <td>[!DNL Workfront] envía un correo electrónico con todos los comentarios, respuestas y decisiones que aparecen solo en los días en que hay actividad además de la suya propia.<p>Esta alerta es una buena manera de ver un resumen del proyecto sin estar abrumado con múltiples actualizaciones a lo largo del día.</p><p>Un ejemplo de caso de uso para este resumen es un jefe de departamento que desea supervisar el progreso general del proyecto.</p><p>Para obtener más información, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Administrar notificaciones para comentarios y decisiones de prueba</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Sin correo electrónico]</td> 
      <td>[!DNL Workfront] no envía ninguna alerta por correo electrónico.<br>Esto es útil para una persona que se agrega a una prueba solo con fines de referencia y no necesita que se le notifique de ningún cambio.<p>El sistema predeterminado es [!UICONTROL Daily summary] (también se ve como [!UICONTROL Not Set]). Si usted o los revisores no realizan ningún otro cambio, todas las pruebas tendrán esta configuración.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cambie cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Confirmación de correo electrónico cuando las pruebas están listas]</td> 
      <td>Especifique si desea recibir un correo electrónico de [!UICONTROL Proof made] al crear una prueba. Para obtener más información, consulte <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">El correo electrónico de [!UICONTROL Proof Made]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Formato de correos electrónicos enviados a mí]</strong> </td> 
      <td> <p>Elija entre correos electrónicos con estilo de HTML y correos electrónicos de texto sin formato. </p> <p>Nota:  La configuración predeterminada de prueba se anula con la configuración en el nivel de prueba. Sin embargo, si las notificaciones de prueba de correo electrónico están deshabilitadas para toda la cuenta en la configuración de [!UICONTROL Account] , no se enviarán alertas de correo electrónico a los colaboradores aunque la [!UICONTROL Disabled email alert] no esté seleccionada en las pruebas.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. En **[!UICONTROL Configuración del mensaje]**, cambie cualquiera de las siguientes opciones:

   | **[!UICONTROL Plantilla del asunto de prueba]** | Se muestra en la página New proof , en la página New version , en la página Message y en la página Remind . Se puede editar antes de enviarlo. |
   |---|---|
   | **[!UICONTROL Plantilla de mensaje de prueba]** | Se muestra en la página New proof , en la página New version , en la página Message y en la página Remind . Se puede editar antes de enviarlo. |

   {style=&quot;table-layout:auto&quot;}

## Cambiar alertas de correo electrónico para un destinatario

Puede cambiar las alertas de correo electrónico para un destinatario determinado en una acción por lotes.

1. Haga clic en **[!UICONTROL Contactos]** en el panel de navegación izquierdo.
1. Haga clic en el **[!UICONTROL Más]** (tres puntos) para el destinatario y, a continuación, haga clic en **[!UICONTROL Ver detalles de miembros]** en el menú desplegable.

1. Abra el **[!UICONTROL Elementos compartidos]** para obtener más información.
1. Seleccione la casilla de verificación a la izquierda de cada elemento para el que desee cambiar la alerta de correo electrónico.
1. Haga clic en **[!UICONTROL Más]** encima de la lista de elementos compartidos, haga clic en **[!UICONTROL Cambiar alerta de correo electrónico]** en el menú desplegable.

1. Cambie la alerta de correo electrónico y haga clic en **[!UICONTROL Submit]**.

## Configuración de los valores predeterminados de prueba para un usuario

Si es [!DNL Workfront Proof] administrador, puede establecer valores predeterminados de prueba para los usuarios de su cuenta.

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la cuenta]**.

1. Abra el **[!UICONTROL Usuarios]** pestaña .
1. Abra el **[!UICONTROL Más]** a la derecha del nombre del usuario. ![More_button_small.png](assets/more-button-small.png)

1. Haga clic en **[!UICONTROL Ver detalles de usuarios]** en el menú desplegable.
1. En **[!UICONTROL Configuración]**, haga clic en **[!UICONTROL Configuración predeterminada de alertas de correo electrónico]** para expandirla.

1. En la lista desplegable a la derecha de las dos configuraciones siguientes, seleccione una de las opciones que se explican en la tabla siguiente:

   * **[!UICONTROL Alerta de correo electrónico predeterminada]**: Afecta a todas las pruebas que se comparten con usted. Esta configuración se puede sobrescribir en el nivel de prueba.
   * **[!UICONTROL Alerta de correo electrónico predeterminada para nuevos revisores invitados]**: Afecta a los revisores que no existían anteriormente como contactos en la cuenta.

   >[!NOTE]
   >
   >Si no elige una de las siguientes opciones para un usuario, [!DNL Workfront Proof] envía a los usuarios un resumen diario de la actividad en sus pruebas.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL Toda actividad]</td>
      <td>[!DNL Workfront] envía un correo electrónico al revisor cada vez que hay alguna actividad en la prueba, como un nuevo comentario, respuesta o decisión. <p>Esta es una buena opción para la persona que está administrando el proceso de prueba porque les permite ver la actividad a medida que pasa. </p><p>Los usuarios no reciben una alerta por correo electrónico sobre su propia actividad.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Respuestas a mis comentarios]</td>
      <td>Solo se envía un correo electrónico al revisor si alguien responde explícitamente a su comentario (esto excluye sus propias respuestas en sus propios comentarios). Esto significa que si alguien de la prueba realiza un comentario nuevo, no se notifica al revisor.<p>Se recomienda este ajuste para los clientes en la prueba, de modo que no se les notifique de ningún otro comentario en la prueba y solo se les notifique de las respuestas a sus propios comentarios.</p><p>Aunque los revisores con esta configuración de alerta de correo electrónico no reciben notificaciones de otros comentarios nuevos, aún pueden ver todos los comentarios de la prueba en el visor de pruebas.</p><p>Para obtener información sobre los comentarios, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Ver y responder comentarios de prueba</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisiones]</td>
      <td>[!DNL Workfront] envía un correo electrónico al revisor solo cuando alguien toma una decisión.<p>Esto puede resultar útil para la persona que administra el proceso de aprobación (como un administrador de proyectos) y necesita monitorizar el progreso de la prueba y ver qué usuarios han tomado su decisión.</p><p>No se le notificará su propia decisión a menos que seleccione una opción de confirmación por correo electrónico al presentar su decisión.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisión final]</td>
      <td>[!DNL Workfront] envía un correo electrónico cuando el último aprobador de la prueba ha tomado una decisión.<p>Esta alerta la utiliza a menudo el diseñador, que no suele necesitar participar en la conversación de revisión real. Cuando se toma la decisión final, se notifica al diseñador y éste puede tomar las medidas necesarias.</p><p>Esta alerta también puede ser útil para un jefe de departamento al que solo se le debe notificar cuando haya terminado el proceso de revisión.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Resumen por hora]</td>
      <td>[!DNL Workfront] envía un correo electrónico al revisor cada hora con un resumen de todos los comentarios, respuestas y decisiones que se hayan producido en la hora.<p>El correo electrónico solo se envía cuando la actividad que no sea la suya tiene lugar en la última hora. </p><p>Esta alerta es una buena forma de ver una descripción general del proyecto.</p><p>Un caso de uso de ejemplo para este resumen es un revisor principal que necesita una descripción general del proyecto, pero no es necesario que se le notifique inmediatamente de toda la actividad de la prueba.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Resumen diario]</td>
      <td>[!DNL Workfront] envía un correo electrónico con todos los comentarios, respuestas y decisiones que aparecen solo en los días en que hay actividad además de la suya propia.<p>Esta alerta es una buena manera de ver un resumen del proyecto sin estar abrumado con múltiples actualizaciones a lo largo del día.</p><p>Un ejemplo de caso de uso para este resumen es un jefe de departamento que desea supervisar el progreso general del proyecto.</p><p>Para obtener más información, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Administrar notificaciones para comentarios y decisiones de prueba</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL Sin correo electrónico]</td>
      <td>[!DNL Workfront] no envía ninguna alerta por correo electrónico.<br>Esto es útil para una persona que se agrega a una prueba solo con fines de referencia y no necesita que se le notifique de ningún cambio.<p>El sistema predeterminado es [!UICONTROL Daily summary] (también se ve como [!UICONTROL Not Set]). Si usted o los revisores no realizan ningún otro cambio, todas las pruebas tendrán esta configuración.</p></td>
     </tr>
    </tbody>
   </table>

1. En el resto **[!UICONTROL Configuración predeterminada de alertas de correo electrónico]**, cambie cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Confirmación de correo electrónico cuando las pruebas están listas]</td> 
      <td>Especifique si desea recibir un correo electrónico de [!UICONTROL Proof made] al crear una prueba. Para obtener más información, consulte <a href="https://support.workfront.com/hc/en-us/article">El Correo Electrónico De [!UICONTROL Proof Made].</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Formato de correos electrónicos enviados a mí]</strong> </td> 
      <td> <p>Elija entre correos electrónicos con estilo de HTML y correos electrónicos de texto sin formato. </p> <p>Nota:  La configuración predeterminada de prueba se anula con la configuración en el nivel de prueba. Sin embargo, si las notificaciones de prueba de correo electrónico están deshabilitadas para toda la cuenta en la configuración de [!UICONTROL Account] , no se enviarán alertas de correo electrónico a los colaboradores aunque la [!UICONTROL Disabled email alert] no esté seleccionada en las pruebas.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
