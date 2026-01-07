---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Instalar  [!DNL Adobe Workfront] para  [!DNL Jira]
description: Puede utilizar  [!DNL Adobe Workfront]  para  [!DNL Jira]  para integrar sus sistemas  [!DNL Jira]  y  [!DNL Workfront] .
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 80%

---

# Instalación de [!DNL Adobe Workfront for Jira]

>[!IMPORTANT]
>
>Para ofrecer integraciones más estables y escalables, estamos adoptando un enfoque de integración moderno y flexible mediante la automatización e integración (Fusion) de Workfront. Como parte de este proceso de transición, la integración de Workfront para Jira no estará disponible después del **28 de febrero de 2026**.
>
>Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Jira.
>
>Para obtener una descripción general de la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obtener información sobre las capacidades específicas de los módulos de integración y automatización de Workfront para Jira, consulte [Módulos de software de Jira](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Puede utilizar [!DNL Adobe Workfront for Jira] para integrar sus sistemas [!DNL Jira] y [!DNL Workfront].

Después de instalar el complemento, puede definir flujos de trabajo que creen automáticamente problemas de [!DNL Jira] cuando se creen elementos de trabajo de [!DNL Workfront]. Los elementos de ambas aplicaciones se vinculan y parte de su información se puede actualizar automáticamente en ambos sistemas.

Todos los usuarios de [!DNL Workfront] y [!DNL Jira] pueden beneficiarse de esta integración. Solo necesitan una licencia para el sistema en el que más trabajan, y no para ambos sistemas.

Este complemento está disponible para las versiones [!UICONTROL Server] y [!UICONTROL OnDemand] (o [!UICONTROL Cloud]) del software de [!DNL Jira]. Este complemento no está disponible en la versión [!DNL Data Center] del software de [!DNL Jira].

Para obtener una lista de las versiones de [!DNL Jira] que [!DNL Workfront for Jira] admite actualmente, consulte [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) en Atlassian Marketplace.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Acceso a Jira</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Se recomienda crear cuentas de administrador del sistema independientes en Jira y Workfront para dedicarlas a esta integración, en lugar de utilizar las existentes que podrían adjuntarse a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Instalación de [!DNL Workfront] para [!DNL Jira]

Instalar [!DNL Workfront] para [!DNL Jira] OnDemand es idéntico a instalarlo en una instancia de [!DNL Jira] Server.

Debe ser administrador de [!DNL Jira] para instalar el complemento de [!DNL Workfront].

Si no es administrador de [!DNL Jira], puede buscar el complemento de [!DNL Workfront] y solicitar que se lo instalen. Su solicitud se envía al administrador de [!DNL Jira] para su aprobación e instalación.

Para obtener más información sobre la solicitud de instalación de un complemento en la aplicación [!DNL Jira], consulte [Administrar solicitudes de usuario para complementos.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html?lang=es)

Para instalar [!DNL Workfront for Jira]:

1. Inicie sesión en [!DNL Jira] como administrador de [!DNL Jira].
1. Busque el complemento de **[!DNL Workfront for Jira]** en [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview).

1. Haga clic en **[!UICONTROL Obtenerlo ahora]** para instalarlo.

   Una vez finalizada la instalación, puede iniciar sesión en [!DNL Workfront] desde [!DNL Jira] y configurar la integración.

   Para obtener más información, consulte [Configuración de Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Consideraciones para una instalación de [!DNL Jira Server]

>[!NOTE]
>
>Estos requisitos no se aplican a la versión [!UICONTROL OnDemand] ([!UICONTROL Cloud]) del software de [!DNL Jira].

Aunque la instalación del complemento de [!DNL Workfront] en los dos entornos de [!DNL Jira] es similar, debe tener en cuenta lo siguiente al trabajar con una instalación de [!DNL Jira Server]:

* Al configurar el complemento en [!DNL Jira], es posible que la dirección especificada en el campo **[!DNL JIRA Base URL]** no tenga la misma URL que usa para obtener acceso a [!DNL Jira] en su servidor privado. **[!DNL JIRA Base URL]** debe ser una dirección de acceso público conectada a su servidor privado mediante protocolos NAT o de proxy inverso, para que [!DNL Workfront] pueda tener acceso a ella para realizar solicitudes al servidor.

* Debe utilizar el cifrado SSL para proteger la comunicación entre [!DNL Jira] y [!DNL Workfront]. Al habilitar SSL, debe tener una pila de certificados SSL completa de una autoridad de certificación. No admitimos certificados autofirmados.
* Debe asegurarse de que se puede acceder al dominio [!DNL jira.workfront.com] desde los servidores corporativos. Actúa como entorno de middleware entre [!DNL Workfront] y [!DNL Jira] y es necesario para que funcione el complemento.

  También es necesario añadir las siguientes direcciones IP estáticas a la lista de permitidos del cortafuegos para conexiones salientes y entrantes.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Para obtener más información sobre cómo configurar el firewall para una funcionalidad óptima con [!DNL Workfront], consulte [Configuración del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
