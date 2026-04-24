---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Cambiar el dominio de Adobe Workfront
description: Como administrador de Adobe Workfront y contacto autorizado de Soporte de Workfront, puede solicitar ayuda al equipo de Soporte de Workfront para cambiar el dominio de Workfront de su organización.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: be11c7417023ce2f310fce3e0cf77724d101b89e
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 19%

---

# Cambiar el dominio de Adobe Workfront

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplicaba únicamente a las organizaciones que aún no se habían incorporado a Admin Console. Dado que todas las organizaciones se han incorporado a Adobe Admin Console, **no es posible cambiar el dominio de Workfront**.
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración entre Adobe Workfront y Adobe Business Platform](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
>Este artículo se eliminará en breve.

Como administrador de Adobe Workfront y contacto autorizado de Soporte de Workfront, puede solicitar ayuda al equipo de Soporte de Workfront para cambiar el dominio de Workfront de su organización.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solicitar un cambio de dominio

1. Comience a crear un ticket de asistencia en Experience League.
1. En el cuadro **Descripción**, incluya el nuevo dominio que desee, así como el periodo de tiempo en el que desea que el nuevo dominio se active.
1. Termine de rellenar las casillas del caso de soporte y luego haga clic en **Enviar**.

También puede llamar al Soporte de Workfront para obtener ayuda sobre el cambio de dominio.

<!--

## Update the new domain if you are an SSO customer

If your company utilizes SSO, the following steps are required after you have your Workfront domain changed.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

{{step-1-to-setup}}

1. In the left sidebar, click **System** > **Customer Info** and make sure that your domain is updated on the Customer Info page.

1. In the left sidebar, click **System** > **Single Sign-On (SSO)**.

1. Click **Download SAML 2.0 Metadata**.
1. After the file is downloaded, open it and make sure of the following:

   1. **entityID** is pointing to the new domain.
   1. All locations within **`<md:AssertionConsumerService>`** point to the new domain.

1. Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.
1. Make sure the domain is updated for all Workfront integrations used by your organization.


-->
