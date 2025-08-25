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
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 75%

---

# Configurar preferencias del sistema

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

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
     <tr> 
      <td role="rowheader">Solicite a los usuarios externos que se registren con una contraseña.</td> 
      <td> <p>Requiere que los usuarios externos se registren antes de poder ver los elementos en Workfront. Esta opción está desactivada de forma predeterminada. Al habilitar esta opción, se solicitará a los usuarios sin cuenta de Workfront incluidos en determinadas actualizaciones por su dirección de correo electrónico que creen una cuenta antes de poder ver el elemento en el que están incluidas. Esto crea una cuenta de usuario externo para ellas.</p> <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr>
<!-- DELETE THIS SECTION MARCH 2026   <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr>  -->
    &lt;tr>
    &lt;td role=&quot;rowheader&quot;>URL de ayuda personalizada&lt;/td>
    &lt;td>Permite definir un sitio de ayuda personalizado interno al que se dirigirá el icono de ayuda del menú principal. Para obtener más información, consulte &lt;a href=&quot;/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md&quot;>Configuración de una URL de ayuda personalizada&lt;/a>.&lt;/p>&lt;/td>
    &lt;/tr>
    &lt;tr>
    &lt;td role=&quot;rowheader&quot;>Los usuarios del sistema verán de forma predeterminada la nueva experiencia de inicio &lt;/td>
    &lt;td>Permite especificar si los usuarios verán la nueva experiencia de inicio de forma predeterminada. Cuando se habilita, los usuarios verán la experiencia Nueva página de inicio de forma predeterminada, pero aún pueden optar por habilitar o deshabilitar la Nueva página de inicio de forma individual. Cuando está desactivado, los usuarios no verán el banner que les permite cambiar a la nueva página de inicio; sin embargo, aún pueden navegar a su nueva página de inicio introduciendo manualmente &lt;code>/home/workspaces&lt;/code> al final de su URL de instancia. Esta opción está desactivada de forma predeterminada.&lt;/td>
    &lt;/tr>
    &lt;tr>
    &lt;td role=&quot;rowheader&quot;>Habilitar la lista de trabajo de prioridades &lt;/td>
    &lt;td>Permite habilitar o deshabilitar la experiencia de la lista de trabajo de prioridades para los usuarios. Los usuarios seguirán viendo los iconos de Prioridades en Workfront, pero no tendrán acceso a la funcionalidad. Para obtener más información acerca de Prioridades, consulte &lt;a href=&quot;/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md&quot;>Introducción a Prioridades&lt;/a>.&lt;/td>
    &lt;/tr>
    &lt;tr>
    &lt;td role=&quot;rowheader&quot;>Entornos de prueba&lt;/td>
    &lt;td>Le permite acceder a sus entornos de prueba de Workfront. Para obtener más información, consulte &lt;a href=&quot;/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md&quot;>Entorno de zona protegida de vista previa de Adobe Workfront&lt;/a>.&lt;/p>&lt;/td>
    &lt;/tbody>
</table>

1. Haga clic en **Guardar**.

   Los cambios que ha guardado aquí afectan a la experiencia de todos los usuarios de Workfront y de cualquier persona que interactúe con el sistema como usuario externo.
