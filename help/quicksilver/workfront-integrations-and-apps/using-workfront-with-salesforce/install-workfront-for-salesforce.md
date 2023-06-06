---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Instalar [!DNL Adobe Workfront] para [!DNL Salesforce]
description: Para instalar la aplicación antes de que esté disponible en el [!DNL Salesforce] AppExchange, consulte Instalación [!DNL Workfront] para Salesforce antes de que esté disponible en AppExchange Marketplace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: 0c49ab99653f390d592bba39bcb92145b8bedd0c
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 1%

---

# Instalar [!DNL Adobe Workfront for Salesforce]

Para instalar la aplicación antes de que esté disponible en el [!DNL Salesforce AppExchange], consulte [Instalación [!DNL Workfront for Salesforce] antes de que esté disponible en la [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

As a [!DNL Salesforce] y [!DNL Adobe Workfront] administrador, puede instalar [!DNL Workfront for Salesforce] para permitir su [!DNL Salesforce] usuarios que enviar [!DNL Workfront] solicita y crea automáticamente proyectos sin salir de Salesforce.

Para obtener una visión general de lo que puede esperar al instalar [!DNL Workfront for Salesforce], consulte [[!DNL Adobe Workfront for Salesforce] descripción general](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

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

* Debe tener un [!DNL Salesforce] instancia de con acceso a una cuenta de administrador del sistema para instalar la aplicación.
* Debe tener un [!DNL Workfront] instancia de con acceso a una cuenta de administrador del sistema para configurar la integración.
* [!UICONTROL Salesforce] los usuarios deben tener un [!DNL Workfront] cuenta para poder hacer lo siguiente:

   * Crear [!DNL Workfront] solicitudes de [!DNL Salesforce] o
   * Ver [!DNL Workfront] solicitudes o proyectos en Salesforce.

## Instalación [!DNL Workfrontfor Salesforce] {#installing-workfront-for-salesforce}

Debe ser un [!DNL Salesforce] y una [!DNL Workfront] administrador del sistema para instalar y configurar [!DNL Workfront for Salesforce].

Las siguientes subsecciones describen cómo realizar la instalación [!DNL Workfront] para su [!DNL Salesforce] Entorno de producción. Puede seguir los mismos pasos para instalar [!DNL Workfront] para su [!DNL Salesforce] Entorno de zona protegida.

* [Instalación [!DNL Workfront for Salesforce] antes de que esté disponible en la [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Instalación [!DNL Workfront for Salesforce] en el [!DNL Salesforce Classic] Marco](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Instalación [!DNL Workfront for Salesforce] en el [!DNL Salesforce Lightning Experience] Marco](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Instalación [!DNL Workfront for Salesforce] antes de que esté disponible en la [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] estará disponible en el [!DNL Salesforce AppExchange] pronto.

Para instalar la aplicación antes de que esté disponible:

1. En el entorno de producción, vaya a

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   En el entorno de espacio aislado, vaya a

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

1. Compruebe la **[!UICONTROL Sí, conceder acceso a estos sitios web de terceros]** cuadro.

   Aparece una pantalla de carga y la instalación puede tardar unos minutos.

1. Clic **[!UICONTROL Listo]** cuando finalice la instalación.

1. Vaya a **[!UICONTROL Configuración>Controles de seguridad>Configuración del sitio remoto]**.
1. (Condicional) Si no ve su [!DNL Workfront] URL enumerada en **[!UICONTROL Todos los sitios remotos]** , haga clic en **[!UICONTROL Nuevo sitio remoto]**.

1. Especifique el **[!UICONTROL Nombre de sitio remoto]**.

   Por ejemplo, *[!DNL Workfront]*.

1. Especifique el **[!UICONTROL URL del sitio remoto]**.

   Por ejemplo, *yourDomain.my.workfront.com*.

1. Haga clic en **[!UICONTROL Guardar]**.

   El [!DNL Workfront] La aplicación ya está instalada en su [!DNL Salesforce] y la **[!UICONTROL Oportunidades de Workfront]** y **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] Se han creado páginas en su entorno.

   [!DNL Salesforce] Los usuarios de podrán utilizar la aplicación cuando haya añadido el [!DNL Workfront] a su sección [!UICONTROL Oportunidad] o [!UICONTROL Cuenta] diseños de página.\
   Para obtener información sobre cómo configurar la sección de Workfront para los usuarios, consulte [Configuración de la sección Adobe Workfront para usuarios de Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Instalación [!DNL Workfront] para [!DNL Salesforce] en el [!DNL Salesforce Classic] Marco

1. Iniciar sesión en [!DNL Salesforce] como administrador del sistema.
1. Ir a **Configurar.**
1. En el **Generar** , haga clic en **AppExchange Marketplace**.

1. En el **Buscar aplicaciones de AppExchange** cuadro, tipo **Workfront**.

1. Haga clic en la aplicación cuando la encuentre y luego haga clic en **Consíguelo ahora**.
1. Clic **[!UICONTROL Instalar en producción]** para instalar el [!DNL Workfront] aplicación en su [!DNL Salesforce] Entorno de producción. (recomendado)
1. Seleccione el **[!UICONTROL He leído y acepto los términos y condiciones]** después de haber leído y aceptado los términos y condiciones.
1. Clic **[!UICONTROL Confirmar e instalar]**.
1. Seleccionar **[!UICONTROL Instalar para todos los usuarios]** (recomendado) y haga clic en **[!UICONTROL Instalar]**.

1. (Condicional) Si se le pregunta si desea aprobar un acceso de terceros, debe seleccionar **[!UICONTROL Sí, conceder acceso a estos sitios web de terceros]**, luego haga clic en **[!UICONTROL Continuar]**.

1. Clic **[!UICONTROL Listo]** cuando finalice la instalación.

   El [!DNL Workfront] La aplicación se enumera en **[!UICONTROL Paquetes instalados]**.


1. Vaya a **[!UICONTROL Configuración>Controles de seguridad>Configuración del sitio remoto]**.
1. (Condicional) Si no ve su [!DNL Workfront] URL enumerada en **[!UICONTROL Todos los sitios remotos]** , haga clic en **[!UICONTROL Nuevo sitio remoto]**.\

1. Especifique el **[!UICONTROL Nombre de sitio remoto]**.\
   Por ejemplo, *[!DNL Workfront]*.

1. Especifique el **[!UICONTROL URL del sitio remoto]**.\
   Por ejemplo, *yourDomain.my.workfront.com*.

1. Haga clic en **[!UICONTROL Guardar]**.\
   El [!DNL Workfront] La aplicación ya está instalada en su [!DNL Salesforce] y la **[!UICONTROL Oportunidades de Workfront]** y **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] Se han creado páginas en su entorno.\
   [!DNL Salesforce] Los usuarios de aún no pueden usar la aplicación hasta que agregue el [!DNL Workfront] a su sección [!UICONTROL Oportunidad] o [!UICONTROL Cuenta] diseños de página.\
   Para obtener información sobre la configuración de [!DNL Workfront] para los usuarios, consulte [Configure las variables [!DNL Adobe Workfront] sección para [!DNL Salesforce] usuarios](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Instalación [!DNL Workfront for Salesforce] en el [!DNL Salesforce Lightning Experience] Marco

1. Iniciar sesión en [!DNL Salesforce] como administrador del sistema.
1. Haga clic en **[!UICONTROL Configurar] icono**, luego haga clic en **[!UICONTROL Configurar]**.

1. En el **[!UICONTROL HERRAMIENTAS DE PLATAFORMA]** sección, expandir **[!UICONTROL Aplicaciones].**

1. Haga clic **[!DNL AppExchange Marketplace]**.
1. En el **[!UICONTROL Buscar [!DNL AppExchange] Aplicaciones]** cuadro, tipo **[!DNL Workfront]**.

1. Haga clic en la aplicación cuando la encuentre y luego haga clic en **[!UICONTROL Consíguelo ahora]**.
1. Clic **[!UICONTROL Abrir pantalla de inicio de sesión]**.\
   Debe iniciar sesión con su [!DNL Workfront] cuenta de administrador para [!DNL Salesforce].

1. Clic **[!UICONTROL Permitir]**.
1. En el **[!UICONTROL Instalar en esta organización]** , haga clic en **[!UICONTROL Instalar aquí]** para instalar [!DNL Workfront] en su [!DNL Salesforce] Entorno de producción. (recomendado)

1. Seleccione el **[!UICONTROL He leído y acepto los términos y condiciones]** después de haber leído y aceptado los términos y condiciones.
1. Clic **[!UICONTROL Confirmar e instalar]**.
1. Seleccionar **[!UICONTROL Instalar para todos los usuarios]** (recomendado) y haga clic en **[!UICONTROL Instalar]**.

1. (Condicional) Si se le pregunta si desea aprobar un acceso de terceros, debe seleccionar **[!UICONTROL Sí, conceder acceso a estos sitios web de terceros]**, luego haga clic en **[!UICONTROL Continuar]**.

1. Clic **[!UICONTROL Listo]** cuando finalice la instalación.

   El [!DNL Workfront] La aplicación se enumera en **[!UICONTROL Paquetes instalados]**.

1. Vaya a **[!UICONTROL Configurar].**
1. En el **[!UICONTROL CONFIGURACIÓN]** , expanda&#x200B;**[!UICONTROL Seguridad].**

1. Clic **[!UICONTROL Configuración del sitio remoto]**.
1. (Condicional) Si no ve su [!DNL Workfront] URL enumerada en **[!UICONTROL Todos los sitios remotos]** , haga clic en **[!UICONTROL Nuevo sitio remoto]**.

1. Especifique el **[!UICONTROL Nombre de sitio remoto]**.

   Por ejemplo, *[!DNL Workfront]*.

1. Especifique el **[!UICONTROL URL del sitio remoto]**.

   Por ejemplo, *yourDomain.my.workfront.com*.

1. Haga clic en **[!UICONTROL Guardar]**.

   El [!DNL Workfront] La aplicación ya está instalada en su [!DNL Salesforce] y la variable **[!DNL Workfront]** Este componente ahora se añade al entorno.

   [!UICONTROL Salesforce] Los usuarios de pueden usar el [!DNL Workfront] aplicación una vez que haya añadido el [!DNL Workfront] a su sección [!UICONTROL Oportunidad] o [!UICONTROL Cuenta] diseños de página.\
   Para obtener información sobre la configuración de [!DNL Workfront] para los usuarios, consulte [Configure las variables [!DNL Adobe Workfront] sección para [!DNL Salesforce] usuarios](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
