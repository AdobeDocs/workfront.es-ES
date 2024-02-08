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
source-git-commit: 5f11e6ccda9fa3b37ec1300edb8f322521013a52
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# Configurar la información básica del sistema

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Como parte de la configuración del sistema de Adobe Workfront, puede administrar los detalles sobre su organización en la sección Información básica de la página Información del cliente.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   O
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

## Acceder a información del cliente

El cliente representa la instancia de Workfront para su organización. Las opciones de esta área son exclusivas suyas, como cliente de Workfront.

Para acceder a la página Información del cliente:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Sistema** > **Información del cliente**.

   Según el plan de Workfront que haya adquirido, es posible que falten algunas secciones de la página Información del cliente. Póngase en contacto con su representante de cuentas si necesita averiguar qué plan de Workfront utiliza su organización.

   Las secciones disponibles en el área Información del cliente son las siguientes:

   * **Información básica**

     Para obtener información sobre la configuración de información básica en Workfront, consulte [Configurar información básica](#configure-basic-info).

   * **Configuración de clave API**

     Para obtener información sobre la configuración de claves API, consulte [Administración de claves API](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **LISTA DE PERMITIDOS IP**

     Para obtener información sobre cómo agregar direcciones IP a la lista de permitidos para saber dónde pueden acceder los usuarios a Workfront, consulte [Configuración de la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **Licencia**

     Para obtener más información sobre las licencias, consulte [Administrar las licencias disponibles en el sistema](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## Configurar información básica {#configure-basic-info}

Dentro del área Información básica de la página Información del cliente, Workfront configura algunos detalles sobre el cliente y se muestran en modo de solo lectura. Usted puede configurar otros detalles. Cualquier opción que pueda editar en esta área tendrá un efecto global en todos los usuarios de Workfront.

Para configurar la sección Información básica en el área Información del cliente:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Sistema** > **Información del cliente**.

1. En el **Información básica** en la parte superior de la **Información del cliente** , busque la siguiente información sobre su instancia con Workfront:

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
      <td> <p>La dirección de correo electrónico del administrador de Workfront. Puede editar este campo para que coincida con la dirección de correo electrónico de uno de sus administradores de Workfront. El usuario asociado con esta dirección de correo electrónico se considera el administrador principal de Workfront de su sistema de Workfront. Cualquier comunicación de todo el sitio desde Workfront se dirige a esta dirección de correo electrónico, por lo que es importante mantenerla actualizada.</p> <p><b>NOTA</b>: no puede desactivar, eliminar ni cambiar el nivel de acceso del usuario asociado al correo electrónico del administrador.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dominio</td> 
      <td> <p>Workfront establece el dominio cuando se crea la cuenta.</p> <p>El dominio identifica el subdominio único de la dirección URL que utiliza para acceder a Workfront.<p>Por ejemplo, si a su organización se le ha asignado el dominio "mycompany", la URL que utiliza para acceder a Workfront es <i>https://mycompany.my.workfront.com.</i></p><p>No puede editar el dominio usted mismo. Si desea cambiar el dominio, puede ponerse en contacto con Asistencia al cliente de Workfront. Para obtener más información sobre cómo ponerse en contacto con Asistencia al cliente de Workfront, consulte <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contactar con Atención al cliente</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zona horaria</td> 
      <td> <p>Esta es la zona horaria predeterminada de la instancia de Workfront. Puede editar este campo para que coincida con la zona horaria de su ubicación principal de Workfront. La zona horaria que seleccione determina lo siguiente: </p> 
       <ul> 
        <li>La fecha y la hora mostradas en los correos electrónicos salientes</li> 
        <li>Zona horaria predeterminada para los nuevos usuarios cuando se crean</li> 
       </ul> <p>Los usuarios pueden modificar la zona horaria de su instancia de Workfront en su perfil. Cuando los usuarios modifican su zona horaria, la fecha y la hora de sus correos electrónicos desde Workfront coinciden con sus preferencias de perfil. Para obtener más información sobre la modificación de las preferencias de perfil de usuario, consulte <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurar mis ajustes</a>. Se selecciona como zona horaria predeterminada al crear una nueva programación. Para obtener más información sobre la creación de programaciones, consulte <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creación de una programación</a>.</p> <p>Para obtener información sobre el uso de programaciones para ayudar a los usuarios a colaborar en Workfront en diferentes zonas horarias, consulte <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Trabajo entre zonas horarias</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuración regional</td> 
      <td>Controla el idioma, la fecha y el formato de número utilizado en los mensajes de correo electrónico salientes. La configuración regional seleccionada aquí es la predeterminada cuando se crean nuevos usuarios. Los usuarios pueden modificar su configuración regional en el perfil de usuario. Cuando los usuarios modifican su configuración regional, el idioma, la fecha y el formato de número de sus correos electrónicos de Workfront coinciden con sus preferencias de perfil. Para obtener más información sobre cómo modificar las preferencias de perfil, consulte <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurar mis ajustes</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuota de almacenamiento</td> 
      <td> <p>Esta es la cantidad de espacio de almacenamiento de documentos disponible en la instancia de Workfront.<br>La cuota contiene documentos que se cargan directamente en Workfront.<br>No incluye:</p> 
       <ul> 
        <li>Documentos que vincula a Workfront desde cualquier otro proveedor de servicios de terceros (SharePoint, Google Drive, Webdam, Box, Dropbox o cualquier otro proveedor de administración de recursos de documentos).</li> 
        <li>Sus datos de Workfront (proyectos, tareas, problemas, usuarios, etc.).</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versión del producto</td> 
      <td>Este es el tipo de instancia de Workfront que se le ha asignado. La versión del producto para la mayoría de los clientes de Workfront es <strong>Empresa</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
