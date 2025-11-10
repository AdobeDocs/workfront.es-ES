---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Instalar y abrir  [!DNL Adobe Workfront for Photoshop]
description: Puede instalar el complemento de Adobe Workfront para Photoshop desde Adobe Marketplace.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: f5e9f121-a711-4b75-8564-54f29c5cfa48
source-git-commit: 61e5b763ec527aeb846e975e06842dc2c4c69918
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 71%

---

# Instalar y abrir [!DNL Adobe Workfront for Photoshop]

Puede instalar el complemento de [!DNL Adobe Workfront for Photoshop] desde [!DNL Adobe Marketplace]. El complemento es compatible con los siguientes idiomas:

* Inglés
* Francés
* Alemán
* Italiano
* Español
* Portugués
* Japonés
* Chino simplificado
* Chino tradicional
* Coreano

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Productos adicionales</td> 
   <td><p>Debe tener una licencia [!DNL Adobe Creative Cloud] además de una licencia [!DNL Workfront].</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

* Debe instalar previamente la aplicación [!DNL Adobe Photoshop]para poder instalar el complemento de [!DNL Workfront].

## Instalación del el complemento de [!DNL Adobe Workfront for Photoshop] para su organización

Si es administrador de [!DNL Adobe Admin Console], puede incluir el complemento en paquetes de implementación de [!DNL Creative Cloud]. Para obtener más información, consulte [Inclusión de complementos en el paquete](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html).

[Ver un tutorial de vídeo aquí](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}.

Los administradores de [!DNL Adobe Admin Console] también pueden crear paquetes de solo complemento para distribuirlos a los usuarios. Para obtener más información, consulte [Creación de [!UICONTROL [!DNL Adobe Workfront]  para paquetes de  [!DNL Creative Cloud]]  para los usuarios en  [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)

## Instalación del complemento de [!DNL Adobe Workfront for Photoshop] individualmente

Puede instalar el complemento de [!DNL Adobe Workfront for Photoshop] usted mismo desde [!DNL Adobe Exchange].

1. Vaya a la [página de instalación de Adobe Workfront para Photoshop](https://adobe.com/go/cc_plugins_discover_plugin?pluginId=37722a55&workflow=share) en Adobe Exchange.
1. En el cuadro de diálogo que aparece, haga clic en **Abrir la aplicación de escritorio de [!DNL Adobe Creative Cloud]**.
1. Una vez que se abra el administrador de complementos de [!DNL Adobe Photoshop], haga clic en **[!UICONTROL Instalar]**.
1. Lea la información del cuadro de diálogo, haga clic en **[!UICONTROL Aceptar]** y siga las instrucciones que aparezcan en pantalla para completar la instalación.

1. Continúe en la siguiente sección para obtener información sobre cómo abrir el complemento.

## Abrir el complemento de [!DNL Adobe Workfront for Photoshop]

1. Abra [!DNL Photoshop].

1. Cree un nuevo archivo o abra uno existente.

1. En el menú superior, haga clic en **[!UICONTROL Complementos]** > **[!UICONTROL Panel de complementos]**.

   ![Panel de complementos](assets/plugins-panel-ps.png)

1. En el **[!UICONTROL Panel de complementos]**, elija la pestaña **[!UICONTROL Complementos]** y busque **[!UICONTROL Workfront para Adobe Photoshop]**.

   >[!TIP]
   >
   >   Si no ve el complemento después de abrirlo desde el [!UICONTROL Panel de complementos], podría estar detrás de la aplicación de Photoshop. Intente minimizar Photoshop para encontrar el complemento.

1. Continúe en la siguiente sección para obtener información sobre cómo iniciar sesión en el complemento.

## Inicie sesión en [!DNL Adobe Workfront for Photoshop].

1. En el menú **[!UICONTROL Complementos]** de la parte superior de la pantalla, seleccione **[!UICONTROL Panel de complementos]**.
1. Seleccionar **[!DNL Adobe Workfront for Photoshop]**.
1. Introduzca su dominio y haga clic en **[!UICONTROL Log in]**. Se abre una página del explorador. Es posible que tenga que dar permiso a Photoshop para abrir el explorador.

   >[!TIP]
   >
   >* Para encontrar el dominio, abra un explorador, vaya a la instancia [!DNL Workfront] y copie la primera parte de la dirección URL:\
   >![Localizar dominio](assets/domain-350x50.png)
   >
   >* Si la instancia de Workfront está integrada con Experience Cloud y el dominio comienza por `experience.adobe.com`, pídale al administrador que le proporcione el dominio de Workfront que se encuentra en Producto > Workfront en Admin Console.

1. En el explorador, introduzca sus credenciales de [!DNL Adobe] y haga clic en **[!UICONTROL Iniciar sesión]**. Si su empresa utiliza un inicio de sesión único (SSO), se le redirigirá a la página de su proveedor de SSO para iniciar sesión.

   >[!NOTE]
   >
   >Es posible que no se le pida que introduzca sus credenciales de [!DNL Workfront] si ha iniciado sesión recientemente.

1. Siga las indicaciones para iniciar sesión en [!DNL Workfront].

   >[!NOTE]
   >
   >* [!DNL Workfront] se conecta a [!DNL Adobe Creative Cloud] mediante OAuth 2.0, un estándar seguro utilizado por la mayoría de las integraciones basadas en la web para la autenticación y autorización de usuarios.


1. Haga clic en **[!UICONTROL Allow Access]** para finalizar el inicio de sesión.
1. Vuelva a [!UICONTROL Adobe Photoshop] para ver su trabajo.

### Solución de problemas de inicio de sesión

**Aparece el error &quot;Se produjo un error&quot; al intentar iniciar sesión**


No puede usar una dirección URL que comience por `experience.adobe.com` para iniciar sesión en el complemento.

![error de inicio de sesión](assets/plugin-log-in-error.png) ![dominio](assets/incorrect-domain.png)


Para solucionar este problema,

1. Elimine la carpeta que almacena el dominio del complemento.

   >[!TIP]
   >
   >En un Mac, vaya a Finder y presione **Comando+Mayús+.** para mostrar las carpetas ocultas, vaya a **/Usuarios//Biblioteca/Compatibilidad con la aplicación** y, a continuación, elimine la carpeta **Workfront**.


1. Vuelva al complemento e introduzca su dominio de Workfront. El dominio debe ser `company-name.my.workfront.com` y no `experience.adobe.com`.

   Para [encontrar tu dominio de Workfront](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md) si estás en la experiencia unificada de Adobe, ve a Configuración, Información del cliente.
