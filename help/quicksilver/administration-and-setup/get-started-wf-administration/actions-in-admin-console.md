---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)
description: Si su organización se ha incorporado a Adobe Business Platform, los usuarios utilizan Adobe Business Platform para acceder a Adobe Workfront. Esto significa que la administración de usuarios se realiza en gran medida a través de Adobe Admin Console y que el inicio de sesión único (SSO) se gestiona a través de Adobe Business Platform en lugar de a través de Workfront. Como administrador de Adobe Workfront, sus responsabilidades y procedimientos de administración difieren en función de si su organización se ha incorporado a Adobe Business Platform. Este artículo enumera los procedimientos que deben gestionarse de forma diferente y los vínculos a las instrucciones tanto para Workfront como para Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: b476c012f825afc4bc48b7172be26accc6bac0d1
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 1%

---

# Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)

Si su organización se ha incorporado a Adobe Business Platform, los usuarios utilizan Adobe Business Platform para acceder a Adobe Workfront. Esto significa lo siguiente:

* Los administradores del sistema se crean mediante Adobe Admin Console
* El inicio de sesión único (SSO) se administra a través de Adobe Business Platform en lugar de Workfront

Como administrador de Adobe Workfront, sus responsabilidades y procedimientos de administración difieren en función de si su organización se ha incorporado a Adobe Business Platform. Este artículo enumera los procedimientos que se gestionan de forma diferente y los vínculos a las instrucciones tanto para Workfront como para Adobe Admin Console.

## Usuarios



>[!NOTE]
>
>Se recomienda añadir usuarios que no sean administradores del sistema directamente en Workfront. Es posible agregar usuarios en Adobe Admin Console, pero agregarlos en Workfront le permite establecer su nivel de acceso al crearlos, lo que le puede ahorrar tiempo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Acción</th> 
   <th>Para obtener instrucciones sobre Workfront, consulte</th> 
   <th>Para obtener instrucciones sobre la Admin Console de Adobe, consulte</th> 
  </tr> 
 </thead> 
 <tbody> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Conceder acceso de administrador a un usuario</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sección "Editar detalles del usuario" en <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Administrar usuarios individualmente</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Añadir un usuario a Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Adición de usuarios</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Administración de usuarios en Adobe Admin Console</a> </p> </li> 
     <li> <p>La sección "Agregar usuarios" en <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Administrar usuarios individualmente</a></p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Desactivar un usuario</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sección "Eliminar usuarios" en <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Administrar usuarios individualmente</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eliminar un usuario</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Eliminar usuarios</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sección "Eliminar usuarios permanentemente" en <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Administrar usuarios de directorio</a>
     </p><p>Nota: Eliminación de un usuario de [!DNL Adobe Admin Console] desactiva el usuario en [!DNL Workfront], pero no las elimina de [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Edición de un perfil de usuario</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edición del perfil de un usuario</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sección "Editar detalles del usuario" en <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Administrar usuarios individualmente</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Edición masiva de perfiles de usuario</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Edición de perfiles de usuario por lotes</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sección "Editar detalles del usuario" en <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Carga masiva de CSV</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Importar usuarios </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importar usuarios</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sección "Agregar usuarios" en <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Carga masiva de CSV</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Iniciar sesión como otro usuario</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Iniciar sesión como otro usuario</a> </p> </li> 
    </ul> </td> 
   <td>No disponible</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Renovar certificado SAML</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Renovación del certificado de metadatos Adobe Workfront SAML 2.0</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sección "La firma digital en la respuesta de SAML no validó..." en <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Federated ID de resolución de problemas</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## SSO (inicio de sesión único)

Dado que Adobe Business Platform controla el inicio de sesión único (SSO) para los usuarios, las siguientes acciones y funcionalidades se gestionan automáticamente a través de Adobe Business Platform. Si su organización aún no se ha incorporado a Adobe Business Platform, debe realizar estas acciones en Workfront.


* [Configuración de Adobe Workfront con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Configuración de Adobe Workfront con SAML 2.0 mediante ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Desactivar el inicio de sesión único en Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [Actualización de metadatos de SAML 2.0 en el proveedor de identidad](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Actualizar usuarios para el inicio de sesión único](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [Configurar directivas de contraseña para la autenticación](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [Configurar las preferencias de seguridad del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
