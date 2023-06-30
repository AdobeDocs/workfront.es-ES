---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurar las preferencias de seguridad del sistema
description: Como administrador de Adobe Workfront, puede configurar las preferencias de seguridad de su sistema Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 9f6338dc79740e13b71e9266fed17f6dc61039e1
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 5%

---

# Configurar las preferencias del sistema

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{highlighted-preview}}

{{important-admin-console-onboard}}

Como administrador de Adobe Workfront, puede configurar las preferencias de su sistema Workfront:

* Acceso a Workfront desde aplicaciones móviles y otras aplicaciones integradas
* Reglas para incrustar Workfront en un iframe

Los cambios que realice en las preferencias del sistema afectan a todos los usuarios del sistema y a su experiencia en Workfront.

Le recomendamos que configure las preferencias del sistema durante la implementación de Workfront y que solo las vuelva a consultar ocasionalmente después de dicha implementación.

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
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar las preferencias del sistema

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Sistema** > **Preferencias**.

1. Seleccione cualquiera de los siguientes campos para establecer la configuración de su organización:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p><span class="preview">Habilitar proceso de revisión rápido</span></p> </td> 
      <td><span class="preview">Permite habilitar versiones mensuales de Workfront para su organización en lugar de versiones trimestrales.</p><p>Para obtener más información sobre el proceso de liberación rápida, consulte <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Activar o desactivar las versiones rápidas para su organización</a>.</span></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Permitir incrustación de <strong>Workfront</strong> en un iframe</p> </td> 
      <td>Permite incrustar Workfront en un iframe.<p>Esta opción está desactivada de forma predeterminada.</p><p><b>IMPORTANTE</b>: La visualización de una aplicación basada en web en un iframe hace que la aplicación sea susceptible a una vulnerabilidad de seguridad por secuestro de clics.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir la autenticación SAML 2.0 en los complementos de Office 365</td> 
      <td> <p>Le permite incrustar Workfront en un iframe solo para complementos de Office 365 cuando Workfront está integrado con una solución de inicio de sesión único de SAML 2.0. </p> <p>Esta opción está habilitada de forma predeterminada.</p> <p><b>NOTA</b>: Si activa la opción anterior, <strong>Permitir incrustación de Workfront en un iframe</strong>, la opción <strong>Permitir la autenticación SAML 2.0 en los complementos de Office 365</strong> está activada y atenuada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Habilitar el uso de la información de sesión al crear direcciones URL de páginas externas</td> 
      <td> <p>Permite a los usuarios utilizar la información de ID de sesión de un sitio al añadir una página externa a un panel.</p> <p>Para obtener más información sobre cómo agregar páginas externas a un panel, consulte <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Incrustar una página web externa en un panel</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que los usuarios usen las aplicaciones móviles de Workfront y <strong>Workfront</strong> Complemento de Outlook</td> 
      <td> <p>Permite a los usuarios acceder a las aplicaciones móviles (vista de Workfront para aplicaciones de iPad y de teléfonos móviles) y a la aplicación de Workfront Outlook.</p> <p>Esta opción está habilitada de forma predeterminada. </p> <p>Para obtener información sobre la vista de Workfront, consulte <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Utilizar la vista de Adobe Workfront</a>. Para obtener más información sobre las aplicaciones móviles, consulte <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Uso de la aplicación móvil de Adobe Workfront</a>.</p> <p>Para obtener más información sobre el complemento de Outlook, consulte <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Configuración de Adobe Workfront para Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Colaborar con usuarios sin cuentas de Workfront mediante el uso de direcciones de correo electrónico</p> </td> 
      <td>Permite a los usuarios de Workfront compartir ciertos elementos con usuarios sin cuenta de Workfront incluyendo su dirección de correo electrónico en lugar de su nombre. Los usuarios pueden compartir los siguientes elementos con usuarios externos mediante su dirección de correo electrónico:
       <ul>
        <li>Documento<br></li>
        <li>Solicitud de documento<br></li>
        <li>Aprobación de documento</li>
        <li>Calendario</li>
       </ul><p>Esta opción está habilitada de forma predeterminada.</p> <p><b>Importante</b>: el nivel de acceso de usuario externo no está disponible en la instancia de Workfront si esta opción está desactivada. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Niveles de acceso integrados en Workfront</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requiera que los usuarios externos se registren con una contraseña</td> 
      <td> <p>Requiere que los usuarios externos se registren antes de poder ver los elementos en Workfront. Esta opción está desactivada de forma predeterminada. Al habilitar esta opción, se solicitará a las personas sin cuenta de Workfront incluidas en determinadas actualizaciones por su dirección de correo electrónico que creen una cuenta antes de poder ver el artículo en el que están incluidas. Esto crea una cuenta de usuario externo para ellos.</p> <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cerrar automáticamente la sesión de los usuarios después de</td> 
      <td> Permite especificar cuándo se cierra la sesión de un usuario en Workfront tras un periodo de inactividad. De forma predeterminada, la sesión de los usuarios se cierra tras ocho horas de inactividad. <p>Esta opción también afecta a los clientes de Workfront que utilizan una solución de inicio de sesión único.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cerrar automáticamente la sesión de los usuarios de dispositivos móviles después de </td> 
      <td>Permite especificar cuándo se cierra la sesión de un usuario de la aplicación Workfront tras un periodo de inactividad. De forma predeterminada, la sesión de los usuarios se cierra tras 7 días de inactividad. <p>Esta opción también afecta a los clientes de Workfront que utilizan una solución de inicio de sesión único.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Los usuarios del sistema verán de forma predeterminada la experiencia Nueva página de inicio </td> 
      <td>Permite especificar si los usuarios verán la experiencia Nueva página de inicio de forma predeterminada. En cualquier caso, los usuarios pueden optar por habilitar o deshabilitar el Nuevo Inicio de forma individual. Esta opción está habilitada de forma predeterminada.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

   Los cambios que ha guardado aquí afectan a la experiencia de todos los usuarios de Workfront y de cualquier persona que interactúe con ellos como usuario externo.
