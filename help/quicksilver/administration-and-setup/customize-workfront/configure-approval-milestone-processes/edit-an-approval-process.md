---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: Editar un proceso de aprobación
description: Si es administrador de Adobe Workfront o tiene acceso administrativo a los procesos de aprobación, puede ver y editar todos los procesos de aprobación del sistema.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: 4440fc50e988da6e446fd9a3195ae94f978b4b74
workflow-type: tm+mt
source-wordcount: '1927'
ht-degree: 6%

---

# Editar un proceso de aprobación

Si es administrador de Adobe Workfront o tiene acceso administrativo a los procesos de aprobación, puede ver y editar todos los procesos de aprobación del sistema.

Si es un administrador de grupos, puede ver y editar los procesos de aprobación asociados al grupo o grupos que administra.

Para obtener información sobre la creación de procesos de aprobación, consulte [Creación de un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>* Cuando edita un proceso de aprobación global que ya está en uso, los cambios afectan a todos los objetos del sistema que ya están asociados a él.
>* Si agrega un aprobador nuevo a la fase actual de un proceso de aprobación que ya se ha iniciado en un objeto, el proceso para ese objeto se restablece y los aprobadores tienen que volver a empezar.
>
>  Sin embargo, si realiza los siguientes cambios en un proceso de aprobación que ya se ha iniciado en un objeto, ese proceso continúa sin interrupción:
>
>* Agregar un escenario más allá del paso actual
>* Agregar un aprobador adicional antes de la fase actual


## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a los procesos de aprobación si no es administrador del sistema</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Editar un proceso de aprobación existente

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).
1. (Condicional) Si está editando un proceso de aprobación a nivel de sistema, haga clic en **Procesos** > **Aprobaciones** en el panel izquierdo.

   O

   Si está editando un proceso de aprobación a nivel de grupo, haga lo siguiente:

   1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).
   1. Haga clic en el nombre del grupo para el que desea enumerar o administrar los procesos de aprobación de grupos.
   1. En el panel izquierdo, haga clic en **Aprobaciones**. Es posible que tenga que hacer clic en **Mostrar más** primero.

1. Haga clic en el **Aprobaciones del proyecto**, **Aprobaciones de tareas** o **Aprobaciones de problemas** , en función del tipo de proceso de aprobación que desee editar.

1. Seleccione el proceso de aprobación que desea editar y, a continuación, haga clic en **Editar** en la parte superior de la lista. Se muestra el cuadro Editar proceso de aprobación .

   ![](assets/edit-approval-process-global-area-new.png)

1. Especifique la siguiente información en el cuadro que aparece:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de proceso de aprobación</td> 
      <td>Escriba un nombre descriptivo para el proceso de aprobación. Los usuarios ven este nombre al aplicar el proceso de aprobación a un objeto, tal como se describe en <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Asociar un proceso de aprobación nuevo o existente al trabajo</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba una descripción del proceso de aprobación. Esto se muestra en la sección <b>Aprobaciones</b> en la sección <b>Configuración</b> junto al nombre del proceso de aprobación.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activo</td> 
      <td> <p>Mantenga esta opción activada si desea que otros usuarios puedan adjuntar el proceso de aprobación a los proyectos, tareas y problemas que creen. </p> <p>Esta opción está activada de forma predeterminada.</p> <p>Sugerencia: Marcar un proceso de aprobación como inactivo resulta útil cuando su organización ya no necesita utilizarlo, pero desea conservar la información histórica sobre su uso.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Este proceso de aprobación lo puede utilizar </td> 
      <td> <p>Si desea que el proceso de aprobación esté disponible para proyectos, tareas, problemas y plantillas que pertenecen solo a un grupo en particular, empiece a escribir el nombre del grupo y, a continuación, seleccione el nombre cuando aparezca:</p> 
       <ul> 
        <li>Si es administrador del sistema o tiene acceso administrativo a los procesos de aprobación, puede ver cualquier grupo del sistema cuando escriba su nombre. <b>Todos los grupos</b> está seleccionado de forma predeterminada. </li> 
        <li>Si es un administrador de grupo sin acceso administrativo a los procesos de aprobación, puede asignar el proceso de aprobación a cualquier grupo que administre al escribir su nombre. La variable <b>Todos los grupos</b> no está disponible.</li> 
       </ul> <p>Esta opción no está disponible para procesos de aprobación de un solo uso.</p> <p><b>ADVERTENCIA</b>: Cuando se realizan cambios en el proceso de aprobación específico del grupo, es posible que cambien los procesos de aprobación existentes que ya se han asociado con elementos de trabajo. Para obtener información sobre estos cambios, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Efecto de los cambios en el grupo y el proceso de aprobación en los procesos de aprobación asignados</a>.</p> <p>Para obtener información sobre cómo enumerar y administrar los procesos de aprobación de su grupo desde la página de su grupo, consulte <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Procesos de aprobación a nivel de grupo</a>. </p> <p>Para obtener información sobre el acceso administrativo a los procesos de aprobación, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Configure una ruta para el proceso de aprobación mediante las siguientes opciones.

   En una ruta se especifica lo que debe suceder en el proceso de aprobación. Puede crear escenarios en una ruta para indicar quién debe realizar el trabajo de aprobación y en qué orden.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Iniciar el proceso de aprobación cuando el estado esté definido como</p> </td> 
      <td> <p>Seleccione el estado que almacenará en déclencheur el proceso de aprobación en los elementos de trabajo. Cuando alguien actualiza un elemento de trabajo a este estado, comienza su proceso de aprobación. </p> <p>No se puede seleccionar el mismo estado para varias rutas de proceso de aprobación.</p> <p>Los estados disponibles se basan en lo que se selecciona en la opción <b>Esta aprobación puede ser utilizada por</b> (explicado en el cuadro anterior):</p> 
      <ul> 
      <li> If <b>Todos los grupos</b> está seleccionada, solo están disponibles los estados bloqueados de todo el sistema. <!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>Si se selecciona un grupo específico, solo están disponibles los estados disponibles para ese grupo</p> </li> 
      </ul> <p>Para obtener información sobre cómo funciona el proceso de aprobación con los estados, consulte la sección <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Cómo dependen los procesos de aprobación de los estados</a> en el artículo <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Información general del proceso de aprobación</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre de la fase</td> 
      <td>(Opcional) Escriba un nombre que describa el primer paso de la ruta. Si no especifica un nombre de escenario, el nombre predeterminado es <b>Etapa 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aprobadores</td> 
      <td> <p>Empiece a escribir el nombre del usuario, equipo o función de trabajo que desea designar como aprobador para esta etapa y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable. Solo puede agregar usuarios activos, funciones de trabajo y equipos. </p>

   <p><b>SUGERENCIA</b>:</p>

   <p>Al agregar un usuario como aprobador, observe el avatar, la función principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos una función de trabajo para verla a medida que los agrega.</p>

   <p><b>NOTA</b>:

   Al agregar un usuario, equipo o función como aprobador, no se les conceden automáticamente permisos para el objeto asociado con esa aprobación. Reciben permisos para el objeto cuando se activa el paso de aprobación. De lo contrario, los objetos deben compartirse con ellos para poder tomar una decisión de aprobación. </p>
   <p>También puede designar a un individuo como aprobador especificando la función del individuo. Por ejemplo, puede asignar como aprobador un propietario del proyecto, un patrocinador del proyecto, un propietario del Portfolio, un propietario del programa o un administrador. Estas opciones aparecen automáticamente cuando empieza a escribir.</p> 
      <p><b>IMPORTANTE</b>:  
      <ul> 
      <li> Cuando se asigna una aprobación al Patrocinador del proyecto y no se designa a nadie como patrocinador de un proyecto, la aprobación se reasigna al Propietario del proyecto. Si no se designa a nadie como propietario del proyecto, la aprobación se asigna al administrador de Workfront. </li> 
      <li> Al asignar una aprobación a una función y la opción <b>No es necesario que el aprobador esté en el equipo del proyecto</b> está desactivado, pero ninguna función del equipo del proyecto coincide con la función de la aprobación, la aprobación se reasigna al propietario del proyecto. Para obtener información sobre la configuración de aprobación, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configuración de la aprobación global</a>.
      </li> 
      <li>Cuando se asigna una aprobación al propietario del proyecto y no se designa a nadie como propietario de un proyecto, la aprobación se reasigna al administrador principal de Workfront, tal como se indica en la sección Información del cliente del área Configuración . Para obtener más información, consulte <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Configurar información básica para el sistema</a>.</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>Cuando asigna funciones de trabajo como aprobadores, todos los usuarios asociados a esa función de trabajo que también están en el equipo del proyecto pueden tomar una decisión sobre la aprobación. </p> 
      <p>Cuando asigna un equipo como aprobador, cualquier usuario de dicho equipo puede tomar una decisión sobre la aprobación. </p> 
      <p>Para obtener más información sobre el equipo del proyecto, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Información general del equipo del proyecto</a>. Para obtener más información sobre la aprobación del trabajo, consulte <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Aprobación del trabajo </a>.</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">Solamente se requiere una decisión</td> 
      <td>(Solo se muestra si se agregan varios aprobadores a la etapa) Seleccione esta opción si alguno de los aprobadores de la etapa puede aprobar o rechazar el elemento de trabajo durante esta fase. Esta acción permite que el elemento de trabajo salga del escenario.  
      <p>Cuando no se selecciona esta opción, todos los aprobadores identificados deben aprobar o rechazar la fase (en cualquier orden) antes de que el elemento salga de la fase. Si alguno de los aprobadores rechaza la etapa, el proceso se interrumpe y se reinicia para que se puedan realizar los cambios necesarios. A continuación, los aprobadores pueden aprobar o rechazar de nuevo la fase.</p> 
      <p>Cuando se designa a un equipo como aprobador, cualquier miembro del equipo puede conceder o rechazar una etapa.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Agregar fase</p> </td> 
      <td>(Opcional) Añada otro escenario a la ruta, utilizando las opciones explicadas en las tres filas anteriores. Puede agregar tantas etapas a la ruta como necesite.</td> 
     </tr>
     <tr> 
      <td role="rowheader"> Decida que debe suceder cuando se rechace una aprobación</td> 
      <td> <p>Seleccione la acción que desee realizar si el elemento de trabajo se rechaza en cualquier etapa de la ruta:</p> 
      <ul> <li><strong>Crear un problema</strong>: (Disponible solo para procesos de aprobación de proyectos y tareas) Se crea un problema en el proyecto o la tarea en el que se está ejecutando el proceso de aprobación. Se asigna al problema el recurso asignado predeterminado de la tarea o el propietario del proyecto. De forma predeterminada, el nombre del problema creado es <strong>Aprobación rechazada (nombre de proyecto o tarea)</strong>. Se trata de un problema de rechazo, introducido en la tarea o en el proyecto, según el proceso de aprobación en el que se haya producido el rechazo.</li> 
      <li> <p><strong>Definir estado como</strong>: Elija una de las siguientes opciones:</p> 
      <ul> <li><strong>Estado anterior</strong>: El proyecto, tarea o problema rechazado vuelve al estado anterior al estado que activa el proceso de aprobación.</li> 
      <li> <p><strong>Cualquier otro estado de la lista</strong>: El objeto rechazado se mueve al estado que elija, como En espera. Puede elegir uno de los estados predeterminados o uno personalizado que agregó al sistema de Workfront.</p> <p>Si selecciona un estado asociado a un proceso de aprobación como estado de rechazo de una ruta de aprobación, el objeto rechazado pasa al estado seleccionado y se marcará como “Pendiente de aprobación”. </p>
      <p>Por ejemplo, si selecciona En espera para el estado de rechazo y el estado de En espera está asociado a un proceso de aprobación, el objeto rechazado se coloca en el estado de “En espera: pendiente de aprobación”, que requiere la aprobación.</p>    <p>Para un proceso de aprobación en todo el sistema, solo están disponibles los estados en todo el sistema.</p> <p>Para un proceso de aprobación específico del grupo, están disponibles todos los estados del grupo. Esto incluye cualquier estado personalizado que el administrador del grupo haya creado específicamente para el grupo, así como cualquier estado de todo el sistema. </p> <p>Para obtener información sobre cómo funciona el proceso de aprobación con los estados, consulte la sección <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Cómo dependen los procesos de aprobación de los estados</a> en el artículo <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Información general del proceso de aprobación</a>.</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Haga clic en **Agregar ruta** para añadir otra ruta al proceso de aprobación, consulte la lista de opciones del paso anterior.

   La nueva ruta debe asociarse con otro estado. La ruta de acceso déclencheur cuando se actualiza el elemento para mostrar este estado. No puede tener dos rutas para el mismo estado.

1. Haga clic en **Guardar**.
1. (Opcional) Realice cualquiera de las siguientes acciones:

   * Asocie el proceso de aprobación con proyectos, tareas o problemas específicos de todo el sistema, tal como se describe en [Asociar un proceso de aprobación nuevo o existente al trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Fuera de Workfront, notifique a los usuarios de que el proceso de aprobación está disponible para que se asocien con sus proyectos, tareas o problemas, tal como se describe en [Asociar un proceso de aprobación nuevo o existente al trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Cree otro proceso de aprobación que se active si se rechaza este proceso de aprobación y el elemento toma otro estado. Esto le ofrece una forma de vincular procesos de aprobación.
