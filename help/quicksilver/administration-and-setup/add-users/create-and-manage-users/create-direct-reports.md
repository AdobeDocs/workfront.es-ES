---
title: Creación de informes directos
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Puede designar a los usuarios como informes directos para otro usuario. Esto le permite crear un organigrama que muestra la estructura de administración de su organización.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: dea77522-d89f-4baa-a701-aea124d2b3a5
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 1%

---

# Creación de informes directos

Puede designar a los usuarios como informes directos para otro usuario. Esto le permite crear un organigrama que muestra la estructura de administración de su organización. Para obtener más información, vea [Ver el organigrama](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener uno de los siguientes:</p> 
    <ul> 
     <li> <p>El nivel de acceso del administrador del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>. </p> </li> 
     <li> <p>Configuración de <b>usuarios</b> en su nivel de acceso configurado para el acceso de <b>Editar</b>, con <b>Crear</b> y al menos una de las dos opciones de <b>Administrador de usuarios</b> habilitadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si el usuario <b>Admin (usuarios del grupo)</b> está habilitado, debe ser administrador de un grupo del que el usuario sea miembro.</p> <p>Para obtener más información sobre la configuración de <b>Usuarios</b> en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a usuarios</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Creación de informes directos

1. Empiece a editar un usuario como se describe en [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
1. En la sección **Organización**, asegúrese de seleccionar una compañía en el campo **Empresa**.

   Este campo no puede estar en blanco.

1. En el campo **Subordinados directos**, especifique los usuarios que informan al usuario que está editando.
1. (Opcional) En el campo **Notificar a**, especifique el nombre del usuario ante el que informa este usuario.
1. Haga clic en **Guardar cambios**.
