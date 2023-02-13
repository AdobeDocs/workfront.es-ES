---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Estados de proyecto del sistema
description: Workfront tiene 9 estados de proyecto integrados del sistema. Los 3 primeros de la tabla siguiente son obligatorios, lo que significa que puede desbloquearlos, cambiarles el nombre y reordenarlos, pero no puede ocultarlos ni eliminarlos. El cambio de estado de un proyecto suele ser un proceso manual. Sin embargo, a veces el estado de un proyecto cambia automáticamente, dependiendo de otros factores que estén ocurriendo en el sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---

# Estados de proyecto del sistema

Workfront tiene 9 estados de proyecto integrados del sistema.

Los 3 primeros de la tabla siguiente son obligatorios, lo que significa que puede desbloquearlos, cambiarles el nombre y reordenarlos, pero no puede ocultarlos ni eliminarlos.

El cambio de estado de un proyecto suele ser un proceso manual. Sin embargo, hay algunos escenarios descritos en la siguiente lista cuando el estado de un proyecto cambia automáticamente, dependiendo de otros factores que estén ocurriendo en el sistema.

Con la instancia de Workfront se proporcionan los siguientes estados de proyecto:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th>Estado del proyecto del sistema</th> 
   <th>Este estado de proyecto se produce cuando</th> 
   <th>Qué sucede en este estado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificación (estado requerido)</td> 
   <td> <p>El director del proyecto está planificando la cronología del proyecto, la asignación de las tareas y las aprobaciones. El administrador de proyectos establece este estado manualmente en un proyecto.</p> <p>Sugerencia: Se recomienda establecer el estado predeterminado de los nuevos proyectos en Workfront en Planning. Como administrador de Workfront, puede cambiar el estado predeterminado de todos los proyectos nuevos en el área Proyectos de Preferencias de proyecto.</p> </td> 
   <td> <p>Los usuarios del equipo del proyecto pueden ver el proyecto en sus listas Proyectos de forma predeterminada, en el área Proyectos de Workfront. Las tareas y los problemas que se les asignan en el proyecto no rellenan su lista de trabajo. En la lista de trabajo principal solo se muestran las aprobaciones y los elementos de trabajo aceptados.</p> <p>No se envían notificaciones mientras un proyecto tiene este estado.</p> <p>Se recomienda que todos los cambios que puedan almacenar en déclencheur una actualización de la cronología del proyecto, o cualquier cambio en las tareas y asignaciones de problemas, se realicen mientras el proyecto esté en estado de Planning. Esto minimiza la cantidad de notificaciones que reciben los usuarios.</p> <p>El sistema no calcula automáticamente la cronología del proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>Actual (estado requerido)</td> 
   <td> <p>Los usuarios están trabajando en ello. El administrador de proyectos debe convertir un proyecto a Actual para indicar que se ha iniciado.</p> <p>Este es el estado predeterminado de los nuevos proyectos en Workfront.</p> <p>Sugerencia: Como administrador de Workfront, puede cambiar el estado predeterminado de los nuevos proyectos en el área Proyectos de Preferencias de proyecto. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </td> 
   <td> <p>Los usuarios del equipo del proyecto pueden ver el proyecto en sus listas Proyectos de forma predeterminada, en el área Proyectos de Workfront. Las tareas y los problemas que se les asignan en el proyecto rellenan su lista de trabajo. Pueden empezar a aceptar trabajos sobre tareas y problemas y moverlos a su lista de trabajo en.</p> <p>Además, en un proyecto actual, todas las notificaciones sobre cambios en la cronología, asignaciones, acciones necesarias y aprobaciones se envían a los usuarios del equipo del proyecto.</p> <p>El sistema calcula automáticamente la cronología del proyecto si el tipo de actualización del proyecto está establecido en Automático, En Cambio o Automático y En Cambio.</p> <p>Sugerencia: Es aconsejable reducir al mínimo los ajustes del plan del proyecto cuando un proyecto esté en este estado, de modo que los usuarios no reciban demasiadas notificaciones.</p> </td> 
  </tr> 
  <tr> 
   <td>Completar (estado requerido)</td> 
   <td> <p> El proyecto se ha completado:</p> 
    <ul> 
     <li> <p>Si el modo de finalización del proyecto está establecido en Manual, el administrador del proyecto elige este estado manualmente para informar a los usuarios del equipo del proyecto de que dejen de trabajar en el proyecto.</p> </li> 
    </ul> 
    <ul> 
     <li>Si el modo de finalización del proyecto está establecido en Automático, Workfront marca automáticamente un proyecto como Completado cuando todas las tareas y problemas del proyecto están marcados como Completado. </li> 
    </ul> <p><b>IMPORTANTE</b>: Puede marcar un proyecto como Completo solo cuando se hayan resuelto todas las tareas, problemas y aprobaciones del proyecto.</p> </td> 
   <td>
    <ul>
     <li>Los usuarios del equipo del proyecto no pueden ver el proyecto en sus listas Proyectos de forma predeterminada, en el área Proyectos de Workfront. Las tareas y los problemas que se les asignan en el proyecto no rellenan sus solicitudes de trabajo ni las listas Trabajo en.</li>
     <li>Todas las notificaciones relacionadas con el proyecto, excepto una notificación de cambio de estado, dejan de enviarse a los usuarios del equipo del proyecto. </li>
     <li>El sistema ya no calcula la cronología del proyecto.</li>
     <li>El proyecto no se puede copiar.</li>
    </ul><p>Puede evitar que los usuarios realicen acciones adicionales cuando un proyecto esté marcado como Completado. </p><p>Para obtener más información sobre cómo restringir acciones en proyectos marcados como Completos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Inactivo</td> 
   <td>El proyecto aún no ha finalizado, pero debido a bloqueos de carreteras o cambios en el alcance, el proyecto no puede seguir trabajando y ha sido abandonado. El administrador de proyectos cambia el estado a Dead para alertar a los usuarios del equipo de proyectos de que este proyecto nunca finalizará y que ya no deberían estar trabajando en él.</td> 
   <td> <p>Los usuarios del equipo del proyecto no pueden ver el proyecto en sus listas Proyectos de forma predeterminada, en el área Proyectos de Workfront. Las tareas y los problemas que se les asignan en el proyecto desaparecen de su lista de trabajo.</p> <p>Las decisiones de aprobación no se pueden conceder a tareas o problemas.</p> <p>Las notificaciones sobre cambios en la cronología, asignaciones, acciones necesarias y aprobaciones no se envían a los usuarios del equipo del proyecto.</p> <p>El sistema no calcula automáticamente la duración del proyecto, ya que se considera que se ha completado.</p> <p>Puede impedir que los usuarios realicen ciertas acciones cuando un proyecto esté marcado como Muerto. Para obtener más información sobre cómo restringir acciones en proyectos muertos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>En espera</td> 
   <td>El proyecto aún no ha finalizado, pero debido a algunos retrasos, el proyecto debe suspenderse temporalmente. El administrador de proyectos decide utilizar este estado para avisar a los usuarios del equipo de proyectos de que dejen de trabajar en el proyecto en el momento actual.</td> 
   <td> <p>Los usuarios del equipo del proyecto no pueden ver el proyecto en sus listas Proyectos de forma predeterminada, en el área Proyectos de Workfront. Las tareas y los problemas que se les asignan en el proyecto desaparecen de su lista de trabajo. </p> <p>Las decisiones de aprobación no se pueden conceder a tareas o problemas.</p> <p>Las notificaciones sobre cambios en la cronología, asignaciones, acciones necesarias y aprobaciones no se envían a los usuarios del equipo del proyecto.</p> <p> <p><b>NOTA</b>: Cuando se coloca un proyecto en espera, la cronología del proyecto no se detiene. El proyecto aún puede mostrarse como En riesgo o En problemas aunque nadie esté trabajando activamente en el proyecto. Es posible que se necesiten algunos ajustes manuales de las fechas de las tareas abiertas restantes al volver a poner el proyecto en Actual para que el proyecto pueda mostrar el progreso actualizado.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>Solicitado</td> 
   <td>El estado del proyecto se marca automáticamente como Solicitado por el sistema, cuando se ha completado el estudio de viabilidad de una solicitud de proyecto y se ha presentado para su aprobación. Para obtener más información sobre la solicitud de un proyecto mediante un caso práctico, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar proyectos solicitados</a>.</td> 
   <td> <p>Los usuarios del equipo del proyecto no pueden ver el proyecto en sus listas Proyectos de forma predeterminada, en el área Proyectos de Workfront. Las tareas y los problemas del proyecto que se les asignan no rellenan su lista de trabajo.</p> <p>Todas las notificaciones relacionadas con el proyecto, excepto una notificación de cambio de estado, no se envían a ningún usuario.</p> <p>El sistema no calcula automáticamente la cronología del proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>Aprobado</td> 
   <td>El estado del proyecto se marca automáticamente como Aprobado cuando se aprueba el caso empresarial de una solicitud de proyecto. Para obtener más información sobre la solicitud de un proyecto mediante un caso práctico, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar proyectos solicitados</a>.</td> 
   <td> <p>Los usuarios del equipo del proyecto pueden ver el proyecto en sus listas Proyectos de forma predeterminada, en el área Proyectos de Workfront. Las tareas y los problemas que se les asignan en el proyecto no rellenan su lista de trabajo.</p> <p>Todas las notificaciones relacionadas con el proyecto, excepto una notificación de cambio de estado, no se envían a ningún usuario.</p> <p>El sistema no calcula automáticamente la cronología del proyecto. </p> </td> 
  </tr> 
  <tr> 
   <td>Rechazado</td> 
   <td>El estado del proyecto se marca automáticamente como Rechazado cuando se rechaza el caso empresarial de una solicitud de proyecto. Para obtener más información sobre la solicitud de un proyecto mediante un caso práctico, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar proyectos solicitados</a>.</td> 
   <td> <p>Los usuarios del equipo del proyecto no pueden ver el proyecto en sus listas Proyectos de forma predeterminada, en el área Proyectos de Workfront. Las tareas y los problemas que se les asignan en el proyecto no rellenan su lista de trabajo.</p> <p>Todas las notificaciones relacionadas con el proyecto, excepto una notificación de cambio de estado, no se envían a ningún usuario.</p> <p>El sistema no calcula automáticamente la cronología del proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>Idea</td> 
   <td>El estado del proyecto se marca automáticamente como Idea cuando se envía una solicitud de proyecto. Para obtener más información sobre la solicitud de un proyecto mediante un caso práctico, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar proyectos solicitados</a>.</td> 
   <td> <p>Los usuarios del equipo del proyecto no pueden ver el proyecto en sus listas Proyectos de forma predeterminada, en el área Proyectos de Workfront. Las tareas y los problemas que se les asignan en el proyecto no rellenan su lista de trabajo.</p> <p>Todas las notificaciones relacionadas con el proyecto, excepto una notificación de cambio de estado, no se envían a ningún usuario.</p> <p>El sistema no calcula automáticamente la cronología del proyecto.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Los siguientes estados de proyecto no se pueden cambiar a estado muerto, en espera o completo:
>
>* Solicitado
>* Idea
>* Aprobado
>* Rechazado (o su equivalente)
>

