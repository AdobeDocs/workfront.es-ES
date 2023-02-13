---
product-area: setup
navigation-topic: notifications
title: Activar o desactivar sus propias notificaciones de eventos
description: El administrador de Adobe Workfront configura qué notificaciones de eventos reciben los usuarios cuando se producen eventos en Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: ea16b13b6ecb6ecea365c6c4d31ee23b7bb712c6
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# Activar o desactivar sus propias notificaciones de eventos

Su Adobe [!DNL Workfront] el administrador configura las notificaciones de eventos que reciben los usuarios cuando se producen eventos en Workfront (tal como se describe en [[!UICONTROL Configurar evento] notificaciones para todos los miembros del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

El administrador del grupo también puede configurar qué notificaciones de eventos se activan para usted y los usuarios del grupo de inicio. Si su [!UICONTROL Grupo de inicio] es un subgrupo, recibe las notificaciones de eventos activadas para el grupo de nivel superior situado encima del grupo.

Puede personalizarlo aún más configurando qué notificaciones recibe. También puede elegir si desea recibir notificaciones a medida que ocurran los eventos o en un correo electrónico de resumen diario.

Para obtener información sobre las notificaciones por correo electrónico, consulte [[!DNL Adobe Workfront] notificaciones](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* Si activa un tipo de notificación y después descubre que no recibe notificaciones de ese tipo, puede deberse a que ese tipo no se aplica a su función.
>* La variable [!DNL Workfront] un administrador o un administrador de grupo no pueden configurar las notificaciones para [!DNL Workfront Goals]. Para obtener más información sobre las notificaciones, la variable [!DNL Workfront] administrador puede configurar, consulte [Configurar notificaciones de eventos para todos los miembros del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Para obtener información sobre la configuración de notificaciones individuales para [!DNL Workfront Goals] siga leyendo este artículo.
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
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Work] o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Ver y modificar la configuración de las notificaciones por correo electrónico

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y, a continuación, haga clic en su nombre de usuario junto a la imagen de perfil.

1. Haga clic en el **[!UICONTROL Más]** icono ![](assets/more-icon.png) y haga clic en **[!UICONTROL Editar]**.

1. En el **[!UICONTROL Editar persona]** que se muestra, vaya a la **[!UICONTROL Notificaciones]** para obtener más información.

1. Haga clic en una categoría para ver la configuración de notificación relacionada con esa categoría.

   ![](assets/my-profile-notifications.png)

1. Seleccione o anule la selección de las casillas de verificación de la derecha para especificar si desea recibir o no notificaciones diariamente, instantáneamente o ambas.

   También puede utilizar las casillas de verificación de una categoría para activar o desactivar todas las notificaciones de esa categoría.

   >[!NOTE]
   >
   >Si es miembro del equipo de un proyecto, seguirá recibiendo notificaciones por correo electrónico hasta que se le elimine del equipo, aunque ya no tenga acceso al proyecto. Para obtener instrucciones sobre cómo quitar usuarios de un equipo, consulte [Eliminar usuarios de proyectos](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   Para la variable **[!UICONTROL Comunicación]** , puede seleccionar notificaciones individuales solo para envío instantáneo. Para que las notificaciones se envíen en un compendio diario, debe seleccionarlas todas.

   Si se activan todas las notificaciones por correo electrónico de una categoría determinada, el cuadro del título de la categoría aparece como seleccionado. Si todas las notificaciones por correo electrónico de una categoría determinada están desactivadas, la casilla no está seleccionada. Si algunas notificaciones están activadas y otras están desactivadas, la casilla de verificación de la categoría aparece como una línea recta.\
   Al modificar una configuración de notificación, la etiqueta **[!UICONTROL Editado]** para esa configuración de notificación, para informarle de que se ha modificado dicha configuración de notificación.

1. Si seleccionó cualquier notificación para enviarla como un compendio diario, seleccione la hora del día en la que desea recibirla en la parte superior del **[!UICONTROL Notificaciones]** en la sección **[!UICONTROL Enviar un resumen diario por correo electrónico después de]** para abrir el Navegador.

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   El compendio diario incluye eventos que cumplen los criterios de las notificaciones 24 horas antes de la hora seleccionada. Recibe un resumen diario por correo electrónico para cada tipo de notificación.\
   El compendio diario puede llegar después del tiempo seleccionado, dependiendo de cuántos correos electrónicos se hayan puesto en cola para su envío en el sistema. La hora que aparece es la hora local, tal como se especifica en la configuración del explorador.

1. (Condicional y opcional) Al modificar la configuración de las notificaciones por correo electrónico en el entorno de Vista previa, habilite la variable **[!UICONTROL Recibir correos electrónicos de este entorno de prueba]** configuración para recibir correos electrónicos. Los correos electrónicos no se generan automáticamente desde el entorno de vista previa.

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. Haga clic en **[!UICONTROL Guardar cambios]**.
