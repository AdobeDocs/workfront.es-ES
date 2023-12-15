---
title: Crear o modificar niveles de acceso personalizados
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede crear niveles de acceso personalizados y aplicarlos a los usuarios.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '1418'
ht-degree: 6%

---

# Crear y modificar niveles de acceso personalizados

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

Como administrador de Adobe Workfront, puede crear niveles de acceso personalizados y aplicarlos a los usuarios. A medida que trabaja con niveles de acceso, es importante comprender cómo funcionan junto con los permisos de objeto que conceden los usuarios cuando comparten objetos entre sí. Para obtener más información sobre los niveles de acceso, consulte:

* [Información general sobre nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Información general sobre niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>Le recomendamos encarecidamente que deje los niveles de acceso integrados sin cambios para que pueda hacer referencia a ellos después de configurar los usuarios. Para personalizar un nivel de acceso, copie el nivel de acceso predeterminado y modifique la copia. Puede hacerlo para cada nivel de acceso, excepto para el administrador del sistema y el usuario externo.

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
   <td>Nuevo: estándar
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

## Crear o editar un nivel de acceso personalizado

{{step-1-to-setup}}

1. Clic **Niveles de acceso** en el panel izquierdo.
1. Seleccione el nivel de acceso que desee copiar y personalizar y, a continuación, haga clic en **Copiar**.

   O

   Si está editando un nivel de acceso existente (que copió anteriormente), haga clic en su nombre.

1. En el cuadro que aparece, realice una de las siguientes acciones para comenzar a configurar el nivel de acceso personalizado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>Escriba un nombre para el nivel de acceso. </p> <p>Si acaba de copiar un nivel de acceso para crear uno nuevo, el nombre predeterminado es Nombre del nivel de acceso (Copiar), donde Nombre del nivel de acceso es el nivel de acceso que ha copiado.</p> <p><strong>Sugerencia</strong>: Se recomienda incluir el nombre original del nivel de acceso en el nombre de la copia. Por ejemplo, en la compañía ACME, una copia del nivel de acceso Estándar podría llamarse ACME Estándar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción </td> 
      <td>Escriba una descripción para el nivel de acceso. Es útil enumerar aquí a qué podrá acceder un usuario con este nivel de acceso.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de licencia</td> 
      <td>Asegúrese de que la licencia seleccionada aquí sea la que esté más estrechamente asociada al tipo de nivel de acceso que está creando o editando. La licencia seleccionada determina qué configuración está disponible para el nivel de acceso. Para obtener más información, consulte <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Información general sobre nuevas licencias</a> o <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Resumen de licencias</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Si **Standard** o **Plan** está seleccionado en la **Tipo de licencia** , desplácese hasta la sección **Permitir acceso administrativo para** y seleccione permisos de acceso administrativo para los que tendrán este nivel de acceso.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Procesos de aprobación</td> 
      <td>Cree y administre procesos de aprobación para su uso en todo el sistema y para grupos específicos.<p>Sin este acceso, los usuarios solo pueden crear procesos de aprobación ad hoc en los elementos que tienen acceso para administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compañías</td> 
      <td>Añada empresas nuevas y edite las existentes en Workfront.<br><p>Sin este acceso, los usuarios solo pueden ver las empresas existentes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td>Cree y administre todos los formularios personalizados de su grupo. <br><p>Sin este acceso, los usuarios solo pueden adjuntar formularios existentes a los objetos a los que tienen acceso para contribuir o administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tasas de cambio</td> 
      <td> Añada una nueva moneda en Workfront. <p>Sin este acceso, el usuario puede agregar una moneda existente solo a un proyecto que cree.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td>Vea todos los gastos en objetos en Workfront.<p>Sin este acceso, el usuario solo puede ver lo siguiente:</p>
       <ul>
        <li>Gastos en proyectos, tareas o problemas que administran</li>
        <li>Sus propios gastos</li>
        <li>Los gastos de sus subordinados</li>
       </ul><p><b>NOTA</b>: Esto no permite al usuario crear nuevos tipos de gastos.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Roles</td> 
      <td> Con este acceso, el usuario puede hacer lo siguiente: 
       <ul> 
        <li>Ver y editar los puestos de trabajo existentes</li> 
        <li>Agregar nuevos roles</li> 
        <li>Editar tarifas de facturación y de costo de rol</li> 
       </ul> 
       <p>Para obtener información importante sobre el acceso a los datos financieros disponibles para un usuario de Standard o Planner con acceso administrativo a las funciones del puesto, consulte <a href="#standard-or-planner-users-with-administrative-access-to-job-roles">Usuarios estándar o planificadores con acceso administrativo a los roles</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hitos de mi grupo</td> 
      <td>Vea todas las rutas de hitos del sistema en el menú Rutas de hitos de Configuración. Los usuarios también pueden editar o eliminar cualquier ruta de hitos que pertenezca a cualquiera de sus grupos. Los usuarios no pueden administrar (editar o eliminar) las rutas de hitos que no están asignadas a su grupo de grupos.<p>Sin este acceso, los usuarios solo pueden ver las rutas de hitos existentes y aplicarlas a los proyectos a los que tienen acceso para administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td>Cree y administre notificaciones de recordatorio en Workfront.<p>Sin este acceso, los usuarios se limitan a recibir y ver notificaciones.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hojas de horas y horas</td> 
      <td> Los administradores de grupos pueden asignar perfiles de hojas de horas a los usuarios en los grupos y subgrupos que administran. <p>Sin esta opción habilitada, los administradores de grupos no pueden asignar perfiles de hojas de horas a otros usuarios en los grupos y subgrupos que administran, aunque sí pueden crearlos.</p> <p>Todos los demás usuarios con licencia estándar o de planificación pueden ver todas las horas y hojas de horas en Workfront.</p> <p>Sin esta opción habilitada, los usuarios solo pueden ver las horas de:</p> 
       <ul> 
        <li>Proyectos, tareas o problemas que administran</li> 
        <li>Su propia hoja de horas</li> 
        <li>Hoja de horas de un subordinado</li> 
        <li>Hoja de horas que aprueban</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Establecer restricciones adicionales**, y establezca cualquiera de las siguientes restricciones para el nivel de acceso.

   >[!IMPORTANT]
   >
   >Para usuarios externos como proveedores (cualquier persona que no pertenezca a su organización), le recomendamos que restrinja el acceso a tareas, proyectos, actualizaciones, anuncios, otras empresas, equipos y grupos.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nunca dar acceso a todo el proyecto al asignar una tarea o un problema</td> 
      <td> Evita que los usuarios asignados a tareas o problemas también obtengan permisos en el proyecto principal, aunque los permisos del proyecto lo permitan.<p>Para obtener más información sobre cómo configurar los permisos en un proyecto, consulte la sección <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> en el artículo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar proyectos</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Nunca heredar el acceso a documentos de proyectos, tareas, problemas, etc.</td> 
      <td>Impide que los documentos hereden los permisos establecidos en su objeto principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ver solamente las actualizaciones en las cuales se les haya incluido en la conversación</td> 
      <td> Permite a los usuarios ver solo comentarios donde se ha incluido su nombre o el nombre de su equipo. <p> <p><b>NOTA</b>: Esto evita que los usuarios se suscriban a los elementos de Workfront. Para obtener más información sobre la suscripción a elementos, consulte <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Suscribirse a elementos en Adobe Workfront</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir que los usuarios eliminen comentarios </td> 
      <td> Impide que los usuarios eliminen los comentarios que realizan sobre los elementos.  <p><b>NOTA</b>: Nadie puede eliminar los comentarios de otros usuarios.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ver solamente compañías, grupos y equipos a los que pertenecen</td> 
      <td>Permite a los usuarios ver y compartir elementos únicamente con compañías, grupos y equipos a los que pertenecen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir visibilidad de horas planificadas u horas reales</td> 
      <td>Impide que los usuarios vean las horas de trabajo planificadas y reales a las que tienen acceso. Sin embargo, pueden ver las horas reales que registran ellos mismos o las horas que registra alguien que depende de ellos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir que los usuarios eliminen anuncios</td> 
      <td>Impide que los usuarios eliminen anuncios en el Centro de anuncios. Para obtener más información, consulte <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Envío de anuncios</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional y opcional) Si el sistema Workfront está configurado para usuarios que pertenecen a varias empresas, limite la visibilidad a otros usuarios en función de la empresa a la que pertenezcan en la sección **Las personas de otras empresas solo deben ver a los usuarios de**.

   Puede restringir el acceso de los usuarios para que solo vean usuarios de su propia compañía o de la compañía que designó como compañía principal. La compañía principal suele representar su cuenta de Workfront, donde trabaja la mayoría de los usuarios. Para obtener más información sobre la empresa principal, consulte [Crear y editar compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >Si dos usuarios pertenecen a dos empresas diferentes, pero ambos pueden ver usuarios de la empresa principal, pueden ver el área de Actualizaciones asociada a la empresa principal.

1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas del nivel de acceso en el que está trabajando, continúe con uno de los artículos enumerados en [Configuración del acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Concesión de acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario (a menos que sea un nivel de acceso de administrador del sistema).

   Para obtener más información, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   Para obtener información sobre cómo un administrador de Adobe asigna un nivel de acceso de administrador del sistema a un usuario, consulte [Conceder a un usuario acceso administrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Usuarios estándar o planificadores con acceso administrativo a los roles {#planner-users}

Si concede a un usuario estándar o planificador acceso administrativo a los roles de trabajo, la configuración Editar tarifas de facturación y de costo de rol se activa automáticamente para el usuario.

Posteriormente, si desactiva el acceso administrativo a los roles para el usuario, los roles de trabajo seguirán siendo visibles para el usuario porque la opción Editar tarifas de facturación y de coste del rol seguirá activada.

Si esto sucede y necesita eliminar el acceso del usuario para ver los roles de trabajo, debe deshabilitar la configuración de permiso Editar tarifas de facturación y de costo de rol del usuario. Para obtener instrucciones, consulte [Concesión de acceso a los datos financieros](grant-access-financial.md).
