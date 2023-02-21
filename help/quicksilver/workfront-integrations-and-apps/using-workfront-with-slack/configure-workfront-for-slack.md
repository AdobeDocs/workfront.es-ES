---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Configurar [!DNL Adobe Workfront] para Slack
description: Integración [!DNL Adobe Workfront] con Slack le permite acceder a y crear [!DNL Workfront] elementos de trabajo, aprobaciones, favoritos, elementos recientes del Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Configurar [!DNL Adobe Workfront for Slack]

Integración [!DNL Adobe Workfront] con [!DNL Slack] le permite hacer lo siguiente:

* Acceda a su [!DNL Workfront] elementos de trabajo, aprobaciones, favoritos, elementos recientes de [!DNL Slack].
* Suscribirse, aprobar, asignar trabajo de [!DNL Slack].
* Crear tareas y problemas desde [!DNL Slack].
* Reciba algunas [!DNL Workfront] notificaciones en [!DNL Slack].

Dependiendo de cómo [!DNL Slack] está configurado, puede instalar y configurar [!DNL Workfront for Slack] usted mismo o su [!DNL Workfront] administrador debe instalarlo y configurarlo primero para poder configurarlo por su cuenta.

Al integrar su [!DNL Slack] instancia con [!DNL Workfront] los usuarios pueden utilizar [!DNL Workfront] mientras colabora dentro de sus [!DNL Slack] canales. La integración se puede utilizar desde cualquier [!DNL Slack] entorno, incluido el [!DNL Slack] aplicación móvil.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.\

## Requisitos previos para utilizar [!DNL Workfront] con [!DNL Slack]

* Debe tener un [!DNL Slack] instancia.
* Su [!DNL Slack] el administrador del sistema debe permitir todo [!DNL Slack] usuarios para instalar [!DNL Workfront for Slack].
* Debe tener un [!DNL Workfront] para poder utilizar las funciones integradas de [!DNL Workfront].

   >[!NOTE]
   >
   >Usuarios con cualquier [!DNL Workfront] el tipo de licencia puede acceder [!DNL Workfront] from [!DNL Slack]. Las acciones que puede realizar desde [!DNL Slack] están limitados a [!DNL Workfront] niveles de licencia y permiso.

Para obtener más información sobre la administración de aplicaciones en [!DNL Slack], consulte [Administrar aplicaciones para su espacio de trabajo.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Instalar [!DNL Workfront for Slack]

Cada [!DNL Slack] El usuario debe instalar la variable [!DNL Workfront] para usar [!DNL Workfront] from [!DNL Slack].

Puede instalar la aplicación de las siguientes maneras:

* [Instale el [!DNL Workfront] aplicación externa [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Instale el [!DNL Workfront] aplicación en [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Instale el [!DNL Workfront] aplicación externa [!DNL Slack] {#install-the-workfront-app-outside-slack}

Siga los pasos a continuación para ejecutar el proceso de instalación y autorizar [!DNL Workfront for Slack] en su [!DNL Slack] instancia.

>[!IMPORTANT]
>
>Cuando una nueva versión de [!DNL Workfront] para que Slack esté disponible, debe volver a autorizar la aplicación para poder seguir utilizándola.

1. Busque la variable [!DNL Adobe Workfront] en el [[!DNL Slack] almacenar](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Haga clic en **[!UICONTROL Abrir en[!DNL Slack]]**.

1. Inicie sesión en su espacio de trabajo especificando su [!DNL Slack] URL y clic **[!UICONTROL Continuar]**.\

1. Examine el acceso que [!DNL Slack] solicita. Si acepta este acceso, haga clic en **[!UICONTROL Permitir acceso]** para autorizar [!DNL Workfront] aplicación.

Ahora puede acceder a [!DNL Workfront] from [!DNL Slack], tal como se describe en la sección [Acceso [!DNL Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### Instale el [!DNL Workfront] aplicación en [!DNL Slack] {#install-the-workfront-app-within-slack}

Puede instalar el [!DNL Workfront] directamente desde la [!DNL Slack] aplicación:

1. Vaya a la [!DNL Slack] URL.

   Por ejemplo: *`<YourTeamName>`.slack.com/apps*.

   O

   Haga clic en el **[!UICONTROL Agregar aplicaciones]** en su [!DNL Slack] instancia.

1. Empezar a escribir *[!DNL Workfront]* en el campo de búsqueda.
1. Pulse Intro.
1. Seleccione el **[!DNL Workfront]** aplicación.
1. Haga clic en **[!UICONTROL Configuración]**.

   Se muestra la página Directorio de aplicaciones .

1. Haga clic en **[!UICONTROL Visite el sitio de la aplicación]**.
1. Haga clic en **[!UICONTROL Agregar a[!DNL Slack]]**.
1. Siga los pasos para finalizar la instalación.
1. Cuando finalice la instalación, puede acceder a [!DNL Workfront] from [!DNL Slack], tal como se describe en la sección [[!UICONTROL Acceso [!DNL Workfront] from [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
