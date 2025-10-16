---
title: Conceder a los usuarios acceso administrativo a determinadas áreas
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para otorgar a los usuarios con una licencia de planificación acceso administrativo a determinadas áreas del sistema.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 99%

---

# Conceder a los usuarios acceso administrativo a determinadas áreas

<!--Linked in several places, do not rename or change URL.-->

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para otorgar a los usuarios con una licencia de planificación acceso administrativo a determinadas áreas del sistema.

>[!NOTE]
>
>Esto es diferente a otorgar a un usuario acceso administrativo completo a Workfront, como se explica en [Conceder a un usuario acceso administrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).&#x200B;

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>   <p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conceder a los usuarios del plan acceso administrativo a ciertas áreas de Workfront

>[!IMPORTANT]
>
>Le recomendamos encarecidamente que no modifique los niveles de acceso integrado para poder consultarlos después de configurar los usuarios. Para personalizar un nivel de acceso, copie el nivel de acceso predeterminado y modifique la copia. (Puede hacerlo para todos los niveles de acceso, excepto para el Administrador del sistema y el Usuario externo).

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Niveles de acceso**.
1. Haga clic en el nombre del nivel de acceso que desee utilizar para otorgar a los usuarios acceso administrativo a determinadas áreas de Workfront.
1. En la sección **Permitir acceso administrativo para**, active las casillas para conceder el acceso administrativo necesario.

   Estas opciones le permiten conceder las siguientes capacidades:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Procesos de aprobación</td> 
      <td><p>Cree y administre procesos de aprobación para su uso en todo el sistema y para grupos específicos.</p><p>Sin este acceso, los usuarios solo pueden crear procesos de aprobación ad-hoc en los elementos a los que tienen acceso para administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compañías</td> 
      <td><p>Añadir compañías nuevas y editar las existentes en Workfront</p>
      <p>Sin este acceso, los usuarios solo pueden ver las empresas existentes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td><p>Cree y edite (añada, edite y elimine los campos) formularios personalizados dentro de su grupo.</p><p>Sin este acceso, los usuarios solo pueden adjuntar formularios existentes a objetos a los que tengan acceso para contribuir o administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipos de cambio</td> 
      <td> <p>Añada una nueva moneda en Workfront.</p> <p>Sin este acceso, el usuario solo puede añadir una moneda existente a un proyecto que cree.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td><p>Vea todos los gastos en objetos en Workfront.</p><p>Esto no permite al usuario crear nuevos tipos de gastos.</p><p>Sin este acceso, el usuario solo puede ver lo siguiente:</p>
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
        <li>Ver y editar las funciones existentes</li> 
        <li>Añadir más funciones</li> 
        <li>Editar las tarifas de facturación y de costes de funciones</li> 
       </ul> <p><b>IMPORTANTE</b>: Si concede a un usuario Planificador acceso administrativo a las funciones, la configuración de acceso a datos financieros Editar tarifas de facturación y de costes de funciones se habilita automáticamente para el usuario. Posteriormente, si deshabilita el acceso administrativo a las funciones para el usuario Planificador, las funciones aún serán visibles para el usuario porque la opción Editar tarifas de facturación y de costes de funciones aún está habilitada. Si esto sucede y necesita eliminar el acceso del usuario para ver las funciones, debe deshabilitar la configuración del permiso del usuario Editar tarifas de facturación y de costo de rol. Para obtener más instrucciones, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acceso a datos financieros</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hitos de mi grupo</td> 
      <td>Vea todas las rutas de hitos del sistema en el menú Rutas de hitos en Configuración. Los usuarios también pueden editar o eliminar cualquier ruta de hitos que pertenezca a cualquiera de sus grupos. Los usuarios no pueden administrar (editar o eliminar) las rutas de hitos que no están asignadas a ninguno de sus grupos.<br><p>Sin este acceso, los usuarios solo pueden ver las rutas de hitos existentes y aplicarlas a los proyectos a los que tienen acceso para administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td>Cree y administre notificaciones de recordatorio en Workfront.<br>Sin este acceso, los usuarios se limitan a recibir y ver notificaciones.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hojas de horas y horas</td> 
      <td> <p>Permite a los usuarios ver todas las horas y plantillas de horas en Workfront.</p> <p>Cuando esta opción está deshabilitada, los usuarios solo pueden ver las horas en:</p> 
       <ul> 
        <li>Proyectos, tareas o problemas que administran</li> 
        <li>Su propia plantilla de horas</li> 
        <li>Una plantilla de horas de un subordinado</li> 
        <li>Una plantilla de horas que aprueban</li> 
       </ul> <p><b>NOTA</b>:  <p>Independientemente de si esta opción está habilitada o deshabilitada, los administradores de grupos pueden crear perfiles de plantillas de horas para los grupos y subgrupos que administran y asignarlas a miembros del grupo cuyos perfiles de usuario tengan acceso para editar.</p> <p>Si se habilita esta opción, es posible que algunos administradores de grupos tengan demasiado acceso, ya que pueden ver las plantillas de horas generadas por los perfiles de la plantilla de horas (y las horas) para todos los usuarios del sistema y no solo las de los grupos que administran. Puede desactivar esta opción para los administradores de grupos que no necesiten tanto acceso.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cuando termine, haga clic en **Guardar**.
1. Asigne el nuevo nivel de acceso a un usuario, tal como se describe en [Añadir usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >Puede permitir que los usuarios tengan acceso administrativo a los usuarios. Para obtener más información sobre cómo otorgar a los usuarios acceso administrativo a usuarios para poder administrar cuentas de usuario, consulte [Conceder acceso a usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
