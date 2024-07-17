---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Configurar la sección  [!DNL Adobe Workfront] para [!DNL Salesforce] usuarios
description: Después de instalar [!DNL Adobe Workfront] for Salesforce como administrador de  [!DNL Workfront] Salesforce, puede ponerlo a disposición de los usuarios agregándolo en una nueva sección a los diseños de página Oportunidad y Cuenta de Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 1%

---

# Configurar la sección [!DNL Adobe Workfront] para usuarios de [!DNL Salesforce]

Se requiere un plan [!UICONTROL Pro] [!DNL Workfront] para usar esta característica. Para obtener más información acerca de los distintos planes disponibles, consulte [[!DNL Workfront] Planes.](https://www.workfront.com/plans)

Después de instalar [!DNL Adobe Workfront] para [!DNL Salesforce] como administrador de [!DNL Workfront], puede ponerlo a disposición de los usuarios agregándolo en una nueva sección a sus [!UICONTROL oportunidades] y [!UICONTROL cuenta]
diseños de página en [!UICONTROL Salesforce].

Para obtener información acerca de la instalación de [!DNL Workfront for Salesforce], vea [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Para que los usuarios tengan [!DNL Workfront] disponibles en los marcos [!DNL Classic] y [!DNL Lightning Experience], debe agregar las páginas [!DNL WorkfrontOpportunities] y [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] a los diseños de página [!UICONTROL Opportunity] y [!UICONTROL Accounts], respectivamente.

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
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Requisitos previos

* Debe tener una instancia de [!DNL Salesforce] con acceso a una cuenta de administrador del sistema.
* Debe tener una instancia de [!DNL Workfront] con acceso a una cuenta de administrador del sistema.

## Configurar la sección [!DNL Workfront] en el marco de trabajo [!DNL Salesforce Classic]

1. Inicie sesión en [!DNL Salesforce] como administrador de Workfront.
1. Haga clic en **[!UICONTROL Configuración].**
1. En la sección **[!UICONTROL Generar]**, expanda **[!UICONTROL Personalizar].**

1. Expanda **[!UICONTROL Oportunidades]** y, a continuación, haga clic en **[!UICONTROL Diseños de página]** para agregar la sección [!DNL Workfront] a una oportunidad.

   O

   Expanda **[!UICONTROL Cuentas]** y luego haga clic en **[!UICONTROL Diseños de página]** para agregar la sección [!DNL Workfront] a una Cuenta
.

1. Haga clic en **[!UICONTROL Editar]** en un diseño existente.

   O

   Haga clic en **[!UICONTROL Nuevo]** para agregar un nuevo diseño.

1. (Opcional) Arrastre el componente **[!UICONTROL Section]** al diseño y suéltelo en la posición deseada.\

1. (Opcional) Especifique un nombre para la nueva sección.

   Le recomendamos que nombre esta sección **[!DNL Workfront]**.

1. (Opcional) Especifique el **[!UICONTROL Diseño]** y el **[!UICONTROL Orden de tabulación]** deseados para la nueva sección.

   Le recomendamos que seleccione el diseño **[!UICONTROL 1-Column]** para la sección [!DNL Workfront].

1. Haga clic en **[!UICONTROL Aceptar]**.
1. En el área **[!UICONTROL Diseño]**, haga clic en **[!UICONTROL Páginas de Visualforce].**

1. Arrastre y suelte el componente **[!UICONTROL WorkfrontOpportunity]** en la nueva sección del diseño **[!UICONTROL Oportunidades]**.

   O

   Arrastre y suelte el componente **[!UICONTROL WorkfrontAccounts]** en la nueva sección del diseño **[!UICONTROL Account]**.\

1. Haga clic en el icono **[!UICONTROL Propiedades]** en la parte superior derecha del componente recién agregado.\

1. Para lograr una visualización óptima, especifique las siguientes propiedades para la página [!DNL Workfront Visualforce]:

   * **[!UICONTROL Anchura (en píxeles o %)]**: 100%
   * **[!UICONTROL Altura (en píxeles)]**: 600
   * Seleccione **[!UICONTROL Mostrar barras de desplazamiento]**.

1. Haga clic en **[!UICONTROL Aceptar]**.
1. Haga clic en **[!UICONTROL Guardar]** para guardar el diseño.

   Todos los usuarios que tienen este diseño asignado ahora pueden ver la sección [!DNL Workfront] en sus objetos [!UICONTROL Oportunidades] o [!UICONTROL Cuentas].

   Los usuarios ven una pantalla de inicio de sesión de [!DNL Workfront] en la sección [!DNL Workfront]. Si no tienen una cuenta de [!DNL Workfront], pueden contraer la sección, pero no quitarla de su diseño.

## Configurar la sección [!DNL Workfront] en el marco de trabajo [!DNL Salesforce Lightning Experience]

Puede agregar la sección [!DNL Workfront] al diseño de una [!DNL Salesforce] [!UICONTROL oportunidad] o cuenta
en el marco de [!DNL Salesforce Lightning Experience], ya sea accediendo al área [!UICONTROL Configuración] o desde una cuenta
o el objeto [!UICONTROL Opportunity].

* [Configurar la sección  [!DNL Workfront]  en el nivel [!UICONTROL Configuración]](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Configurar la sección  [!DNL Workfront] en el nivel de oportunidad o cuenta](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Configurar la sección [!DNL Workfront] en el nivel [!UICONTROL Configuración] {#configure-the-workfront-section-at-the-setup-level}

1. Inicie sesión en [!DNL Salesforce] como administrador del sistema.
1. Haz clic en el icono **[!UICONTROL Configuración]** y luego haz clic en **[!UICONTROL Configuración]**.

1. Expanda **[!UICONTROL Objeto y campos]** y, a continuación, haga clic en **[!UICONTROL Administrador de objetos]**.

1. Haga clic en **[!UICONTROL Oportunidad]** para personalizar el diseño de una oportunidad.

   O

   Haga clic en **[!UICONTROL Cuenta]** para personalizar el diseño de una Cuenta.

1. Haga clic en **[!UICONTROL Diseños de página]**.
1. Haga clic en el nombre de un diseño de página existente para editarlo.

   O

   Haga clic en **[!UICONTROL Nuevo]** para crear un nuevo diseño de página.

1. Continúe con [Configurar la sección  [!DNL Workfront] en el nivel de oportunidad o cuenta](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) a continuación.

### Configurar la sección [!DNL Workfront] en el nivel de oportunidad o cuenta {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Inicie sesión en [!DNL Salesforce] como administrador del sistema.
1. Vaya a una **[!UICONTROL oportunidad]** o a una **[!UICONTROL cuenta]**.

1. Haga clic en el icono **[!UICONTROL Configurar]** y, a continuación, haga clic en **[!UICONTROL Editar página]**.\

1. Expanda la sección **[!UICONTROL Administrada a medida]**.
1. Arrastre y suelte el componente **[!DNL Workfront]** en su [!UICONTROL oportunidad] o cuenta
página.

   Se recomienda utilizar el ancho completo de la página para la sección [!DNL Workfront] en lugar de una de las columnas del diseño.

1. Haga clic en **[!UICONTROL Guardar]**.

   Todos los usuarios que tienen este diseño asignado ahora pueden ver la sección [!DNL Workfront] en sus objetos [!UICONTROL Oportunidades] o [!UICONTROL Cuentas].

   >[!NOTE]
   >
   >Los usuarios ven una pantalla de inicio de sesión de [!DNL Workfront] en la sección [!DNL Workfront]. Si no tienen una cuenta de [!DNL Workfront], pueden contraer la sección, pero no quitarla de su diseño. Los usuarios pueden iniciar sesión utilizando el método de autenticación que ha habilitado: Autenticación mejorada o su URL de Lenguaje de marcado de aserción de seguridad (SAML).

