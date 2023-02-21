---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Configure las variables [!DNL Adobe Workfront] para [!DNL Salesforce] usuarios
description: Después de la instalación [!DNL Adobe Workfront] para Salesforce as a [!DNL Workfront] administrador, puede ponerlo a disposición de los usuarios agregándolo en una nueva sección a sus diseños de página Oportunidad y Cuenta en Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 1%

---

# Configure las variables [!DNL Adobe Workfront] para [!DNL Salesforce] usuarios

A [!UICONTROL Pro] [!DNL Workfront] Se requiere un plan para utilizar esta función. Para obtener más información sobre los distintos planes disponibles, consulte [[!DNL Workfront] Planes.](https://www.workfront.com/plans)

Después de la instalación [!DNL Adobe Workfront] para [!DNL Salesforce] como [!DNL Workfront] administrador, puede ponerlo a disposición de los usuarios agregándolo en una nueva sección a sus [!UICONTROL Oportunidad] y [!UICONTROL Cuenta]
diseños de página en [!UICONTROL Salesforce].

Para obtener información sobre la instalación [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Para que los usuarios tengan [!DNL Workfront] disponible en ambos [!DNL Classic] y [!DNL Lightning Experience] marcos, debe agregar la variable [!DNL WorkfrontOpportunities] y [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] a [!UICONTROL Oportunidad] y [!UICONTROL Cuentas] diseños de página, respectivamente.

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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

* Debe tener un [!DNL Salesforce] con acceso a una cuenta de administrador del sistema.
* Debe tener un [!DNL Workfront] con acceso a una cuenta de administrador del sistema.

## Configure las variables [!DNL Workfront] en la sección [!DNL Salesforce Classic] marco

1. Iniciar sesión en [!DNL Salesforce] como administrador de Workfront.
1. Haga clic en **[!UICONTROL Configuración].**
1. En el **[!UICONTROL Generar]** sección, expandir **[!UICONTROL Personalizar].**

1. Expandir **[!UICONTROL Oportunidades]** y haga clic en **[!UICONTROL Diseños de página]** para agregar la variable [!DNL Workfront] a Oportunidad.

   O

   Expandir **[!UICONTROL Cuentas]** y haga clic en **[!UICONTROL Diseños de página]** para agregar la variable [!DNL Workfront] a una cuenta .

1. Haga clic en **[!UICONTROL Editar]** en un diseño existente.

   O

   Haga clic en **[!UICONTROL Nuevo]** para añadir un nuevo diseño.

1. (Opcional) Arrastre el **[!UICONTROL Sección]** en el diseño y colóquelo en la posición deseada.\

1. (Opcional) Especifique un nombre para la nueva sección.

   Le recomendamos que asigne un nombre a esta sección **[!DNL Workfront]**.

1. (Opcional) Especifique la **[!UICONTROL Diseño]** y **[!UICONTROL Orden de las teclas de tabulación]** para la nueva sección.

   Le recomendamos que seleccione **[!UICONTROL 1 columna]** para el [!DNL Workfront] para obtener más información.

1. Haga clic en **[!UICONTROL OK]**.
1. En el **[!UICONTROL Diseño]** área, haga clic en **[!UICONTROL Páginas de VisualForce].**

1. Arrastre y suelte la **[!UICONTROL Oportunidades del frente de trabajo]** a la nueva sección de la sección **[!UICONTROL Oportunidades]** Diseño.

   O

   Arrastre y suelte la **[!UICONTROL WorkfrontAccounts]** a la nueva sección de la sección  **[!UICONTROL Cuenta]** Diseño.\

1. Haga clic en el **[!UICONTROL Propiedades]** en la parte superior derecha del componente recién agregado.\

1. Para lograr una visualización óptima, especifique las siguientes propiedades para la variable [!DNL Workfront Visualforce] página:

   * **[!UICONTROL Anchura (en píxeles o %)]**: 100 %
   * **[!UICONTROL Altura (en píxeles)]**: 600
   * Select **[!UICONTROL Mostrar barras de desplazamiento]**.

1. Haga clic en **[!UICONTROL OK]**.
1. Haga clic en **[!UICONTROL Guardar]** para guardar el diseño.

   Todos los usuarios que tienen este diseño asignado ahora pueden ver la variable [!DNL Workfront] en la sección [!UICONTROL Oportunidades] o [!UICONTROL Cuentas] objetos.

   Los usuarios ven una [!DNL Workfront] pantalla de inicio de sesión en [!DNL Workfront] para obtener más información. Si no tienen un [!DNL Workfront] pueden contraer la sección, pero no eliminarla de su diseño.

## Configure las variables [!DNL Workfront] en la sección [!DNL Salesforce Lightning Experience] marco

Puede añadir la variable [!DNL Workfront] a la presentación de un [!DNL Salesforce] [!UICONTROL Oportunidad] o Cuenta en la variable [!DNL Salesforce Lightning Experience] para acceder a la [!UICONTROL Configuración] o de una cuenta o [!UICONTROL Oportunidad] objeto.

* [Configure las variables [!DNL Workfront] en la sección [!UICONTROL Configuración] level](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Configure las variables [!DNL Workfront] Sección en el nivel de oportunidad o cuenta](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Configure las variables [!DNL Workfront] en la sección [!UICONTROL Configuración] level {#configure-the-workfront-section-at-the-setup-level}

1. Iniciar sesión [!DNL Salesforce] como administrador del sistema.
1. Haga clic en el **[!UICONTROL Configuración]** y, a continuación, haga clic en **[!UICONTROL Configuración]**.

1. Expandir **[!UICONTROL Objeto y campos]** y haga clic en **[!UICONTROL Administrador de objetos]**.

1. Haga clic en **[!UICONTROL Oportunidad]** para personalizar el diseño de una oportunidad.

   O

   Haga clic en **[!UICONTROL Cuenta]** para personalizar el diseño de una cuenta.

1. Haga clic en **[!UICONTROL Diseños de página]**.
1. Haga clic en el nombre de un diseño de página existente para editarlo.

   O

   Haga clic en **[!UICONTROL Nuevo]** para crear un nuevo diseño de página.

1. Continuar con [Configure las variables [!DNL Workfront] Sección en el nivel de oportunidad o cuenta](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) más abajo.

### Configure las variables [!DNL Workfront] Sección en el nivel de oportunidad o cuenta {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Iniciar sesión en [!DNL Salesforce] como administrador del sistema.
1. Vaya a un **[!UICONTROL Oportunidad]** o **[!UICONTROL Cuenta]**.

1. Haga clic en el **[!UICONTROL Configuración]** y, a continuación, haga clic en **[!UICONTROL Editar página]**.\

1. Expanda el **[!UICONTROL Gestionado a medida]** para obtener más información.
1. Arrastre y suelte la **[!DNL Workfront]** en su [!UICONTROL Oportunidad] o la página Cuenta.

   Se recomienda utilizar la anchura completa de la página para la variable [!DNL Workfront] en lugar de una de las columnas de la presentación.

1. Haga clic en **[!UICONTROL Guardar]**.

   Todos los usuarios que tienen este diseño asignado ahora pueden ver la variable [!DNL Workfront] en la sección [!UICONTROL Oportunidades] o [!UICONTROL Cuentas] objetos.

   >[!NOTE]
   >
   >Los usuarios ven una [!DNL Workfront] pantalla de inicio de sesión en [!DNL Workfront] para obtener más información. Si no tienen un [!DNL Workfront] pueden contraer la sección, pero no eliminarla de su diseño. Los usuarios pueden iniciar sesión con el método de autenticación que ha habilitado: Autenticación mejorada o su URL de Lenguaje de marcado de aserción de seguridad (SAML).

