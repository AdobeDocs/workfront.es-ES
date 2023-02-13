---
title: Configuración de la aprobación global
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Como administrador de Adobe Workfront, puede determinar la configuración global para los procesos de aprobación en Workfront. Esta configuración afecta a todos los procesos de aprobación de elementos de trabajo del sistema.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 1%

---

# Configuración de la aprobación global

Como administrador de Adobe Workfront, puede determinar la configuración global para los procesos de aprobación en Workfront. Esta configuración afecta a todos los procesos de aprobación de elementos de trabajo del sistema.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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
   <td> <p>Debe ser administrador del sistema o tener una licencia de plan con acceso administrativo a los procesos de aprobación</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Configuración de la aprobación global

1. Inicie sesión en Workfront como administrador de Workfront .
1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Procesos** > **Aprobaciones** .

1. Haga clic en el **Configuración** icono ![](assets/gear-icon-settings.png) junto a la variable **Aprobaciones** nombre del área.

1. En el **Configuración de aprobación** especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Agregar &lt;number&gt; Días hasta la fecha de finalización planificada para adaptarse a los procesos de aprobación</td> 
      <td> <p>Especifique el número de minutos, horas, días, semanas o meses para agregar hora a la fecha de finalización planificada de la tarea que necesita aprobación. Seleccione "Transcurridos" minutos, horas, días o semanas para agregar tiempo que incluya cualquier fin de semana, festivos y horas no laborables que se hayan designado en el calendario de programación de trabajo del sistema.</p> 
      <p>Por ejemplo, si una tarea está asignada el viernes y tiene una duración de 3 días transcurridos, la fecha de finalización de la tarea se establece para el lunes (suponiendo que sábado y domingo sean un fin de semana). Si la tarea tiene una duración de 3 días (no transcurrido), la fecha de finalización de la tarea se establece para el miércoles.</p>
      <p><b>NOTA</b>: Si se habilita la adición de tiempo adicional para dar cabida a la aprobación en las tareas, se verá afectada la cronología de la tarea y la del proyecto.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">No es necesario que el aprobador esté en el equipo del proyecto (para procesos de aprobación que incluyen una función)</td> 
      <td> <p>Seleccione esta opción si no es necesario que un aprobador esté en el equipo del proyecto cuando un proceso de aprobación incluya una función. Al asignar la decisión de aprobación a una función de trabajo, solo los usuarios que tengan una función asociada en el proyecto verán la aprobación. Si habilita esta configuración, cualquier usuario con esa función de trabajo recibe la solicitud de aprobación tanto si está en el equipo del proyecto como si no. Para obtener información sobre cómo editar la función de proyecto de un usuario, consulte <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Administrar el equipo del proyecto</a>. </p> 
      <p><b>SUGERENCIA</b>: Al asignar una aprobación a una función y la opción <b>No es necesario que el aprobador esté en el equipo del proyecto (para procesos de aprobación que incluyen una función)</b> está desactivado, pero no hay funciones en el equipo del proyecto que coincidan con la función de aprobación, la aprobación se reasigna al propietario del proyecto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deshabilitar delegación de aprobación</td> 
      <td> <p>Seleccione esta opción para deshabilitar la funcionalidad de que los usuarios del sistema deleguen aprobaciones a otro usuario. Cuando se selecciona esta opción, se elimina de Workfront la opción para delegar aprobaciones y se detiene cualquier delegación de aprobación existente.</p> <p>Para obtener más información sobre la delegación de aprobaciones en Workfront, consulte <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Delegar solicitud de aprobación</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir edición del formulario personalizado cuando el proyecto, la tarea o el problema están en estado de aprobación pendiente</td> 
      <td> <p>Seleccione esta opción para permitir que los usuarios editen la forma personalizada de proyectos, tareas y problemas en el estado Pendiente de aprobación . Esta es la configuración predeterminada.</p> 
      <p>Cuando se selecciona esta opción:</p> 
       <ul> 
       <li>Todos los aprobadores (y cualquier otro usuario que tenga acceso para editar el formulario personalizado) pueden realizar cambios en el formulario personalizado cuando el objeto está pendiente de aprobación, independientemente de la ruta de aprobación o del paso de aprobación actual.</li> 
       <li>Los cambios realizados en el formulario personalizado durante un proceso de aprobación no afectan a las decisiones de aprobación que se tomaron antes del cambio.</li> 
       <li> <p>Cualquier cambio realizado en el proyecto, la tarea o el problema se rastrea del mismo modo, independientemente de esta configuración. </p> <p>Por ejemplo, si agregó campos de formulario personalizados para rastrearlos en la secuencia de actualización, cualquier cambio en el formulario se rastreará en la secuencia de actualización del objeto.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que los usuarios recuperen las solicitudes recién creadas con aprobación pendiente</td> 
      <td> <p>Seleccione esta opción para configurar si los usuarios pueden recuperar un problema o una solicitud en espera de aprobación para su primer estado. Puede asociar el primer estado de un problema o una solicitud a un proceso de aprobación configurando las colas de solicitudes. </p> 
      <p>Para obtener más información sobre las colas de solicitud, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitud</a>.</p> 
      <p>Realice una de las siguientes acciones:</p> 
       <ul> 
       <li>Seleccione esta opción para permitir a los usuarios recuperar una aprobación para el primer estado de un problema o una solicitud. En este caso, pueden ver un botón Recall&lt; en un nuevo problema o solicitud que está pendiente de aprobación. Cuando decidan recordar el problema, recibirán una advertencia de que el problema también será eliminado. El problema se borra después de que confirmen que lo recuerdan. </li> 
       <li> <p>Anule la selección de esta opción para evitar que los usuarios vuelvan a llamar a un problema o a una solicitud cuyo primer estado esté pendiente de aprobación. No pueden ver un botón Recall&lt; en el nuevo número o solicitud y se debe conceder la aprobación. Esta es la opción predeterminada.</p> 
       <p>Para obtener más información sobre la revisión de elementos en espera de aprobación, consulte <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Ver aprobaciones </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guarde los cambios.**
