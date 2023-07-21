---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: Edición de un proceso de aprobación
description: Si es administrador de Adobe Workfront o tiene acceso administrativo a los procesos de aprobación, puede ver y editar todos los procesos de aprobación en el sistema.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '1953'
ht-degree: 5%

---

# Edición de un proceso de aprobación

Si es administrador de Adobe Workfront o tiene acceso administrativo a los procesos de aprobación, puede ver y editar todos los procesos de aprobación en el sistema.

Si es administrador de un grupo, puede ver y editar los procesos de aprobación asociados con el grupo o grupos que administra.

Para obtener información sobre la creación de procesos de aprobación, consulte [Crear un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>* Cuando edita un proceso de aprobación global que ya está en uso, los cambios afectan a todos los objetos del sistema que ya están asociados a él.
>* Si añade un nuevo aprobador a la fase actual en un proceso de aprobación que ya se ha iniciado en un objeto, el proceso para ese objeto se restablece y los aprobadores tienen que volver a empezar.
>
>  Sin embargo, si realiza los siguientes cambios en un proceso de aprobación que ya se ha iniciado en un objeto, ese proceso continúa sin interrupción:
>
>* Agregar una etapa más allá de la etapa actual
>* Agregar un aprobador adicional antes de la fase actual

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a los procesos de aprobación si no es administrador del sistema</p> <p><b>NOTA</b>: si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Editar un proceso de aprobación existente

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).
1. (Condicional) Si está editando un proceso de aprobación de nivel de sistema, haga clic en **Procesos** > **Aprobaciones** en el panel izquierdo.

   O

   Si está editando un proceso de aprobación de nivel de grupo, haga lo siguiente:

   1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).
   1. Haga clic en el nombre del grupo para el que desea enumerar o administrar los procesos de aprobación del grupo.
   1. En el panel izquierdo, haga clic en **Aprobaciones**. Es posible que tenga que hacer clic en **Mostrar más** primero.

1. Haga clic en **Aprobaciones de proyecto**, **Aprobaciones de tarea**, o **Aprobaciones de problema** , según el tipo de proceso de aprobación que desee editar.

1. Seleccione el proceso de aprobación que desee editar y haga clic en **Editar** al principio de la lista. Aparece el cuadro Editar proceso de aprobación.

   ![](assets/edit-approval-process-global-area-new.png)

1. Especifique la siguiente información en el cuadro que se muestra:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de proceso de aprobación</td> 
      <td>Escriba un nombre descriptivo para el proceso de aprobación. Los usuarios ven este nombre al aplicar el proceso de aprobación a un objeto, como se describe en <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Asociar un proceso de aprobación nuevo o existente con el trabajo</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba una descripción del proceso de aprobación. Esto se muestra en la <b>Aprobaciones</b> de la sección <b>Configurar</b> junto al nombre del proceso de aprobación.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activo</td> 
      <td> <p>Mantenga esta opción habilitada si desea que otros usuarios puedan adjuntar el proceso de aprobación a los proyectos, tareas y problemas que creen. </p> <p>Esta opción está habilitada de forma predeterminada.</p> <p>Sugerencia: Marcar un proceso de aprobación como inactivo resulta útil cuando su organización ya no necesita utilizarlo, pero desea conservar la información histórica sobre su uso.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Este proceso de aprobación lo puede utilizar </td> 
      <td> <p>Si desea que el proceso de aprobación esté disponible para proyectos, tareas, problemas y plantillas que solo pertenezcan a un grupo en particular, empiece a escribir el nombre del grupo y, a continuación, seleccione el nombre cuando aparezca:</p> 
       <ul> 
        <li>Si es administrador del sistema o tiene acceso administrativo a los procesos de aprobación, puede ver cualquier grupo del sistema cuando escriba su nombre. <b>Todos los grupos</b> está seleccionado de forma predeterminada. </li> 
        <li>Si es administrador de un grupo sin acceso administrativo a los procesos de aprobación, puede asignar el proceso de aprobación a cualquier grupo que administre al escribir su nombre. El <b>Todos los grupos</b> La opción no está disponible.</li> 
       </ul> <p>Esta opción no está disponible para procesos de aprobación de un solo uso.</p> <p><b>ADVERTENCIA</b>: Cuando realiza cambios en el proceso de aprobación específico del grupo, los procesos de aprobación existentes que ya se han asociado con elementos de trabajo pueden cambiar. Para obtener más información sobre estos cambios, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Cómo afectan los cambios en los procesos de aprobación y de grupo a los procesos de aprobación asignados</a>.</p> <p>Para obtener información sobre cómo enumerar y administrar los procesos de aprobación de su grupo desde la página de su grupo, consulte <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Procesos de aprobación de nivel de grupo</a>. </p> <p>Para obtener información sobre el acceso administrativo a los procesos de aprobación, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
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
      <td> <p>Seleccione el estado que almacenará en déclencheur el proceso de aprobación en los elementos de trabajo. Cuando alguien actualiza un elemento de trabajo a este estado, comienza su proceso de aprobación. </p> <p>No se puede seleccionar el mismo estado para varias rutas de proceso de aprobación.</p> <p>Los estados disponibles se basan en lo que se selecciona en la opción <b>Esta aprobación puede ser utilizada por</b> (explicado en la tabla anterior):</p> 
      <ul> 
      <li> If <b>Todos los grupos</b> está seleccionada, solo están disponibles los estados bloqueados de todo el sistema. <!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>Si se selecciona un grupo específico, solo están disponibles los estados disponibles para ese grupo</p> </li> 
      </ul> <p>Para obtener información sobre cómo funciona el proceso de aprobación con los estados, consulte la sección <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Cómo dependen los procesos de aprobación de los estados</a> en el artículo <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Resumen del proceso de aprobación</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre de la fase</td> 
      <td>(Opcional) Escriba un nombre que describa el primer paso de la ruta. Si no especifica un nombre de etapa, el nombre predeterminado es <b>Fase 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aprobadores</td> 
      <td> <p>Empiece escribiendo el nombre del usuario, equipo o función del trabajo que desea designar como aprobador para esta fase y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable. Solo puede agregar usuarios activos, roles y equipos. </p>

   <p><b>SUGERENCIA</b>:</p>

   <p>Cuando agregue un usuario como aprobador, observe el avatar, la función principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos un rol para verlo a medida que los agregue.</p>
      <p>Debe tener activada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">Concesión de acceso a los usuarios</a></p>.

   <p><b>NOTA</b>:

   Añadir un usuario, equipo o función como aprobador no les otorga automáticamente permisos para el objeto asociado con esa aprobación. Reciben permisos para el objeto cuando se activa el paso de aprobación. De lo contrario, los objetos deben compartirse con ellos antes de que puedan tomar una decisión de aprobación. </p>
   <p>También puede designar a una persona como aprobador si especifica su función. Por ejemplo, puede asignar un Propietario del proyecto, Patrocinador del proyecto, Propietario del Portfolio, Propietario del programa o Administrador como aprobador. Estas opciones aparecen automáticamente cuando empieza a escribir.</p> 
      <p><b>IMPORTANTE</b>:  
      <ul> 
      <li> Cuando asigna una aprobación al patrocinador del proyecto y no se designa a nadie como patrocinador, la aprobación se reasigna al propietario del proyecto. Si no se designa a nadie como propietario del proyecto, la aprobación se asigna al administrador de Workfront. </li> 
      <li> Al asignar una aprobación a un rol y la opción <b>No se requiere que el aprobador esté en el equipo del proyecto</b> está deshabilitada, pero ningún rol del equipo del proyecto coincide con el rol de la aprobación, la aprobación se reasigna al propietario del proyecto. Para obtener información sobre la configuración de aprobación, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configuración de la aprobación global</a>.
      </li> 
      <li>Cuando asigna una aprobación al Propietario del proyecto y no se designa a nadie como propietario de un proyecto, la aprobación se reasigna al administrador principal de Workfront, tal como se indica en la sección Información del cliente del área de Configuración. Para obtener más información, consulte <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Configurar la información básica del sistema</a>.</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>Cuando asigna roles como aprobadores, todos los usuarios asociados a ese rol que también están en el equipo del proyecto pueden tomar una decisión sobre la aprobación. </p> 
      <p>Cuando asigna un equipo como aprobador, cualquier usuario de ese equipo puede tomar una decisión sobre la aprobación. </p> 
      <p>Para obtener más información sobre el equipo del proyecto, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Información general del equipo del proyecto</a>. Para obtener más información sobre la aprobación de trabajo, consulte <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Aprobación del trabajo </a>.</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">Solamente se requiere una decisión</td> 
      <td>(Solo se muestra si agrega varios aprobadores a la fase) Seleccione esta opción si alguno de los aprobadores de la fase puede aprobar o rechazar el elemento de trabajo durante esta fase. Esta acción permite que el elemento de trabajo abandone el escenario.  
      <p>Cuando esta opción no está seleccionada, todos los aprobadores identificados deben aprobar o rechazar la fase (en cualquier orden) antes de que el elemento abandone la fase. Si alguno de los aprobadores rechaza la fase, el proceso se interrumpe y se inicia de nuevo para que se puedan realizar los cambios necesarios. A continuación, los aprobadores pueden aprobar o rechazar la fase una vez más.</p> 
      <p>Cuando se designa un equipo como aprobador, cualquier miembro del equipo puede conceder o rechazar una etapa.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Agregar fase</p> </td> 
      <td>(Opcional) Añada otra etapa a la ruta, utilizando las opciones explicadas en las tres filas anteriores. Puede agregar tantas fases a la ruta como necesite.</td> 
     </tr>
     <tr> 
      <td role="rowheader"> Decida que debe suceder cuando se rechace una aprobación</td> 
      <td> <p>Seleccione la acción que desea realizar si el elemento de trabajo se rechaza en cualquier fase de la ruta:</p> 
      <ul> <li><strong>Crear una incidencia</strong>: (disponible solo para procesos de aprobación de proyectos y tareas) Se crea un problema en el proyecto o la tarea en los que se está ejecutando el proceso de aprobación. El recurso asignado de forma predeterminada en la tarea o el propietario del proyecto se asignan al problema. De forma predeterminada, el nombre del problema creado es <strong>Aprobación rechazada (nombre del proyecto o de la tarea)</strong>. Se trata de un problema de rechazo, introducido en la tarea o el proyecto, según el proceso de aprobación en el que se produjo el rechazo.</li> 
      <li> <p><strong>Definir estado como</strong>: elija una de las siguientes opciones:</p> 
      <ul> <li><strong>Estado anterior</strong>: el proyecto, tarea o problema rechazado vuelve al estado anterior al estado que activa el proceso de aprobación.</li> 
      <li> <p><strong>Cualquier otro estado de la lista</strong>: el objeto rechazado pasa al estado que elija, como En espera. Puede elegir uno de los estados predeterminados o uno personalizado que agregó a su sistema de Workfront.</p> <p>Si selecciona un estado asociado a un proceso de aprobación como estado de rechazo de una ruta de aprobación, el objeto rechazado pasa al estado seleccionado y se marcará como “Pendiente de aprobación”. </p>
      <p>Por ejemplo, si selecciona En espera para el estado de rechazo y el estado de En espera está asociado a un proceso de aprobación, el objeto rechazado se coloca en el estado de “En espera: pendiente de aprobación”, que requiere la aprobación.</p>    <p>Para un proceso de aprobación de todo el sistema, solo están disponibles los estados de todo el sistema.</p> <p>Para un proceso de aprobación específico de un grupo, todos los estados de grupo están disponibles. Esto incluye cualquier estado personalizado que el administrador del grupo haya creado específicamente para el grupo, así como cualquier estado del sistema. </p> <p>Para obtener información sobre cómo funciona el proceso de aprobación con los estados, consulte la sección <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Cómo dependen los procesos de aprobación de los estados</a> en el artículo <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Resumen del proceso de aprobación</a>.</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Haga clic en **Añadir ruta** para añadir otra ruta al proceso de aprobación, consulte la lista de opciones en el paso anterior.

   La nueva ruta debe estar asociada a otro estado. La ruta entra en déclencheur cuando el elemento se actualiza para mostrar este estado. No puede tener dos rutas para el mismo estado.

1. Haga clic en **Guardar**.
1. (Opcional) Realice una de las siguientes acciones:

   * Asocie el proceso de aprobación con proyectos, tareas o problemas específicos de su sistema, tal como se describe en [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Fuera de Workfront, notifique a los usuarios que el proceso de aprobación está disponible para que se asocien a sus proyectos, tareas o problemas, tal como se describe en [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Cree otro proceso de aprobación que se active si este proceso de aprobación se rechaza y el elemento adquiere otro estado. Esto le ofrece una forma de vincular los procesos de aprobación.
