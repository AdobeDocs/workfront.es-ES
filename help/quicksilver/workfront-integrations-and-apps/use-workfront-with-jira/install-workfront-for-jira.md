---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Instalar [!DNL Adobe Workfront] para [!DNL Jira]
description: Puede utilizar [!DNL Adobe Workfront] para [!DNL Jira] para integrar su [!DNL Jira] y [!DNL Workfront] sistemas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: b98a7fa48e60f1f2c2ea938b14b88e0c5a2ee418
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Instalar [!DNL Adobe Workfront for Jira]

Puede utilizar [!DNL Adobe Workfront for Jira] para integrar su [!DNL Jira] y [!DNL Workfront] sistemas.

Después de instalar el complemento, puede definir los flujos de trabajo que crean [!DNL Jira] problemas automáticamente al [!DNL Workfront] los elementos de trabajo se crean. Los elementos de ambas aplicaciones se vinculan y parte de su información se puede actualizar automáticamente en ambos sistemas.

Todos los usuarios en [!DNL Workfront] y [!DNL Jira] puede beneficiarse de esta integración. Solo necesitan una licencia para el sistema en el que más trabajan, y no para ambos sistemas.

Este complemento está disponible para el [!UICONTROL Servidor] y [!UICONTROL OnDemand] (o [!UICONTROL Nube]) versiones de [!DNL Jira] Software. Este complemento no está disponible para el [!DNL Data Center] versión de [!DNL Jira] Software.

Para obtener una lista de [!DNL Jira] versiones que [!DNL Workfront for Jira] admite actualmente, consulte [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) en Atlassian Marketplace.

## Requisitos de acceso

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
   <td role="rowheader">Adobe [!DNL Workfront] información general sobre licencias</td> 
   <td> 
   <p>Nuevo: estándar</p>
   <p>Actual: [!UICONTROL plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Le recomendamos que cree cuentas de administrador del sistema independientes en [!DNL Jira] y [!DNL Workfront] para dedicarse a esta integración, en lugar de utilizar las existentes que podrían adjuntarse a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td><p>Debe ser un [!DNL Workfront] administrador.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Instalar [!DNL Workfront] para [!DNL Jira]

Instalación [!DNL Workfront] para [!DNL Jira] OnDemand es idéntico a instalarlo en un [!DNL Jira] Instancia de servidor.

Debe ser un [!DNL Jira] para instalar el [!DNL Workfront] complemento de.

Si no es un [!DNL Jira] administrador, puede buscar el [!DNL Workfront] y solicite que se instale. Su solicitud se enviará a [!DNL Jira] administrador para la aprobación y la instalación.

Para obtener más información sobre cómo solicitar la instalación de un complemento en su [!DNL Jira] aplicación, consulte [Administración de solicitudes de usuario para complementos.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Para instalar [!DNL Workfront for Jira]:

1. Iniciar sesión en [!DNL Jira] as a [!DNL Jira] administrador.
1. Busque el **[!DNL Workfront for Jira]** complemento de en el [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Clic **[!UICONTROL Consíguelo ahora]** para instalarlo.

   Una vez finalizada la instalación, puede iniciar sesión en [!DNL Workfront] de [!DNL Jira] y configure la integración.

   Para obtener más información, consulte [Configuración de Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Consideraciones para un [!DNL Jira Server] instalación

>[!NOTE]
>
>Estos requisitos no se aplican al [!UICONTROL OnDemand] ([!UICONTROL Nube]) versión de [!DNL Jira] Software.

Aunque instale el [!DNL Workfront] complemento en los dos [!DNL Jira] entornos es similar, debe tener en cuenta lo siguiente al trabajar con un [!DNL Jira Server] instalación:

* Al configurar el complemento en [!DNL Jira], la dirección especificada en la **[!DNL JIRA Base URL]** Este campo puede no ser la misma URL que utiliza para acceder a [!DNL Jira] en su servidor privado. El **[!DNL JIRA Base URL]** debe ser una dirección de acceso público conectada al servidor privado mediante protocolos NAT o de proxy inverso, por lo que [!DNL Workfront] Puede acceder a él para realizar solicitudes al servidor.

* Debe utilizar el cifrado SSL para proteger la comunicación entre [!DNL Jira] y [!DNL Workfront]. Al habilitar SSL, debe tener una pila de certificados SSL completa de una autoridad de certificación. No se admiten certificados autofirmados.
* Debe asegurarse de que la variable [!DNL jira.workfront.com] es accesible desde los servidores corporativos. Sirve como entorno de middleware entre [!DNL Workfront] y [!DNL Jira] y es necesario para que funcione el complemento.

  También debe añadir las siguientes direcciones IP estáticas a la lista de permitidos del cortafuegos para conexiones salientes y entrantes.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Para obtener más información sobre la configuración del cortafuegos para obtener una funcionalidad óptima con [!DNL Workfront], consulte [Configuración del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
