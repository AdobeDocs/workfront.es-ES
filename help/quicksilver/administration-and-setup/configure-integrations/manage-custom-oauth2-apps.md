---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Ver y administrar aplicaciones OAuth2 personalizadas
description: Como administrador de Adobe Workfront, puede ver y administrar las aplicaciones OAuth2 para su instancia de Workfront, que permiten que otras aplicaciones accedan a Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Becky
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# Ver y administrar aplicaciones OAuth2 personalizadas

Como administrador de [!DNL Adobe Workfront], puede ver y administrar las aplicaciones OAuth2 para su instancia de [!DNL Workfront], que permiten que otras aplicaciones tengan acceso a [!UICONTROL Workfront].

>[!NOTE]
>
>* En el contexto de OAuth2, &quot;aplicación Oauth2&quot; hace referencia a este tipo de vínculo de acceso entre una aplicación y un servidor como [!DNL Workfront]. Para obtener más información, consulte [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* Puede tener hasta un total de diez aplicaciones OAuth2 a la vez.

* Para obtener información sobre cómo crear aplicaciones OAuth2 personalizadas, consulte [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Para obtener instrucciones sobre cómo configurar y utilizar la aplicación OAuth2 con credenciales de usuario (flujo de código de autorización), consulte [Configurar y utilizar las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo de código de autorización](../../wf-api/api/oauth-app-code-token-flow.md).
* Para obtener instrucciones sobre cómo configurar y utilizar la aplicación OAuth2 mediante la autenticación de servidor (flujo JWT), consulte [Configurar y utilizar las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Para obtener instrucciones sobre cómo configurar y utilizar la aplicación OAuth2 mediante PKCE, consulte [Configurar y utilizar las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td> Debe ser administrador de [!DNL Workfront]. </p>
    <p>Para obtener información sobre los administradores de [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

+++

## Requisitos previos

Debe crear [!UICONTROL aplicaciones OAuth2] para su organización antes de poder verlas o administrarlas.

Para obtener más información, consulte [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Administrar aplicaciones OAuth2 personalizadas

* [Ver y editar aplicaciones OAuth2 personalizadas](#view-and-edit-custom-oauth2-applications)
* [Eliminar aplicaciones OAuth2 personalizadas](#delete-custom-oauth2-applications)

### Ver y editar aplicaciones OAuth2 personalizadas {#view-and-edit-custom-oauth2-applications}

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]** y, a continuación, seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Haga clic en **[!UICONTROL Crear integración de aplicación]**.
1. Pase el ratón sobre la aplicación y haga clic en **[!UICONTROL Editar]** ![](assets/edit-icon.png) cuando aparezca en el extremo derecho.
1. (Opcional) Edite cualquier detalle de la aplicación.

   Para los campos relacionados con las aplicaciones OAuth2 y JWT, consulte [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Eliminar aplicaciones OAuth2 personalizadas {#delete-custom-oauth2-applications}

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]** y, a continuación, seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Haga clic en ** **.
1. Pase el ratón sobre la aplicación y haga clic en **[!UICONTROL Eliminar]** ![](assets/delete.png) cuando aparezca en el extremo derecho.

## Administrar secretos de cliente en aplicaciones OAuth2

* [Ver detalles del Secreto del cliente](#view-client-secret-details)
* [Agregar o editar notas para Secreto del cliente](#add-or-edit-notes-for-client-secret)
* [Eliminar secreto de cliente](#delete-client-secret)

### Ver detalles del Secreto del cliente {#view-client-secret-details}

>[!IMPORTANT]
>
>No puede ver el propio Secreto de cliente. Si ha perdido el Secreto del cliente, debe eliminarlo y crear uno nuevo.
>
>* Para eliminar un secreto de cliente, consulte [Eliminar secreto de cliente](#delete-client-secret) en este artículo.
>* Para crear un nuevo Secreto de cliente, consulte [Crear una aplicación OAuth2](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) en [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]** y, a continuación, seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Pase el ratón sobre la aplicación y haga clic en el icono **[!UICONTROL Editar]** cuando aparezca en el extremo derecho.
1. Vea los detalles en el área Secreto del cliente:

   * Fecha de creación
   * Fecha de último uso
   * Notas

     Para agregar notas a un Secreto de cliente, consulte [Agregar o editar notas para el Secreto de cliente](#add-or-edit-notes-for-client-secret).

### Agregar o editar notas para Secreto del cliente {#add-or-edit-notes-for-client-secret}

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]** y, a continuación, seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Haga clic en **[!UICONTROL Crear integración de aplicación]**.
1. Pase el ratón sobre la aplicación y haga clic en el icono **[!UICONTROL Editar]** cuando aparezca en el extremo derecho.
1. Busque el Secreto de cliente para el que desea agregar o editar una nota.
1. Haga clic en el cuadro que contiene los detalles del Secreto del cliente.

   Ahora puede agregar texto de nota o editar el texto de nota existente.

   >[!NOTE]
   >
   >El texto de la nota tiene un máximo de 64 caracteres.

1. Haga clic fuera del cuadro o presione **[!UICONTROL Entrar]** para guardar el texto de la nota.

### Eliminar secreto de cliente {#delete-client-secret}

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]** y, a continuación, seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Haga clic en **[!UICONTROL Crear integración de aplicación]**.
1. Pase el ratón sobre la aplicación y haga clic en el icono **[!UICONTROL Editar]** cuando aparezca en el extremo derecho.
1. Busque el Secreto de cliente que desea eliminar.
1. Haga clic en el icono **[!UICONTROL Eliminar]** ![](assets/delete.png) junto al Secreto del cliente.
