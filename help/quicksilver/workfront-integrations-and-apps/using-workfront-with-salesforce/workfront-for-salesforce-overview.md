---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Información general de Adobe Workfront for Salesforce
description: Puede instalar [!DNL Adobe Workfront] para que Salesforce permita que los usuarios de Salesforce envíen [!DNL Workfront] solicita y crea proyectos automáticamente sin salir nunca de Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] información general

A [!UICONTROL Pro] [!DNL Workfront] Se requiere un plan para utilizar esta función. Para obtener más información sobre los distintos planes disponibles, consulte [[!DNL Workfront] Planes.](https://www.workfront.com/plans)

Puede instalar [!DNL Adobe Workfront for Salesforce] para permitir que [!DNL Salesforce] usuarios a enviar [!DNL Workfront] solicita y crea proyectos automáticamente sin salir [!DNL Salesforce].

Como [!DNL Workfront] administrador, puede descargar y configurar [!DNL Workfront for Salesforce]. Entonces, puede compartirlo todo lo demás [!DNL Salesforce] usuarios.

Para obtener más información sobre la instalación [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Para obtener más información sobre cómo configurar la variable [!DNL Workfront] en [!DNL Salesforce] para todos los usuarios, consulte [Configure las variables [!DNL Adobe Workfront] para [!DNL Salesforce] usuarios](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

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

## [!DNL Workfront for Salesforce]

Puede hacer lo siguiente al utilizar [!DNL Workfront for Salesforce]:

* Crear manualmente [!DNL Workfront] solicitudes de [!DNL Salesforce] dentro de una oportunidad o una cuenta.

   Para obtener más información sobre la creación de [!DNL Workfront] solicitudes de [!DNL Salesforce], consulte [Submit [!DNL Adobe Workfront] solicitudes de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Déclencheur automático de la creación de proyectos en [!DNL Workfront] cuando se cumplen determinados criterios en [!DNL Salesforce]. Su [!DNL Salesforce] el administrador del sistema debe configurar los déclencheur para la creación de proyectos desde [!DNL Salesforce].

   Para obtener más información sobre la creación de [!DNL Workfront] proyectos de [!DNL Salesforce], consulte [Crear [!DNL Adobe Workfront] proyectos de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Tenga en cuenta lo siguiente al trabajar con [!DNL Workfront] para [!DNL Salesforce]:

* Apoyamos ambas [!DNL Salesforce Classic] y [!DNL Lightning Experience] marcos.
* Los elementos solo se pueden crear desde [!DNL Salesforce] en [!DNL Workfront].
* Puede ver información sobre el [!DNL Workfront] elementos en [!DNL Salesforce].

   Esta información no se puede personalizar.

   Para obtener una lista de [!DNL Workfront] campos desde los que se puede ver [!DNL Salesforce], consulte  [Submit [!DNL Adobe Workfront] solicitudes de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)  y [Crear [!DNL Adobe Workfront] proyectos de [!DNL Salesforce] objetos](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Puede acceder directamente a los elementos vinculados a [!DNL Salesforce] haciendo clic en el botón **[!UICONTROL Ir a Salesforce]** vínculo desde Workfront.

   No puede ver ninguna información sobre el [!DNL Salesforce] elementos en [!DNL Workfront], pero tiene un vínculo a la variable [!UICONTROL Salesforce] elemento de [!DNL Workfront] para revisarlo en [!DNL Salesforce].

   [!UICONTROL La variable **Ir a Salesforce**] se muestra en las siguientes áreas:

   * La variable [!UICONTROL Detalles] sección de un proyecto o problema
   * Encabezado de un proyecto o problema.

      El administrador del sistema o del grupo debe agregar la variable [!UICONTROL Integraciones] para ver el [!UICONTROL Ir a Salesforce] en el encabezado del proyecto o del problema.
   * La variable [!DNL Summary] de un problema al seleccionar el problema en una lista, después de hacer clic en [!UICONTROL Abrir resumen] ![](assets/summary-panel-icon.png) en la barra de herramientas de la lista.

      >[!NOTE]
      >
      >La variable [!UICONTROL Ir a Salesforce] el vínculo es visible para todos [!DNL Workfront] usuarios que pueden ver el proyecto o el problema. Debe tener un [!DNL Salesforce] para poder ir a la [!DNL Salesforce] Oportunidad o cuenta en la que se registró el problema.

* La actualización de campos en un elemento de una aplicación no actualiza ninguna información sobre elementos vinculados en la otra aplicación.
