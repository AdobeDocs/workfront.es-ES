---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Instalar [!DNL Adobe Workfront] para [!DNL Jira]
description: Puedes usar [!DNL Adobe Workfront] for [!DNL Jira] para integrar tus [!DNL Jira] sistemas y [!DNL Workfront] sistemas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Instalar [!DNL Adobe Workfront for Jira]

Puede usar [!DNL Adobe Workfront for Jira] para integrar sus sistemas [!DNL Jira] y [!DNL Workfront].

Después de instalar el complemento, puede definir flujos de trabajo que creen [!DNL Jira] problemas automáticamente cuando se creen [!DNL Workfront] elementos de trabajo. Los elementos de ambas aplicaciones se vinculan y parte de su información se puede actualizar automáticamente en ambos sistemas.

Todos los usuarios de [!DNL Workfront] y [!DNL Jira] pueden beneficiarse de esta integración. Solo necesitan una licencia para el sistema en el que más trabajan, y no para ambos sistemas.

Este complemento está disponible para las versiones de [!UICONTROL Server] y [!UICONTROL OnDemand] (o [!UICONTROL Cloud]) del software [!DNL Jira]. Este complemento no está disponible para la versión [!DNL Data Center] del software [!DNL Jira].

Para obtener una lista de [!DNL Jira] versiones que [!DNL Workfront for Jira] admite actualmente, consulte [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) en Atlassian Marketplace.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> 
   <p>Nuevo: Cualquiera</p>
   <p>Actual: [!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Resumen de licencias de Adobe [!DNL Workfront]</td> 
   <td> 
   <p>Nuevo: estándar</p>
   <p>Actual: [!UICONTROL plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Se recomienda crear cuentas de administrador del sistema independientes en [!DNL Jira] y [!DNL Workfront] para dedicarlas a esta integración, en lugar de usar las existentes que podrían adjuntarse a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td><p>Debe ser administrador de [!DNL Workfront].</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Instalar [!DNL Workfront] para [!DNL Jira]

Instalar [!DNL Workfront] para [!DNL Jira] OnDemand es idéntico a instalarlo en una instancia de servidor [!DNL Jira].

Debe ser administrador de [!DNL Jira] para instalar el complemento [!DNL Workfront].

Si no es administrador de [!DNL Jira], puede buscar el complemento [!DNL Workfront] y solicitar que se instale. Su solicitud se envía al administrador de [!DNL Jira] para su aprobación e instalación.

Para obtener más información acerca de cómo solicitar la instalación de un complemento en la aplicación [!DNL Jira], vea [Administrar solicitudes de usuario para complementos.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Para instalar [!DNL Workfront for Jira]:

1. Inicie sesión en [!DNL Jira] como administrador de [!DNL Jira].
1. Busque el complemento **[!DNL Workfront for Jira]** en [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Haga clic en **[!UICONTROL Obtenerlo ahora]** para instalarlo.

   Una vez finalizada la instalación, puede iniciar sesión en [!DNL Workfront] desde [!DNL Jira] y configurar la integración.

   Para obtener más información, consulte [Configuración de Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Consideraciones para una instalación de [!DNL Jira Server]

>[!NOTE]
>
>Estos requisitos no se aplican a la versión de [!UICONTROL OnDemand] ([!UICONTROL Cloud]) del software [!DNL Jira].

Aunque la instalación del complemento [!DNL Workfront] en los dos entornos [!DNL Jira] es similar, debe tener en cuenta lo siguiente al trabajar con una instalación de [!DNL Jira Server]:

* Al configurar el complemento en [!DNL Jira], es posible que la dirección especificada en el campo **[!DNL JIRA Base URL]** no sea la misma URL que usa para obtener acceso a [!DNL Jira] en su servidor privado. **[!DNL JIRA Base URL]** debe ser una dirección de acceso público conectada a su servidor privado mediante protocolos NAT o de proxy inverso, de modo que [!DNL Workfront] pueda tener acceso a ella para realizar solicitudes al servidor.

* Debe utilizar el cifrado SSL para proteger la comunicación entre [!DNL Jira] y [!DNL Workfront]. Al habilitar SSL, debe tener una pila de certificados SSL completa de una autoridad de certificación. No se admiten certificados autofirmados.
* Debe asegurarse de que se puede obtener acceso al dominio [!DNL jira.workfront.com] desde los servidores corporativos. Sirve como entorno de middleware entre [!DNL Workfront] y [!DNL Jira] y es necesario para que funcione el complemento.

  También debe añadir las siguientes direcciones IP estáticas a la lista de permitidos del cortafuegos para conexiones salientes y entrantes.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Para obtener más información sobre cómo configurar el firewall para obtener una funcionalidad óptima con [!DNL Workfront], consulte [Configurar el firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
