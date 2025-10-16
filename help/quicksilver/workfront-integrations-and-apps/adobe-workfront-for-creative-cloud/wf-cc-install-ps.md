---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Instalar y abrir  [!DNL Adobe Workfront for Photoshop]
description: Puede instalar el complemento de Adobe Workfront para Photoshop desde Adobe Marketplace.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: f5e9f121-a711-4b75-8564-54f29c5cfa48
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 97%

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
  <!--<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td>Any</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> 
   <p>Standard</p>
   <p>Work or higher</p> </td> 
  </tr> -->
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
1. Lea la información del cuadro de diálogo y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

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
   > * Si la instancia de Workfront está integrada con Experience Cloud, pídale a su administrador que le proporcione el dominio de Workfront que se encuentra en Product > Workfront en el Admin Console.

1. En el explorador, introduzca sus credenciales de [!DNL Workfront] y haga clic en **[!UICONTROL Iniciar sesión]**. Si su empresa utiliza un inicio de sesión único (SSO), se le redirigirá a la página de su proveedor de SSO para iniciar sesión.

   >[!NOTE]
   >
   >Es posible que no se le pida que introduzca sus credenciales de [!DNL Workfront] si ha iniciado sesión recientemente.

   Siga las indicaciones para iniciar sesión en [!DNL Workfront].

   >[!NOTE]
   >
   >* [!DNL Workfront] se conecta a [!DNL Adobe Creative Cloud] mediante OAuth 2.0, un estándar seguro utilizado por la mayoría de las integraciones basadas en la web para la autenticación y autorización de usuarios.
   >* Cuando se le pida que introduzca el [dominio o host] de su cuenta de [!DNL Workfront], escríbalo con este formato: *yourCompany&#39;sDomain.my.workfront.com*. El dominio de su empresa suele ser el nombre de su empresa.

1. Haga clic en **[!UICONTROL Allow Access]** para finalizar el inicio de sesión.
1. Vuelva a [!UICONTROL Adobe Photoshop] para ver su trabajo.
