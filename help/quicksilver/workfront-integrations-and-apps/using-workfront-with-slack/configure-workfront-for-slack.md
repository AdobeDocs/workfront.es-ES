---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Configurar  [!DNL Adobe Workfront]  para Slack
description: Al integrar  [!DNL Adobe Workfront]  con Slack, podrá acceder a elementos de trabajo, aprobaciones, favoritos y elementos recientes de Slack y crearlos en  [!DNL Workfront] .
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 95%

---

# Configurar [!DNL Adobe Workfront for Slack]

Al integrar [!DNL Adobe Workfront] con [!DNL Slack], puede hacer lo siguiente:

* Acceder a sus elementos de trabajo, aprobaciones, favoritos y elementos recientes de [!DNL Workfront] desde [!DNL Slack].
* Suscribirse, aprobar o asignar trabajo desde [!DNL Slack].
* Crear tareas y problemas desde [!DNL Slack].
* Recibir algunas notificaciones de [!DNL Workfront] en [!DNL Slack].

Según la configuración del entorno de [!DNL Slack], puede instalar y configurar [!DNL Workfront for Slack] usted mismo, o bien el administrador de [!DNL Workfront] debe instalarlo y configurarlo primero antes de que pueda configurarlo usted mismo.

Al integrar su instancia de [!DNL Slack] con [!DNL Workfront], los usuarios pueden usar [!DNL Workfront] mientras colaboran en sus canales de [!DNL Slack]. La integración se puede usar desde cualquier entorno de [!DNL Slack], incluida la aplicación móvil [!DNL Slack]. ## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Cualquiera</p>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos para usar [!DNL Workfront] con [!DNL Slack]

* Debe tener una instancia de [!DNL Slack].
* El administrador del sistema [!DNL Slack] debe permitir que todos los usuarios de [!DNL Slack] instalen [!DNL Workfront for Slack].
* Debe tener una licencia de [!DNL Workfront] para poder usar las características integradas en [!DNL Workfront].

  >[!NOTE]
  >
  >Los usuarios con cualquier tipo de licencia [!DNL Workfront] pueden acceder a [!DNL Workfront] desde [!DNL Slack]. Las acciones que puede realizar desde [!DNL Slack] se limitan a los niveles de licencia y permiso de [!DNL Workfront].

Para obtener más información acerca de la administración de aplicaciones en [!DNL Slack], consulte [Administrar aplicaciones para su Workspace.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Instalar [!DNL Workfront for Slack]

Cada usuario de [!DNL Slack] debe instalar la aplicación [!DNL Workfront] por sí mismo para poder usar [!DNL Workfront] desde [!DNL Slack].

Puede instalar la aplicación de las siguientes maneras:

* [Instalar la aplicación  [!DNL Workfront]  fuera de [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Instalar la aplicación  [!DNL Workfront]  dentro de [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Instalar la aplicación [!DNL Workfront] fuera de [!DNL Slack] {#install-the-workfront-app-outside-slack}

Siga los pasos a continuación para ejecutar el proceso de instalación y autorizar a [!DNL Workfront for Slack] en su instancia de [!DNL Slack].

>[!IMPORTANT]
>
>Cuando se lanza una nueva versión de [!DNL Workfront] para Slack, debe volver a autorizar la aplicación para poder seguir usándola.

1. Busque el complemento [!DNL Adobe Workfront] en el [[!DNL Slack] almacén](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Haga clic en **[!UICONTROL Abrir en[!DNL Slack]]**.

1. Inicie sesión en su espacio de trabajo especificando su dirección URL de [!DNL Slack] y haciendo clic en **[!UICONTROL Continuar]**.\

1. Examine el acceso que [!DNL Slack] solicita. Si acepta este acceso, haga clic en **[!UICONTROL Permitir acceso]** para autorizar la aplicación [!DNL Workfront].

Ahora puede tener acceso a [!DNL Workfront] desde [!DNL Slack], tal como se describe en el [Acceso [!DNL Workfront] desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### Instalar la aplicación [!DNL Workfront] en [!DNL Slack] {#install-the-workfront-app-within-slack}

Puede instalar la aplicación [!DNL Workfront] directamente desde la aplicación [!DNL Slack]:

1. Vaya a la dirección URL [!DNL Slack].

   Por ejemplo: *`<YourTeamName>`.slack.com/apps*.

   O

   Haga clic en el icono **[!UICONTROL Añadir aplicaciones]** de su instancia de [!DNL Slack].

1. Empiece a escribir *[!DNL Workfront]* en el campo de búsqueda.
1. Pulse Intro.
1. Seleccione la aplicación **[!DNL Workfront]**.
1. Haga clic en **[!UICONTROL Configuración]**.

   Se muestra la página del Directorio de aplicaciones.

1. Haga clic en **[!UICONTROL Visitar sitio de aplicaciones]**.
1. Haga clic en **[!UICONTROL Añadir a[!DNL Slack]]**.
1. Siga los pasos para finalizar la instalación.
1. Cuando finalice la instalación, puede obtener acceso a [!DNL Workfront] desde [!DNL Slack], tal como se describe en [[!UICONTROL Access] [!DNL Workfront] desde [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
