---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)
description: Si su organización se ha incorporado a Adobe Business Platform, los usuarios utilizan Adobe Business Platform para acceder a Adobe Workfront. Esto significa que la administración de usuarios se realiza en gran medida a través de Adobe Admin Console y que el inicio de sesión único (SSO) se gestiona a través de Adobe Business Platform en lugar de hacerlo a través de Workfront. Como administrador de Adobe Workfront, sus responsabilidades y procedimientos de administración difieren en función de si su organización se ha incorporado a Adobe Business Platform. En este artículo se enumeran los procedimientos que deben gestionarse de forma diferente y los vínculos a las instrucciones tanto para Workfront como para Adobe Admin Console.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: eb68357ed4fd8f323707aa4a54a0f946253bf4e0
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 96%

---

# Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)

Como administrador de Adobe Workfront, sus responsabilidades y procedimientos de administración pueden diferir en función de si su organización se ha incorporado a Adobe Business Platform. En este artículo se enumeran los procedimientos que se gestionan de forma diferente y los vínculos a las instrucciones tanto para Workfront como para Adobe Admin Console.

Si su organización se ha incorporado a Adobe Business Platform, los usuarios utilizan Adobe Business Platform para acceder a Adobe Workfront. Esto significa lo siguiente:

* Los administradores del sistema se crean mediante Adobe Admin Console
* La renovación de un certificado SAML se gestiona mediante Adobe Admin Console.
* El inicio de sesión único (SSO) se gestiona mediante Adobe Business Platform en lugar de mediante Workfront

## Creación de administradores del sistema de Workfront en Adobe Admin Console

>[!NOTE]
>
>Recomendamos añadir usuarios que no sean administradores del sistema directamente en Workfront. Es posible añadir usuarios en Adobe Admin Console, pero añadirlos en Workfront le permite establecer su nivel de acceso mientras los crear, lo que le puede ahorrar tiempo.

Para obtener instrucciones sobre cómo crear administradores de sistemas de Workfront, consulte [Administrar usuarios en Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Action</th> 
   <th>For instructions in Workfront, see</th> 
   <th>For instructions in the Adobe Admin console, see</th> 
  </tr> 
 </thead> 
 <tbody> 
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
  <tr> 
   <td role="rowheader">Grant a user admin access</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Add a user to Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
     <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
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
  <tr> 
   <td role="rowheader">Deactivate a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Remove users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Delete a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Delete users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Permanently delete users" in <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Manage directory users</a>
     </p><p>Note: Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Edit a user profile</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bulk edit user profiles</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Edit user profiles in bulk</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Import users </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Import users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Add users" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Log in as another user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Log in as another user</a> </p> </li> 
    </ul> </td> 
   <td>Not available</td> 
  </tr> 
  <tr> 
    -->

## Renovación del certificado SAML

Para obtener instrucciones sobre la renovación del certificado SAML en Adobe Admin Console, consulte la sección &quot;No se ha validado la firma digital en la respuesta SAML...&quot; en [Solución de problemas de Federated ID](https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html?lang=es)

<!--

   <td role="rowheader">Renew SAML certificate</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Renew the Adobe Workfront SAML 2.0 metadata certificate</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "The digital signature in the SAML response did not validate..." in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Troubleshooting Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

-->

## SSO (inicio de sesión único)

Dado que Adobe Business Platform controla el inicio de sesión único (SSO) para los usuarios, las siguientes acciones y funcionalidades se gestionan automáticamente a través de Adobe Business Platform. Si su organización aún no se ha incorporado a Adobe Business Platform, debe realizar estas acciones en Workfront.


* [Configurar Adobe Workfront con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Configurar Adobe Workfront con SAML 2.0 usando ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Desactivar el inicio de sesión único en Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [Actualizar metadatos de SAML 2.0 en su proveedor de identidad](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Actualizar usuarios para inicio de sesión único](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [Configurar políticas de contraseña para la autenticación](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [Configurar preferencias de seguridad del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
