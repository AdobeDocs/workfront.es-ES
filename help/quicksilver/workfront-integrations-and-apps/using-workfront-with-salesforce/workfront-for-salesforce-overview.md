---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Información general de Adobe Workfront para Salesforce
description: Puede instalar  [!DNL Adobe Workfront]  para Salesforce para permitir que los usuarios de Salesforce envíen solicitudes de  [!DNL Workfront]  y creen proyectos automáticamente sin salir de Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 94%

---

# Información general de [!DNL Adobe Workfront for Salesforce]

Se requiere un plan [!UICONTROL Pro] [!DNL Workfront] para usar esta característica. Para obtener más información sobre los distintos planes disponibles, consulte [[!DNL Workfront] Planes.](https://www.workfront.com/plans)

Puede instalar [!DNL Adobe Workfront for Salesforce] para permitir que los usuarios de [!DNL Salesforce] envíen solicitudes de [!DNL Workfront] y creen proyectos automáticamente sin salir de [!DNL Salesforce].

Como administrador de [!DNL Workfront], puede descargar y configurar [!DNL Workfront for Salesforce]. A continuación, puede compartirlo con todos los demás usuarios de [!DNL Salesforce].

Para obtener más información sobre la instalación de [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Para obtener más información sobre cómo configurar la sección [!DNL Workfront] en [!DNL Salesforce] para todos los usuarios, consulte [Configurar la sección  [!DNL Adobe Workfront]  para los usuarios de  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad que se describe en este artículo:

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

## [!DNL Workfront for Salesforce]

Puede hacer lo siguiente al usar [!DNL Workfront for Salesforce]:

* Crear manualmente nuevas solicitudes de [!DNL Workfront] desde [!DNL Salesforce] en una oportunidad o una cuenta.

  Para obtener más información sobre la creación de solicitudes de [!DNL Workfront] desde [!DNL Salesforce], consulte [Enviar solicitudes de  [!DNL Adobe Workfront]  desde objetos de  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Activar automáticamente la creación de proyectos en [!DNL Workfront] cuando se cumplen determinados criterios en [!DNL Salesforce]. El administrador del sistema [!DNL Salesforce] debe configurar los activadores para crear proyectos desde [!DNL Salesforce].

  Para obtener más información sobre la creación de proyectos de [!DNL Workfront] desde [!DNL Salesforce], consulte [Crear proyectos de  [!DNL Adobe Workfront]  desde objetos de  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Tenga en cuenta lo siguiente al trabajar con [!DNL Workfront] para [!DNL Salesforce]:

* Admitimos los marcos de trabajo [!DNL Salesforce Classic] y [!DNL Lightning Experience].
* Los elementos solo se pueden crear desde [!DNL Salesforce] hasta [!DNL Workfront].
* Puede ver información sobre los elementos de [!DNL Workfront] en [!DNL Salesforce].

  Esta información no se puede personalizar.

  Para obtener una lista de campos de [!DNL Workfront] que puede ver desde [!DNL Salesforce], consulte [Enviar solicitudes de  [!DNL Adobe Workfront]  desde objetos de  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) y [Crear proyectos de  [!DNL Adobe Workfront]  desde objetos de  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Puede acceder directamente a los elementos vinculados a [!DNL Salesforce] haciendo clic en el vínculo **[!UICONTROL Ir a Salesforce]** desde Workfront.

  No puede ver ninguna información sobre los elementos de [!DNL Salesforce] en [!DNL Workfront], pero dispone de un vínculo al elemento de [!UICONTROL Salesforce] desde [!DNL Workfront] para revisarlo en [!DNL Salesforce].

  [!UICONTROL El vínculo **Ir a Salesforce**] se muestra en las siguientes áreas:

   * La sección [!UICONTROL Detalles] de un proyecto o problema
   * El encabezado de un proyecto o un problema.

     El administrador del sistema o de grupos debe añadir el campo [!UICONTROL Integraciones] a la plantilla de diseño para ver el vínculo [!UICONTROL Ir a Salesforce] en el encabezado del proyecto o problema.
   * El panel [!DNL Summary] de un problema al seleccionar el problema en una lista, después de hacer clic en [!UICONTROL Abrir resumen] ![icono del panel de resumen](assets/summary-panel-icon.png) en la barra de herramientas de la lista.

     >[!NOTE]
     >
     >El vínculo [!UICONTROL Ir a Salesforce] es visible para todos los usuarios de [!DNL Workfront] que puedan ver el proyecto o el problema. Debe tener una cuenta de [!DNL Salesforce] para poder ir a la oportunidad o cuenta de [!DNL Salesforce] en la que se registró el problema.

* Al actualizar los campos de un elemento en una aplicación, no se actualiza la información sobre los elementos vinculados en la otra aplicación.
