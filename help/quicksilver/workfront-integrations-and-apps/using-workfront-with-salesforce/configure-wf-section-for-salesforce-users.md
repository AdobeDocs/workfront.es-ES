---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: 'Configurar la sección de  [!DNL Adobe Workfront]  para usuarios de  [!DNL Salesforce] '
description: Después de instalar  [!DNL Adobe Workfront]  para Salesforce como persona con la función de administrador de  [!DNL Workfront] , puede ponerlo a disposición de los usuarios añadiéndolo en una nueva sección a los diseños de página de Salesforce Oportunidad y Cuenta.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 87%

---

# Configurar la sección de [!DNL Adobe Workfront] para usuarios de [!DNL Salesforce]

>[!IMPORTANT]
>
>Para ofrecer integraciones más estables y escalables, estamos adoptando un enfoque de integración moderno y flexible mediante la automatización e integración (Fusion) de Workfront. Como parte de este proceso de transición, la integración de Workfront para Salesforce no estará disponible después del **28 de febrero de 2026**.
>
>Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Salesforce.
>
>Para obtener una descripción general de la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obtener información sobre las capacidades específicas de los módulos de integración y automatización de Workfront para Salesforce, consulte [módulos de Salesforce](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Después de instalar [!DNL Adobe Workfront] para [!DNL Salesforce] como persona con la función de administrador de [!DNL Workfront], puede ponerlo a disposición de los usuarios añadiéndolo en una nueva sección a sus 
diseños de página de [!UICONTROL Salesforce] [!UICONTROL Opportunity] y [!UICONTROL Account].

Para obtener información acerca de la instalación de [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Para que los usuarios tengan [!DNL Workfront] disponible en las plataformas [!DNL Classic] y [!DNL Lightning Experience], debe añadir las páginas de [!UICONTROL Visualforce] [!DNL WorkfrontOpportunities] y [!DNL WorkfrontAccounts] a los diseños de página [!UICONTROL Opportunity] y [!UICONTROL Accounts], respectivamente.



## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
   <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

* Debe tener una instancia de [!DNL Salesforce] con acceso a una cuenta de administrador del sistema.
* Debe tener una instancia de [!DNL Workfront] con acceso a una cuenta de administrador del sistema.

## Configurar la sección de [!DNL Workfront] en la plataforma [!DNL Salesforce Classic]

1. Inicie sesión en [!DNL Salesforce] como persona con la función de administrador de Workfront.
1. Haga clic en **[!UICONTROL Setup].**
1. En la sección **[!UICONTROL Build]**, expanda **[!UICONTROL Customize].**

1. Expanda **[!UICONTROL Opportunities]** y, a continuación, haga clic en **[!UICONTROL Page Layouts]** para añadir la sección de [!DNL Workfront] a una oportunidad.

   O

   Expanda **[!UICONTROL Accounts]** y, a continuación, haga clic en **[!UICONTROL Page Layouts]** para añadir la sección de [!DNL Workfront] a una cuenta
.

1. Haga clic en **[!UICONTROL Edit]** en un diseño existente.

   O

   Haga clic en **[!UICONTROL New]** para añadir un nuevo diseño.

1. (Opcional) Arrastre el componente **[!UICONTROL Section]** al diseño y suéltelo en la posición deseada.\

1. (Opcional) Especifique un nombre para la nueva sección.

   Le recomendamos que nombre esta sección **[!DNL Workfront]**.

1. (Opcional) Especifique el **[!UICONTROL Layout]** y el **[!UICONTROL Tab-key Order]** deseados para la nueva sección.

   Le recomendamos que seleccione el diseño **[!UICONTROL 1-Column]** para la sección de [!DNL Workfront].

1. Haga clic en **[!UICONTROL OK]**.
1. En el área **[!UICONTROL Layout]**, haga clic en **[!UICONTROL Visualforce Pages].**

1. Arrastre y suelte el componente **[!UICONTROL WorkfrontOpportunities]** en la nueva sección del diseño **[!UICONTROL Opportunities]**.

   O

   Arrastre y suelte el componente **[!UICONTROL WorkfrontAccounts]** en la nueva sección del diseño **[!UICONTROL Account]**.\

1. Haga clic en el icono **[!UICONTROL Properties]** en la parte superior derecha del componente recién añadido.\

1. Para lograr una visualización óptima, especifique las siguientes propiedades para la página de [!DNL Workfront Visualforce]:

   * **[!UICONTROL Anchura (en píxeles o %)]**: 100 %
   * **[!UICONTROL Altura (en píxeles)]**: 600
   * Seleccione **[!UICONTROL Mostrar barras de desplazamiento]**.

1. Haga clic en **[!UICONTROL OK]**.
1. Haga clic en **[!UICONTROL Guardar]** para guardar el diseño.

   Todos los usuarios que tengan este diseño asignado ahora podrán ver la sección de [!DNL Workfront] en sus objetos de [!UICONTROL Oportunidades] o [!UICONTROL Cuentas].

   Los usuarios verán una pantalla de inicio de sesión de [!DNL Workfront] en la sección de [!DNL Workfront]. Si no tienen una cuenta de [!DNL Workfront], podrán contraer la sección, pero no quitarla de su diseño.

## Configurar la sección de [!DNL Workfront] en la plataforma [!DNL Salesforce Lightning Experience]

Es posible añadir la sección [!DNL Workfront] al diseño de una [!UICONTROL oportunidad] de [!DNL Salesforce] o cuenta
en el marco de [!DNL Salesforce Lightning Experience], ya sea accediendo al área [!UICONTROL Configuración] o desde una cuenta
o el objeto [!UICONTROL Oportunidad].

* [Configure la sección [!DNL Workfront] en el nivel [!UICONTROL Configuración]](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Configure la sección [!DNL Workfront] en el nivel de oportunidad o cuenta](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Configure la sección [!DNL Workfront] en el nivel [!UICONTROL Configuración] {#configure-the-workfront-section-at-the-setup-level}

1. Inicie sesión en [!DNL Salesforce] como administrador del sistema.
1. Haga clic en el icono **[!UICONTROL Configuración]** y, a continuación, haga clic en **[!UICONTROL Configuración]**.

1. Expanda **[!UICONTROL Objeto y campos]** y, a continuación, haga clic en **[!UICONTROL Administrador de objetos]**.

1. Haga clic en **[!UICONTROL Oportunidad]** para personalizar el diseño de una oportunidad.

   O

   Haga clic en **[!UICONTROL Cuenta]** para personalizar el diseño de una cuenta.

1. Haga clic en **[!UICONTROL Diseños de página]**.
1. Haga clic en el nombre de un diseño de página existente para editarlo.

   O

   Haga clic en **[!UICONTROL Nuevo]** para crear un nuevo diseño de página.

1. Continúe con [Configurar la sección [!DNL Workfront] en el nivel de oportunidad o cuenta](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) a continuación.

### Configurar la sección [!DNL Workfront] en el nivel de oportunidad o cuenta {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Inicie sesión en [!DNL Salesforce] como administrador del sistema.
1. Vaya a una **[!UICONTROL oportunidad]** o a una **[!UICONTROL cuenta]**.

1. Haga clic en el icono **[!UICONTROL Configurar]** y luego haga clic en **[!UICONTROL Editar página]**.

1. Expanda la sección **[!UICONTROL Administrado a medida]**.
1. Arrastre y suelte el componente **[!DNL Workfront]** en la página de la [!UICONTROL oportunidad] o cuenta.

   Se recomienda utilizar el ancho completo de la página para la sección [!DNL Workfront] en lugar de una de las columnas del diseño.

1. Haga clic en **[!UICONTROL Guardar]**.

   Todos los usuarios que tengan este diseño asignado ya pueden ver la sección [!DNL Workfront] en sus objetos de [!UICONTROL oportunidades] o [!UICONTROL cuentas].

   >[!NOTE]
   >
   >Los usuarios verán una pantalla de inicio de sesión de [!DNL Workfront] en la sección [!DNL Workfront]. Si no tuvieran una cuenta de [!DNL Workfront], podrán contraer la sección, pero no quitarla del diseño. Los usuarios pueden iniciar sesión utilizando el método de autenticación que habilitó: la autenticación mejorada o su URL de Lenguaje de marcado para confirmaciones de seguridad (SAML).

