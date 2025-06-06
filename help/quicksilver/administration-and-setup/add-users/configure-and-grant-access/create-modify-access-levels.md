---
title: Creación y modificación de niveles de acceso personalizados
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede crear niveles de acceso personalizados y aplicarlos a los usuarios.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 674c46b699ba445abba06bec3e4da4a710c60d63
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 94%

---

# Creación y modificación de niveles de acceso personalizados

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

Como administrador de Adobe Workfront, puede crear niveles de acceso personalizados y aplicarlos a los usuarios. Al trabajar con niveles de acceso, es importante comprender cómo funcionan junto con los permisos de objeto que conceden los usuarios cuando comparten objetos entre sí. Para obtener más información sobre los niveles de acceso, consulte:

* [Información general sobre nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Información general de los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>Le recomendamos encarecidamente que no modifique los niveles de acceso integrado para poder consultarlos después de configurar los usuarios. Para personalizar un nivel de acceso, copie el nivel de acceso predeterminado y modifique la copia. Puede hacerlo para cada nivel de acceso, excepto para el administrador del sistema y el usuario externo.

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

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación o edición de un nivel de acceso personalizado

{{step-1-to-setup}}

1. Haga clic en **Niveles de acceso** en el panel izquierdo.
1. &#x200B;
   * En el entorno de producción:
Seleccione el nivel de acceso que quiera copiar y personalizar y luego haga clic en **Copiar**.

     O

     Si está editando un nivel de acceso existente (que copió anteriormente), haga clic en su nombre.

   * <span class="preview">En el entorno de vista previa:</span>

     <span class="preview">Seleccione el nivel de acceso que desee copiar y personalizar y, a continuación, haga clic en el icono **Copiar** ![Icono Copiar](assets/copy-icon.png). </span>

     <span class="preview">O </span>

     <span class="preview">Si está editando un nivel de acceso existente, seleccione el nivel de acceso haciendo clic en el cuadro situado a la izquierda de dicho nivel de acceso y, a continuación, haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png). </span>

1. Realice una de las siguientes acciones en el cuadro que aparece para comenzar a configurar el nivel de acceso personalizado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>Escriba un nombre para el nivel de acceso. </p> <p>Si acaba de copiar un nivel de acceso para crear uno nuevo, el nombre predeterminado será Nombre del nivel de acceso (Copiar), que es el nivel de acceso que ha copiado.</p> <p><strong>Sugerencia</strong>: Se recomienda incluir el nombre original del nivel de acceso en el nombre de la copia. Por ejemplo, en la compañía ACME, la copia del nivel de acceso Estándar podría llamarse ACME Estándar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción </td> 
      <td>Escriba una descripción para el nivel de acceso. Aquí, resulta útil enumerar a qué podrá acceder un usuario con este nivel de acceso.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de licencia</td> 
      <td>Asegúrese de que la licencia seleccionada aquí sea la que esté más estrechamente asociada al tipo de nivel de acceso que está creando o editando. La licencia seleccionada determina qué configuración está disponible para el nivel de acceso. Para obtener más información, consulte <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Información general sobre nuevas licencias</a> o <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Información general sobre licencias</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Si **Estándar** o **Plan** está seleccionado en el cuadro **Tipo de licencia**, desplácese hasta la sección **Permitir acceso administrativo para** y seleccione permisos de acceso administrativo para los que vayan a tener este nivel de acceso.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Procesos de aprobación</td> 
      <td>Cree y administre procesos de aprobación para su uso en todo el sistema y para grupos específicos.<p>Sin este acceso, los usuarios pueden crear únicamente procesos de aprobación ad hoc en los elementos a los que tienen acceso para administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compañías</td> 
      <td>Añada compañías nuevas y edite las existentes en Workfront.<br><p>Sin este acceso, los usuarios solo pueden ver las empresas existentes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td>Cree y administre todos los formularios personalizados de su grupo. <br><p>Sin este acceso, los usuarios solo pueden adjuntar formularios existentes a los objetos a los que tienen acceso de aportación o administración.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipos de cambio</td> 
      <td> Añada una nueva moneda en Workfront. <p>Sin este acceso, el usuario puede añadir una moneda existente solo a un proyecto que cree.</p> </td> 
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
        <li>Ver y editar las funciones existentes</li> 
        <li>Añadir más funciones</li> 
        <li>Editar las tarifas de facturación y de costes de funciones</li> 
       </ul> 
       <p>Para obtener información importante sobre el acceso a los datos financieros disponibles para un usuario con licencia estándar o de planificador y acceso administrativo a las funciones, consulte <a href="#standard-or-planner-users-with-administrative-access-to-job-roles">Usuarios con licencia estándar o de planificador y acceso administrativo a las funciones</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hitos de mi grupo</td> 
      <td>Vea todas las rutas de hitos del sistema en el menú Rutas de hitos en Configuración. Los usuarios también pueden editar o eliminar cualquier ruta de hitos que pertenezca a cualquiera de sus grupos. Los usuarios no pueden administrar (editar o eliminar) las rutas de hitos que no estén asignadas a sus grupos.<p>Sin este acceso, los usuarios solo pueden ver las rutas de hitos existentes y aplicarlas a los proyectos a los que tienen acceso para administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td>Cree y administre notificaciones de recordatorio en Workfront.<p>Sin este acceso, los usuarios se limitan a recibir y ver notificaciones.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hojas de horas y horas</td> 
      <td> Los administradores de grupos pueden asignar perfiles de plantilla de horas a los usuarios en los grupos y subgrupos que administran. <p>Sin esta opción habilitada, los administradores de grupos no pueden asignar perfiles de plantilla de horas a otros usuarios en los grupos y subgrupos que administran, aunque sí pueden crearlos.</p> <p>Todos los demás usuarios con licencia estándar o de planificación pueden ver todas las horas y plantillas de horas en Workfront.</p> <p>Sin esta opción habilitada, los usuarios solo pueden ver las horas de:</p> 
       <ul> 
        <li>Proyectos, tareas o problemas que administran</li> 
        <li>Su propia plantilla de horas</li> 
        <li>Una plantilla de horas de un subordinado</li> 
        <li>Una plantilla de horas que aprueban</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Establecer restricciones adicionales** y, a continuación, establezca cualquiera de las restricciones siguientes de nivel de acceso.

   >[!IMPORTANT]
   >
   >Para usuarios externos como proveedores (cualquier persona que no pertenezca a su organización), le recomendamos que restrinja el acceso a tareas, proyectos, actualizaciones, anuncios, otras compañías, equipos y grupos.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nunca dar acceso a todo el proyecto al asignar una tarea o un problema</td> 
      <td> Evita que los usuarios asignados a tareas o problemas también obtengan permisos sobre el proyecto principal, aunque los permisos de proyecto lo permitan.<p>Para obtener más información sobre la configuración de los permisos de proyecto, consulte la sección <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> del artículo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar proyectos</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Nunca heredar el acceso a documentos de proyectos, tareas, problemas, etc.</td> 
      <td>Impide que los documentos hereden los permisos establecidos sobre su objeto principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ver solamente las actualizaciones en las cuales se les haya incluido en la conversación</td> 
      <td> Permite a los usuarios ver solo comentarios donde se ha incluido su nombre o el nombre de su equipo. <p> <p><b>NOTA</b>: Esto evita que los usuarios se suscriban a elementos en Workfront. Para obtener más información acerca de la suscripción a elementos, consulte <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Suscribirse a elementos en Adobe Workfront</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir que los usuarios eliminen comentarios </td> 
      <td> Impide que los usuarios eliminen los comentarios que realizan sobre los elementos.  <p><b>NOTA</b>: Nadie puede eliminar los comentarios de otros usuarios.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ver solamente compañías, grupos y equipos a los que pertenecen</td> 
      <td>Permite a los usuarios ver y compartir elementos únicamente con compañías, grupos y equipos a los que pertenecen.<p><strong>NOTA</strong>: los usuarios con licencias de Solicitante o Colaborador no pueden ver las empresas a las que no pertenecen, aunque se haya seleccionado esta opción.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir visibilidad de horas planificadas u horas reales</td> 
      <td>Impide que los usuarios vean las horas de trabajo planificadas y reales a las que tienen acceso. Sin embargo, pueden ver las horas reales que registran ellos mismos o las horas que registra alguien que esté bajo sus órdenes.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir que los usuarios eliminen anuncios</td> 
      <td>Impide que los usuarios eliminen anuncios en el Centro de anuncios. Para obtener más información, consulte <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Enviar anuncios</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional y opcional) Si el sistema Workfront está configurado para usuarios que pertenecen a varias compañías, limite la visibilidad a otros usuarios en función de la compañía a la que pertenezcan en la sección **Las personas de otras compañías deberán ver solamente a los usuarios de**.

   Puede restringir el acceso de los usuarios para que solo vean usuarios de su propia compañía o de la compañía que designó como compañía principal. La compañía principal suele representar su cuenta de Workfront, donde trabaja la mayoría de los usuarios. Para obtener más información sobre la compañía principal, consulte [Crear y editar compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >Si dos usuarios pertenecen a dos compañías diferentes, pero ambos pueden ver usuarios de la compañía principal, pueden ver el área de Actualizaciones asociada a la compañía principal.

1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas en el nivel de acceso en el que está trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a las tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario (a menos que sea un nivel de acceso de administrador del sistema).

   Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   Para obtener información sobre cómo un administrador de Adobe asigna un nivel de acceso de administrador del sistema a un usuario, consulte [Conceder a un usuario acceso administrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Usuarios Estándar o Planificador con acceso administrativo a las funciones {#planner-users}

Si concede a un usuario Estándar o Planificador acceso administrativo a las funciones, la configuración Editar tarifas de facturación y de costes de funciones se activa automáticamente para el usuario.

Posteriormente, si deshabilita el acceso administrativo a las funciones para el usuario, las funciones aún serán visibles para el usuario porque la opción Editar tarifas de facturación y de costes de funciones aún está habilitada.

Si esto sucede y necesita eliminar el acceso del usuario para ver las funciones, debe deshabilitar la configuración del permiso del usuario Editar tarifas de facturación y de costo de rol. Para obtener más instrucciones, consulte [Concesión de acceso a los datos financieros](grant-access-financial.md).



