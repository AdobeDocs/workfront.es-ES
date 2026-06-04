---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurar la información básica del sistema
description: Como parte de la configuración del sistema de Adobe Workfront, puede administrar los detalles sobre su organización en la sección Información básica de la página Información del cliente.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
last-update: 2026-04-29T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/4536sfZCe8ugbGGuFUQeyFXnNNifG0e5MZ4npIlH1iI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 766
ht-degree: 10%

---

# Configurar la información básica del sistema

{{highlighted-preview}}

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Como parte de la configuración del sistema de Adobe Workfront, puede administrar los detalles sobre su organización en la sección Información básica de la página Información del cliente.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Acceder a información del cliente

El cliente representa la instancia de Workfront para su organización. Las opciones de esta área son exclusivas suyas, como cliente de Workfront.

Para acceder a la página Información del cliente:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Sistema** > **Información del cliente**.

   Según el paquete de Workfront que haya adquirido, es posible que falten algunas secciones de la página Información del cliente. Póngase en contacto con su representante de cuentas si necesita averiguar qué paquete de Workfront utiliza su organización.

   Las secciones disponibles en el área Información del cliente son las siguientes:

   | Sección | Más información |
   |---------|-----------------|
   | **Información básica** | Para obtener información acerca de cómo configurar información básica en Workfront, vea [Configurar información básica](#configure-basic-info). |
   | <span class="preview">**Información general sobre almacenamiento**</span> | <span class="preview">Para obtener información acerca de cómo comprobar el uso y la cuota del almacenamiento de documentos, vea [Comprobar los límites del almacenamiento de documentos](../../documents/managing-documents/check-document-storage.md).</span> |
   | **Configuración de clave API** | Para obtener información acerca de la configuración de claves API, consulte [Administrar claves API](../../administration-and-setup/manage-workfront/security/manage-api-keys.md). |
   | **Lista de permitidos IP** | Para obtener información acerca de cómo agregar direcciones IP a la lista de permitidos para que los usuarios tengan acceso a Workfront, consulte [Configuración de la lista de permitidos del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md). |
   | **Lista de permitidos por correo electrónico** | Para obtener información sobre cómo agregar correos electrónicos a la lista de permitidos, consulte [Configuración de la lista de permitidos por correo electrónico](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md). |

   <!--
   * **License**

     For information about licenses, see [Manage available licenses in your system](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
     -->

## Configurar información básica {#configure-basic-info}

Dentro del área Información básica de la página Información del cliente, Workfront configura algunos detalles sobre el cliente y se muestran en modo de solo lectura. Usted puede configurar otros detalles. Cualquier opción que pueda editar en esta área tendrá un efecto global en todos los usuarios de Workfront.

Para configurar la sección Información básica en el área Información del cliente:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Sistema** > **Información del cliente**.

1. En la sección **Información básica** de la parte superior de la página **Información del cliente**, encuentre la siguiente información sobre su instancia con Workfront:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td>El nombre de su organización, que también coincide con el nombre de su compañía. Workfront lo añade y no se puede editar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuración de clúster </td> 
      <td>El número de clúster de la instancia.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Correo electrónico de administrador</td> 
      <td> <p>La dirección de correo electrónico del administrador de Workfront. Puede editar este campo para que coincida con la dirección de correo electrónico de uno de sus administradores de Workfront. El usuario asociado con esta dirección de correo electrónico se considera el administrador principal de Workfront de su sistema de Workfront. Cualquier comunicación de todo el sitio desde Workfront se dirige a esta dirección de correo electrónico, por lo que es importante mantenerla actualizada.</p> <p><b>NOTA</b>: no puede desactivar, eliminar ni cambiar el nivel de acceso del usuario asociado con el correo electrónico del administrador.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dominio</td> 
      <td> <p>Workfront establece el dominio cuando se crea la cuenta.</p> <p>El dominio identifica el subdominio único de la dirección URL que utiliza para acceder a Workfront.<p>Por ejemplo, si a su organización se le ha asignado el dominio "mycompany", la dirección URL que utiliza para acceder a Workfront es <i>https://mycompany.my.workfront.com.</i></p><p>No puede editar el dominio usted mismo. Si desea cambiar el dominio, puede ponerse en contacto con Asistencia al cliente de Workfront. Para obtener más información sobre cómo ponerse en contacto con la Atención al cliente de Workfront, consulte <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contactar con la Atención al cliente</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zona horaria</td> 
      <td> <p>Esta es la zona horaria predeterminada de la instancia de Workfront. Puede editar este campo para que coincida con la zona horaria de su ubicación principal de Workfront. La zona horaria que seleccione determina lo siguiente: </p> 
       <ul> 
        <li>La fecha y la hora mostradas en los correos electrónicos salientes</li> 
        <li>Zona horaria predeterminada para los nuevos usuarios cuando se crean</li> 
       </ul> <p>Los usuarios pueden modificar la zona horaria de su instancia de Workfront en su perfil. Cuando los usuarios modifican su zona horaria, la fecha y la hora de sus correos electrónicos desde Workfront coinciden con sus preferencias de perfil. Para obtener más información acerca de cómo modificar las preferencias del perfil de usuario, vea <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurar mis opciones</a>. Se selecciona como zona horaria predeterminada al crear una nueva programación. Para obtener más información acerca de cómo crear programaciones, vea <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>.</p> <p>Para obtener información sobre cómo usar las programaciones para ayudar a los usuarios a colaborar en Workfront en diferentes zonas horarias, consulte <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Uso entre zonas horarias</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuración regional predeterminada del correo electrónico</td> 
      <td>Controla el idioma, la fecha y el formato de número utilizado en los mensajes de correo electrónico salientes. La configuración regional seleccionada aquí es la predeterminada cuando se crean nuevos usuarios. Los usuarios pueden modificar su configuración regional en el perfil de usuario. Cuando los usuarios modifican su configuración regional, el idioma, la fecha y el formato de número de sus correos electrónicos de Workfront coinciden con sus preferencias de perfil. Para obtener más información acerca de cómo modificar las preferencias de perfil, consulte <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurar mi configuración</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
