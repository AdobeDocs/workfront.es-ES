---
title: Crear un proceso de aprobación para elementos de trabajo
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Cree un proceso de aprobación que los usuarios puedan adjuntar a un elemento de trabajo (proyecto, tarea, problema, plantilla o tarea de plantilla), un documento o una prueba. Un proceso de aprobación garantiza que los usuarios asignados al objeto revisen ciertos cambios antes de que el objeto progrese en el sistema.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 92%

---

# Crear un proceso de aprobación para los elementos de trabajo

<!-- Audited: 08/2025-->

<!--see below the "hidden" content for the redesigned tabs - August 2023-->

Cree un proceso de aprobación que los usuarios puedan adjuntar a un elemento de trabajo (proyecto, tarea, problema, plantilla o tarea de plantilla), un documento o una prueba. Un proceso de aprobación garantiza que los usuarios asignados al objeto revisen ciertos cambios antes de que el objeto progrese en el sistema.

En este artículo se describe cómo crear procesos de aprobación globales de nivel de sistema o de grupo para elementos de trabajo (proyecto, tarea, problema, plantilla o tarea de plantilla).

Para obtener información sobre las aprobaciones asociadas con documentos o pruebas, consulte los siguientes artículos:

* [Solicitar aprobaciones de documentos](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [Información general sobre flujos de trabajo automatizados](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>Los usuarios también pueden crear procesos de aprobación de un solo uso para un proyecto, tarea, problema, plantilla o tarea de plantilla en el que tengan permisos de administración.
>
>En este artículo se utiliza el término “proceso de aprobación global” para diferenciarlo de los procesos de aprobación de un solo uso. Un proceso de aprobación global se puede utilizar repetidamente.
>
>En el nivel de grupo, un proceso de aprobación global está restringido a los elementos de trabajo y estados que pertenezcan al grupo.
>
>Para obtener información acerca de los procesos de aprobación de un solo uso, consulte [Introducción a los procesos de aprobación](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md) y [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete Adobe Workfront*</td> 
   <td><p>Para el proceso de aprobación de un solo uso o de nivel de sistema:</p><ul><li><p>Cualquier paquete</p></li></ul>
   <p>Para el proceso de aprobación a nivel de grupo:</p>
   <ul><li><p>Flujo de trabajo de Prime o Ultimate</p></li>
   <li><p>WORKFRONT PRIME o ULTIMATE</p></li></ul>
   </td>

</tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
 <p>Plan</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Si es administrador del sistema o tiene acceso administrativo a los procesos de aprobación, puede crear un proceso de aprobación de nivel de sistema o de nivel de grupo para un grupo determinado.</p> 
   <p>Si es administrador de un grupo y tiene acceso administrativo a los procesos de aprobación, puede crear procesos de aprobación de nivel de grupo para los grupos que administra.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td><p>System-level or single-use approval process: Any</p>
   <p>Group-level approval process: Prime or Ultimate</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p>
 <p>or</p> 
<p>Current: Plan </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>If you are a system administrator or you have administrative access to approval processes, you can create a system-level approval process, or a group-level approval process for a particular group.</p> 
   <p>If you are a group administrator, you can create group-level approval processes for groups that you manage.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->


## Crear un proceso de aprobación global de nivel de sistema o de grupo para elementos de trabajo

{{step-1-to-setup}}

1. (Condicional) Si crea un proceso de aprobación de nivel de sistema, haga clic en **Procesos** > **Aprobaciones** en el panel izquierdo.

   O

   Si está creando un proceso de aprobación de nivel de grupo, haga clic en **Grupos** ![Icono de grupos](assets/groups-icon.png), haga clic en el nombre del grupo y luego haga clic en **Aprobaciones**.

   <!--hidden for the new tab redesign - August 2023: 
   ![Approvals area in setup](assets/approvals-area-in-setup-processes.png)
   -->

1. Elija la pestaña **Aprobaciones de proyectos**, **Aprobaciones de tareas** o **Aprobaciones de problemas**.

1. Haga clic en **Nuevo proceso de aprobación**.
1. Especifique la siguiente información en el cuadro que se muestra:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de proceso de aprobación</td> 
      <td><p>Escriba un nombre descriptivo para el proceso de aprobación. Los usuarios ven este nombre al aplicar el proceso de aprobación a un objeto, como se describe en <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Asociar un proceso de aprobación nuevo o existente con el trabajo</a>.</p> <p> Este campo es obligatorio. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td><p>Escriba una descripción del proceso de aprobación. Esto se muestra en la sección <b>Aprobaciones</b> en el área <b>Configuración</b>, junto al nombre del proceso de aprobación.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activo</td> 
      <td> <p>Mantenga esta opción habilitada si desea que otros usuarios puedan adjuntar el proceso de aprobación a los proyectos, tareas y problemas que creen. </p> <p>Esta opción está habilitada de forma predeterminada.</p> <p> Consejo: Marcar un proceso de aprobación como inactivo es útil cuando su organización ya no necesita utilizarlo, pero desea conservar la información histórica sobre su uso.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Este proceso de aprobación lo puede utilizar </td> 
      <td> <p>Si desea que el proceso de aprobación esté disponible para proyectos, tareas, problemas y plantillas que pertenezcan solo a un grupo en particular, comience a escribir el nombre del grupo y seleccione el nombre cuando aparezca:</p> 
       <ul> 
       <li>Si es administrador del sistema o tiene acceso administrativo a los procesos de aprobación, puede ver cualquier grupo del sistema cuando escriba su nombre. <b>Todos los grupos</b> está seleccionado de forma predeterminada. </li> 
       <li>Si es un administrador de grupo sin acceso administrativo a los procesos de aprobación, puede asignar el proceso de aprobación a cualquier grupo que administre cuando escriba su nombre. La opción <b>Todos los grupos</b> no está disponible.</li> 
       </ul> 
       <p>Este campo es obligatorio.</p>
       <p>Esta opción no está disponible para procesos de aprobación de un solo uso.</p> 
       <p><b>ADVERTENCIA</b></p> <p> Al realizar cambios en el proceso de aprobación específico del grupo, es posible que cambien los procesos de aprobación existentes que ya se han asociado con elementos de trabajo. Para obtener información acerca de estos cambios, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Cómo afectan los cambios de grupos y procesos de aprobación a los procesos de aprobación asignados</a>.</p> 
       <p>Para obtener información sobre cómo listar y gestionar los procesos de aprobación de su grupo desde la página de su grupo, consulte <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Procesos de aprobación a nivel de grupo</a>. </p> 
       <p>Para obtener información acerca del acceso administrativo a los procesos de aprobación, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Configure una ruta para el proceso de aprobación mediante las siguientes opciones.

   Una ruta es donde se especifica lo que debe suceder en el proceso de aprobación. Las fases se crean en una ruta para indicar quién debe realizar el trabajo de aprobación y en qué orden.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Iniciar el proceso de aprobación cuando el estado esté definido como</p> </td> 
      <td> <p>Seleccione el estado que activa el proceso de aprobación en los elementos de trabajo. Cuando alguien actualiza un elemento de trabajo a este estado, comienza su proceso de aprobación. </p> 
      <p>Este campo es obligatorio. </p>
      <p>No se puede seleccionar el mismo estado para varias rutas de proceso de aprobación.</p> <p>Los estados disponibles se basan en lo seleccionado en la opción <b>Esta aprobación puede ser utilizada por </b> (explicado en la tabla anterior):</p> 
       <ul> 
       <li> Si se ha seleccionado <b>Todos los grupos</b>, solo están disponibles los estados de todo el sistema
       <li> <p>Si se selecciona un grupo específico, solo están disponibles los estados disponibles para ese grupo</p> </li> 
       </ul> <p>Para obtener información sobre cómo los procesos de aprobación funcionan con los estados, consulte la sección <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Cómo dependen los procesos de aprobación de los estados</a> en el artículo <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Información general del proceso de aprobación</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre de la fase</td> 
      <td>(Opcional) Escriba un nombre que describa el primer paso de la ruta. Si no especifica un nombre de etapa, el nombre predeterminado es <b>Fase 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aprobadores</td> 
      <td> <p>Comience a escribir el nombre del usuario, equipo o función que desea designar como aprobador para esta etapa, luego seleccione el nombre cuando aparezca en la lista. Solo puede añadir usuarios activos, <span>funciones</span> y equipos. </p> 
      <p>Este campo es obligatorio.</p>

   <p><b>Sugerencia</b></p>

   <p>Al añadir un usuario como aprobador, preste atención al avatar, el Rol Principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos una función para verla a medida que los añade.</p>
      <p>Debe tener habilitada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">Conceder acceso a usuarios</a>. </p>

   <p><b>NOTA</b>

   Añadir un usuario, equipo o función como aprobador no les otorga automáticamente permisos para el objeto asociado con esa aprobación. Reciben permisos para el objeto cuando se activa el paso de aprobación. De lo contrario, los objetos deben compartirse con ellos antes de que puedan tomar una decisión de aprobación. </p> <p>También puede designar a una persona como aprobador si especifica su función. Por ejemplo, puede asignar un propietario del proyecto, patrocinador del proyecto, propietario del portafolio, propietario del programa o administrador como aprobador. Estas opciones aparecen automáticamente cuando empieza a escribir.</p>

   <p><b>IMPORTANTE</b>  
       <ul> 
       <li> <p>Cuando asigna una aprobación al patrocinador del proyecto y no se designa a nadie como patrocinador, la aprobación se reasigna al Propietario del Proyecto. Si no se designa a nadie como propietario del proyecto, la aprobación se asigna al administrador de Workfront. </p> </li> 
      </ul> 
       <ul> 
       <li> <p>Cuando se asigne una aprobación a una función y la opción <b>No se requiere que el aprobador esté en el equipo del proyecto (para los procesos de aprobación que incluyan una función)</b> esté deshabilitada, pero no haya funciones en el equipo del proyecto que coincidan con la función en la aprobación, esta última se reasignará al propietario del proyecto. Para obtener información sobre la configuración de aprobaciones, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configuración de la aprobación global</a>.</p> </li> 
       </ul> 
       <ul> 
       <li> <p>Cuando asigna una aprobación al Propietario del Proyecto y no se designa a nadie como propietario de un proyecto, la aprobación se reasigna al administrador principal de Workfront, tal como se indica en la sección de Información del Cliente en el área de Configuración. Para obtener información, consulte <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Configurar información básica para el sistema</a>.  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>Puede repetir este proceso para añadir varios aprobadores a la fase. Una sola fase puede incluir una combinación de usuarios, equipos y funciones como aprobadores. No hay límite en el número de aprobadores que puede añadir a una fase.</p> <p><b>IMPORTANTE</b></p> <p>Cuando asigna funciones laborales como aprobadores, todos los usuarios asociados con esa función que también formen parte del equipo del proyecto pueden tomar una decisión sobre la aprobación. </p> <p>Cuando asigna un equipo como aprobador, cualquier usuario de ese equipo puede tomar una decisión sobre la aprobación. </p> <p>Para obtener más información sobre el equipo del proyecto, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Descripción general del equipo del proyecto</a>. Para obtener más información sobre la aprobación de un trabajo, consulte <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Aprobación del trabajo </a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Solamente se requiere una decisión <br> <br>(solo se mostrará si se añaden varios aprobadores a la fase) </td> 
      <td> <p>Seleccione esta opción si alguno de los aprobadores de la fase puede aprobar o rechazar el elemento de trabajo durante esta fase. Esta acción permite que el elemento de trabajo abandone el escenario. </p> <p>Cuando esta opción no está seleccionada, todos los aprobadores identificados deben aprobar o rechazar la fase (en cualquier orden) antes de que el elemento abandone la fase. Si cualquiera de los aprobadores rechaza la etapa, el proceso se interrumpe y comienza de nuevo para que se puedan realizar los cambios necesarios. A continuación, los aprobadores pueden aprobar o rechazar la fase una vez más.</p> <p>Cuando se designa un equipo como aprobador, cualquier miembro del equipo puede conceder o rechazar una etapa.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Agregar fase</p> </td> 
      <td><p>(Opcional) Añada otra etapa al camino, usando las opciones explicadas en las tres filas anteriores. Puede añadir tantas fases a la ruta como necesite.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decida qué debe suceder cuando se rechace una aprobación</p> </td> 
      <td> <p>Seleccione la acción que desea realizar si el elemento de trabajo se rechaza en cualquier fase de la ruta:</p> 
       <ul> 
       <li><b>Crear un problema</b>: (Disponible solo para procesos de aprobación de proyectos y tareas) Se crea un problema en el proyecto o tarea donde se está ejecutando el proceso de aprobación. El recurso asignado de forma predeterminada en la tarea o el propietario del proyecto se asignan al problema. De manera predeterminada, el nombre del problema creado es <b>Aprobación rechazada (&lt;Nombre de proyecto o tarea&gt;)</b>. Se trata de un problema de rechazo, introducido en la tarea o el proyecto, según el proceso de aprobación en el que se produjo el rechazo.</li> 
       <li> <p><b>Establecer estado en</b>: complete uno de los siguientes pasos:</p> 
       <ul> 
       <li><b>Estado anterior</b>: el proyecto, tarea o problema rechazado vuelve al estado anterior al estado que activa el proceso de aprobación.</li> 
       <li><p><b>Cualquier otro estado de la lista</b>: el objeto rechazado pasa al estado que elija, como En espera. Puede elegir uno de los estados predeterminados o uno personalizado que añadió a su sistema de Workfront.</p>
       <p>Al seleccionar un estado asociado a un proceso de aprobación como estado de rechazo, el objeto rechazado pasará al estado seleccionado y se marcará como “Pendiente de aprobación”. </p> 
       <p> Por ejemplo, al seleccionar En espera para el estado de rechazo y el estado de En espera estuviera asociado a un proceso de aprobación, el objeto rechazado se colocará en el estado “En espera: pendiente de aprobación”, y requerirá la aprobación.</p>

   </tr> 
    </tbody> 
   </table>

1. (Opcional) Haga clic en **Añadir ruta** para añadir otra ruta al proceso de aprobación, haciendo referencia a la lista de opciones del paso anterior.

   La nueva ruta debe estar asociada a otro estado. La ruta se activa cuando el elemento se actualiza para mostrar este estado. No puede tener dos rutas para el mismo estado.

1. Haga clic en **Guardar**.
1. Después de crear el proceso de aprobación, continúe con cualquiera de las siguientes acciones:

   * Asocie el proceso de aprobación con proyectos, tareas o problemas específicos del sistema, tal y como se describe en [Asociar procesos de aprobación nuevos o existentes con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Fuera de Workfront, notifique a los usuarios que el proceso de aprobación está disponible para que lo asocien con sus proyectos, tareas o problemas, como se describe en [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Cree otro proceso de aprobación que se active si este proceso de aprobación se rechaza y el elemento adquiere otro estado. Esto le ofrece una forma de vincular los procesos de aprobación.

Para obtener información sobre cómo editar procesos de aprobación, consulte [Editar procesos de aprobación](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

## Asociación de procesos de aprobación a un elemento de trabajo

Para crear un proceso de aprobación para un elemento de trabajo (proyecto, tarea o problema), es necesario

1. Crear primero el proceso de aprobación
1. Crear el elemento de trabajo
1. Asociar el proceso de aprobación con el elemento de trabajo

Para obtener instrucciones acerca de cómo asociar procesos de aprobación con elementos de trabajo, consulte [Asociar procesos de aprobación nuevos o existentes con trabajos](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>Cualquier usuario de Workfront con permisos de administración de un proyecto, tarea o problema podrá crear procesos de aprobación de un solo uso para usarlos únicamente en el objeto en el que se creen. Para obtener más información, consulte [Asociar procesos de aprobación nuevos o existentes con trabajos](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Permitir que los usuarios modifiquen los procesos de aprobación globales para un solo elemento de trabajo

De forma predeterminada, los usuarios que tengan permisos de administración en proyectos, tareas y problemas podrán crear procesos de aprobación de un solo uso en ellos. Para obtener información acerca de cómo añadir procesos de aprobación de un solo uso a proyectos, tareas y problemas, consulte la sección [Asociar procesos de aprobación de un solo uso a proyectos, tareas, problemas, plantillas o tareas de plantilla](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process) del artículo [Asociar procesos de aprobación nuevos o existentes con trabajos](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

Los usuarios también pueden cambiar la configuración de los procesos de aprobación globales asociados a elementos de trabajo. Estos cambios afectan únicamente al proyecto, tarea o problema asociado con el proceso de aprobación de nivel de sistema. Para obtener más información, vea la sección &quot;Modificar un proceso de aprobación global para utilizarlo en un objeto específico&quot; en el artículo [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
