---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Ver y administrar aplicaciones OAuth2 personalizadas
description: Como administrador de Adobe Workfront, puedes ver y gestionar las aplicaciones OAuth2 de tu instancia de Workfront, las cuales permiten que otras aplicaciones accedan a Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Becky
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 711812d9fd4bf48bb7612c0339cee2cdbe08ef10
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 92%

---

# Ver y gestionar aplicaciones OAuth2 personalizadas

Como [!DNL Adobe Workfront] administrador, puedes ver y gestionar las aplicaciones OAuth2 de tu instancia de [!DNL Workfront], las cuales permiten que otras aplicaciones accedan a [!UICONTROL Workfront].

>[!NOTE]
>
>* En el contexto de OAuth2, “aplicación Oauth2” se refiere a este tipo de enlace de acceso entre una aplicación y un servidor, como [!DNL Workfront]. Para obtener más información, consulte [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* Puede tener hasta un total de diez aplicaciones OAuth2 a la vez.

* Para obtener información sobre cómo crear aplicaciones OAuth2 personalizadas, consulta [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Para obtener instrucciones sobre cómo configurar y utilizar la aplicación OAuth2 con credenciales de usuario (flujo de código de autorización), consulte [Configure y utilice las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo del código de autorización](../../wf-api/api/oauth-app-code-token-flow.md).
* Para obtener instrucciones sobre cómo configurar y utilizar la aplicación OAuth2 con la autenticación de servidor (flujo JWT), consulte [Configurar y utilizar las aplicaciones personalizadas OAuth 2 de su organización mediante el flujo JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Para instrucciones sobre cómo configurar y usar la aplicación OAuth2 utilizando PKCE, consulta [Configure y utilice las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Debe crear aplicaciones [!UICONTROL OAuth2] para su organización antes de que pueda ver o administrar.

Para obtener más información, consulte [Crear aplicaciones OAuth2 para  [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Gestionar aplicaciones OAuth2 personalizadas

* [Ver y editar aplicaciones OAuth2 personalizadas](#view-and-edit-custom-oauth2-applications)
* [Eliminar aplicaciones OAuth2 personalizadas](#delete-custom-oauth2-applications)

### Ver y editar aplicaciones OAuth2 personalizadas {#view-and-edit-custom-oauth2-applications}

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]**, y luego seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Haga clic en **[!UICONTROL Crear integración de aplicaciones]**.
1. Pase el ratón sobre la aplicación y haga clic en **[!UICONTROL Editar]** ![Editar icono](assets/edit-icon.png) cuando aparezca en el extremo derecho.
1. (Opcional) Edite cualquier detalle de la aplicación.

   Para campos relacionados con aplicaciones OAuth2 y JWT, consulte [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Eliminar aplicaciones OAuth2 personalizadas {#delete-custom-oauth2-applications}

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]**, y luego seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Pase el ratón sobre la aplicación y haga clic en **[!UICONTROL Eliminar]** ![Eliminar](assets/delete.png) cuando aparezca en el extremo derecho.

## Administrar secretos de cliente en aplicaciones OAuth2

* [Ver detalles del Secreto del cliente](#view-client-secret-details)
* [Agregar o editar notas para el Secreto de cliente](#add-or-edit-notes-for-client-secret)
* [Eliminar secreto de cliente](#delete-client-secret)

### Ver detalles del Secreto del cliente {#view-client-secret-details}

>[!IMPORTANT]
>
>No puede ver el propio Secreto de cliente. Si ha perdido el Secreto del cliente, debe eliminarlo y crear uno nuevo.
>
>* Para eliminar un Secreto de Cliente, consulta [Eliminar Secreto de Cliente](#delete-client-secret) en este artículo.
>* Para crear un nuevo Secreto de Cliente, consulta [Creación de una aplicación OAuth2](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) en [Crear aplicaciones OAuth2 para [!DNL Workfront] integraciones](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haz clic en **[!UICONTROL Sistema]**, y luego selecciona **[!UICONTROL Aplicaciones OAuth]**.
1. Pase el puntero por encima de la aplicación y haga clic en el icono de **[!UICONTROL Editar]** cuando aparezca en el extremo derecho.
1. Vea los detalles en el área Secreto del cliente:

   * Fecha de creación
   * Fecha de último uso
   * Notas

     Para agregar notas a un Secreto de cliente, consulte [Agregar o editar notas para el Secreto de cliente](#add-or-edit-notes-for-client-secret).

### Agregar o editar notas para el Secreto de cliente {#add-or-edit-notes-for-client-secret}

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]**, y luego seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Haz clic en **[!UICONTROL Crear integración de aplicaciones]**.
1. Pase el puntero por encima de la aplicación y haga clic en el icono de **[!UICONTROL Editar]** cuando aparezca en el extremo derecho.
1. Busque el Secreto de cliente para el que desea agregar o editar una nota.
1. Haga clic en el cuadro que contiene los detalles del Secreto del cliente.

   Ahora puede agregar texto de nota o editar el texto de nota existente.

   >[!NOTE]
   >
   >El texto de la nota tiene un máximo de 64 caracteres.

1. Haz clic fuera del cuadro o presiona **[!UICONTROL Intro]** para guardar el texto de la nota.

### Eliminar secreto de cliente {#delete-client-secret}

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]**, y luego seleccione **[!UICONTROL Aplicaciones OAuth]**.
1. Haz clic en **[!UICONTROL Crear integración de aplicaciones]**.
1. Pase el puntero por encima de la aplicación y haga clic en el icono de **[!UICONTROL Editar]** cuando aparezca en el extremo derecho.
1. Busque el Secreto de cliente que desea eliminar.
1. Haga clic en el icono **[!UICONTROL Eliminar]** ![Eliminar](assets/delete.png) que está junto al Secreto del cliente.
