---
product-area: setup
navigation-topic: notifications
keywords: modificar,correo electrónico,notificación,configuración
title: Modificar sus propias notificaciones por correo electrónico
description: Este artículo describe cómo administrar las notificaciones por correo electrónico en el perfil de usuario.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# Modificar sus propias notificaciones por correo electrónico

<!-- Audited: 1/2024 -->

Su Adobe [!DNL Workfront] El administrador configura las notificaciones por correo electrónico que reciben los usuarios cuando se producen eventos en Workfront (como se describe en ). [[!UICONTROL Configurar evento] notificaciones para todos los usuarios del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

El administrador del grupo también puede configurar qué notificaciones están activadas para usted y los usuarios de su [!UICONTROL Grupo de inicio]. Si su [!UICONTROL Grupo de inicio] es un subgrupo y recibe las notificaciones activadas para el grupo de nivel superior sobre el grupo.

Puede personalizarlo aún más configurando las notificaciones que recibe. También puede elegir si desea recibir notificaciones cuando se produzcan eventos o en un correo electrónico de resumen diario.

Para obtener más información sobre las notificaciones por correo electrónico, consulte [[!DNL Adobe Workfront] notificaciones](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* Si activa un tipo de notificación y, a continuación, observa que no recibe notificaciones de ese tipo, puede deberse a que ese tipo no se aplica a su función.
>* El [!DNL Workfront] Un administrador de o un administrador de grupo no puede configurar notificaciones para [!DNL Workfront Goals]. Para obtener más información sobre las notificaciones, consulte [!DNL Workfront] El administrador puede configurar, consulte [Configurar notificaciones de eventos para todos los usuarios del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Para obtener información sobre cómo configurar notificaciones individuales para [!DNL Workfront Goals] siga leyendo este artículo.
>

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia</strong></td> 
   <td>  <p>Nuevo:</p> 
   <ul><li>Colaborador o superior</li></ul>
   <p>Actual:</p>
   <ul><li>Solicitud o superior</li></ul>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Ver y modificar la configuración de las notificaciones por correo electrónico

{{step1-click-profile-pic}}

1. Haga clic en **[!UICONTROL Más]** icono ![](assets/more-icon.png) junto a su nombre y haga clic en **[!UICONTROL Editar]**.

1. En el **[!UICONTROL Editar persona]** que se muestra, vaya al **[!UICONTROL Notificaciones]** sección.

1. Haga clic en una categoría para ver la configuración de notificaciones relacionada con esa categoría.

   ![](assets/my-profile-notifications.png)

1. Seleccione o anule la selección de las casillas de verificación de la derecha para especificar si desea recibir o no notificaciones diariamente, al instante o ambas.

   También puede utilizar las casillas de verificación de una categoría para activar o desactivar todas las notificaciones de esa categoría.

   >[!NOTE]
   >
   >Si es miembro del equipo de un proyecto, seguirá recibiendo notificaciones por correo electrónico hasta que se le elimine del equipo, incluso si ya no tiene acceso al proyecto. Para obtener instrucciones sobre cómo quitar usuarios de un equipo, consulte [Quitar usuarios de proyectos](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   Para el **[!UICONTROL Comunicación]** categoría, puede seleccionar notificaciones individuales solo para envío instantáneo. Para que las notificaciones se envíen en un resumen diario, debe seleccionarlas todas.

   Si se activan todas las notificaciones por correo electrónico de una categoría determinada, la casilla del título de la categoría aparece como seleccionada. Si todas las notificaciones por correo electrónico de una categoría determinada están desactivadas, la casilla no está seleccionada. Si algunas notificaciones están activadas y otras desactivadas, la casilla de verificación de la categoría aparece como una línea recta.\
   Al modificar una configuración de notificación, la etiqueta **[!UICONTROL Editado]** aparece para esa configuración de notificación, para hacerle saber que esa configuración de notificación se ha modificado.

1. Si seleccionó cualquier notificación para enviarla como un compendio diario, seleccione la hora del día a la que desea recibirla en la parte superior de la **[!UICONTROL Notificaciones]** de la sección **[!UICONTROL Enviar correo electrónico de resumen diario después de]** menú.

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   El compendio diario incluye eventos que cumplen los criterios de las notificaciones 24 horas antes de la hora seleccionada. Recibirá un correo electrónico de resumen diario para cada tipo de notificación.\
   El resumen diario puede llegar después del tiempo seleccionado, según la cantidad de correos electrónicos en cola para su envío en el sistema. La hora indicada es la hora local según se especifica en la configuración del explorador.

1. (Condicional y opcional) Al modificar la configuración de las notificaciones por correo electrónico en el entorno de vista previa, habilite la variable **[!UICONTROL Recibir correos electrónicos de este entorno de prueba]** configuración para recibir correos electrónicos. Los correos electrónicos no se generan automáticamente desde el entorno de vista previa.

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. Haga clic en **[!UICONTROL Guardar cambios]**.
