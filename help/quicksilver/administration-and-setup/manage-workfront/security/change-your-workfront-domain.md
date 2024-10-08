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
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Cambiar el dominio de Adobe Workfront

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica sólo a las organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, no es posible cambiar el dominio de Workfront.
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador de Adobe Workfront y contacto autorizado de Soporte de Workfront, puede solicitar ayuda al equipo de Soporte de Workfront para cambiar el dominio de Workfront de su organización.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Solicitar un cambio de dominio

1. Empiece a crear un vale de soporte en el Experience League.
1. En el cuadro **Descripción**, incluya el nuevo dominio que desee, así como el periodo de tiempo en el que desea que el nuevo dominio se active.
1. Termine de rellenar las casillas del caso de soporte y luego haga clic en **Enviar**.

También puede llamar al Soporte de Workfront para obtener ayuda sobre el cambio de dominio.

## Actualice el nuevo dominio si es cliente de SSO

Si su empresa utiliza SSO, se requieren los siguientes pasos después de cambiar el dominio de Workfront.

>[!NOTE]
>
>Esto no está disponible si la instancia de Workfront de su organización está habilitada con Adobe IMS. Consulte al administrador de red o de TI si necesita más información.

{{step-1-to-setup}}

1. En la barra lateral izquierda, haga clic en **Sistema** > **Información del cliente** y asegúrese de que su dominio se actualice en la página Información del cliente.

1. En la barra lateral izquierda, haga clic en **Sistema** > **Inicio de sesión único (SSO)**.

1. Haga clic en **Descargar metadatos de SAML 2.0**.
1. Una vez descargado el archivo, ábralo y asegúrese de lo siguiente:

   1. **entityID** señala al nuevo dominio.
   1. Todas las ubicaciones dentro de **`<md:AssertionConsumerService>`** apuntan al nuevo dominio.

1. Proporcione el archivo de metadatos descargado a su proveedor de identidad para que pueda actualizarlo por su cuenta.
1. Asegúrese de que el dominio esté actualizado para todas las integraciones de Workfront utilizadas por su organización.
