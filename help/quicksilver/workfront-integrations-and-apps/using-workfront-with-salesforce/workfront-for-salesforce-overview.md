---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Información general de Adobe Workfront para Salesforce
description: Puede instalar  [!DNL Adobe Workfront]  para Salesforce para permitir que los usuarios de Salesforce envíen solicitudes de  [!DNL Workfront]  y creen proyectos automáticamente sin salir de Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 66%

---

# Información general de [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>Para ofrecer integraciones más estables y escalables, estamos adoptando un enfoque de integración moderno y flexible mediante la automatización e integración (Fusion) de Workfront. Como parte de este proceso de transición, la integración de Workfront para Salesforce no estará disponible después del **28 de febrero de 2026**.
>
>Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Salesforce.
>
>Para obtener una descripción general de la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obtener información sobre las capacidades específicas de los módulos de integración y automatización de Workfront para Salesforce, consulte [módulos de Salesforce](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Puede instalar [!DNL Adobe Workfront for Salesforce] para permitir que los usuarios de [!DNL Salesforce] envíen solicitudes de [!DNL Workfront] y creen proyectos automáticamente sin salir de [!DNL Salesforce].

Como administrador de [!DNL Workfront], puede descargar y configurar [!DNL Workfront for Salesforce]. A continuación, puede compartirlo con los demás [!DNL Salesforce] usuarios.

Para obtener más información sobre la instalación de [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Para obtener más información sobre cómo configurar la sección [!DNL Workfront] en [!DNL Salesforce] para todos los usuarios, consulte [Configurar la sección  [!DNL Adobe Workfront]  para los usuarios de  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

>[!NOTE]
>
>Se requiere un plan [!UICONTROL Pro] de [!DNL Workfront] para usar esta característica. Para obtener más información acerca de los distintos planes disponibles, consulte [[!DNL Workfront] Planes](https://business.adobe.com/products/workfront/pricing.html).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad que se describe en este artículo:

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>Nuevo: estándar<p>
   <p>O</p>
   <p>Actual: plan</p>


</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## [!DNL Workfront for Salesforce]

Puede hacer lo siguiente al usar [!DNL Workfront for Salesforce]:

* Crear manualmente nuevas solicitudes de [!DNL Workfront] desde [!DNL Salesforce] en una oportunidad o una cuenta.

  Para obtener más información, consulte [Enviar [!DNL Adobe Workfront] solicitudes de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Activar automáticamente la creación de proyectos en [!DNL Workfront] cuando se cumplen determinados criterios en [!DNL Salesforce]. El administrador del sistema [!DNL Salesforce] debe configurar los activadores para crear proyectos desde [!DNL Salesforce].

  Para obtener más información sobre la creación de proyectos de [!DNL Workfront] desde [!DNL Salesforce], consulte [Crear proyectos de  [!DNL Adobe Workfront]  desde objetos de  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Tenga en cuenta lo siguiente al trabajar con [!DNL Workfront] para [!DNL Salesforce]:

* Admitimos los marcos de trabajo [!DNL Salesforce Classic] y [!DNL Lightning Experience].
* Los elementos solamente se pueden crear de [!DNL Salesforce] a [!DNL Workfront].
* Puede ver información sobre los elementos de [!DNL Workfront] en [!DNL Salesforce]. Esta información no se puede personalizar.

  Para obtener una lista de campos de [!DNL Workfront] que puede ver desde [!DNL Salesforce], consulte [Enviar solicitudes de  [!DNL Adobe Workfront]  desde objetos de  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) y [Crear proyectos de  [!DNL Adobe Workfront]  desde objetos de  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Puede acceder directamente a los elementos vinculados a [!DNL Salesforce] haciendo clic en el vínculo [!UICONTROL Ir a Salesforce] desde Workfront.

  No puede ver ninguna información sobre los [!DNL Salesforce] elementos de [!DNL Workfront], pero hay un vínculo en Workfront que le lleva al elemento en Salesforce para que pueda revisarlo allí.

  [!UICONTROL El vínculo Ir a Salesforce] se muestra en las siguientes áreas:

   * La sección [!UICONTROL Detalles] de un proyecto o problema.
   * El encabezado de un proyecto o un problema.

     El administrador del sistema o de grupos debe añadir el campo [!UICONTROL Integraciones] a la plantilla de diseño para ver el vínculo [!UICONTROL Ir a Salesforce] en el encabezado del proyecto o problema.
   * El panel [!DNL Summary] de un problema al seleccionar el problema en una lista, después de hacer clic en [!UICONTROL Abrir resumen] ![icono del panel de resumen](assets/summary-panel-icon.png) en la barra de herramientas de la lista.

     >[!NOTE]
     >
     >El vínculo [!UICONTROL Ir a Salesforce] es visible para todos los usuarios de [!DNL Workfront] que puedan ver el proyecto o el problema. Debe tener una cuenta de [!DNL Salesforce] para poder ir a la oportunidad o cuenta de [!DNL Salesforce] en la que se registró el problema.

* Al actualizar los campos de un elemento en una aplicación, no se actualiza la información sobre los elementos vinculados en la otra aplicación.
