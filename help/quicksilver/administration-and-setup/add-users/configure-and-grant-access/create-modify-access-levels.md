---
title: Crear o modificar niveles de acceso personalizados
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede crear niveles de acceso personalizados y aplicarlos a los usuarios.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '1402'
ht-degree: 6%

---

# Crear y modificar niveles de acceso personalizados

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help.-->

Como administrador de Adobe Workfront, puede crear niveles de acceso personalizados y aplicarlos a los usuarios. Al trabajar con niveles de acceso, es importante comprender cómo funcionan junto con los permisos de objeto que los usuarios conceden cuando comparten objetos entre sí. Para obtener más información sobre los niveles de acceso, consulte

* [Información general sobre los nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!IMPORTANT]
>
>Se recomienda dejar los niveles de acceso integrados sin cambios para poder consultarlos después de configurar los usuarios. Para personalizar un nivel de acceso, copie el nivel de acceso predeterminado y modifique la copia. Puede hacerlo para todos los niveles de acceso excepto para el administrador del sistema y el usuario externo.

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
   <td>Plan actual: Estándar
   <p>o</p>
   <p>Plan heredado: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

## Crear o editar un nivel de acceso personalizado

{{step-1-to-setup}}

1. Haga clic en **Niveles de acceso** en el panel izquierdo.
1. Seleccione el nivel de acceso que desea copiar y personalizar y, a continuación, haga clic en **Copiar**.

   O

   Si está editando un nivel de acceso existente (que ha copiado anteriormente), haga clic en su nombre.

1. En el cuadro que aparece, realice una de las acciones siguientes para comenzar a configurar el nivel de acceso personalizado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>Escriba un nombre para el nivel de acceso. </p> <p>Si acaba de copiar un nivel de acceso para crear uno nuevo, el nombre predeterminado es Nombre de nivel de acceso (copia), donde Nombre de nivel de acceso es el nivel de acceso que ha copiado.</p> <p><strong>Sugerencia</strong>: Se recomienda incluir el nombre original del nivel de acceso en el nombre de la copia. Por ejemplo, en la empresa ACME, una copia del nivel de acceso estándar podría llamarse ACME Standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción </td> 
      <td>Escriba una descripción para el nivel de acceso. Es útil enumerar aquí a qué puede acceder un usuario con este nivel de acceso.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de licencia</td> 
      <td>Asegúrese de que la licencia seleccionada aquí sea la que esté más estrechamente asociada con el tipo de nivel de acceso que está creando o editando. La licencia seleccionada determina qué configuración está disponible para el nivel de acceso. Para obtener más información, consulte <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Información general sobre nuevas licencias</a> o <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Información general sobre licencias</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Si **Estándar** o **Plan** se selecciona en la variable **Tipo de licencia** , desplácese hasta la sección **Permitir acceso administrativo para** y seleccione permisos de acceso administrativo para aquellos que tengan este nivel de acceso.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Procesos de aprobación</td> 
      <td>Cree y administre procesos de aprobación para utilizarlos en todo el sistema y para grupos específicos.<p>Sin este acceso, los usuarios solo pueden crear procesos de aprobación específicos en los elementos a los que tienen acceso para administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compañías</td> 
      <td>Agregue nuevas empresas y edite las existentes en Workfront.<br><p>Sin este acceso, los usuarios solo pueden ver las empresas existentes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td>Cree y administre todos los formularios personalizados dentro de su grupo. <br><p>Sin este acceso, los usuarios solo pueden adjuntar formularios existentes a los objetos a los que tienen acceso para contribuir o administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tasas de cambio</td> 
      <td> <p>Añada nueva moneda en Workfront.</p> <p>Sin este acceso, el usuario puede agregar una moneda existente solo a un proyecto que cree.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td>Ver todos los gastos de los objetos en Workfront.<p>Sin este acceso, el usuario solo puede ver lo siguiente:</p>
       <ul>
        <li>Gastos en proyectos, tareas o problemas que administran</li>
        <li>Sus propios gastos</li>
        <li>Los gastos de sus subordinados</li>
       </ul><p><b>NOTA</b>: Esto no permite al usuario crear nuevos tipos de gastos.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Roles</td> 
      <td> <p>Con este acceso, el usuario puede hacer lo siguiente:</p> 
       <ul> 
        <li>Ver y editar las funciones de trabajo existentes</li> 
        <li>Añadir nuevas funciones de trabajo</li> 
        <li>Editar facturación de funciones y tasas de coste</li> 
       </ul> 
       <p>Para obtener información importante sobre el acceso a los datos financieros disponibles para un usuario estándar o planificador con acceso administrativo a funciones de trabajo, consulte <a href="#planner-users-with-administrative-access-to-job-roles">Usuarios estándar o de planificación con acceso administrativo a funciones de trabajo</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hitos de mi grupo</td> 
      <td>Vea todas las rutas de hitos del sistema en el menú Rutas de hitos (Milestone Paths) de Configuración. Los usuarios también pueden editar o eliminar cualquier ruta de hito que pertenezca a cualquiera de sus grupos. Los usuarios no pueden administrar (editar o eliminar) rutas de hitos que no estén asignadas a sus grupos.<p>Sin este acceso, los usuarios solo pueden ver las rutas de hitos existentes y aplicarlas a los proyectos a los que tengan acceso para administrarlos.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td>Cree y administre notificaciones de recordatorio en Workfront.<p>Sin este acceso, los usuarios se limitan a recibir y ver notificaciones.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hojas de horas y horas</td> 
      <td> <p>Los administradores de grupos pueden asignar perfiles de parte de horas a usuarios de los grupos y subgrupos que administran.</p> <p>Sin esta opción habilitada, los administradores de grupos no pueden asignar perfiles de parte de horas a otros usuarios de los grupos y subgrupos que administran, aunque sí pueden crearlos.</p> <p>Todos los demás usuarios con una licencia de Standard o Plan pueden ver todas las horas y partes de horas en Workfront.</p> <p>Sin esta opción habilitada, los usuarios solo pueden ver las horas en:</p> 
       <ul> 
        <li>Proyectos, tareas o problemas que administran</li> 
        <li>Su propio parte de horas</li> 
        <li>Un parte de horas de alguien que les informa</li> 
        <li>Un parte de horas que aprueban</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Establecer restricciones adicionales**, establezca cualquiera de las siguientes restricciones para el nivel de acceso.

   >[!IMPORTANT]
   >
   >Para usuarios externos como proveedores (cualquier persona que no pertenezca a su organización), se recomienda restringir el acceso a tareas, proyectos, actualizaciones, anuncios, otras empresas, equipos y grupos.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nunca dar acceso a todo el proyecto al asignar una tarea o un problema</td> 
      <td> Evita que los usuarios asignados a tareas o problemas también obtengan permisos para el proyecto principal, incluso si los permisos del proyecto lo permiten.<p>Para obtener más información sobre la configuración de los permisos de un proyecto, consulte la sección <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> en el artículo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar proyectos</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Nunca heredar el acceso a documentos de proyectos, tareas, problemas, etc.</td> 
      <td>Evita que los documentos hereden los permisos establecidos en su objeto principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ver solamente las actualizaciones en las cuales se les haya incluido en la conversación</td> 
      <td> <p>Permite a los usuarios ver solo los comentarios en los que se ha incluido su nombre o el nombre de su equipo.</p> <p> <p><b>NOTA</b>: Esto evita que los usuarios se suscriban a elementos en Workfront. Para obtener más información sobre la suscripción a elementos, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Agregar usuarios</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir que los usuarios eliminen comentarios </td> 
      <td> <p>Impide que los usuarios eliminen los comentarios que realizan sobre los elementos. </p> <p><b>NOTA</b>: Nadie puede eliminar los comentarios de otros usuarios.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ver solamente compañías, grupos y equipos a los que pertenecen</td> 
      <td>Permite a los usuarios ver y compartir artículos únicamente con empresas, grupos y equipos a los que pertenecen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir visibilidad de horas planificadas u horas reales</td> 
      <td>Impide que los usuarios vean los elementos de horas de trabajo planeadas y reales a los que tienen acceso. Sin embargo, pueden ver las horas reales en las que se registran por sí mismos o las horas registradas por alguien que les informa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir que los usuarios eliminen anuncios</td> 
      <td>Impide que los usuarios eliminen anuncios del Centro de anuncios. Para obtener más información, consulte <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Enviar anuncios</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional y opcional) Si el sistema de Workfront está configurado para usuarios que pertenecen a varias empresas, restrinja la visibilidad a otros usuarios en función de la empresa a la que pertenezcan en la sección **Las personas de otras empresas solo deben ver los usuarios de**.

   Puede restringir el acceso de los usuarios solo a los usuarios de su propia empresa o de la empresa que designó como empresa principal. Para obtener más información sobre la empresa principal, consulte [Crear y editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >Si dos usuarios pertenecen a dos empresas diferentes, pero ambas pueden ver usuarios de la empresa principal, pueden ver el área Actualizaciones asociada con la empresa principal.

1. (Opcional) Para configurar las opciones de acceso de otros objetos y áreas del nivel de acceso en el que esté trabajando, continúe con uno de los artículos enumerados en [Configuración del acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Concesión de acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario (a menos que sea un nivel de acceso del administrador del sistema).

   Para obtener más información, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   Para obtener información sobre cómo un administrador de Adobe asigna un nivel de acceso de administrador del sistema a un usuario, consulte [Conceder a un usuario acceso administrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Usuarios estándar o de planificación con acceso administrativo a funciones de trabajo {#planner-users}

Si concede acceso administrativo de usuario de Standard o Planner a las funciones de trabajo, la configuración Editar tasas de costes y facturación de funciones se habilita automáticamente para el usuario.

Posteriormente, si deshabilita el acceso administrativo a las funciones de trabajo para el usuario, las funciones de trabajo seguirán estando visibles para el usuario porque la opción Editar tasas de costes y facturación de funciones sigue habilitada.

Si esto sucede y necesita eliminar el acceso del usuario para ver las funciones de trabajo, debe desactivar la configuración de permiso Editar tasas de costes y facturación de funciones del usuario. Para obtener instrucciones, consulte [Concesión de acceso a datos financieros](grant-access-financial.md).
