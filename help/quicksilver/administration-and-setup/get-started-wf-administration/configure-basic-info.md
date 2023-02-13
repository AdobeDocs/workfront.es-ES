---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurar información básica para el sistema
description: Como parte de la configuración del sistema de Adobe Workfront, puede administrar los detalles de su organización en la sección Información básica de la página Información del cliente .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 2%

---

# Configurar información básica para el sistema

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Como parte de la configuración del sistema de Adobe Workfront, puede administrar los detalles de su organización en la sección Información básica de la página Información del cliente .

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Acceso a la información del cliente

El cliente representa la instancia de Workfront de su organización. Las opciones de esta área son únicas para usted, como cliente de Workfront.

Para acceder a la página Información del cliente:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Sistema** > **Información del cliente**.

   Según el plan de Workfront que haya comprado, es posible que falten algunas secciones en la página Información del cliente. Póngase en contacto con su representante de cuentas si necesita saber qué plan de Workfront utiliza su organización.

   Las secciones disponibles en el área Información del cliente son:

   * **Información básica**

      Para obtener información sobre la configuración de información básica en Workfront, consulte [Configurar información básica](#configure-basic-info).

   * **Configuración de clave API**

      Para obtener información sobre la configuración de claves de API, consulte [Administrar claves de API](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **Lista de direcciones IP permitidas**

      Para obtener información sobre cómo agregar direcciones IP a la lista de permitidos para ver dónde pueden acceder los usuarios a Workfront, consulte [Configurar la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **Licencia**

      Para obtener información sobre las licencias, consulte [Administre las licencias disponibles en su sistema](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## Configurar información básica {#configure-basic-info}

En el área Información básica de la página Información del cliente , Workfront configura algunos detalles sobre el cliente y se muestran en modo de solo lectura. Usted puede configurar otros detalles. Las opciones que puede editar en esta área tienen un efecto global en todos los usuarios de Workfront.

Para configurar la sección Información básica en el área Información del cliente:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Sistema** > **Información del cliente**.

1. En el **Información básica** en la parte superior del **Información del cliente** busque la siguiente información sobre su instancia con Workfront:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td>El nombre de su organización, que también coincide con el nombre de su empresa. Workfront lo agrega y no se puede editar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuración de clúster </td> 
      <td>El número de clúster de la instancia.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Correo electrónico de administrador</td> 
      <td> <p>La dirección de correo electrónico del administrador de Workfront. Puede editar este campo para que coincida con la dirección de correo electrónico de uno de los administradores de Workfront. El usuario asociado con esta dirección de correo electrónico se considera el administrador principal de Workfront de su sistema Workfront. Cualquier comunicación de Workfront a nivel de sitio se dirige a esta dirección de correo electrónico, por lo que es importante mantenerla actualizada.</p> <p><b>NOTA</b>: No puede desactivar, eliminar ni cambiar el nivel de acceso del usuario asociado al correo electrónico del administrador.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dominio</td> 
      <td> <p>Workfront establece el dominio cuando se crea la cuenta.</p> <p>El dominio identifica su subdominio único de la URL que utiliza para acceder a Workfront.<p>Por ejemplo, si a su organización se le ha asignado el dominio "mycompany", la dirección URL que utiliza para acceder a Workfront es <i>https://mycompany.my.workfront.com.</i></p><p>No puede editar el dominio usted mismo. Si desea cambiar su dominio, puede ponerse en contacto con el servicio de atención al cliente de Workfront. Para obtener más información sobre cómo ponerse en contacto con el servicio de asistencia al cliente de Workfront, consulte <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contactar con el servicio de atención al cliente</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zona horaria</td> 
      <td> <p>Esta es la zona horaria predeterminada de la instancia de Workfront. Puede editar este campo para que coincida con la zona horaria de su ubicación Workfront principal. La zona horaria que seleccione determina lo siguiente: </p> 
       <ul> 
        <li>La fecha y la hora mostradas en los correos electrónicos salientes</li> 
        <li>El huso horario predeterminado para los nuevos usuarios cuando se crean</li> 
       </ul> <p>Los usuarios pueden modificar la zona horaria de su instancia de Workfront en su perfil. Cuando los usuarios modifican su zona horaria, la fecha y la hora de sus correos electrónicos de Workfront coinciden con sus preferencias de perfil. Para obtener más información sobre la modificación de las preferencias de perfil de usuario, consulte <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurar mis ajustes</a>. Se selecciona como zona horaria predeterminada al crear una nueva programación. Para obtener más información sobre la creación de programaciones, consulte <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>.</p> <p>Para obtener información sobre el uso de programaciones para ayudar a los usuarios a colaborar en Workfront en zonas horarias, consulte <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Trabajo en zonas horarias</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuración regional</td> 
      <td>Controla el formato de idioma, fecha y número utilizado en los mensajes de correo electrónico salientes. La configuración regional seleccionada aquí es la predeterminada cuando se crean nuevos usuarios. Los usuarios pueden modificar su configuración regional en su perfil de usuario. Cuando los usuarios modifican su configuración regional, el formato de idioma, fecha y número de sus correos electrónicos de Workfront coincide con sus preferencias de perfil. Para obtener más información sobre cómo modificar las preferencias de perfil, consulte <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurar mis ajustes</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuota de almacenamiento</td> 
      <td> <p>Esta es la cantidad de espacio de almacenamiento de documentos disponible en la instancia de Workfront.<br>La cuota contiene documentos que se cargan directamente en Workfront.<br>No incluye:</p> 
       <ul> 
        <li>Documentos que vincula a Workfront desde cualquier otro proveedor de servicios de terceros (SharePoint, Google Drive, Webdam, Box, Dropbox, cualquier otro proveedor de Document Asset Management).</li> 
        <li>Los datos de Workfront (proyectos, tareas, problemas, usuarios, etc.).</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versión del producto</td> 
      <td>Este es el tipo de instancia de Workfront que se le asigna. La versión del producto para la mayoría de los clientes de Workfront es <strong>Empresa</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
