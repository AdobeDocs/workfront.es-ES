---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-microsoft-teams
title: Instalar [!DNL Adobe Workfront] para Microsoft Teams
description: La aplicación  [!DNL Adobe Workfront for Microsoft Teams] te permite realizar acciones básicas en [!DNL Workfront] sin salir de los canales de chat de [!DNL Microsoft Teams] i.
author: Becky
feature: Workfront Integrations and Apps
exl-id: a8d4e48c-1ccc-4e6e-a0a0-9b68748590c0
source-git-commit: 69fdb5c23bb501fc81e4ef3c3ab7c94e78e69d29
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 17%

---

# Instalar [!DNL Adobe Workfront] para Microsoft Teams

<!-- Audited: 1/2024 -->

<!--

>[!IMPORTANT]
>
>As of July 1, 2025, Microsoft will remove support for the Classic Teams desktop app. As a result, the Workfront integration with Microsoft Teams will not be supported after the Classic Teams desktop app is no longer available.

-->


La aplicación [!DNL Adobe Workfront for Microsoft Teams] le permite realizar acciones básicas en [!DNL Workfront] sin salir de los canales de chat de [!DNL Microsoft Teams].

>[!NOTE]
>
>[!DNL Microsoft Teams] ya no admite [!DNL Internet Explorer]. Para usar [!DNL Adobe Workfront for Microsoft Teams integration], debe usar un explorador web que no sea [!DNL Internet Explorer].


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
    <p>Actual: [!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Debe ser propietario de equipo en [!DNL Microsoft Teams] para instalar [!DNL Workfront] para [!DNL Microsoft Teams].

## Instalar [!DNL Workfront for Microsoft Teams]

Como propietario de equipo en [!DNL Microsoft Teams], puede instalar la aplicación [!DNL Workfront for Microsoft Teams] para cada uno de sus equipos desde la tienda [!DNL Microsoft] o desde un archivo proporcionado por [!DNL Workfront].

### Instalar [!DNL Workfront for Microsoft Teams] desde el almacén [!DNL Microsoft]

1. Inicie sesión en [!DNL Microsoft Teams] como propietario del equipo.
1. Seleccione el equipo en el que desea instalar la aplicación [!DNL Workfront for Microsoft Teams].
1. Haga clic en **[!UICONTROL Almacenar]** en la barra de navegación lateral.

1. En el cuadro **[!UICONTROL Buscar todos]**, escriba *[!DNL Workfront]*.

1. Haga clic en la tarjeta **[!DNL Workfront]** y siga las instrucciones del asistente.
1. (Recomendado) Seleccione un equipo del menú desplegable **[!UICONTROL Agregar a un equipo]** y habilite la opción **[!UICONTROL Sí]** para agregar la aplicación a un equipo.

   ![ms_team_add_to_a_team_option.png](assets/ms-teams-add-to-a-team-option-350x122.png)

1. Para el canal, selecciona **[!UICONTROL General]** para usar la aplicación en ese canal para el equipo seleccionado y, a continuación, haz clic en **[!UICONTROL Configurar]** para las funciones que desees.

1. Una vez finalizada la instalación, aparecerá una notificación que indica que la instalación se ha realizado correctamente en el canal [!UICONTROL General] del equipo seleccionado. Todos los miembros del equipo pueden ver esta notificación.
1. (Opcional) Anclar la aplicación [!DNL Workfront] para facilitar el acceso:

   1. Haga clic en el icono **[!UICONTROL Más]** bajo el campo de mensaje en el canal [!UICONTROL General].

   1. Pase el cursor sobre la aplicación [!DNL Workfront] en la lista, luego haga clic en el icono **[!UICONTROL Más]** a su derecha.

   1. Haga clic en **[!UICONTROL Fijar]**.

      Esto agrega un icono [!DNL Workfront] debajo del campo de chat. Puede acceder rápidamente al área [!UICONTROL Buscar] desde aquí.

      Para obtener información sobre la búsqueda de [!DNL Workfront] elementos, consulte [Search y compartir [!DNL Adobe Workfront] elementos en [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md).

1. Haga clic **[!UICONTROL en Iniciar sesión para acceder [!DNL Workfront from Microsoft Teams]a[!DNL Workfront]]** .

   Para obtener información sobre registro en [!DNL Workfront], consulte la [sección Iniciar sesión en Workfront desde Microsoft Teams](#log-in-to-workfront-from-microsoft-teams) de este artículo.

### Instalar [!DNL Workfront for Microsoft Teams] desde un archivo privado

Si su organización restringe el acceso a la descarga de aplicaciones de la tienda [!DNL Microsoft], debe ponerse en contacto con nuestro equipo de soporte técnico y solicitar un archivo privado de la aplicación [!DNL Workfront for Microsoft Teams] para instalar la aplicación.

Para obtener información sobre cómo comunicarse con nuestro Equipo de soporte, consulte [Póngase en contacto con el servicio de atención al cliente](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

Para instalar [!DNL Workfront for Microsoft Teams] desde un archivo privado:

1. Guarde el archivo privado que recibió de [!DNL Workfront] en el equipo.
1. Inicie sesión en [!DNL Microsoft Teams] como propietario de equipo de [!DNL Microsoft].
1. Haga clic en el icono **[!UICONTROL Más]** del equipo en el que desea instalar [!DNL Workfront for Microsoft Teams].

1. Haz clic en **[!UICONTROL Administrar equipo]**.
1. Seleccione la ficha **[!UICONTROL Aplicaciones]** y, a continuación, haga clic en **[!UICONTROL Cargar una aplicación personalizada]** en la esquina inferior derecha de la pantalla.

1. Busque el archivo privado que guardó en el equipo y siga los pasos de instalación para instalar [!DNL Workfront for Microsoft Teams].
1. Cuando finaliza la instalación, aparece una notificación que indica que la instalación se ha realizado correctamente en el canal General del equipo seleccionado. Todos los miembros del equipo pueden ver esta notificación.
1. (Opcional) Haga clic en el icono **[!UICONTROL Más]** (tres puntos) bajo el campo **[!UICONTROL Escriba sus preguntas aquí]**.

1. (Opcional) Pase el cursor sobre la aplicación [!DNL Workfront] en la lista, luego haga clic en el icono **[!UICONTROL Más]** a su derecha.

1. (Opcional) Haga Clic En **[!UICONTROL Fijar]**.

   Esto agrega un icono [!DNL Workfront] bajo el campo [!UICONTROL Escriba sus preguntas aquí]. Puede acceder rápidamente al [!UICONTROL área de Search] desde aquí.\
   Para obtener información sobre la búsqueda de elementos de Workfront, consulte [Search y compartir [!DNL Adobe Workfront] elementos en [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md).

## Iniciar sesión en [!DNL Workfront] desde [!DNL Microsoft] equipos

Como propietario de equipo de [!DNL Microsoft Teams], debe instalar la aplicación [!DNL Workfront for Microsoft Teams] para su equipo antes de que usted o cualquier miembro del equipo pueda iniciar sesión en [!DNL Workfront from Microsoft Teams].

Cuando haya iniciado sesión en [!DNL Workfront] desde [!DNL Microsoft Teams], puede recibir [!DNL Workfront] notificaciones en el canal de bots [!DNL Workfront] o puede realizar ciertas acciones en [!DNL Workfront] desde [!DNL Microsoft Teams].

Para obtener información sobre cómo instalar la aplicación [!DNL Workfront], consulte la sección [Instalar [!DNL Workfront for Microsoft Teams]](#install-workfront-for-microsoft-teams) en este artículo.

Para obtener información sobre cómo obtener acceso a [!DNL Workfront] desde [!DNL Microsoft Teams] para realizar determinadas acciones, consulte [Obtener acceso [!DNL Adobe Workfront] desde [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/access-workfront-from-ms-teams.md).

Para iniciar sesión en [!DNL Workfront] desde [!DNL Microsoft Teams]:

1. Vaya al canal **[!UICONTROL General]** del equipo donde se ha instalado la aplicación [!DNL Workfront for Microsoft Teams] y haga clic en **[!UICONTROL Iniciar sesión en Workfront]**.

   El canal de chat de bots [!DNL Workfront] se ha agregado a sus [!DNL Microsoft Teams] canales de chat.

1. Vaya al canal de chat de bots [!DNL Workfront] en [!DNL Microsoft Teams] y escriba *[!UICONTROL iniciar sesión]* en el campo **[!UICONTROL Escriba sus preguntas aquí]**.

   O

   Haga clic en **[!UICONTROL Iniciar sesión]**.

   Se abre una nueva pestaña del explorador.

1. Sigue las indicaciones para iniciar sesión en [!DNL Workfront] utilizando la Autenticación Mejorada, OAuth 2.0 o tu URL de Security Assertion Markup Language (SAML).

   >[!NOTE]
   >
   >* Cuando se le pida que introduzca el dominio de su cuenta de [!DNL Workfront], escríbalo con este formato: *eldominiodesucompañía.my.workfront.com*. El dominio de su empresa suele ser el nombre de su empresa.
   >* La autenticación mejorada no está disponible hasta que un administrador de [!DNL Workfront] la habilite para esta integración.


1. Cierre la ficha del explorador que utilizó para iniciar sesión y vuelva a [!DNL Microsoft Teams].

   Aparece una notificación en el canal de chat de bots [!DNL Workfront] para confirmar que ha iniciado sesión en [!DNL Workfront] correctamente.
