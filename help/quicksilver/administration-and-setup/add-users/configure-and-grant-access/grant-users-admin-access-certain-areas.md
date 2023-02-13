---
title: Conceder a los usuarios acceso administrativo a determinadas áreas
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para otorgar a los usuarios con una licencia de Plan acceso administrativo a ciertas áreas del sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 2%

---

# Conceder a los usuarios acceso administrativo a determinadas áreas

<!--Linked in several places, do not rename or change URL.-->

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para otorgar a los usuarios con una licencia de Plan acceso administrativo a ciertas áreas del sistema.

>[!NOTE]
>
>Esto es diferente de conceder a un usuario acceso administrativo completo a Workfront, como se explica en [Conceder a un usuario acceso administrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)&#x200B;

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

## Conceder a los usuarios del plan acceso administrativo a determinadas áreas de Workfront

>[!IMPORTANT]
>
>Se recomienda dejar los niveles de acceso integrados sin cambios para poder consultarlos después de configurar los usuarios. Para personalizar un nivel de acceso, copie el nivel de acceso predeterminado y modifique la copia. (Puede hacerlo para todos los niveles de acceso excepto para el administrador del sistema y el usuario externo).

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Niveles de acceso**.
1. Haga clic en el nombre del nivel de acceso que desee utilizar para otorgar a los usuarios acceso administrativo a ciertas áreas de Workfront.
1. En el **Permitir acceso administrativo para** para conceder el acceso administrativo necesario.

   Estas opciones le permiten conceder las siguientes capacidades:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Procesos de aprobación</td> 
      <td><p>Cree y administre procesos de aprobación para utilizarlos en todo el sistema y para grupos específicos.</p><p>Sin este acceso, los usuarios solo pueden crear procesos de aprobación específicos en los elementos a los que tienen acceso para administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compañías</td> 
      <td><p>Añadir nuevas empresas y editar las existentes en Workfront</p>
      <p>Sin este acceso, los usuarios solo pueden ver las empresas existentes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td><p>Cree y edite (añada, edite y elimine los campos) formularios personalizados dentro de su grupo.</p><p>Sin este acceso, los usuarios solo pueden adjuntar formularios existentes a objetos a los que tengan acceso para contribuir o administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tasas de cambio</td> 
      <td> <p>Añada nueva moneda en Workfront.</p> <p>Sin este acceso, el usuario solo puede añadir una moneda existente a un proyecto que cree.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td><p>Ver todos los gastos de los objetos en Workfront.</p><p>Esto no permite al usuario crear nuevos tipos de gastos.</p><p>Sin este acceso, el usuario solo puede ver lo siguiente:</p>
       <ul>
        <li>Gastos en proyectos, tareas o problemas que administran</li>
        <li>Sus propios gastos</li>
        <li>Los gastos de sus subordinados</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Roles</td> 
      <td> <p>Con este acceso, el usuario puede hacer lo siguiente:</p> 
       <ul> 
        <li>Ver y editar las funciones de trabajo existentes</li> 
        <li>Añadir nuevas funciones de trabajo</li> 
        <li>Editar facturación de funciones y tasas de coste</li> 
       </ul> <p><b>IMPORTANTE</b>: Si concede a un usuario planificador acceso administrativo a funciones de trabajo, la configuración de acceso a datos financieros Editar función Facturación y tasas de coste se habilita automáticamente para el usuario. Posteriormente, si deshabilita el acceso administrativo a las funciones de trabajo para el usuario de Planificador, las funciones de trabajo seguirán estando visibles para el usuario porque la opción Editar tasas de costo y facturación de funciones sigue habilitada. Si esto sucede y necesita eliminar el acceso del usuario para ver las funciones de trabajo, debe desactivar la configuración de permiso Editar tasas de costes y facturación de funciones del usuario. Para obtener instrucciones, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Concesión de acceso a datos financieros</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hitos de mi grupo</td> 
      <td>Vea todas las rutas de hitos del sistema en el menú Rutas de hitos (Milestone Paths) de Configuración. Los usuarios también pueden editar o eliminar cualquier ruta de hito que pertenezca a cualquiera de sus grupos. Los usuarios no pueden administrar (editar o eliminar) las rutas de hitos que no están asignadas a ninguno de sus grupos.<br><p>Sin este acceso, los usuarios solo pueden ver las rutas de hitos existentes y aplicarlas a los proyectos a los que tengan acceso para administrarlos.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td>Cree y administre notificaciones de recordatorio en Workfront.<br>Sin este acceso, los usuarios se limitan a recibir y ver notificaciones.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hojas de horas y horas</td> 
      <td> <p>Permite a los usuarios ver todas las horas y partes de horas en Workfront.</p> <p>Cuando esta opción está desactivada, los usuarios solo pueden ver las horas siguientes:</p> 
       <ul> 
        <li>Proyectos, tareas o problemas que administran</li> 
        <li>Su propio parte de horas</li> 
        <li>Un parte de horas de alguien que les informa</li> 
        <li>Un parte de horas que aprueban</li> 
       </ul> <p><b>NOTA</b>:  <p>Tanto si esta opción está habilitada como si está deshabilitada, los administradores de grupos pueden crear perfiles de parte de horas para los grupos y subgrupos que administran y asignarlos a miembros de grupo cuyos perfiles de usuario tienen acceso para editar.</p> <p>Al habilitar esta opción, es posible que algunos administradores de grupos tengan demasiado acceso, ya que pueden ver las hojas de horas generadas por los perfiles de hojas de horas (y las horas) para todos los usuarios del sistema, no solo para los usuarios de los grupos que administran. Puede desactivar esta opción para los administradores de grupos que no necesitan este acceso.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cuando haya terminado, haga clic en **Guardar**.
1. Asigne el nuevo nivel de acceso a un usuario, tal como se describe en [Agregar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >Puede permitir que los usuarios tengan acceso administrativo a los usuarios. Para obtener más información sobre cómo otorgar acceso administrativo a los usuarios para que puedan administrar cuentas de usuario, consulte [Conceder acceso a los usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
