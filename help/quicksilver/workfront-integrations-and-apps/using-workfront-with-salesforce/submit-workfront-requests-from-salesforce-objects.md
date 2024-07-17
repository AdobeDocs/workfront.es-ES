---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Enviar  [!DNL Adobe Workfront] solicitudes de [!DNL Salesforce] objetos
description: Después de instalar  [!DNL Adobe Workfront] para [!DNL Salesforce], you can submit [!DNL Workfront] solicitudes de [!DNL Salesforce] oportunidades y cuentas. Esta funcionalidad existe tanto en el marco de trabajo clásico como en el de Lightning Experience.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 1%

---

# Enviar [!DNL Adobe Workfront] solicitudes desde [!DNL Salesforce] objetos

Después de instalar [!DNL Adobe Workfront for Salesforce], puede enviar [!DNL Workfront] solicitudes desde [!DNL Salesforce] oportunidades y cuentas. Esta funcionalidad existe en los marcos [!DNL Classic] y [!DNL Lightning Experience].

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad descrita en este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] plan*</p></td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] licencia*</p></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Requisitos previos

Para enviar una solicitud [!DNL Workfront] desde una oportunidad o cuenta de [!DNL Salesforce], asegúrese de que dispone de lo siguiente en su entorno:

* El administrador de [!DNL Workfront] ha instalado [!DNL Workfront for Salesforce].\
   Para obtener más información acerca de la instalación de [!DNL Workfront for Salesforce], vea [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* El administrador de [!DNL Workfront] ha agregado la sección [!DNL Workfront] a los diseños de página de [!UICONTROL Oportunidad] y [!UICONTROL Cuenta].\
   Para obtener más información sobre cómo agregar la sección [!DNL Workfront] a un diseño de página, consulte [Configurar la sección  [!DNL Adobe Workfront] para [!DNL Salesforce] usuarios](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Tiene una cuenta de [!DNL Workfront] y puede iniciar sesión en ella desde la sección [!DNL Workfront] dentro de su oportunidad o cuenta.\
   Una vez que inicie sesión, verá la ficha [!UICONTROL Nuevas solicitudes], donde podrá empezar a escribir solicitudes.

## Enviar [!DNL Workfront] solicitudes de [!DNL Salesforce]

1. Vaya a una oportunidad o cuenta en Salesforce.
1. Vaya a la sección [!DNL Workfront].
1. En la pestaña **[!UICONTROL Nuevas solicitudes]**, seleccione un tipo de solicitud en el menú desplegable **[!UICONTROL Seleccionar un tipo de solicitud]**.

   Puede ver las mismas colas de solicitudes a las que tiene acceso en Workfront.

1. Empiece a rellenar los campos disponibles para la solicitud.

   Enviar una solicitud desde [!DNL Salesforce] es idéntico a enviar una solicitud en la aplicación web [!DNL Workfront].

   >[!NOTE]
   >
   >La carga de un documento mediante el complemento [!DNL Workfront] en [!DNL Salesforce] no está disponible temporalmente.

   Siga los pasos descritos en [Crear y enviar [!DNL Adobe Workfront] solicitudes](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Haga clic en **[!UICONTROL Enviar]**.

## Ver [!DNL Workfront] solicitudes

1. Ir a una oportunidad o cuenta en [!DNL Salesforce].
1. Vaya a la sección **[!DNL Workfront]**.

   >[!NOTE]
   >
   >Dependiendo de cómo haya configurado el administrador de [!DNL Workfront] esta sección, podría tener un nombre diferente.

1. Seleccione la pestaña **[!UICONTROL Solicitudes enviadas]**.

   Puede ver todas las solicitudes que usted u otros usuarios han enviado desde esta oportunidad o cuenta en esta ficha. Las solicitudes enviadas a esta cola de solicitudes en la aplicación web no se muestran en esta lista en [!DNL Salesforce].

   >[!NOTE]
   >
   >Las solicitudes enviadas a esta cola de solicitudes en la aplicación web no se muestran en esta lista en Salesforce.

   ![salesforce_submitted_requests.png](assets/salesforce-submitted-requests-350x58.png)

   Puede ver la siguiente información sobre las solicitudes enviadas:

   * Nombre de solicitud (en la columna [!UICONTROL Asunto])
   * Número de referencia
   * Tipo de solicitud
   * Estado
   * Enviado el día
   * Solicitado por nombre
   * Asignado a nombre\

     Cuando esta información se actualiza en [!DNL Workfront], también se actualiza en esta lista.

1. (Opcional) Haga clic en el nombre de la solicitud para abrirla en [!DNL Workfront].

1. (Opcional) Haga clic **[!UICONTROL Ir a[!DNL Salesforce]]** para acceder a la oportunidad o cuenta donde se originó el problema desde las siguientes áreas de Workfront:

   * En la sección [!UICONTROL Detalles] del problema
   * En el Panel de resumen, al seleccionar el problema en una lista, después de hacer clic en [!UICONTROL Abrir resumen] ![](assets/summary-panel-icon.png) en la barra de herramientas de la lista.
   * En el encabezado del problema, cuando el campo [!UICONTROL Integraciones] esté disponible. El administrador del sistema o del grupo debe agregar el campo [!UICONTROL Integraciones] a la plantilla de diseño para ver el vínculo Ir a Salesforce en el encabezado del problema. Para obtener más información, vea [Personalizar encabezados de objeto mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >El vínculo [!UICONTROL Ir a Salesforce] es visible para todos los usuarios de [!DNL Workfront] que puedan ver el problema. Debe tener una cuenta de [!DNL Salesforce] para poder ir a la oportunidad o cuenta de [!DNL Salesforce] en la que se registró el problema.
