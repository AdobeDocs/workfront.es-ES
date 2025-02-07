---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configurar Adobe Workfront con SAML 2.0 utilizando ADFS
description: Puede habilitar la autenticación en Workfront con SAML 2.0.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 99%

---

# Configurar Adobe Workfront con SAML 2.0 utilizando ADFS

{{important-admin-console-onboard}}

Como administrador de Adobe Workfront, puede integrar Workfront con una solución de Lenguaje de marcado para confirmaciones de seguridad (SAML) 2.0 para el inicio de sesión único mientras utiliza los Servicios de federación de Active Directory (ADFS).

Esta guía se centra en la configuración de ADFS sin aprovisionamiento automático ni asignaciones de atributos. Le recomendamos que complete la configuración y la pruebe antes de configurar cualquier aprovisionamiento automático.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Habilitar la autenticación en Workfront con SAML 2.0

Para habilitar la autenticación en la aplicación web de Workfront y la aplicación móvil de Workfront con SAML 2.0, complete las siguientes secciones:

* [Recuperar el archivo de metadatos SSO de Workfront](#retrieve-the-workfront-sso-metadata-file)
* [Configurar la confianza de usuarios de confianza](#configure-relying-party-trusts)
* [Configurar reglas de notificación](#configure-claim-rules)
* [Cargue el archivo de metadatos y pruebe la conexión](#upload-the-metadata-file-and-test-the-connection)

### Recuperación del archivo de metadatos SSO de Workfront {#retrieve-the-workfront-sso-metadata-file}

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Sistema** > **Inicio de sesión único (SSO)**.
1. En el menú desplegable **Tipo**, haga clic en **SAML 2.0** para mostrar información y opciones adicionales.
1. Copie la dirección URL que se muestra después de la **URL de metadatos**.
1. Continúe a la sección siguiente, [Configurar la confianza de usuarios de confianza](#configure-relying-party-trusts).

### Configuración de la confianza de usuarios de confianza {#configure-relying-party-trusts}

1. Abra el **Administrador de ADFS** con Windows Server 2008 R2 (la versión puede variar).
1. Vaya a **Inicio.**
1. Haga clic en **Herramientas de administración.**
1. Haga clic en **Administración de ADFS 2.0.**
1. Seleccione **ADFS** y expanda **Relaciones de confianza**.
1. Haga clic con el botón secundario en **Confianza de usuarios de confianza** y, a continuación, seleccione **Añadir confianza a un usuario de confianza** para iniciar el asistente para añadir confianza a los usuarios de confianza.
1. En la **página de bienvenida**, seleccione **Inicio**.
1. En la sección **Seleccionar origen de fecha**, pegue la URL de metadatos desde Workfront.
1. Haga clic en **Siguiente**.
1. Haga clic en **Aceptar** para confirmar el mensaje de advertencia.
1. En la sección **Especificar nombre para mostrar**, añada un **Nombre para mostrar** y **Notas** para distinguir la confianza y, a continuación, haga clic en **Siguiente**.
1. Seleccione **Permitir que todos los usuarios tengan acceso a este usuario de confianza** (o **Ninguno** si desea configurarlo más adelante).
1. Haga clic en **Siguiente**.

   Esto lo lleva a la sección **Listo para añadir confianza**.

1. Continúe en la siguiente sección [Configurar reglas de notificación](#configure-claim-rules).

### Configurar reglas de notificación {#configure-claim-rules}

1. Haga clic en **Siguiente** en la sección **Listo para añadir confianza** y, a continuación, asegúrese de que la opción **Abrir el cuadro de diálogo Editar reglas de notificación** esté seleccionada.

   Esto le permitirá editar las reglas de notificación en un paso futuro.

1. Haga clic en **Cerrar**.
1. Haga clic en **Añadir regla.**
1. Seleccione **Enviar atributo LDAP como notificaciones**.
1. Haga clic en **Siguiente** para mostrar el paso **Configurar regla de notificación**.
1. Especifique los siguientes requisitos mínimos para configurar la regla de notificación: (esto irá en el **identificador de federación**, en la configuración de usuario, y se utiliza para distinguir quién inicia sesión).


   <table >                
      <tbody>
            <tr>
               <td>Nombre de la regla de notificación
               </td>
               <td>Especifique un nombre para la regla de notificación. Por ejemplo, “Workfront”.</td>
            </tr>
            <tr>
               <td>Almacén de atributos</td>
               <td >Seleccione <b>directorio activo</b> en el menú desplegable.</td>
            </tr>
            <tr>
               <td>Atributo LDAP</td>
               <td>Puede ser cualquier tipo de atributo. Se recomienda usar <b>SAM-Cuenta-Nombre</b> para este atributo.</td>
            </tr>
            <tr>
               <td>Tipo de notificación saliente</td>
               <td>Debe seleccionar <b>ID del nombre</b> como tipo de notificación saliente</td>
            </tr>
      </tbody>
   </table>

1. (Opcional) Para establecer el aprovisionamiento automático, añada las siguientes notificaciones adicionales tanto en el atributo LDAP como en el tipo de notificación saliente:

   * Nombre dado
   * Apellido
   * Dirección de correo electrónico

1. Haga clic en **Finalizar** y, a continuación, haga clic en **Aceptar** en la pantalla siguiente.
1. Haga clic con el botón secundario en la nueva **Confianza del usuario de confianza** y, a continuación, seleccione **Propiedades**.
1. Seleccione la **pestaña Avanzada**. Y en **Algoritmo hash seguro**, seleccione SHA-1 o SHA-256.

   >[!NOTE]
   >
   >La opción que seleccione en Algoritmo hash seguro debe coincidir con el campo Algoritmo hash seguro de Workfront en Configuración > Sistema > Inicio de sesión único (SSO).

1. Continúe con la siguiente sección [Cargar el archivo de metadatos y probar la conexión](#upload-the-metadata-file-and-test-the-connection).

### Cargue el archivo de metadatos y pruebe la conexión {#upload-the-metadata-file-and-test-the-connection}

1. Abra un explorador y vaya a `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml`.

   Debería descargarse un archivo de metadatos FederationMetadata.xml.

1. Haga clic en **Elegir archivo** en **Rellenar campos a partir de metadatos del proveedor de identidad** y seleccione el archivo **FederationMetadata.xml**.

1. (Opcional) Si la información del certificado no se rellenó con el archivo de metadatos, puede cargar un archivo por separado. Seleccione **Elegir archivo** en la sección **Certificado**.

1. Haga clic en **Probar conexión**. Si está configurado correctamente, debería ver una página similar a la que se muestra a continuación:

   ![Mensaje de éxito de SAML 2](assets/success-saml-2.png)

   >[!NOTE]
   >
   >Si desea configurar la asignación de atributos, asegúrese de copiar los atributos de la conexión de prueba al atributo directorio. Para obtener más información, consulte Asignación de atributos de usuario.

1. Seleccione **Exención de administrador** para permitir que los administradores de Workfront inicien sesión con credenciales de Workfront con la URL de omisión.

   Los marcadores que apuntan a `<yourdomain>`.my.workfront.com/login omiten la redirección.

1. Seleccione la casilla **Habilitar** para habilitar la configuración.
1. Haga clic en **Guardar**.

## Acerca de la actualización de usuarios para SSO

Siguiendo esta guía, el **nombre de usuario SSO** será su **nombre de usuario de Active Directory**.

Como administrador de Workfront, puede actualizar usuarios en lote para SSO. Para obtener más información sobre cómo actualizar usuarios para SSO, consulte [Actualizar usuarios para el inicio de sesión único](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

Como administrador de Workfront, también puede asignar manualmente un ID de federación si edita el perfil del usuario y completa el campo ID de federación. Para obtener más información sobre cómo editar un usuario, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>Al editar los perfiles de los usuarios para incluir un ID de federación, al seleccionar **Permitir solo la autenticación SAML 2.0** se elimina la capacidad de iniciar sesión en Workfront mediante la URL de omisión (`<yourdomain>`.my.workfront.com/login).
