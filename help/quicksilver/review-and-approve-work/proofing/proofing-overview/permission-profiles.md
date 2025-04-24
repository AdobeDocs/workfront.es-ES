---
content-type: overview
product-area: documents
keywords: prueba,permiso
navigation-topic: proofing-overview
title: Información general del perfil de permiso de revisión
description: Los perfiles de permisos de prueba determinan qué permisos generales tienen los usuarios sobre todas las pruebas de la cuenta. Los perfiles de permisos de prueba se asignan a los usuarios en su perfil de usuario. Los perfiles de permisos de prueba son diferentes de las funciones de prueba.
author: Courtney
feature: Digital Content and Documents
exl-id: fb6faa48-d97b-4b7b-83ae-fe39d40b3963
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 100%

---

# Información general del perfil de permiso de revisión

<!--Audited: 12/2023-->

Los perfiles de permisos de prueba determinan qué permisos generales tienen los usuarios sobre todas las pruebas de la cuenta. Los perfiles de permisos de prueba se asignan a los usuarios en su perfil de usuario.

Los perfiles de permisos de prueba son diferentes de las funciones de prueba. Para obtener más información sobre las funciones de prueba, consulte [Información general sobre funciones de prueba](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).

>[!NOTE]
>
>Si es administrador, puede crear perfiles personalizados para los usuarios de su organización. Para obtener más información, consulte [Configuración de perfiles personalizados en Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Consider the following about roles and permissions:</p>
-->

<!--
<ul data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li> <p>Assigned profile permissions relate only to the users and items in your own account. The exception is in the case of Satellite accounts, where the Administrator and Billing Administrator for the main (hub) accounts can access and manage the account settings and billing of those accounts from the hub account level.</p> </li>
<li> <p>Billing Administrators and Administrators can delete users. This can only be done in Account settings.</p> </li>
<li>When Billing Administrators and Administrators view proofs that are owned by other users in their account, they view them with the role of a Reviewer.</li>
<li>Using the Read Only role, Billing Administrators and Administrators can access proofs in folders shared with them or in folders created by them. </li>
</ul>
-->

## Perfiles de permisos de prueba

La siguiente tabla muestra los permisos disponibles con cada perfil de permisos de prueba.

<table style="table-layout:auto">
  <tr>
   <td colspan="1" ><strong></strong>
   </td>
   <td colspan="4" ><strong>Elementos propios</strong>
   </td>
   <td colspan="3" ><strong>Otros elementos de otros usuarios</strong>
   </td>
   <td><strong>Administrador</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>Añadir</strong>
   </td>
   <td><strong>Vista</strong>
   </td>
   <td><strong>Editar</strong>
   </td>
   <td><strong>Eliminar</strong>
   </td>
   <td><strong>Vista</strong>
   </td>
   <td><strong>Editar</strong>
   </td>
   <td><strong>Eliminar</strong>
   </td>
   <td><strong>Editar y eliminar</strong>
   </td>
  </tr>
  <tr>
   <td>Administrador
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
  </tr>
  <tr>
   <td>Supervisor
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Gerente
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

### Administrador

Los administradores tienen acceso a [Configuración de la cuenta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings) y tienen los permisos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Los administradores pueden:</td> 
   <td>Los administradores no pueden:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Crear pruebas, cargar archivos y crear carpetas</p> </li> 
     <li> <p>Ver, editar y eliminar pruebas y archivos que han creado</p> </li> 
     <li> <p>Ver, editar y eliminar pruebas y archivos creados por todos los usuarios de la organización</p> </li> 
     <li> <p>Eliminar las carpetas públicas de otros usuarios</p> </li> 
     <li> <p>Editar todas las pruebas creadas en la cuenta</p> </li> 
     <li> <p>Se debe establecer como propietario de Dropzone*</p> </li> 
     <li> <p>Acceder a la página Configuración de la cuenta y editar los detalles de la cuenta</p> </li> 
     <li> <p>Vaciar la papelera</p> </li> 
     <li> <p>Añadir, editar y eliminar usuarios</p> </li> 
     <li> <p>Crear grupos y añadir nuevos contactos</p> </li> 
     <li> <p>Eliminar contactos</p> </li> 
     <li> <p>Editar pruebas si no hay respuestas en ellas</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Editar respuestas de prueba.</p> </li> 
     <li> <p>Eliminar las carpetas privadas de otros usuarios</p> </li> 
     <li> <p>Acceder a la página Facturación o editar los detalles de facturación</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Disponible únicamente en el producto independiente de Workfront Proof.

### Supervisor

Los supervisores tienen los siguientes permisos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Los supervisores pueden hacer lo siguiente:</td> 
   <td>Los supervisores no pueden hacer lo siguiente:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Crear pruebas, cargar archivos y crear carpetas</p> </li> 
     <li> <p>Ver, editar y eliminar pruebas y archivos que han creado</p> </li> 
     <li> <p>Ver, editar y eliminar pruebas y archivos creados por todos los usuarios de la organización</p> </li> 
     <li> <p>Eliminar las carpetas públicas de otros usuarios</p> </li> 
     <li> <p>Editar todas las pruebas creadas en la cuenta</p> </li> 
     <li> <p>Crear grupos y añadir nuevos contactos</p> </li> 
     <li> <p>Eliminar contactos</p> </li> 
     <li> <p>Editar pruebas si no hay respuestas en ellas</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Editar respuestas de prueba.</p> </li> 
     <li> <p>Eliminar las carpetas privadas de otros usuarios</p> </li> 
     <li> <p>Acceder a la página Facturación o editar los detalles de facturación</p> </li> 
     <li> <p>Añadir, editar o eliminar usuarios</p> </li> 
     <li> <p>Vaciar la papelera</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gerente

Los administradores tienen los siguientes permisos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Los administradores pueden hacer lo siguiente:</td> 
   <td>Los administradores no pueden hacer lo siguiente:</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Crear pruebas, cargar archivos y crear carpetas</p> </li> 
     <li> <p>Ver, editar y eliminar pruebas y archivos que han creado</p> </li> 
     <li> <p>Ver, revisar y aprobar pruebas de otros usuarios que se hayan compartido explícitamente con ellos (derechos de solo lectura para todo lo que hay en una carpeta compartida)</p> </li> 
     <li> <p>Editar todas las pruebas creadas en la cuenta</p> </li> 
     <li> <p>Crear grupos y añadir nuevos contactos</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Ver, editar o eliminar pruebas y archivos creados por otros usuarios de la organización. </p> </li><li><p>Editar respuestas de prueba.</p> </li> 
     <li> <p>Eliminar las carpetas privadas o públicas de otros usuarios</p> </li> 
     <li> <p>Acceder a la página Facturación o editar los detalles de facturación</p> </li> 
     <li> <p>Añadir, editar o eliminar usuarios</p> </li> 
     <li> <p> Eliminar contactos</p> </li> 
     <li> <p>Vaciar la papelera</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Observer</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers have the following permissions:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can see, review, and approve proofs of other users that are explicitly shared with them (Read-only rights to everything in a shared folder). For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create proofs, upload files, and create folders. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md" class="MCXref xref">Upload Files and Web Content to Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot view, edit, or delete proofs and files created by other users in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot edit proofs or replies.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete any items created in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Billing page or Account settings. For more information, see <a href="../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md" class="MCXref xref">The Workfront Proof Billing Page</a> and <a href="../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md" class="MCXref xref">Account settings in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be set as the Dropzone owner. For more information, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md" class="MCXref xref">Configure the dropzone in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot empty the trash. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md" class="MCXref xref">Restore and Empty the Trash in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot add, edit, or delete users. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create groups or add new contacts. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete contacts. </p>
-->


><!--
><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Menus and functions available to Observers are limited. </p>>
>-->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the Header menu or the green New menu in their Dashboard</li>>
>  -->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the following links in their Settings: Account settings, Billing </li>>
>  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Guest</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Guest profile is used to give access to proofs for reviewers who do not have their own Workfront Proof account. Guests can access proofs shared with them directly via their personal email notifications.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view, review, and approve proofs that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Dashboard.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot have folders shared with them. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md" class="MCXref xref">Manage Folders in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be added as Authors or Moderators to the proofs. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<note type="note">
 Guests are not Workfront Proof users, so they cannot see all the proofs shared with them in their own Dashboard.
</note>
-->
