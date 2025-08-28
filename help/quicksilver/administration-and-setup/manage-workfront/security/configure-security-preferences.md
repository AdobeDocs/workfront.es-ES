---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurar preferencias del sistema
description: Como administrador de Adobe Workfront, puede configurar las preferencias de su sistema Workfront, incluidas las preferencias de seguridad.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: cb9a6536c4995080887032aa84539eff040338f8
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 75%

---

# Configurar preferencias del sistema

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{important-admin-console-onboard}}

Como administrador de Adobe Workfront, puede configurar las preferencias de su sistema Workfront, lo que incluye:

* Acceso a Workfront desde aplicaciones móviles y otras aplicaciones integradas
* Reglas para incrustar Workfront en un iframe

Los cambios que realice en las preferencias del sistema afectan a todos los usuarios del sistema y a su experiencia en Workfront.

Le recomendamos que configure las preferencias del sistema durante la implementación de Workfront y que solo las vuelva a consultar ocasionalmente después de dicha implementación.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuración de las preferencias del sistema

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Sistema** > **Preferencias**.

1. Seleccione cualquiera de los siguientes campos para establecer la configuración de su organización:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Permitir un proceso de publicación rápida</p> </td> 
      <td>Permite habilitar versiones mensuales de Workfront para su organización en lugar de versiones trimestrales.</p><p>Para obtener más información sobre el proceso de publicación rápida, consulte <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">Habilitar o deshabilitar las publicaciones rápidas para su organización</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Permitir una incrustación en Workfront en un iframe</p> </td> 
      <td>Permite incrustar Workfront en un iframe.<p>Esta opción está desactivada de forma predeterminada.</p><p><b>IMPORTANTE</b>: si se muestra una aplicación basada en web en un iframe, la aplicación será susceptible a una vulnerabilidad de seguridad por secuestro de clics.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir la autenticación SAML 2.0 en los complementos de Office 365</td> 
      <td> <p>Le permite incrustar Workfront en un iframe solo para complementos de Office 365 cuando Workfront está integrado con una solución de inicio de sesión único de SAML 2.0. </p> <p>Esta opción está habilitada de forma predeterminada.</p> <p><b>NOTA</b>: Si habilita la opción anterior, <strong>Permitir incrustación de Workfront en un iframe</strong>, la opción <strong>Permitir autenticación SAML 2.0 en complementos de Office 365</strong> se habilitará y se atenuará.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Habilite el uso de la información de sesión al crear direcciones URL de páginas externas.</td> 
      <td> <p>Permite a los usuarios utilizar la información de ID de sesión de un sitio al añadir una página externa a un panel.</p> <p>Esta opción no es segura y está desactivada de forma predeterminada. Se recomienda utilizar en su lugar OAuth para integraciones.</p> <p>Para obtener más información sobre cómo añadir páginas externas a un panel, consulte <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Incrustar una página web externa en un panel</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permita que los usuarios usen las aplicaciones móviles de Workfront y el complemento Workfront Outlook.</td> 
      <td> <p>Permite a los usuarios acceder a las aplicaciones móviles (vista de Workfront para aplicaciones de iPad y de teléfonos móviles) y a la aplicación de Workfront Outlook.</p> <p>Esta opción está habilitada de forma predeterminada. </p> <p>Para obtener información sobre la vista de Workfront, consulte <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Utilizar la vista de Adobe Workfront</a>. Para obtener más información acerca de las aplicaciones móviles, consulte <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Usar la aplicación móvil de Adobe Workfront: índice de artículos</a>.</p> <p>Para obtener más información sobre el complemento de Outlook, consulte <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Configurar Adobe Workfront para Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Colaborar con usuarios sin cuentas Workfront mediante el uso de sus direcciones de correo electrónico.</p> </td> 
      <td>Permite a los usuarios de Workfront compartir ciertos elementos con usuarios sin cuenta de Workfront incluyendo su dirección de correo electrónico en lugar de su nombre. Los usuarios pueden compartir los siguientes elementos con usuarios externos mediante su dirección de correo electrónico:
       <ul>
        <li>Documento<br></li>
        <li>Solicitud de documento<br></li>
        <li>Aprobación de documento</li>
        <li>Calendario</li>
       </ul><p>Esta opción está habilitada de forma predeterminada.</p> <p><b>Importante</b>: el nivel de acceso de usuario externo no está disponible en la instancia de Workfront si esta opción está deshabilitada. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Niveles de acceso integrados</a>.</p> </td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Require external users to register with a password</td> 
      <td> <p>Requires external users to register before they are able to view items in Workfront. By default, this option is disabled. When you enable this option, people without a Workfront account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> -->
     <tr> 
      <td role="rowheader">URL de ayuda personalizada</td> 
      <td>Permite definir un sitio de ayuda personalizado interno al que se dirigirá el icono de ayuda del menú principal. Para obtener más información, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Configurar una dirección URL de ayuda personalizada</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Habilitar la lista de trabajo Prioridades </td> 
      <td>Permite habilitar o deshabilitar la experiencia de lista de trabajo Prioridades para los usuarios. Los usuarios seguirán viendo los iconos de Prioridades en Workfront, pero no tendrán acceso a la funcionalidad. Para obtener más información acerca de Prioridades, vea <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Introducción a Prioridades</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Habilitar IA </td> 
      <td>Permite habilitar la IA, incluido el Asistente de IA. <p><b>Nota</b>: su organización debe cumplir con los requisitos específicos para habilitar IA. Para obtener más información acerca de la IA, incluidos los requisitos, consulte <a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md">Descripción general del Asistente para IA</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Completar automáticamente el formulario </td> 
      <td>Permite habilitar la capacidad de rellenar automáticamente formularios de solicitud basados en datos de solicitudes anteriores. Para obtener más información acerca de la cumplimentación automática de formularios, vea <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">Rellenar automáticamente una solicitud de datos anteriores</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Inclusión en las apuestas de IA </td> 
      <td>Permite habilitar las funciones de IA que se encuentran actualmente en Beta. Si activa esta opción, puede seleccionar qué funciones de AI Beta desea habilitar. Para obtener más información acerca de cada función de AI Beta, haga clic en el icono de información situado junto a ella.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Entornos de prueba</td> 
      <td>Permite acceder a los entornos de prueba de Workfront. Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">Entorno de la zona protegida de previsualización de Adobe Workfront</a>.</p></td> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

   Los cambios que ha guardado aquí afectan a la experiencia de todos los usuarios de Workfront y de cualquier persona que interactúe con el sistema como usuario externo.
