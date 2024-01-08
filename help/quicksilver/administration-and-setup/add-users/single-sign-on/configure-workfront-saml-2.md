---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configuración de Adobe Workfront con SAML 2.0
description: Como administrador de Adobe Workfront, puede configurar las aplicaciones web y móviles de Workfront para que se integren con una solución de lenguaje de marcado de aserción de seguridad (SAML) 2.0 para el inicio de sesión único (SSO).
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 7%

---

# Configuración de Adobe Workfront con SAML 2.0

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

<!-- Audited: 12/2023 -->

{{important-admin-console-onboard}}

Como administrador de Adobe Workfront, puede configurar las aplicaciones web y móviles de Workfront para que se integren con una solución de lenguaje de marcado de aserción de seguridad (SAML) 2.0 para el inicio de sesión único (SSO).

Después de configurar SAML 2.0 en Workfront, tal como se describe en las secciones siguientes, puede mantener la configuración, tal como se describe en [Actualización de metadatos de SAML 2.0 en el proveedor de identidad](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

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
   <td><p>Nuevo: estándar </p>
       <p>o</p> 
       <p>Actual: plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Habilitar la autenticación en Workfront con SAML 2.0

{{step-1-to-setup}}

1. Clic **Sistema** > **Inicio de sesión único (SSO).**

1. En el **Tipo** , seleccione la opción **SAML 2.0.**

1. Cerca de la parte superior de las opciones que aparecen, haga clic en **Descargar metadatos de SAML 2.0** para descargar el archivo en el equipo.

   El proveedor de identidad de SAML 2.0 requiere un archivo XML con información generada en la instancia de Workfront. Después de descargar el archivo, debe acceder al servidor del proveedor de identidad de SAML 2.0 y cargar allí el archivo XML de metadatos SAML 2.0 de Workfront.

1. Especifique la siguiente información en Workfront:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Identificador de proveedor de servicios </td>
      <td> Esta dirección URL, que ya se ha rellenado automáticamente, identifica a Workfront con su proveedor de identidad. Por ejemplo: <code>&lt;yourcompany&gt;.com/SAML2</code>.</td>
     </tr>
     <tr>
      <td role="rowheader">Tipo de enlace</span> </td>
      <td> <p>Seleccione el método admitido por el servidor IDP para enviar información de autenticación:</p>
       <ul>
       <li>POST</li>
       <li>REDIRECCIONAR</li>
       </ul> </td>
     </tr>
     <tr>
      <td role="rowheader">Completar campos a partir de metadatos del proveedor de identidad </td> 
      <td>En su solución de proveedor de identidad de SAML 2.0, exporte un archivo XML de metadatos de proveedor de servicios y guárdelo en una ubicación temporal de su equipo. Seleccionar <strong>Elegir archivo</strong>, a continuación, busque y seleccione el archivo que guardó para añadirlo a la configuración de Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL del portal de inicio de sesión</span> </td> 
      <td>Introduzca el portal de inicio de sesión común de su organización. Dirección URL donde los usuarios inician sesión para acceder a Workfront y a todas las demás aplicaciones integradas con SAML 2.0.</td> 
     </tr>
     <tr>
      <td role="rowheader">URL de cierre de sesión</span> </td> 
      <td> <p>Introduzca la URL de cierre de sesión del servidor IDP. Workfront envía una solicitud HTTP a esta dirección URL antes de cerrar sesión en Workfront. Esto cierra la sesión del usuario en el servidor remoto cuando se cierra la sesión de Workfront.</p> <p><b>NOTA</b>: se le redirige a la dirección URL de cierre de sesión solo si tiene la opción <strong>Solamente permitir autenticación de SAML 2.0</strong> habilitado en su perfil de usuario.</p> </td>
     </tr>
     <tr>
      <td role="rowheader">Cambiar URL de contraseña </td> 
      <td> <p> Especifique la dirección URL a la que se redirigirá a los usuarios para cambiar sus contraseñas. </p> <p>Dado que las credenciales de SAML 2.0 se utilizan para acceder a Workfront, los usuarios deben ser redirigidos a una página en la que pueden cambiar su contraseña de SAML 2.0 en lugar de completar esta actividad a través de Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Algoritmo hash seguro </td> 
      <td> <p>Seleccione el Algoritmo de hash seguro (SHA) que admite su IDP:</p> 
       <ul> 
       <li>SHA-1</li> 
       <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aprovisionar usuarios automáticamente</span> </td> 
      <td> <p>Esta opción crea automáticamente un usuario en el sistema cuando un nuevo usuario con un nombre de usuario y una contraseña de directorio intenta iniciar sesión en Workfront por primera vez.</p> <p>Para crear usuarios en Workfront, debe asignar los atributos de datos de Workfront con los siguientes atributos de datos de usuario en su proveedor de directorios:</p> 
       <ul> 
       <li>Nombre</li> 
       <li>Apellido</li> 
       <li>Dirección de correo electrónico</li> 
       </ul> 
       <p>Al seleccionar la casilla de verificación, se muestran las siguientes opciones:</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>Seleccione el atributo de usuario de Workfront que desee asignar en la lista desplegable y, a continuación, especifique el atributo de directorio correspondiente en el directorio de usuario.</p> 
       <p>El <strong>Atributo de directorio</strong> debe contener el Nombre de atributo de directorio de la tabla de atributos de usuario que guardó al probar correctamente la configuración de SAML 2.0.</p> 
       <p>Puede establecer un Valor de Workfront predeterminado en la variable <strong>Valor predeterminado</strong> field. También puede establecer reglas basadas en los valores de su proveedor de identidad de SAML 2.0.</p> 
       <p><b>ADVERTENCIA</b>: Workfront intenta asignar los atributos que se enumeran a continuación cada vez que un usuario inicia sesión en el sistema. Debido a esto, no se recomienda asignar niveles de acceso. Puede eliminar fácilmente el acceso administrativo si un atributo se asigna incorrectamente. Clic <strong>Agregar asignación</strong> para agregar reglas adicionales.
       </p> 
       <p>Puede asignar los siguientes atributos de Workfront:</p> 
      <ul> 
      <li> <p>Nivel de acceso</p> </li> 
      <li> <p>Dirección</p> </li> 
      <li> <p>Dirección2</p> </li> 
      <li> <p>Facturación por hora</p> </li> 
      <li> <p>Ciudad</p> </li> 
      <li> <p>Compañía</p> </li> 
      <li> <p>Coste por hora</p> </li> 
      <li> <p>Dirección de correo electrónico</p> </li> 
      <li> <p>Extensión</p> </li> 
      <li> <p>Nombre</p> </li> 
      <li> <p>Grupo de inicio</p> </li> 
      <li> <p>Equipo de inicio</p> </li> 
      <li> <p>Función</p> </li> 
      <li> <p>Apellido</p> </li> 
      <li> <p>Plantilla de diseño</p> </li> 
      <li> <p>Gerente</p> </li> 
      <li> <p>Teléfono móvil</p> </li> 
      <li> <p>Número de teléfono</p> </li> 
      <li> <p>Código postal</p> </li> 
      <li> <p>Programación</p> </li> 
      <li> <p>Estado</p> </li> 
      <li> <p>Perfil de hoja de horas</p> </li> 
      <li> <p>Título</p> </li> 
      </ul>
      <p>Clic <strong>Guardar</strong> cuando haya terminado de asignar atributos de usuario.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Certificado </td> 
      <td> <p>Cargue un certificado SSL válido para garantizar una conexión segura entre el servicio de autenticación y Workfront. Para las cuentas OnDemand, siempre se requiere un certificado. Puede obtener este certificado de su administrador del sistema SAML 2.0.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exención de administrador </td> 
      <td> <p>Permite a los administradores de Workfront acceder a Workfront mediante el inicio de sesión en Workfront. Si no se selecciona esta opción, los administradores de Workfront deben utilizar su nombre de usuario y contraseña de SAML 2.0.</p> 
      <p>En primer lugar, Workfront intenta iniciar sesión en Workfront a través de SAML 2.0 para los usuarios con nivel de acceso de administrador del sistema de Workfront. Si la autenticación SAML 2.0 falla, Workfront utiliza la autenticación local para los administradores de Workfront.</p> 
      <p>Le recomendamos que siempre tenga seleccionada esta opción para que su administrador de Workfront pueda iniciar sesión en Workfront si su proveedor de SAML 2.0 alguna vez no está disponible temporalmente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activar </td> 
      <td> <p>Activa el SSO en el sistema de Workfront. Asegúrese de haber comunicado las instrucciones de inicio de sesión a los usuarios.</p> <p>Después de habilitar la configuración de SSO en Workfront, debe habilitar el <strong>Solamente permitir autenticación de SAML 2.0</strong> configuración para todos los usuarios de modo que puedan utilizar SSO.</p> <p>Para obtener más información sobre la actualización de usuarios para SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Actualizar usuarios para el inicio de sesión único</a>.</p> <p>Para obtener más información sobre la configuración de usuario, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edición del perfil de un usuario</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Confirmar configuración </td> 
      <td> 
      <p>Clic <strong>Probar conexión</strong> para comprobar que Workfront y el proveedor de identidad de SAML 2.0 pueden comunicarse entre sí. Esta conexión sólo es correcta si ha intercambiado los archivos XML.
      </p> 
      <p>Después de probar correctamente el vínculo entre su proveedor de identidad de SAML 2.0 y Workfront, verá una pantalla similar a la de la imagen siguiente.</p>
      <p><b>NOTA</b>: Esta pantalla se muestra en una ventana emergente del explorador, por lo que debe asegurarse de desactivar los bloqueadores de ventanas emergentes.</p>
      <p>Guarde la información mostrada en la tabla para usarla más adelante.</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Guardar** para guardar la configuración de SAML 2.0.
