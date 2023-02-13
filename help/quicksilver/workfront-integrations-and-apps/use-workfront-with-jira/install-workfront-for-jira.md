---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Instalar [!DNL Adobe Workfront] para [!DNL Jira]
description: Puede usar [!DNL Adobe Workfront] para [!DNL Jira] para integrar su [!DNL Jira] y [!DNL Workfront] sistemas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Instalar [!DNL Adobe Workfront for Jira]

Puede usar [!DNL Adobe Workfront for Jira] para integrar su [!DNL Jira] y [!DNL Workfront] sistemas.

Después de instalar el complemento, puede definir los flujos de trabajo que crean [!DNL Jira] se emite automáticamente cuando [!DNL Workfront] se crean elementos de trabajo. Los elementos de ambas aplicaciones se vinculan y parte de su información se puede actualizar automáticamente en ambos sistemas.

Todos los usuarios de [!DNL Workfront] y [!DNL Jira] puede beneficiarse de esta integración. Sólo necesitan una licencia para el sistema en el que funcionan más y no para ambos sistemas.

Este complemento está disponible para el [!UICONTROL Servidor] y [!UICONTROL OnDemand] (o [!UICONTROL Cloud]) versiones de [!DNL Jira] Software. Este complemento no está disponible para la variable [!DNL Data Center] versión de [!DNL Jira] Software.

Para obtener una lista de [!DNL Jira] versiones que [!DNL Workfront for Jira] admite actualmente, consulte [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) en el Atlassian Marketplace.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] información general sobre licencias</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Se recomienda crear cuentas de administrador del sistema independientes en [!DNL Jira] y [!DNL Workfront] para dedicarse a esta integración, en lugar de usar las existentes que se podrían adjuntar a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Instalar [!DNL Workfront] para [!DNL Jira]

Instalación [!DNL Workfront] para [!DNL Jira] OnDemand es idéntico a instalarlo en un [!DNL Jira] Instancia del servidor.

Debe ser [!DNL Jira] para instalar el [!DNL Workfront] complemento.

Si no es [!DNL Jira] administrador, puede buscar el [!DNL Workfront] y solicite que se instale. La solicitud se envía al [!DNL Jira] administrador para aprobación e instalación.

Para obtener más información sobre cómo solicitar la instalación de un complemento en su [!DNL Jira] aplicación, consulte [Administración de solicitudes de complementos de usuario.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Para instalar [!DNL Workfront for Jira]:

1. Iniciar sesión en [!DNL Jira] como [!DNL Jira] administrador.
1. Busque la **[!DNL Workfront for Jira]** en el [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Haga clic en **[!UICONTROL Consígalo ahora]** para instalarlo.

   Una vez finalizada la instalación, puede iniciar sesión en [!DNL Workfront] from [!DNL Jira] y configure la integración.
   [!DNL ]
Para obtener más información, consulte [Configuración de Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Consideraciones para un [!DNL Jira Server] instalación

>[!NOTE]
>
>Estos requisitos no se aplican al [!UICONTROL OnDemand] ([!UICONTROL Cloud]) versión de [!DNL Jira] Software.

Aunque se instala la variable [!DNL Workfront] en los dos [!DNL Jira] entornos similares, debe tener en cuenta lo siguiente al trabajar con un [!DNL Jira Server] instalación:

* Al configurar el complemento en [!DNL Jira], la dirección especificada en la variable **[!DNL JIRA Base URL]** puede que el campo no sea la misma dirección URL que utiliza para acceder a [!DNL Jira] en su servidor privado. La variable **[!DNL JIRA Base URL]** debe ser una dirección accesible al público conectada a su servidor privado mediante protocolos NAT o proxy inverso, por lo que [!DNL Workfront] puede acceder a él para realizar solicitudes al servidor.

* Debe utilizar el cifrado SSL para proteger la comunicación entre [!DNL Jira] y [!DNL Workfront]. Cuando habilite SSL, debe tener una pila de certificados SSL completa de una autoridad de certificación. No se admiten certificados con firma personal.
* Debe asegurarse de que la variable [!DNL jira.workfront.com] es accesible desde los servidores corporativos. Sirve como un entorno de software intermedio entre [!DNL Workfront] y [!DNL Jira] y es necesario para que funcione el complemento.

   También debe añadir las siguientes direcciones IP estáticas a la lista de permitidos del cortafuegos para las conexiones salientes e entrantes.

   `35.162.128.73`

   `34.213.36.118`

   `35.160.0.242`

   `3.209.27.146`

   `18.205.251.4`

   Para obtener más información sobre la configuración del cortafuegos para una funcionalidad óptima con [!DNL Workfront], consulte [Configuración del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
