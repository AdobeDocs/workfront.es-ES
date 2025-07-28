---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Instalar  [!DNL Adobe Workfront]  para  [!DNL Salesforce]
description: Para instalar la aplicación antes de que esté disponible en AppExchange  [!DNL Salesforce] , consulte Instalar  [!DNL Workfront]  for Salesforce antes de que esté disponible en Marketplace de AppExchange.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '1092'
ht-degree: 92%

---

# Instalar [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>Para ofrecer integraciones más estables y escalables, estamos adoptando un enfoque de integración moderno y flexible mediante la automatización e integración (Fusion) de Workfront. Como parte de este proceso de transición, la integración de Workfront para Salesforce no estará disponible después del **28 de febrero de 2026**.
>
>Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Salesforce.
>
>Para obtener una descripción general de la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obtener información sobre las capacidades específicas de los módulos de integración y automatización de Workfront para Salesforce, consulte [módulos de Salesforce](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Como administrador de [!DNL Salesforce] y [!DNL Adobe Workfront], puede instalar [!DNL Workfront for Salesforce] para permitir que los usuarios de [!DNL Salesforce] envíen solicitudes de [!DNL Workfront] y creen automáticamente proyectos sin salir de Salesforce.

Para obtener información general sobre lo que cabe esperar de la instalación de [!DNL Workfront for Salesforce], consulte [[!DNL Adobe Workfront for Salesforce] información general](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Requisitos previos para instalar y usar  [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Instalando  [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para utilizar la funcionalidad que se describe en este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>Nuevo: [!UICONTROL Standard]</p><p>O</p><p>Actual: [!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos para instalar y usar [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* Debe tener una instancia de [!DNL Salesforce] con acceso a una cuenta de administrador del sistema para instalar la aplicación.
* Debe tener una instancia de [!DNL Workfront] con acceso a una cuenta de administrador del sistema para configurar la integración.
* Los usuarios de [!UICONTROL Salesforce] deben tener una cuenta de [!DNL Workfront] para poder hacer lo siguiente:

   * Crear solicitudes de [!DNL Workfront] a partir de [!DNL Salesforce]
   * Ver solicitudes de [!DNL Workfront] o proyectos en Salesforce

## Instalando [!DNL Workfront for Salesforce]  {#installing-workfront-for-salesforce}

Debe ser administrador del sistema de [!DNL Salesforce] y [!DNL Workfront] para instalar y configurar [!DNL Workfront for Salesforce].

Las siguientes subsecciones describen cómo instalar [!DNL Workfront] para su entorno de producción de [!DNL Salesforce]. Puede seguir los mismos pasos para instalar [!DNL Workfront] en su entorno de zona protegida de [!DNL Salesforce].

* [Instalando  [!DNL Workfront for Salesforce] antes de que esté disponible en  [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Instalando  [!DNL Workfront for Salesforce]  en el marco de trabajo de  [!DNL Salesforce Classic] ](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Instalando  [!DNL Workfront for Salesforce]  en el marco de trabajo de  [!DNL Salesforce Lightning Experience] ](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Instalando [!DNL Workfront for Salesforce] antes de que esté disponible en [!DNL AppExchange]Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] estará disponible próximamente en [!DNL Salesforce AppExchange].

Para instalar la aplicación antes de que esté disponible:

1. En el entorno de producción, vaya a

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   En el entorno de zona protegida, vaya a

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   >[!NOTE]
   >
   >Debe haber iniciado sesión en Salesforce para acceder a estas páginas.

1. Marque el cuadro **[!UICONTROL Sí, conceder acceso a estos sitios web de terceros]**.

   Se muestra una pantalla de carga. La instalación puede tardar unos instantes.

1. Haga clic en **[!UICONTROL Listo]** cuando finalice la instalación.

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Controles de]Seguridad** > **[!UICONTROL Configuración del sitio remoto]**.
1. (Condicional) Seleccione Workfront en la lista.

   O

   Si no ve su URL [!DNL Workfront] en la lista **[!UICONTROL Todos los sitios remotos]**, haga clic en **[!UICONTROL Nuevo sitio remoto]**.

1. (Condicional) Si añade el sitio, especifique el **[!UICONTROL Nombre del sitio remoto]**.

   Por ejemplo, *[!DNL Workfront]*

1. (Condicional) Si añade el sitio, especifique la **[!UICONTROL URL del sitio remoto]**.

   Por ejemplo, *yourDomain.my.workfront.com*.

1. Haga clic en **[!UICONTROL Guardar]**.

   La aplicación [!DNL Workfront] está ahora instalada en su instancia de [!DNL Salesforce], y se han creado las páginas **[!UICONTROL WorkfrontOpportunity]** y **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] en su entorno.

   Los usuarios de [!DNL Salesforce] pueden usar la aplicación una vez que añada la sección de [!DNL Workfront] a sus diseños de página de [!UICONTROL Oportunidad] o [!UICONTROL Cuenta].\
   Para obtener más información sobre cómo configurar la sección de Workfront para los usuarios, consulte [Configurar la sección de Adobe Workfront para los usuarios de Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Instalando [!DNL Workfront] para [!DNL Salesforce] en el marco de [!DNL Salesforce Classic]

1. Inicie sesión en [!DNL Salesforce] como administrador del sistema.
1. Vaya a **Configuración**.
1. En la sección **Generar**, haga clic en **Marketplace de AppExchange**.

1. En el cuadro **Buscar aplicaciones de AppExchange**, escriba **Workfront**.

1. Haga clic en la aplicación de Workfront cuando la encuentre y, a continuación, haga clic en **Obtenerlo ahora**.
1. Haga clic en **[!UICONTROL Instalar en producción]** para instalar la aplicación [!DNL Workfront] en el entorno de producción de [!DNL Salesforce]. (Recomendado)
1. Después de leer y aceptar los términos y condiciones, habilite el campo **[!UICONTROL He leído y acepto los términos y condiciones]**.
1. Haga clic en **[!UICONTROL Confirmar e instalar]**.
1. Seleccione **[!UICONTROL Instalar para todos los usuarios]** (recomendado) y luego haga clic en **[!UICONTROL Instalar]**.

1. (Condicional) Si se le pregunta si desea aprobar el acceso de terceros, debe seleccionar **[!UICONTROL Sí, conceder acceso a estos sitios web de terceros]** y, a continuación, hacer clic en **[!UICONTROL Continuar]**.

1. Haga clic en **[!UICONTROL Listo]** cuando finalice la instalación.

   La aplicación [!DNL Workfront] aparece en **[!UICONTROL Paquetes instalados]**.


1. Vaya a **[!UICONTROL Configuración>Controles de seguridad>Configuración del sitio remoto]**.
1. (Condicional) Si la dirección URL [!DNL Workfront] no aparece en la lista **[!UICONTROL Todos los sitios remotos]**, haga clic en **[!UICONTROL Nuevo sitio remoto]**.

1. (Condicional) Si añade el sitio, especifique el **[!UICONTROL Nombre del sitio remoto]**.
Por ejemplo, *[!DNL Workfront]*.

1. (Condicional) Si añade el sitio, especifique la dirección **[!UICONTROL URL del sitio remoto]**.
Por ejemplo, *yourDomain.my.workfront.com*.

1. Haga clic en **[!UICONTROL Guardar]**.\
   La aplicación [!DNL Workfront] está ahora instalada en su instancia [!DNL Salesforce]. Las páginas **[!UICONTROL WorkfrontOpportunities]** y **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] se han creado en su entorno.\
   Los usuarios de [!DNL Salesforce] todavía no pueden usar la aplicación hasta que añada la sección [!DNL Workfront] a sus diseños de página de [!UICONTROL Oportunidad] o [!UICONTROL Cuenta].\
   Para obtener información sobre cómo configurar la sección [!DNL Workfront] para los usuarios, consulte [Configurar la sección  [!DNL Adobe Workfront] para [!DNL Salesforce] usuarios](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Instalando [!DNL Workfront for Salesforce] en el marco de [!DNL Salesforce Lightning Experience]

1. Inicie sesión en [!DNL Salesforce] como administrador del sistema.
1. Haga clic en el icono **[!UICONTROL Configuración]** y, a continuación, en **[!UICONTROL Configuración]**.

1. En la sección **[!UICONTROL HERRAMIENTAS DE PLATAFORMA]**, expanda **[!UICONTROL Aplicaciones].**

1. Haga clic en **[!DNL AppExchange Marketplace]**.
1. En el cuadro **[!UICONTROL Buscar [!DNL AppExchange] aplicaciones]**, escriba **[!DNL Workfront]**.

1. Haga clic en la aplicación de Workfront cuando la encuentre y, a continuación, haga clic en **Obtenerlo ahora**.
1. Haga clic en **[!UICONTROL Abrir pantalla de inicio de sesión]**.\
   Debe iniciar sesión con su cuenta de administrador de [!DNL Workfront] para [!DNL Salesforce].

1. Haga clic en **[!UICONTROL Aceptar]**.
1. En el cuadro **[!UICONTROL Instalar en esta organización]**, haga clic en **[!UICONTROL Instalar aquí]** para instalar [!DNL Workfront] en su entorno de producción de [!DNL Salesforce]. (Recomendado)

1. Después de leer y aceptar los términos y condiciones, habilite el campo **[!UICONTROL He leído y acepto los términos y condiciones]**.
1. Haga clic en **[!UICONTROL Confirmar e instalar]**.
1. Seleccione **[!UICONTROL Instalar para todos los usuarios]** (recomendado) y luego haga clic en **[!UICONTROL Instalar]**.

1. (Condicional) Si se le pregunta si desea aprobar el acceso de terceros, debe seleccionar **[!UICONTROL Sí, conceder acceso a estos sitios web de terceros]** y, a continuación, hacer clic en **[!UICONTROL Continuar]**.

1. Haga clic en **[!UICONTROL Listo]** cuando finalice la instalación.

   La aplicación [!DNL Workfront] aparece en **[!UICONTROL Paquetes instalados]**.

1. Vaya a **[!UICONTROL Configuración].**
1. En la sección **[!UICONTROL CONFIGURACIÓN]**, expanda **[!UICONTROL Seguridad].**

1. Haga clic en **[!UICONTROL Configuración del sitio remoto]**.
1. (Condicional) Si la dirección URL de [!DNL Workfront] no aparece en la lista **[!UICONTROL Todos los sitios remotos]**, haga clic en **[!UICONTROL Nuevo sitio remoto]**.

1. (Condicional) Si añade el sitio, especifique el **[!UICONTROL Nombre del sitio remoto]**.
Por ejemplo, *[!DNL Workfront]*.

1. (Condicional) Si añade el sitio, especifique la dirección **[!UICONTROL URL del sitio remoto]**.
Por ejemplo, *yourDomain.my.workfront.com*.

1. Haga clic en **[!UICONTROL Guardar]**.

   La aplicación de [!DNL Workfront] se ha instalado en la instancia de [!DNL Salesforce] y el componente **[!DNL Workfront]** se ha añadido al entorno.

   Los usuarios de [!UICONTROL Salesforce] pueden usar la aplicación [!DNL Workfront] una vez que añada la sección [!DNL Workfront] a sus diseños de página [!UICONTROL Oportunidad] o [!UICONTROL Cuenta].\
   Para obtener información sobre cómo configurar la sección [!DNL Workfront] para los usuarios, consulte [Configurar la sección [!DNL Adobe Workfront] para los usuarios de [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Configurar permisos para la integración de Workfront para Salesforce

### Permisos para `workfront_business`

1. Vaya a **Configuración** > **Seguridad** > **URL de confianza**.
1. Seleccione `workfront_business` en la lista.
1. Haga clic en **Editar**.
1. En Directivas CSP, marque las siguientes opciones:

   * connect-src (scripts)
   * font-src (fuentes)
   * frame-src (contenido de iframe)
   * img-src (imágenes)
   * media-src (audio y vídeo)
   * style-src (hojas de estilo)

1. Haga clic en **Guardar**.


### Permisos para workfront_session

1. Vaya a **Configuración** > **Seguridad** > **URL de confianza**.
1. Seleccione `workfront_session` en la lista.
1. Haga clic en **Editar**.
1. En Directivas CSP, marque las siguientes opciones:

   * connect-src (scripts)
   * font-src (fuentes)
   * frame-src (contenido de iframe)
   * img-src (imágenes)
   * media-src (audio y vídeo)
   * style-src (hojas de estilo)

1. Haga clic en **Guardar**.

