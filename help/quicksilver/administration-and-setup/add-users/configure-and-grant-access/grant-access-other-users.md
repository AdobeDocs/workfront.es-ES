---
title: Conceder acceso a los usuarios
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a otros usuarios en Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 29%

---


# Concesión de acceso a los usuarios

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a otros usuarios en Workfront, como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo los administradores de Workfront pueden modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creación o modificación de niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configuración del acceso a los usuarios

Puede administrar la información que los usuarios pueden ver y editar para otros usuarios mediante un nivel de acceso predeterminado o personalizado que usted cree. Los usuarios con las licencias de planificación y trabajo predeterminadas pueden ver la información de contacto de otros usuarios. Cualquiera de los siguientes usuarios puede crear y editar otros usuarios:

* Un administrador de Workfront.

  Para obtener más información, consulte [Conceder acceso administrativo completo a un usuario](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* Un usuario con una licencia de Plan predeterminada que también tiene acceso a los usuarios, como se explica en este artículo.

  Los usuarios con restricciones para ver solo los usuarios de su compañía o de la compañía principal tienen acceso para editar solo los usuarios que pueden ver. Para obtener más información, consulte [Creación o modificación de niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Usuario con una licencia de planificación predeterminada que también se especifica como administrador de otro usuario.

  Los usuarios a los que se concede acceso de edición a los usuarios de su nivel de acceso pueden administrar los usuarios que dependen de ellos. Para obtener información acerca de cómo administrar un usuario, vea [Ver el organigrama](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* Un usuario con una licencia de planificación predeterminada que haya creado un usuario puede desactivar, eliminar o editar el usuario que ha creado. Para obtener información sobre cómo crear usuarios nuevos, consulte [Agregar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configurar el acceso de los usuarios para editar usuarios con un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Para cambiar la capacidad de los usuarios con una licencia de planificación o de trabajo para ver los perfiles de otros usuarios:

   1. Haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en el botón **Ver** a la derecha de **Usuarios**.

   1. Deshabilite **Ver información de contacto** y, a continuación, haga clic en la X para cerrar el cuadro **Ajustar la configuración**.

      ![ajustar la configuración de usuario](assets/fine-tune-users.png)

1. Para modificar la capacidad de los usuarios con acceso a una licencia de planificación para editar otros usuarios, haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en el botón **Editar** a la derecha de **Usuarios** y, a continuación, seleccione las capacidades que desee conceder:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Crear</strong> </td> 
      <td> <p>Permite a los usuarios crear usuarios.<br>Esta opción está desactivada de forma predeterminada.</p> 
     <p><b>NOTA</b>: Esto no está disponible si su organización se ha incorporado a Adobe Admin Console. Consulte al administrador de red o de TI si necesita más información.</p>
        </td>  
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Eliminar</strong> </td> 
      <td> <p> Permite a los usuarios eliminar los usuarios que ellos mismos han creado.<br>Esta opción está desactivada de forma predeterminada.</p> <p><b>NOTA</b>: Esto no está disponible si su organización se ha incorporado a Adobe Admin Console. Consulte al administrador de red o de TI si necesita más información.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrador de usuarios (todos los usuarios)</strong> </td> 
      <td> <p>Permite a los usuarios hacer lo siguiente para cualquier usuario de Workfront:</p> 
       <ul> 
        <li>Editar, eliminar o desactivar el usuario</li> 
        <li>Inicie sesión como usuario<p><b>NOTA</b>: no puede iniciar sesión como ningún usuario que sea administrador del sistema.</p></li> 
        <li>Restablecer la contraseña del usuario</li> 
       </ul> <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrador de usuarios (usuarios de grupo)</strong> </td> 
      <td> <p>Permite a los usuarios hacer lo siguiente para cualquier usuario de un grupo que administren: 
        <ul>
         <li><p>Editar, eliminar o desactivar el usuario</p></li>
         <li>Inicie sesión como usuario</li>
         <li><p>Restablecer la contraseña del usuario</p><p><b>NOTA</b>: un administrador de grupo no puede iniciar sesión como o restablecer la contraseña de un administrador de Workfront.</p></li>
        </ul><p>Esta opción está desactivada de forma predeterminada.</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Si no desea conceder acceso a los administradores de grupos a todos los miembros de los grupos que administran, desactive las dos opciones Administración de usuarios mencionadas anteriormente. Los administradores de grupo seguirán teniendo acceso a los miembros del grupo que agreguen a Workfront o que dependan de ellos en Workfront.

1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas en el nivel de acceso en el que esté trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a las tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando termine, haga clic en **Guardar**.

## Acceso a usuarios por tipo de licencia

Para obtener información acerca de lo que los usuarios de cada nivel de acceso pueden hacer con los usuarios, vea la sección [Usuarios](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
