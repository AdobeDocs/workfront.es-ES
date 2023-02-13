---
navigation-topic: notifications
title: Habilitar el envío de correos electrónicos desde el entorno de Preview Sandbox
description: Si desea recibir notificaciones por correo electrónico del entorno de espacio aislado de vista previa, debe habilitar esta funcionalidad en la configuración de usuario mientras ha iniciado sesión en Vista previa.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Habilitar el envío de correos electrónicos desde el entorno de Preview Sandbox

[!UICONTROL Adobe Workfront] Desactiva toda la comunicación por correo electrónico desde los entornos Preview y Custom Refresh Sandbox. Para obtener información sobre el entorno limitado de vista previa, consulte [Entorno de espacio aislado de vista previa de Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Para obtener información sobre el entorno limitado de actualización personalizada, consulte [Entorno de espacio aislado de actualización personalizado de Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Si desea recibir las siguientes notificaciones por correo electrónico del entorno de la zona de pruebas de vista previa, debe activar esta funcionalidad en la configuración del usuario mientras ha iniciado sesión en Vista previa:

* Notificaciones de correo electrónico activadas por notificaciones de eventos
* Notificaciones de recordatorio
* Notificaciones automáticas de recordatorio atrasado o anticipado
* Invitaciones por correo electrónico

Puede hacerlo por sí mismo o por cualquier usuario al que tenga acceso para editar. Para obtener más información sobre el acceso necesario para editar usuarios, consulte [Conceder acceso a los usuarios](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>El envío de informes y las notificaciones push en la aplicación móvil siempre están desactivadas para el entorno de espacio aislado de vista previa. Ni tú ni el [!DNL Workfront] el administrador puede activar el envío de informes o las notificaciones push para la aplicación móvil al acceder al entorno de espacio aislado de vista previa.
>
>Para obtener información sobre los envíos de informes, consulte [Resumen del envío de informes](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

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
   <td> <p>[!UICONTROL Request] o superior para cambiar su propia configuración</p> <p>[!UICONTROL Plan] para editar la configuración para otros usuarios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Debe tener una de las siguientes opciones:</p> 
    <ul> 
     <li> <p>Nivel de acceso de [!UICONTROL System Administrator].</p> <p> Para obtener información sobre este nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
     <li> <p>En el nivel de acceso, debe seleccionar [!UICONTROL Edit] para la configuración [!UICONTROL Users]. Y, para la configuración [!UICONTROL Usuarios], en [!UICONTROL Ajustar la configuración] <img src="assets/gear-icon-in-access-levels.png"> , la opción [!UICONTROL Crear] y al menos una de las dos opciones [!UICONTROL User Admin] deben estar activadas. </p> <p>Si utiliza la opción [!UICONTROL User Admin (Group Users)], debe ser administrador de grupo de un grupo del que sea miembro el usuario.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>Para obtener información sobre la configuración [!UICONTROL Usuarios] en un nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
    </ul> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Activación del envío de correos electrónicos desde el entorno de espacio aislado de vista previa

1. Inicie sesión en el entorno limitado de vista previa.
1. Haga clic en la imagen de perfil en la esquina superior derecha de [!DNL Adobe Workfront]. A continuación, haga clic en el **[!UICONTROL Más]** y seleccione **[!UICONTROL Editar]**.

   O

   Busque un usuario en [!DNL Workfront] y haga clic en su nombre. A continuación, haga clic en el **[!UICONTROL Más]** y seleccione **[!UICONTROL Editar]**.

   O

   Para varios usuarios: Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **[!UICONTROL Usuarios]** ![](assets/users-icon-in-main-menu.png).  A continuación, seleccione varios usuarios y haga clic en **[!UICONTROL Editar]**.

1. Haga clic en **[!UICONTROL Preferencias]**.
1. Select **[!UICONTROL Recibir correos electrónicos de este entorno de prueba]**.

   >[!NOTE]
   >
   >Esta opción no está disponible si se encuentra en un entorno de producción.

1. Haga clic en **[!UICONTROL Guardar cambios]**.
