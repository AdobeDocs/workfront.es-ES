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
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/46D3BBajFk39FP-dMDk0SuSSGM5nYPKas11Bs159R9Y
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9d28f52ace4d443bdffc475baf79d482152d4157
workflow-type: tm+mt
source-wordcount: 964
ht-degree: 57%

---

# Configurar preferencias del sistema

{{preview-fast-release-general}}

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
      <td> <p>Permite a los usuarios utilizar la información de ID de sesión de un sitio al añadir una página externa a un panel de control.</p> <p>Esta opción no es segura y está desactivada de forma predeterminada. Se recomienda utilizar en su lugar OAuth para integraciones.</p> <p>Para obtener más información sobre cómo añadir páginas externas a un panel de control, consulte <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Incrustar una página web externa en un panel de control</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que los usuarios usen las aplicaciones móviles de Workfront</td> 
      <td> <p>Permite a los usuarios acceder a las aplicaciones móviles (vista de Workfront para aplicaciones de iPad y de teléfonos móviles)</p> <p>Esta opción está habilitada de forma predeterminada. </p> <p>Para obtener información sobre la vista de Workfront, consulte <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Utilizar la vista de Adobe Workfront</a>. Para obtener más información acerca de las aplicaciones móviles, consulte <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Usar la aplicación móvil de Adobe Workfront: índice de artículos</a>.</p> </td> 
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
     <!--
     <tr> 
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
     </tr>
     -->
     <tr> 
      <td role="rowheader">URL de ayuda personalizada</td> 
      <td>Permite definir un sitio de ayuda personalizado interno al que se dirigirá el icono de ayuda del menú principal. Para obtener más información, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Configurar una dirección URL de ayuda personalizada</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Habilitar la lista de trabajo Prioridades </td> 
      <td>Permite habilitar o deshabilitar la experiencia de lista de trabajo Prioridades para los usuarios. Los usuarios seguirán viendo los iconos de Prioridades en Workfront, pero no tendrán acceso a la funcionalidad. Para obtener más información acerca de Prioridades, vea <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Introducción a Prioridades</a>.</td> 
     </tr>
     <tr>
      <td><span class="preview">Aplicar siempre los campos obligatorios en la edición por lotes</span></td>
      <td><span class="preview"><p>Permite elegir si se fuerza a los usuarios a introducir información en los campos obligatorios al editar objetos por lotes.</p> <p>Si se selecciona esta opción, los campos obligatorios deben tener valores antes de guardarlos en el modo de edición por lotes. Si en el campo obligatorio falta un valor para al menos un objeto seleccionado en bloque, no se permite guardar.</p> <p>Cuando esta opción no está seleccionada, los campos obligatorios solo se aplican cuando un usuario modifica el campo. Si un campo no se modifica, se trata como opcional y no se valida.</p></span></td>
     </tr>
     <tr> 
      <td role="rowheader">Habilitar el almacenamiento en la nube de Adobe </td> 
      <td>Permite habilitar o deshabilitar el almacenamiento en la nube de Adobe para toda la organización o para grupos específicos. Para obtener más información sobre el almacenamiento en la nube de Adobe, consulte <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md">Habilitar el almacenamiento en la nube de Adobe para su organización</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Seleccione portafolios para convertirlos en almacenamiento en la nube de Adobe </td> 
      <td>Permite convertir portafolios de almacenamiento de Workfront heredados existentes al almacenamiento en la nube de Adobe. Para obtener más información, consulte <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md">Convertir portafolios heredados al almacenamiento en la nube de Adobe</a>.</td> 
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
      <td role="rowheader">Inclusión a las betas de IA </td> 
      <td>Permite habilitar las funciones de IA que se encuentran actualmente en Beta. Si activa esta opción, puede seleccionar qué funciones de AI Beta desea habilitar. Para obtener más información acerca de cada función de AI Beta, haga clic en el icono de información situado junto a ella.</td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Herramientas MCP de solo lectura</span></td> 
      <td><span class="preview">Permite que el servidor MCP de Workfront realice acciones de lectura en los datos de Workfront como, por ejemplo, buscar o enumerar proyectos, tareas u otros elementos. Esta opción está habilitada de forma predeterminada.<p>Para obtener más información sobre el servidor MCP de Workfront, consulte <a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">Configuración del servidor MCP de Adobe Workfront</a>.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Herramientas MCP de escritura</span></td> 
      <td><span class="preview">Permite que el servidor MCP de Workfront realice acciones de creación, actualización y eliminación en los datos de Workfront. Esta opción está desactivada de forma predeterminada.<p>Para obtener más información sobre el servidor MCP de Workfront, consulte <a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">Configuración del servidor MCP de Adobe Workfront</a>.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader">Entornos de prueba</td> 
      <td>Permite acceder a los entornos de prueba de Workfront. Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">Entorno de la zona protegida de previsualización de Adobe Workfront</a>.</p></td> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

   Los cambios que ha guardado aquí afectan a la experiencia de todos los usuarios de Workfront y de cualquier persona que interactúe con el sistema como usuario externo.
