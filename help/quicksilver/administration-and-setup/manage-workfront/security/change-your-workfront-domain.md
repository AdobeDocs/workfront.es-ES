---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Cambio del dominio de Adobe Workfront
description: Como administrador de Adobe Workfront y contacto autorizado de asistencia técnica de Workfront, puede solicitar ayuda al equipo de asistencia de Workfront para cambiar el dominio de Workfront de su organización.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: b413ffc2416439629e073b32b5e9828df2f5de90
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Cambio del dominio de Adobe Workfront

>[!IMPORTANT]
>
>El procedimiento descrito en esta página solo se aplica a organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Para cambiar el dominio de Adobe Workfront si su organización se ha incorporado a Adobe Admin Console, consulte [Configuración de dominios](https://helpx.adobe.com/enterprise/using/set-up-identity.html#setup-domains).
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador de Adobe Workfront y contacto autorizado de asistencia técnica de Workfront, puede solicitar ayuda al equipo de asistencia de Workfront para cambiar el dominio de Workfront de su organización.

## Requisitos de acceso

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
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solicitar un cambio de dominio

1. Haga clic en el **Asistencia** en la página Workfront One y, a continuación, empiece a crear un caso de asistencia.
1. En el **Descripción** , incluya el nuevo dominio que desee, así como el intervalo de tiempo en el que desee que se active el nuevo dominio.
1. Termine de rellenar las casillas del caso de asistencia y, a continuación, haga clic en **Submit**.

También puede llamar a la asistencia de Workfront para obtener ayuda para cambiar su dominio.

## Actualizar el nuevo dominio si es cliente de SSO

Si su empresa utiliza SSO, se requieren los siguientes pasos después de cambiar el dominio de Workfront.

>[!NOTE]
>
>Esto no está disponible si la instancia de Workfront de su organización está habilitada con Adobe IMS. Si necesita más información, consulte con su administrador de red o TI.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En la barra lateral izquierda, haga clic en **Sistema** > **Información del cliente** y asegúrese de que su dominio se actualiza en la página Información del cliente .

1. En la barra lateral izquierda, haga clic en **Sistema** > **Inicio de sesión único (SSO)**.

1. Haga clic en **Descargar metadatos de SAML 2.0**.
1. Una vez descargado el archivo, ábralo y asegúrese de lo siguiente:

   1. **entityID** señala al nuevo dominio.
   1. Todas las ubicaciones dentro de **`<md:AssertionConsumerService>`** dirija al nuevo dominio.

1. Proporcione el archivo de metadatos descargado a su proveedor de identidad para que pueda actualizarlo en su extremo.
1. Asegúrese de que el dominio se actualice para todas las integraciones de Workfront que utilice su organización.
