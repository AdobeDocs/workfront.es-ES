---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-microsoft-teams
title: Instalar [!DNL Adobe Workfront] para Microsofts Teams
description: El [!DNL Adobe Workfront for Microsoft Teams] La aplicación de le permite realizar acciones básicas en [!DNL Workfront] sin salir de su [!DNL Microsoft Teams] canales de chat.
author: Becky
feature: Workfront Integrations and Apps
exl-id: a8d4e48c-1ccc-4e6e-a0a0-9b68748590c0
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---

# Instalar [!DNL Adobe Workfront] para Microsofts Teams

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>Actualmente, la integración de Adobe Workfront para Microsoft Teams solo es compatible con la experiencia clásica de Microsoft Teams.


El [!DNL Adobe Workfront for Microsoft Teams] La aplicación de le permite realizar acciones básicas en [!DNL Workfront] sin salir de su [!DNL Microsoft Teams] canales de chat.

>[!NOTE]
>
>[!DNL Microsoft Teams] ya no es compatible [!DNL Internet Explorer]. Para usar la variable [!DNL Adobe Workfront for Microsoft Teams integration], debe utilizar un explorador web distinto de [!DNL Internet Explorer].


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Nuevo: estándar</p>
    <p>Actual: [!UICONTROL Trabajo], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Debe ser el propietario de un equipo en [!DNL Microsoft Teams] para instalar [!DNL Workfront] para [!DNL Microsoft Teams].

## Instalar [!DNL Workfront for Microsoft Teams]

Como propietario de equipo en [!DNL Microsoft Teams], puede instalar el [!DNL Workfront for Microsoft Teams] aplicación para cada uno de sus equipos desde el [!DNL Microsoft] Almacenar o a partir de un archivo proporcionado por [!DNL Workfront].

### Instalar [!DNL Workfront for Microsoft Teams] desde el [!DNL Microsoft] Almacenar

1. Iniciar sesión en [!DNL Microsoft Teams] como propietario de un equipo.
1. Seleccione el equipo para el que desea instalar el [!DNL Workfront for Microsoft Teams] aplicación.
1. Clic **[!UICONTROL Almacenar]** en la barra de navegación lateral.

1. En el **[!UICONTROL Buscar todos]** cuadro, tipo *[!DNL Workfront]*.

1. Haga clic en **[!DNL Workfront]** y siga las instrucciones del asistente.
1. (Recomendado) Seleccione un equipo del **[!UICONTROL Añadir a un equipo]** menú desplegable y habilite la variable **[!UICONTROL Sí]** opción para agregar la aplicación a un equipo.

   ![ms_team_add_to_a_team_option.png](assets/ms-teams-add-to-a-team-option-350x122.png)

1. Para el canal, seleccione **[!UICONTROL General]** para usar la aplicación en ese canal para el equipo seleccionado, haga clic en **[!UICONTROL Configuración de]** para las funciones que desee.

1. Cuando finaliza la instalación, aparece una notificación que indica que la instalación se ha realizado correctamente en la [!UICONTROL General] canal del equipo seleccionado. Todos los miembros del equipo pueden ver esta notificación.
1. (Opcional) Fije el [!DNL Workfront] aplicación para un acceso más fácil:

   1. Haga clic en **[!UICONTROL Más]** icono debajo del campo de mensaje en la [!UICONTROL General] canal.

   1. Pase el ratón sobre [!DNL Workfront] aplicación en la lista y, a continuación, haga clic en **[!UICONTROL Más]** a la derecha de la imagen.

   1. Clic **[!UICONTROL Fijar]**.

      Esto añade un [!DNL Workfront] en el campo chat. Puede acceder rápidamente a la [!UICONTROL Buscar] área de aquí.

      Para obtener información acerca de la búsqueda de [!DNL Workfront] elementos, consulte [Buscar y compartir [!DNL Adobe Workfront] elementos en [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md).

1. Clic **[!UICONTROL Iniciar sesión en[!DNL Workfront]]** para acceder a [!DNL Workfront from Microsoft Teams].

   Para obtener información sobre cómo iniciar sesión en [!DNL Workfront], consulte la [Inicie sesión en Workfront desde Microsoft Teams](#log-in-to-workfront-from-microsoft-teams) de este artículo.

### Instalar [!DNL Workfront for Microsoft Teams] desde un archivo privado

Si su organización restringe el acceso a la descarga de aplicaciones desde el [!DNL Microsoft] Almacén, debe ponerse en contacto con nuestro Equipo de Soporte y solicitar un archivo privado del [!DNL Workfront for Microsoft Teams] para instalar la aplicación.

Para obtener información sobre cómo ponerse en contacto con nuestro Equipo de soporte, consulte [Contactar con Atención al cliente](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

Para instalar [!DNL Workfront for Microsoft Teams] desde un archivo privado:

1. Guarde el archivo privado recibido de [!DNL Workfront] en el equipo.
1. Iniciar sesión en [!DNL Microsoft Teams] as a [!DNL Microsoft] propietario del equipo.
1. Haga clic en **[!UICONTROL Más]** icono del equipo para el que desea realizar la instalación [!DNL Workfront for Microsoft Teams].

1. Clic **[!UICONTROL Administrar equipo]**.
1. Seleccione el **[!UICONTROL Aplicaciones]** y haga clic en **[!UICONTROL Cargar una aplicación personalizada]** en la esquina inferior derecha de la pantalla.

1. Busque el archivo privado que guardó en el equipo y siga los pasos de instalación para instalar [!DNL Workfront for Microsoft Teams].
1. Cuando finaliza la instalación, aparece una notificación que indica que la instalación se ha realizado correctamente en el canal General del equipo seleccionado. Todos los miembros del equipo pueden ver esta notificación.
1. (Opcional) Haga clic en **[!UICONTROL Más]** Icono (tres puntos) debajo de **[!UICONTROL Escriba sus preguntas aquí]** field.

1. (Opcional) Pase el ratón sobre [!DNL Workfront] aplicación en la lista y, a continuación, haga clic en **[!UICONTROL Más]** a la derecha de la imagen.

1. (Opcional) Haga clic en **[!UICONTROL Fijar]**.

   Esto añade un [!DNL Workfront] bajo el icono [!UICONTROL Escriba sus preguntas aquí] field. Puede acceder rápidamente a la [!UICONTROL Buscar] área de aquí.\
   Para obtener información sobre la búsqueda de elementos de Workfront, consulte [Buscar y compartir [!DNL Adobe Workfront] elementos en [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md).

## Iniciar sesión en [!DNL Workfront] de [!DNL Microsoft] Equipos

As a [!DNL Microsoft Teams] propietario del equipo, debe instalar el [!DNL Workfront for Microsoft Teams] aplicación para su equipo antes de que usted o cualquier miembro del equipo pueda iniciar sesión en [!DNL Workfront from Microsoft Teams].

Cuando haya iniciado sesión en [!DNL Workfront] de [!DNL Microsoft Teams], puede recibir [!DNL Workfront] notificaciones en la [!DNL Workfront] canal de bots o puede realizar determinadas acciones en [!DNL Workfront] de [!DNL Microsoft Teams].

Para obtener información acerca de la instalación de [!DNL Workfront] aplicación, consulte la [Instalar [!DNL Workfront for Microsoft Teams]](#install-workfront-for-microsoft-teams) de este artículo.

Para obtener información sobre el acceso [!DNL Workfront] de [!DNL Microsoft Teams] para realizar determinadas acciones, consulte [Acceso [!DNL Adobe Workfront] de [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/access-workfront-from-ms-teams.md).

Para iniciar sesión en [!DNL Workfront] de [!DNL Microsoft Teams]:

1. Vaya a la **[!UICONTROL General]** canal del equipo donde se [!DNL Workfront for Microsoft Teams] La aplicación se ha instalado y haga clic en **[!UICONTROL Iniciar sesión en Workfront]**.

   El [!DNL Workfront] el canal de chat de bots se agrega a su [!DNL Microsoft Teams] canales de chat.

1. Vaya a la [!DNL Workfront] canal de chat de bots en [!DNL Microsoft Teams] y tipo *[!UICONTROL iniciar sesión]* en el **[!UICONTROL Escriba sus preguntas aquí]** field.

   O

   Clic **[!UICONTROL Iniciar sesión]**.

   Se abre una nueva pestaña del explorador.

1. Siga las indicaciones para iniciar sesión en [!DNL Workfront] mediante la autenticación mejorada, OAuth 2.0 o su URL de lenguaje de marcado de aserción de seguridad (SAML).

   >[!NOTE]
   >
   >* Cuando se le pida que introduzca el dominio de su [!DNL Workfront] , escríbalo con este formato: *yourCompany&#39;sDomain.my.workfront.com*. El dominio de su empresa suele ser el nombre de su empresa.
   >* La autenticación mejorada no está disponible hasta que [!DNL Workfront] El administrador lo habilita para esta integración.


1. Cierre la pestaña del explorador que utilizó para iniciar sesión y volver a [!DNL Microsoft Teams].

   Se muestra una notificación en la [!DNL Workfront] canal de chat de bot para confirmar que ha iniciado sesión en [!DNL Workfront] correctamente.
