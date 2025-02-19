---
navigation-topic: notifications
title: Habilitación del envío de correos electrónicos desde el entorno de zona protegida de vista previa
description: Si desea recibir notificaciones por correo electrónico desde el entorno de zona protegida de vista previa, debe habilitar esta funcionalidad en la configuración del usuario mientras inicia sesión en la vista previa.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: 6a1152bb86a856d60585db7d6ffd43a59a212a72
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 95%

---

# Habilitación del envío de correos electrónicos desde el entorno de zona protegida de vista previa

[!UICONTROL Adobe Workfront] deshabilita todas las comunicaciones por correo electrónico de los entornos de vista previa y de zona protegida de actualización personalizados. Para obtener información sobre el entorno de zona protegida de vista previa, consulte [El entorno de zona protegida de vista previa de Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Para obtener información sobre el entorno de zona protegida de actualización personalizada, consulte [El entorno de zona protegida de actualización personalizada de Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Si desea recibir las siguientes notificaciones por correo electrónico desde el entorno de zona protegida de vista previa, debe habilitar esta funcionalidad en la configuración del usuario mientras inicia sesión en la vista previa:

* Notificaciones por correo electrónico activadas por notificaciones de eventos
* Notificaciones de recordatorio
* Notificaciones automáticas de recordatorio tardías o tempranas
* Invitaciones por correo electrónico

Puede hacerlo por su cuenta o mediante cualquier usuario al que tenga acceso de edición. Para obtener más información sobre el acceso necesario para editar usuarios, consulte [Conceder acceso a usuarios](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>Las notificaciones push y de envío de informes en la aplicación móvil siempre están desactivadas para el entorno de zona protegida de vista previa. Ni usted ni el administrador de [!DNL Workfront] pueden habilitar la entrega de informes ni las notificaciones push para la aplicación móvil al acceder al entorno de zona protegida de vista previa.
>
>Para obtener información sobre las entregas de informes, consulte [Información general de entrega de informes](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

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
   <td> <p>Debe tener uno de los siguientes elementos:</p> 
    <ul> 
     <li> <p>Nivel de acceso de [!UICONTROL System Administrator].</p> <p> Para obtener información acerca de este nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>. </p> </li> 
     <li> <p>En su nivel de acceso, [!UICONTROL Edit] debe estar seleccionado para la configuración [!UICONTROL Users]. Y, para la configuración de [!UICONTROL Users], en [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> , la opción [!UICONTROL Create] y al menos una de las dos opciones de [!UICONTROL User Admin] deben estar habilitadas. </p> <p>Si utiliza la opción [!UICONTROL User Admin (Group Users)], debe ser administrador de un grupo del que sea miembro el usuario.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>Para obtener información acerca de la configuración de [!UICONTROL Users] en un nivel de acceso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
    </ul> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Habilitación del envío de correos electrónicos desde el entorno de zona protegida de vista previa

1. Inicie sesión en el entorno de zona protegida de vista previa.
1. Haga clic en la imagen de perfil, en la esquina superior derecha de [!DNL Adobe Workfront]. A continuación, haga clic en el menú **[!UICONTROL More]** y seleccione **[!UICONTROL Edit]**.

   O

   Busque un usuario en [!DNL Workfront] y haga clic en su nombre. A continuación, haga clic en el menú **[!UICONTROL Más]** y seleccione **[!UICONTROL Editar]**.

   O

   Para varios usuarios: haga clic en el icono **[!UICONTROL Menú principal]** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Workfront y, a continuación, haga clic en **[!UICONTROL Usuarios]** ![Icono del usuario](assets/users-icon-in-main-menu.png).  A continuación, seleccione varios usuarios y haga clic en **[!UICONTROL Editar]**.

1. Haga clic en **[!UICONTROL Preferencias]**.
1. Seleccione **[!UICONTROL Recibir mensajes de correo electrónico de este entorno de prueba]**.

   >[!NOTE]
   >
   >Esta opción no está disponible si se encuentra en un entorno de producción.

1. Haga clic en **[!UICONTROL Guardar cambios]**.
