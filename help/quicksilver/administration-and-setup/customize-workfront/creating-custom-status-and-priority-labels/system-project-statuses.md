---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Estados del proyecto del sistema
description: Workfront tiene 9 estados de proyecto del sistema integrados. Los 3 primeros elementos de la tabla siguiente son obligatorios, lo que significa que puede desbloquearlos, cambiarles el nombre y reordenarlos, pero no puede ocultarlos ni eliminarlos. Cambiar el estado de un proyecto suele ser un proceso manual. Sin embargo, a veces el estado de un proyecto cambia automáticamente en función de otros factores que están ocurriendo en el sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: f4ef463ebdc9a4a7a0802e5394d7820ebc447aa9
workflow-type: tm+mt
source-wordcount: '1572'
ht-degree: 0%

---

# Estados del proyecto del sistema

Workfront tiene 9 estados de proyecto del sistema integrados.

Los 3 primeros elementos de la tabla siguiente son obligatorios, lo que significa que puede desbloquearlos, cambiarles el nombre y reordenarlos, pero no puede ocultarlos ni eliminarlos.

Cambiar el estado de un proyecto suele ser un proceso manual. Sin embargo, en la siguiente lista se describen algunos escenarios en los que el estado de un proyecto cambia automáticamente según otros factores que estén ocurriendo en el sistema.

La instancia de Workfront proporciona los siguientes estados de proyecto:

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
   <th>Este estado del proyecto se produce cuando</th> 
   <th>Qué sucede en este estado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificación (estado requerido)</td> 
   <td> <p>El administrador del proyecto está planificando la cronología del proyecto, la asignación de las tareas y las aprobaciones. El jefe de proyecto establece manualmente este estado en un proyecto.</p> <p><b>SUGERENCIA</p> <p> Le recomendamos que establezca el estado predeterminado de los nuevos proyectos en Workfront en Planning. Como administrador de Workfront, puede cambiar el estado predeterminado de todos sus nuevos proyectos en el área de Proyectos de Preferencias de proyecto.</p> </td> 
   <td> <p>Los usuarios del equipo del proyecto pueden ver el proyecto en sus listas de proyectos de forma predeterminada (sin un filtro personalizado), en el área de Proyectos de Workfront. Las tareas y los problemas asignados a ellos en el proyecto no rellenan su Lista de trabajos. En la Lista de trabajoss en Inicio solo se muestran las aprobaciones y los elementos de trabajo aceptados.</p> <p>No se envían notificaciones mientras un proyecto tenga este estado.</p> <p>Recomendamos que todos los cambios que puedan almacenar en déclencheur una actualización de la escala de tiempo del proyecto, o cualquier cambio en las tareas y asignaciones de problemas, se realicen mientras el proyecto se encuentra en estado de Planificación. Esto minimiza la cantidad de notificaciones que reciben los usuarios.</p> <p>El sistema no calcula automáticamente la cronología del proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>Actual (estado obligatorio)</td> 
   <td> <p>Los usuarios están trabajando en ello. El jefe de proyecto debe convertir un proyecto a Actual para indicar que se ha iniciado.</p> <p>Este es el estado predeterminado de los nuevos proyectos en Workfront.</p> <p><b>SUGERENCIA</b></p>

<p> Como administrador de Workfront, puede cambiar el estado predeterminado de los nuevos proyectos en el área Proyectos de Preferencias de proyecto. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </td> 
   <td> <p>Los usuarios del equipo del proyecto pueden ver el proyecto en sus listas de proyectos de forma predeterminada (sin un filtro personalizado), en el área de Proyectos de Workfront. Las tareas y problemas asignados a ellos en el proyecto rellenan su Lista de trabajos. Pueden empezar a aceptar trabajo en tareas y problemas y moverlos a la lista Trabajando en.</p> <p>Además, en un proyecto actual, todas las notificaciones sobre cambios de escala de tiempo, asignaciones, acciones necesarias y aprobaciones se envían a los usuarios del equipo del proyecto.</p> <p>Y el sistema calcula automáticamente la cronología del proyecto si el tipo de actualización del proyecto está establecido en Automático, Al cambiar o Automático y al cambiar.</p> <p>Sugerencia: Es aconsejable reducir al mínimo los ajustes del plan del proyecto cuando un proyecto se encuentra en este estado para que los usuarios no reciban demasiadas notificaciones.</p> </td> 
  </tr> 
  <tr> 
   <td>Completado (estado obligatorio)</td> 
   <td> <p> El proyecto se ha completado:</p> 
     <p>Si el modo de finalización del proyecto se establece en Manual, el administrador del proyecto elige este estado manualmente para informar a los usuarios del equipo del proyecto de que dejen de trabajar en el proyecto.</p> 
    <p>Si el modo de finalización del proyecto se establece en automático, Workfront marca automáticamente un proyecto como Completo cuando todas las tareas y problemas del proyecto se marcan como Completo. 
    <p><b>IMPORTANTE</b> </p>
    <p>Puede marcar un proyecto como Completo solo cuando se hayan resuelto todas las tareas, problemas y aprobaciones del proyecto.</p> </td> 
   <td>
    <p>Los usuarios del equipo del proyecto no pueden ver el proyecto en sus listas de proyectos de forma predeterminada (sin un filtro personalizado), en el área de Proyectos de Workfront. Las tareas y los problemas que se les asignan en el proyecto no rellenan sus listas Solicitudes de trabajo o Trabajando en. </p>
    <p>Todas las notificaciones relacionadas con el proyecto, excepto una notificación de cambio de estado, dejan de enviarse a los usuarios del equipo del proyecto.</p>
    <p>El sistema ya no calcula la cronología del proyecto. </p>
    <p>No se puede copiar el proyecto.</p>
    <p>Puede impedir que los usuarios realicen acciones adicionales cuando un proyecto se marque como Completo. </p><p>Para obtener más información sobre cómo restringir las acciones en proyectos que están marcados como Completados, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Inactivo</td> 
   <td>El proyecto aún no ha finalizado, pero debido a bloqueos de carreteras o cambios de ámbito, el proyecto no puede continuar trabajando y se ha abandonado. El administrador del proyecto cambia el estado a Inactivo para avisar a los usuarios del equipo del proyecto de que este proyecto nunca terminará y de que ya no deben trabajar en él.</td> 
   <td> <p>Los usuarios del equipo del proyecto no pueden ver el proyecto en sus listas de proyectos de forma predeterminada (sin un filtro personalizado), en el área de Proyectos de Workfront. Las tareas y problemas asignados a ellos en el proyecto desaparecen de su Lista de trabajos.</p> <p>Las decisiones de aprobación no se pueden conceder a tareas o problemas.</p> <p>Las notificaciones sobre cambios de escala de tiempo, asignaciones, acciones necesarias y aprobaciones no se envían a los usuarios del equipo del proyecto.</p> <p>El sistema no calcula automáticamente la cronología del proyecto, ya que el proyecto se percibe como una finalización.</p> <p>Puede impedir que los usuarios realicen determinadas acciones cuando un proyecto se marque como Inactivo. Para obtener más información sobre cómo restringir acciones en proyectos inactivados, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>En espera</td> 
   <td>El proyecto aún no ha terminado, pero debido a algunos retrasos, el proyecto necesita ser suspendido temporalmente. El jefe de proyecto decide utilizar este estado para avisar a los usuarios del equipo del proyecto de que dejen de trabajar en el proyecto en este momento.</td> 
   <td> <p>Los usuarios del equipo del proyecto no pueden ver el proyecto en sus listas de proyectos de forma predeterminada (sin un filtro personalizado), en el área de Proyectos de Workfront. Las tareas y problemas asignados a ellos en el proyecto desaparecen de su Lista de trabajos. </p> <p>Las decisiones de aprobación no se pueden conceder a tareas o problemas.</p> <p>Las notificaciones sobre cambios de escala de tiempo, asignaciones, acciones necesarias y aprobaciones no se envían a los usuarios del equipo del proyecto.</p> <p> <p><b>NOTA</b>: Cuando se coloca un proyecto en espera, la cronología del proyecto no se detiene. El proyecto aún puede mostrarse como En riesgo o Con problemas aunque nadie esté trabajando activamente en el proyecto. Es posible que se necesiten algunos ajustes manuales de las fechas de las tareas abiertas restantes al volver a poner el proyecto en Actual, de modo que el proyecto pueda mostrar el progreso actualizado.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>Solicitada</td> 
   <td>El estado del proyecto se marca automáticamente como Solicitado por el sistema, cuando el caso comercial de una solicitud de proyecto se ha completado y enviado para su aprobación. Para obtener más información sobre cómo solicitar un proyecto mediante un caso empresarial, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar proyectos solicitados</a>.</td> 
   <td> <p>Los usuarios del equipo del proyecto no pueden ver el proyecto en sus listas de proyectos de forma predeterminada (sin un filtro personalizado), en el área de Proyectos de Workfront. Las tareas y los problemas del proyecto que se les han asignado no rellenan su Lista de trabajos.</p> <p>Todas las notificaciones relacionadas con el proyecto, excepto una notificación de cambio de estado, no se envían a ningún usuario.</p> <p>El sistema no calcula automáticamente la cronología del proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>Aprobado</td> 
   <td>El estado del proyecto se marca automáticamente como Aprobado cuando se aprueba el caso empresarial de una solicitud de proyecto. Para obtener más información sobre cómo solicitar un proyecto mediante un caso empresarial, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar proyectos solicitados</a>.</td> 
   <td> <p>Los usuarios del equipo del proyecto pueden ver el proyecto en sus listas de proyectos de forma predeterminada (sin un filtro personalizado), en el área de Proyectos de Workfront. Las tareas y los problemas asignados a ellos en el proyecto no rellenan su Lista de trabajos.</p> <p>Todas las notificaciones relacionadas con el proyecto, excepto una notificación de cambio de estado, no se envían a ningún usuario.</p> <p>El sistema no calcula automáticamente la cronología del proyecto. </p> </td> 
  </tr> 
  <tr> 
   <td>Rechazado</td> 
   <td>El estado del proyecto se marca automáticamente como Rechazado cuando se ha rechazado el caso comercial de una solicitud de proyecto. Para obtener más información sobre cómo solicitar un proyecto mediante un caso empresarial, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar proyectos solicitados</a>.</td> 
   <td> <p>Los usuarios del equipo del proyecto no pueden ver el proyecto en sus listas de proyectos de forma predeterminada (sin un filtro personalizado), en el área de Proyectos de Workfront. Las tareas y los problemas asignados a ellos en el proyecto no rellenan su Lista de trabajos.</p> <p>Todas las notificaciones relacionadas con el proyecto, excepto una notificación de cambio de estado, no se envían a ningún usuario.</p> <p>El sistema no calcula automáticamente la cronología del proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>Idea</td> 
   <td>El estado del proyecto se marca automáticamente como Idea cuando envía una solicitud de proyecto. Para obtener más información sobre cómo solicitar un proyecto mediante un caso empresarial, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar proyectos solicitados</a>.</td> 
   <td> <p>Los usuarios del equipo del proyecto no pueden ver el proyecto en sus listas de proyectos de forma predeterminada (sin un filtro personalizado), en el área de Proyectos de Workfront. Las tareas y los problemas asignados a ellos en el proyecto no rellenan su Lista de trabajos.</p> <p>Todas las notificaciones relacionadas con el proyecto, excepto una notificación de cambio de estado, no se envían a ningún usuario.</p> <p>El sistema no calcula automáticamente la cronología del proyecto.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Los siguientes estados de proyecto no se pueden cambiar a estado Cancelado, En espera o Completado:
>
>* Solicitada
>* Idea
>* Aprobado
>* Rechazado (o su equivalente)
>
