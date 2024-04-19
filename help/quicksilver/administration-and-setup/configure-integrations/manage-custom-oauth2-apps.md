---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Ver y administrar aplicaciones OAuth2 personalizadas
description: Como administrador de Adobe Workfront, puede ver y administrar las aplicaciones OAuth2 para su instancia de Workfront, que permiten que otras aplicaciones accedan a Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---

# Ver y administrar aplicaciones OAuth2 personalizadas

Como un [!DNL Adobe Workfront] administrador, puede ver y administrar las aplicaciones OAuth2 para su instancia de [!DNL Workfront], que permiten a otras aplicaciones acceder a [!UICONTROL Workfront].

>[!NOTE]
>
>* En el contexto de OAuth2, &quot;aplicación Oauth2&quot; hace referencia a este tipo de vínculo de acceso entre una aplicación y un servidor como [!DNL Workfront]. Para obtener más información, consulte [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* Puede tener hasta un total de diez aplicaciones OAuth2 a la vez.

* Para obtener información sobre la creación de aplicaciones OAuth2 personalizadas, consulte [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Para obtener instrucciones sobre la configuración y el uso de la aplicación OAuth2 con credenciales de usuario (flujo de código de autorización), consulte [Configure y utilice las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo del código de autorización](../../wf-api/api/oauth-app-code-token-flow.md).
* Para obtener instrucciones sobre la configuración y el uso de la aplicación OAuth2 mediante la autenticación del servidor (flujo JWT), consulte [Configure y utilice las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Para obtener instrucciones sobre la configuración y el uso de la aplicación OAuth2 mediante PKCE, consulte [Configure y utilice las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> Debe ser un [!DNL Workfront] administrador. </p>
    <p>Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Debe crear [!UICONTROL OAuth2] aplicaciones para su organización antes de poder verlas o administrarlas.

Para obtener más información, consulte [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Administrar aplicaciones OAuth2 personalizadas

* [Ver y editar aplicaciones OAuth2 personalizadas](#view-and-edit-custom-oauth2-applications)
* [Eliminar aplicaciones OAuth2 personalizadas](#delete-custom-oauth2-applications)

### Ver y editar aplicaciones OAuth2 personalizadas {#view-and-edit-custom-oauth2-applications}

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]**, luego seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Clic **[!UICONTROL Crear integración de aplicaciones]**.
1. Pase el ratón sobre la aplicación y haga clic en **[!UICONTROL Editar]** ![](assets/edit-icon.png) cuando aparece en el extremo derecho.
1. (Opcional) Edite cualquier detalle de la aplicación.

   Para ver los campos relacionados con las aplicaciones OAuth2 y JWT, consulte [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Eliminar aplicaciones OAuth2 personalizadas {#delete-custom-oauth2-applications}

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]**, luego seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Haga clic en ** **.
1. Pase el ratón sobre la aplicación y haga clic en **[!UICONTROL Eliminar]** ![](assets/delete.png) cuando aparece en el extremo derecho.

## Administrar secretos de cliente en aplicaciones OAuth2

* [Ver detalles del Secreto del cliente](#view-client-secret-details)
* [Agregar o editar notas para Secreto del cliente](#add-or-edit-notes-for-client-secret)
* [Eliminar secreto de cliente](#delete-client-secret)

### Ver detalles del Secreto del cliente {#view-client-secret-details}

>[!IMPORTANT]
>
>No puede ver el propio Secreto de cliente. Si ha perdido el Secreto del cliente, debe eliminarlo y crear uno nuevo.
>
>* Para eliminar un Secreto de cliente, consulte [Eliminar secreto de cliente](#delete-client-secret) en este artículo.
>* Para crear un nuevo Secreto de cliente, consulte [Creación de una aplicación OAuth2](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>



1. Haga clic en *[!UICONTROL *Menú principal]* Icono * ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]**, luego seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Pase el ratón sobre la aplicación y haga clic en **[!UICONTROL Editar]** cuando aparece en el extremo derecho.
1. Vea los detalles en el área Secreto del cliente:

   * Fecha de creación
   * Fecha de último uso
   * Notas

     Para agregar notas a un Secreto de cliente, consulte [Agregar o editar notas para Secreto del cliente](#add-or-edit-notes-for-client-secret).

### Agregar o editar notas para Secreto del cliente {#add-or-edit-notes-for-client-secret}

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]**, luego seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Clic **[!UICONTROL Crear integración de aplicaciones]**.
1. Pase el ratón sobre la aplicación y haga clic en **[!UICONTROL Editar]** cuando aparece en el extremo derecho.
1. Busque el Secreto de cliente para el que desea agregar o editar una nota.
1. Haga clic en el cuadro que contiene los detalles del Secreto del cliente.

   Ahora puede agregar texto de nota o editar el texto de nota existente.

   >[!NOTE]
   >
   >El texto de la nota tiene un máximo de 64 caracteres.

1. Haga clic fuera del cuadro o presione **[!UICONTROL Entrar]** para guardar el texto de la nota.

### Eliminar secreto de cliente {#delete-client-secret}

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]**, luego seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Clic **[!UICONTROL Crear integración de aplicaciones]**.
1. Pase el ratón sobre la aplicación y haga clic en **[!UICONTROL Editar]** cuando aparece en el extremo derecho.
1. Busque el Secreto de cliente que desea eliminar.
1. Haga clic en **[!UICONTROL Eliminar]** icono ![](assets/delete.png) junto al Secreto del cliente.
