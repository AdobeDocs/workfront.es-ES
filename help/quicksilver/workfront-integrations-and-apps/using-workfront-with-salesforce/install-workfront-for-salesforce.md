---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Instalar [!DNL Adobe Workfront] para [!DNL Salesforce]
description: Para instalar la aplicación antes de que esté disponible en el [!DNL Salesforce] AppExchange, consulte Instalación [!DNL Workfront] para Salesforce antes de que esté disponible en AppExchange Marketplace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 1%

---

# Instalar [!DNL Adobe Workfront for Salesforce]

Para instalar la aplicación antes de que esté disponible en el [!DNL Salesforce AppExchange], consulte [Instalación [!DNL Workfront for Salesforce] antes de que esté disponible en la [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

Como [!DNL Salesforce] y [!DNL Adobe Workfront] administrador, puede instalar [!DNL Workfront for Salesforce] para permitir que [!DNL Salesforce] usuarios a enviar [!DNL Workfront] solicita y crea proyectos automáticamente sin salir nunca de Salesforce.

Para obtener información general sobre lo que puede esperar instalando [!DNL Workfront for Salesforce], consulte [[!DNL Adobe Workfront for Salesforce] información general](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Requisitos previos para la instalación y el uso [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce-prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Instalación [!DNL Workfront for Salesforce]](#install-adobe-workfront-for-salesforce)

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad descrita en este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos para la instalación y el uso [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* Debe tener un [!DNL Salesforce] con acceso a una cuenta de administrador del sistema para instalar la aplicación.
* Debe tener un [!DNL Workfront] con acceso a una cuenta de administrador del sistema para configurar la integración.
* [!UICONTROL Salesforce] los usuarios deben tener un [!DNL Workfront] para poder

   * Crear [!DNL Workfront] solicitudes de [!DNL Salesforce] o
   * Ver [!DNL Workfront] solicitudes o proyectos en Salesforce.

## Instalación [!DNL Workfrontfor Salesforce] {#installing-workfront-for-salesforce}

Debe ser [!DNL Salesforce] y [!DNL Workfront] administrador del sistema para instalar y configurar [!DNL Workfront for Salesforce].

Las siguientes subsecciones describen cómo instalar [!DNL Workfront] para su [!DNL Salesforce] Entorno de producción. Puede seguir los mismos pasos para instalar [!DNL Workfront] para su [!DNL Salesforce] Entorno de espacio aislado.

* [Instalación [!DNL Workfront for Salesforce] antes de que esté disponible en la [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Instalación [!DNL Workfront for Salesforce] en el [!DNL Salesforce Classic] Marco](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Instalación [!DNL Workfront for Salesforce] en el [!DNL Salesforce Lightning Experience] Marco](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Instalación [!DNL Workfront for Salesforce] antes de que esté disponible en la [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] estará disponible en el [!DNL Salesforce AppExchange] pronto.

Para instalar la aplicación antes de que esté disponible:

1. En el entorno de producción, vaya a

   `https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002aUZY`

   En el entorno de espacio aislado, vaya a

   `https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002aUZY`

1. Marque la **[!UICONTROL Sí, conceder acceso a estos sitios web de terceros]** en la ventana

   Aparece una pantalla de carga y la instalación puede tardar un rato.

1. Haga clic en **[!UICONTROL Listo]** cuando se complete la instalación.

1. Vaya a **[!UICONTROL Configuración>Controles de seguridad>Configuración del sitio remoto]**.
1. (Condicional) Si no ve su [!DNL Workfront] La URL que aparece en la sección **[!UICONTROL Todos los sitios remotos]** lista, haga clic en **[!UICONTROL Nuevo sitio remoto]**.

1. Especifique la variable **[!UICONTROL Nombre del sitio remoto]**.

   Por ejemplo, *[!DNL Workfront]*.

1. Especifique la variable **[!UICONTROL Dirección URL del sitio remoto]**.

   Por ejemplo, *yourDomain.my.workfront.com*.

1. Haga clic en **[!UICONTROL Guardar]**.

   La variable [!DNL Workfront] la aplicación ya está instalada en su [!DNL Salesforce] y **[!UICONTROL Oportunidades del frente de trabajo]** y **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] Las páginas se han creado en su entorno.

   [!DNL Salesforce] los usuarios pueden usar la aplicación una vez que haya agregado la variable [!DNL Workfront] para [!UICONTROL Oportunidad] o [!UICONTROL Cuenta] diseños de página.\
   Para obtener información sobre la configuración de la sección Workfront para usuarios, consulte [Configuración de la sección Adobe Workfront para usuarios de Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Instalación [!DNL Workfront] para [!DNL Salesforce] en el [!DNL Salesforce Classic] Marco

1. Iniciar sesión en [!DNL Salesforce] como administrador del sistema.
1. Vaya a **Configuración.**
1. En el **Generar** , haga clic en **AppExchange Marketplace**.

1. En el **Aplicaciones de AppExchange de búsqueda** cuadro, tipo **Workfront**.

1. Haga clic en la aplicación cuando la encuentre y, a continuación, haga clic en **Get It Now**.
1. Haga clic en **[!UICONTROL Instalar en producción]** para instalar el [!DNL Workfront] en su [!DNL Salesforce] Entorno de producción. (recomendado)
1. Seleccione el **[!UICONTROL He leído y acepto los términos y condiciones]** después de haber leído y aceptado los términos y condiciones.
1. Haga clic en **[!UICONTROL Confirmar e instalar]**.
1. Select **[!UICONTROL Instalar para todos los usuarios]** (recomendado) y, a continuación, haga clic en **[!UICONTROL Instalar]**.

1. (Condicional) Si se le pregunta si desea aprobar un acceso de terceros, debe seleccionar **[!UICONTROL Sí, conceder acceso a estos sitios web de terceros]** y haga clic en **[!UICONTROL Continuar]**.

1. Haga clic en **[!UICONTROL Listo]** cuando se complete la instalación.

   La variable [!DNL Workfront] la aplicación aparece en **[!UICONTROL Paquetes instalados]**.


1. Vaya a **[!UICONTROL Configuración>Controles de seguridad>Configuración del sitio remoto]**.
1. (Condicional) Si no ve su [!DNL Workfront] La URL que aparece en la sección **[!UICONTROL Todos los sitios remotos]** lista, haga clic en **[!UICONTROL Nuevo sitio remoto]**.\

1. Especifique la variable **[!UICONTROL Nombre del sitio remoto]**.\
   Por ejemplo, *[!DNL Workfront]*.

1. Especifique la variable **[!UICONTROL Dirección URL del sitio remoto]**.\
   Por ejemplo, *yourDomain.my.workfront.com*.

1. Haga clic en **[!UICONTROL Guardar]**.\
   La variable [!DNL Workfront] la aplicación ya está instalada en su [!DNL Salesforce] y **[!UICONTROL Oportunidades del frente de trabajo]** y **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] Las páginas se han creado en su entorno.\
   [!DNL Salesforce] los usuarios no podrán usar la aplicación hasta que no agregue la variable [!DNL Workfront] a su [!UICONTROL Oportunidad] o [!UICONTROL Cuenta] diseños de página.\
   Para obtener información sobre cómo configurar la variable [!DNL Workfront] para los usuarios, consulte [Configure las variables [!DNL Adobe Workfront] para [!DNL Salesforce] usuarios](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Instalación [!DNL Workfront for Salesforce] en el [!DNL Salesforce Lightning Experience] Marco

1. Iniciar sesión en [!DNL Salesforce] como administrador del sistema.
1. Haga clic en el **[!UICONTROL Configuración] icono** y haga clic en **[!UICONTROL Configuración]**.

1. En el **[!UICONTROL HERRAMIENTAS DE PLATAFORMA]** sección, expandir **[!UICONTROL Aplicaciones].**

1. Haga clic **[!DNL AppExchange Marketplace]**.
1. En el **[!UICONTROL Buscar [!DNL AppExchange] Aplicaciones]** cuadro, tipo **[!DNL Workfront]**.

1. Haga clic en la aplicación cuando la encuentre y, a continuación, haga clic en **[!UICONTROL Get It Now]**.
1. Haga clic en **[!UICONTROL Abrir pantalla de inicio de sesión]**.\
   Debe iniciar sesión con su [!DNL Workfront] cuenta de administrador para [!DNL Salesforce].

1. Haga clic en **[!UICONTROL Permitir]**.
1. En el **[!UICONTROL Instalar en esta organización]** , haga clic en **[!UICONTROL Instalar aquí]** para instalar [!DNL Workfront] en su [!DNL Salesforce] Entorno de producción. (recomendado)

1. Seleccione el **[!UICONTROL He leído y acepto los términos y condiciones]** después de haber leído y aceptado los términos y condiciones.
1. Haga clic en **[!UICONTROL Confirmar e instalar]**.
1. Select **[!UICONTROL Instalar para todos los usuarios]** (recomendado) y, a continuación, haga clic en **[!UICONTROL Instalar]**.

1. (Condicional) Si se le pregunta si desea aprobar un acceso de terceros, debe seleccionar **[!UICONTROL Sí, conceder acceso a estos sitios web de terceros]** y haga clic en **[!UICONTROL Continuar]**.

1. Haga clic en **[!UICONTROL Listo]** cuando se complete la instalación.

   La variable [!DNL Workfront] la aplicación aparece en **[!UICONTROL Paquetes instalados]**.

1. Vaya a **[!UICONTROL Configuración].**
1. En el **[!UICONTROL CONFIGURACIÓN]** expandir &#x200B;**[!UICONTROL Seguridad].**

1. Haga clic en **[!UICONTROL Configuración del sitio remoto]**.
1. (Condicional) Si no ve su [!DNL Workfront] La URL que aparece en la sección **[!UICONTROL Todos los sitios remotos]** lista, haga clic en **[!UICONTROL Nuevo sitio remoto]**.

1. Especifique la variable **[!UICONTROL Nombre del sitio remoto]**.

   Por ejemplo, *[!DNL Workfront]*.

1. Especifique la variable **[!UICONTROL Dirección URL del sitio remoto]**.

   Por ejemplo, *yourDomain.my.workfront.com*.

1. Haga clic en **[!UICONTROL Guardar]**.

   La variable [!DNL Workfront] la aplicación ya está instalada en su [!DNL Salesforce] y la **[!DNL Workfront]** ahora se añade a su entorno.

   [!UICONTROL Salesforce] los usuarios pueden usar la variable [!DNL Workfront] una vez que haya agregado la variable [!DNL Workfront] a su [!UICONTROL Oportunidad] o [!UICONTROL Cuenta] diseños de página.\
   Para obtener información sobre cómo configurar la variable [!DNL Workfront] para los usuarios, consulte [Configure las variables [!DNL Adobe Workfront] para [!DNL Salesforce] usuarios](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
