---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 'Envío de solicitudes de  [!DNL Adobe Workfront]  desde objetos de  [!DNL Salesforce] '
description: Después de instalar  [!DNL Adobe Workfront]  para  [!DNL Salesforce], you can submit [!DNL Workfront] , puede enviar solicitudes desde Oportunidades y cuentas de  [!DNL Salesforce] . Esta funcionalidad existe tanto en el marco de trabajo Classic como en el de Lightning Experience.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 83%

---

# Envío de solicitudes de [!DNL Adobe Workfront] desde objetos de [!DNL Salesforce]

>[!IMPORTANT]
>
>Para ofrecer integraciones más estables y escalables, estamos adoptando un enfoque de integración moderno y flexible mediante la automatización e integración (Fusion) de Workfront. Como parte de este proceso de transición, la integración de Workfront para Salesforce no estará disponible después del **28 de febrero de 2026**.
>
>Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Salesforce.
>
>Para obtener una descripción general de la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obtener información sobre las capacidades específicas de los módulos de integración y automatización de Workfront para Salesforce, consulte [módulos de Salesforce](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Después de instalar [!DNL Adobe Workfront for Salesforce], puede enviar solicitudes de [!DNL Workfront] desde Oportunidades y cuentas de [!DNL Salesforce]. Esta funcionalidad existe en los marcos de trabajo [!DNL Classic] y [!DNL Lightning Experience].

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad que se describe en este artículo:

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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con la persona con la función de administrador de [!DNL Workfront].

## Requisitos previos

Para enviar una solicitud de [!DNL Workfront] desde una oportunidad o cuenta de [!DNL Salesforce], asegúrese de que dispone de lo siguiente en su entorno:

* El administrador de [!DNL Workfront] ha instalado [!DNL Workfront for Salesforce].\
   Para obtener más información sobre la instalación de [!DNL Workfront for Salesforce], consulte [Instalar  [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* El administrador de [!DNL Workfront] ha añadido la sección [!DNL Workfront] a los diseños de página [!UICONTROL Oportunidad] y [!UICONTROL Cuenta].\
   Para obtener más información sobre cómo añadir la sección [!DNL Workfront] a un diseño de página, consulte [Configurar la sección  [!DNL Adobe Workfront]  para los usuarios de  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Tiene una cuenta de [!DNL Workfront] y puede iniciar sesión en ella desde la sección [!DNL Workfront] dentro de su oportunidad o cuenta.\
   Una vez que inicie sesión, verá la pestaña [!UICONTROL Nuevas solicitudes], donde podrá empezar a escribir solicitudes.

## Envío de solicitudes de [!DNL Workfront] desde [!DNL Salesforce]

1. Vaya a una oportunidad o cuenta en Salesforce.
1. Vaya a la sección [!DNL Workfront].
1. En la pestaña **[!UICONTROL Nuevas solicitudes]**, seleccione un tipo de solicitud en el menú desplegable **[!UICONTROL Seleccionar un tipo de solicitud]**.

   Puede ver las mismas colas de solicitudes a las que tiene acceso en Workfront.

1. Empiece a rellenar los campos disponibles de la solicitud.

   Enviar una solicitud desde [!DNL Salesforce] es idéntico a enviar una solicitud en la aplicación web de [!DNL Workfront].

   >[!NOTE]
   >
   >La carga de un documento mediante el complemento de [!DNL Workfront] en [!DNL Salesforce] no está disponible temporalmente.

   Siga los pasos que se describen en [Crear y enviar solicitudes de  [!DNL Adobe Workfront] ](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Haga clic en **[!UICONTROL Enviar]**.

## Visualización de las solicitudes de [!DNL Workfront]

1. Vaya a una oportunidad o cuenta en [!DNL Salesforce].
1. Vaya a la sección **[!DNL Workfront]**.

   >[!NOTE]
   >
   >Dependiendo de cómo haya configurado el administrador de [!DNL Workfront] esta sección, podría tener un nombre diferente.

1. Seleccione la pestaña **[!UICONTROL Solicitudes enviadas]**.

   Puede ver todas las solicitudes que usted u otras personas han enviado desde esta oportunidad o cuenta en esta pestaña. Las solicitudes enviadas a esta cola de solicitudes en la aplicación web no se muestran en esta lista en [!DNL Salesforce].

   >[!NOTE]
   >
   >Las solicitudes enviadas a esta cola de solicitudes en la aplicación web no se muestran en esta lista en Salesforce.

   ![salesforce_submitted_requests.png](assets/salesforce-submitted-requests-350x58.png)

   Puede ver la siguiente información sobre las solicitudes enviadas:

   * Nombre de solicitud (en la columna [!UICONTROL Asunto])
   * Número de referencia
   * Tipo de solicitud
   * Estado
   * Aprobado en la fecha
   * Solicitado por Nombre
   * Asignado a Nombre\

     Cuando esta información se actualiza en [!DNL Workfront], también se actualiza en esta lista.

1. Haga clic en el nombre del objeto para abrirla en [!DNL Workfront]

1. (Opcional) Haga clic en **[!UICONTROL Ir a[!DNL Salesforce]]** para acceder a la oportunidad o cuenta donde se originó el problema desde las siguientes áreas de Workfront:

   * En la sección [!UICONTROL Detalles] del problema
   * En el Panel de resumen, al seleccionar el problema en una lista, después de hacer clic en [!UICONTROL Abrir resumen] ![icono del Panel de resumen](assets/summary-panel-icon.png) en la barra de herramientas de la lista.
   * En el encabezado del problema, cuando el campo [!UICONTROL Integraciones] esté disponible. El administrador del sistema o de grupos debe añadir el campo [!UICONTROL Integraciones] a la plantilla de diseño para ver el vínculo Ir a Salesforce en el encabezado del problema. Para obtener más información, vea [Personalizar encabezados de objeto mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >El vínculo [!UICONTROL Ir a Salesforce] está visible para todos los usuarios de [!DNL Workfront] que puedan ver el problema. Debe tener una cuenta de [!DNL Salesforce] para poder ir a la oportunidad o a la cuenta de [!DNL Salesforce] en la que se registró el problema.
