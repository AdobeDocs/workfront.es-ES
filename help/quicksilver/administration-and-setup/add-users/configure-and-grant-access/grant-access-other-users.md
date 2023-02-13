---
title: Conceder acceso a los usuarios
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a otros usuarios de Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: d1fe7165932fb6f2aff3c8488bdb8e1dfae3b6d3
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---

# Conceder acceso a los usuarios

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a otros usuarios en Workfront, tal como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configuración del acceso a los usuarios

Puede administrar la información que los usuarios pueden ver y editar para otros usuarios mediante un nivel de acceso predeterminado o un nivel de acceso personalizado que cree. Los usuarios con las licencias de Plan y Trabajo predeterminadas pueden ver la información de contacto de otros usuarios. Cualquiera de los siguientes usuarios puede crear y editar otros usuarios:

* Un administrador de Workfront.

   Para obtener más información, consulte [Conceder a un usuario acceso administrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* Un usuario con una licencia Plan predeterminada que también tiene acceso a los usuarios, tal como se explica en este artículo.

   Los usuarios restringidos para ver solo los usuarios de su empresa o de la empresa principal tienen acceso para editar solo los usuarios que puedan ver. Para obtener más información, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Usuario con licencia de Plan predeterminada que también se especifica como administrador de otro usuario.

   Los usuarios a los que se concede acceso de edición a los usuarios en su nivel de acceso pueden administrar los usuarios que informan a ellos. Para obtener información sobre la administración de un usuario, consulte [Ver el organigrama](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* Un usuario con una licencia Plan predeterminada que haya creado un usuario puede desactivar, eliminar o editar el usuario que ha creado. Para obtener información sobre la creación de usuarios nuevos, consulte [Agregar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configuración del acceso de los usuarios para editar los usuarios mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Para cambiar la capacidad de los usuarios con una licencia de Plan o de Trabajo para ver los perfiles de otros usuarios:

   1. Haga clic en el icono del engranaje ![](assets/gear-icon-settings.png) en el **Ver** a la derecha de **Usuarios**.

   1. Deshabilitar **Ver información de contacto** y, a continuación, haga clic en la X para cerrar la **Ajustar la configuración** en la ventana

1. Para modificar la capacidad de los usuarios con una licencia Plan para editar otros usuarios, haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en el **Editar** a la derecha de **Usuarios** y, a continuación, seleccione las capacidades que desee conceder:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Crear</strong> </td> 
      <td> <p>Permite a los usuarios crear usuarios.<br>Esta opción está activada de forma predeterminada.</p> 
      &lt;!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Asegúrese de que este cambio se esté realizando antes de desredactar estas 2 notas. El 29 de marzo, el documento de solicitud dice que esto depende de los resultados de la investigación.</p>

       &lt;p>&lt;b>NOTA&lt;/b>: Esto no está disponible si su organización se ha incorporado a Adobe Admin Console. Si necesita más información, consulte con su administrador de red o TI.&lt;/p>
       —>  &lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Eliminar</strong> </td> 
      <td> <p> Permite a los usuarios eliminar los usuarios que ellos mismos han creado.<br>Esta opción está activada de forma predeterminada.</p> <p><b>NOTA</b>: Esto no está disponible si su organización se ha incorporado a Adobe Admin Console. Si necesita más información, consulte con su administrador de red o TI.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrador de usuarios (todos los usuarios)</strong> </td> 
      <td> <p>Permite a los usuarios hacer lo siguiente para cualquier usuario de Workfront:</p> 
       <ul> 
        <li>Editar, eliminar o desactivar el usuario</li> 
        <li>Iniciar sesión como usuario</li> 
        <li>Restablecer la contraseña del usuario</li> 
       </ul> <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrador de usuarios (usuarios de grupo)</strong> </td> 
      <td> <p>Permite a los usuarios hacer lo siguiente para cualquier usuario de un grupo que administran: 
        <ul>
         <li><p>Editar, eliminar o desactivar el usuario</p></li>
         <li>Iniciar sesión como usuario</li>
         <li><p>Restablecer la contraseña del usuario</p><p><b>NOTA</b>: Un administrador de grupo no puede iniciar sesión como o restablecer la contraseña de un administrador de Workfront.</p></li>
        </ul><p>Esta opción está desactivada de forma predeterminada.</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Si no desea conceder acceso a los administradores de grupos a todos los miembros de los grupos que administran, desactive las dos opciones de Administración de usuarios mencionadas anteriormente. Los administradores de grupos aún podrán acceder a los miembros del grupo a los que añadan a Workfront o a los que informan en Workfront.

1. (Opcional) Para configurar las opciones de acceso de otros objetos y áreas del nivel de acceso en el que esté trabajando, continúe con uno de los artículos enumerados en [Configuración del acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Concesión de acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando haya terminado, haga clic en **Guardar**.

## Acceso de los usuarios por tipo de licencia

Para obtener información sobre lo que los usuarios de cada nivel de acceso pueden hacer con los usuarios, consulte la sección [Usuarios](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
