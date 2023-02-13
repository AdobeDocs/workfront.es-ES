---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Ver y administrar aplicaciones OAuth2 personalizadas
description: Como administrador de Adobe Workfront, puede ver y administrar las aplicaciones OAuth2 de su instancia de Workfront, lo que permite que otras aplicaciones accedan a Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: f7e3182776e6b62103cd755b2fbd5057efc95394
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Ver y administrar aplicaciones OAuth2 personalizadas

Como [!DNL Adobe Workfront] administrador, puede ver y administrar las aplicaciones OAuth2 para su instancia de [!DNL Workfront], que permiten acceder a otras aplicaciones [!UICONTROL Workfront].

>[!NOTE]
>
>En el contexto de OAuth2, &quot;Aplicación Oauth2&quot; se refiere a este tipo de vínculo de acceso entre una aplicación y un servidor como [!DNL Workfront]. Para obtener más información, consulte [Creación de aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md)

* Para obtener información sobre la creación de aplicaciones OAuth2 personalizadas, consulte [Creación de aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Para obtener instrucciones sobre la configuración y el uso de la aplicación OAuth2 con credenciales de usuario (flujo de código de autorización), consulte [Configure y utilice las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo de código de autorización](../../wf-api/api/oauth-app-code-token-flow.md).
* Para obtener instrucciones sobre cómo configurar y usar la aplicación OAuth2 mediante autenticación de servidor (flujo JWT), consulte [Configure y utilice las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo JWT](../../wf-api/api/oauth-app-jwt-flow.md).
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
   <td> Debe ser [!DNL Workfront] administrador. </p>
    <p>Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Debe crear [!UICONTROL OAuth2] aplicaciones para su organización antes de poder verlas o administrarlas.

Para obtener más información, consulte [Creación de aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Administrar aplicaciones OAuth2 personalizadas

* [Ver y editar aplicaciones OAuth2 personalizadas](#view-and-edit-custom-oauth2-applications)
* [Eliminar aplicaciones OAuth2 personalizadas](#delete-custom-oauth2-applications)

### Ver y editar aplicaciones OAuth2 personalizadas {#view-and-edit-custom-oauth2-applications}

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]** y, a continuación, seleccione **[!UICONTROL Aplicaciones de OAuth]**.
1. Haga clic en **[!UICONTROL Crear integración de aplicaciones]**.
1. Pase el ratón sobre la aplicación y haga clic en **[!UICONTROL Editar]** ![](assets/edit-icon.png) cuando aparece en el extremo derecho.
1. (Opcional) Edite cualquier detalle de la aplicación.

   Para campos relacionados con aplicaciones OAuth2 y JWT, consulte [Creación de aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Eliminar aplicaciones OAuth2 personalizadas {#delete-custom-oauth2-applications}

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]** y, a continuación, seleccione **[!UICONTROL Aplicaciones de OAuth]**.
1. Haga clic **  **.
1. Pase el ratón sobre la aplicación y haga clic en **[!UICONTROL Eliminar]** ![](assets/delete.png) cuando aparece en el extremo derecho.

## Administrar secretos de cliente en aplicaciones OAuth2

* [Ver detalles del secreto del cliente](#view-client-secret-details)
* [Agregar o editar notas para Client Secret](#add-or-edit-notes-for-client-secret)
* [Eliminar secreto del cliente](#delete-client-secret)

### Ver detalles del secreto del cliente {#view-client-secret-details}

>[!IMPORTANT]
>
>No puede ver el propio Secreto del cliente. Si ha perdido el secreto del cliente, debe eliminarlo y crear uno nuevo.
>
>* Para eliminar un secreto de cliente, consulte [Eliminar secreto del cliente](#delete-client-secret) en este artículo.
>* Para crear un nuevo Secreto de cliente, consulte [Creación de una aplicación OAuth2](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) en [Creación de aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>




1. Haga clic en el *[!UICONTROL *Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]** y, a continuación, seleccione **[!UICONTROL Aplicaciones de OAuth]**.
1. Pase el ratón sobre la aplicación y haga clic en la **[!UICONTROL Editar]** cuando aparezca en el extremo derecho.
1. Ver detalles en el área Secreto del cliente:

   * Fecha de creación
   * Última fecha de uso
   * Notas

      Para añadir notas a un Secreto de cliente, consulte [Agregar o editar notas para Client Secret](#add-or-edit-notes-for-client-secret).

### Agregar o editar notas para Client Secret {#add-or-edit-notes-for-client-secret}

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]** y, a continuación, seleccione **[!UICONTROL Aplicaciones de OAuth]**.
1. Haga clic en **[!UICONTROL Crear integración de aplicaciones]**.
1. Pase el ratón sobre la aplicación y haga clic en la **[!UICONTROL Editar]** cuando aparezca en el extremo derecho.
1. Busque el Secreto del cliente para el que desea agregar o editar una nota.
1. Haga clic en la casilla que contiene los detalles del Secreto del cliente.

   Ahora puede agregar texto de nota o editar texto de nota existente.

   >[!NOTE]
   >
   >El texto de la nota tiene un máximo de 64 caracteres.

1. Haga clic fuera de la caja o presione **[!UICONTROL Entrar]** para guardar el texto de la nota.

### Eliminar secreto del cliente {#delete-client-secret}

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]** y, a continuación, seleccione **[!UICONTROL Aplicaciones de OAuth]**.
1. Haga clic en **[!UICONTROL Crear integración de aplicaciones]**.
1. Pase el ratón sobre la aplicación y haga clic en la **[!UICONTROL Editar]** cuando aparezca en el extremo derecho.
1. Busque el Secreto del cliente que desea eliminar.
1. Haga clic en el **[!UICONTROL Eliminar]** icono ![](assets/delete.png) junto al Secreto del cliente.
