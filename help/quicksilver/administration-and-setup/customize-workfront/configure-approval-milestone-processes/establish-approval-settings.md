---
title: Configuración de la aprobación global
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Como administrador de Adobe Workfront, puede determinar la configuración global de los procesos de aprobación en Workfront. Esta configuración afecta a todos los procesos de aprobación de elementos de trabajo del sistema.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 2%

---

# Configuración de la aprobación global

Como administrador de Adobe Workfront, puede determinar la configuración global de los procesos de aprobación en Workfront. Esta configuración afecta a todos los procesos de aprobación de elementos de trabajo del sistema.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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
   <td> <p>Debe ser administrador del sistema o tener una licencia de planificación con acceso administrativo a los procesos de aprobación</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Configuración de la aprobación global

{{step-1-to-setup}}

1. Haga clic en **Procesos** > **Aprobaciones**.

1. Haga clic en el icono **Configuración** ![](assets/gear-icon-settings.png) junto al nombre del área **Aprobaciones**.

1. En el cuadro **Configuración de aprobación** que aparece, especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Agregar &lt;number&gt; días a la fecha planificada de finalización para dar cabida a los procesos de aprobación</td> 
      <td> <p>Especifique el número de minutos, horas, días, semanas o meses para agregar tiempo a la fecha planificada de finalización de la tarea que necesita aprobación. Seleccione "Transcurridos" minutos, horas, días o semanas para agregar tiempo que incluya cualquier fin de semana, festivo y jornada no laboral que se haya designado en el calendario de trabajo del sistema.</p> 
      <p>Por ejemplo, si una tarea se asigna el viernes y tiene una duración de 3 días transcurridos, la fecha de finalización de la tarea se establece en lunes (suponiendo que sábado y domingo sea fin de semana). Si la tarea tiene una duración de 3 días (no transcurridos), la fecha de finalización de la tarea se establece en miércoles.</p>
      <p><b>NOTA</b>: si se habilita la adición de tiempo adicional para la aprobación de tareas, se afectará la cronología de la tarea y la del proyecto.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">No se requiere que el aprobador esté en el equipo del proyecto (para procesos de aprobación que incluyen un rol)</td> 
      <td> <p>Seleccione esta opción si no se requiere que un aprobador esté en el equipo del proyecto cuando un proceso de aprobación incluya un rol. Al asignar la decisión de aprobación a una función de trabajo, solo los usuarios que tengan una función asociada a ellos en el proyecto verán la aprobación. Si habilita esta configuración, cualquier usuario con ese rol de trabajo recibe la solicitud de aprobación tanto si está en el equipo del proyecto como si no. Para obtener información sobre cómo editar el rol de proyecto de un usuario, consulte <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Administrar el equipo del proyecto</a>. </p> 
      <p><b>SUGERENCIA</b>: Cuando asigna una aprobación a un rol y la opción <b>No se requiere que el aprobador esté en el equipo del proyecto (para los procesos de aprobación que incluyen un rol)</b> está deshabilitada, pero no hay roles en el equipo del proyecto que coincidan con el rol en la aprobación, la aprobación se reasigna al propietario del proyecto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deshabilitar delegación de aprobación</td> 
      <td> <p>Seleccione esta opción para deshabilitar la funcionalidad para que los usuarios del sistema deleguen aprobaciones a otro usuario. Cuando se selecciona esta opción, se elimina de Workfront la opción para delegar aprobaciones y se detienen las delegaciones de aprobación existentes.</p> <p>Para obtener más información sobre la delegación de aprobaciones en Workfront, consulte <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Delegar solicitud de aprobación</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir edición del formulario personalizado cuando el proyecto, la tarea o el problema tengan el estado de aprobación pendiente</td> 
      <td> <p>Seleccione esta opción para permitir que los usuarios editen el formulario personalizado de proyectos, tareas y problemas cuando se encuentren en el estado de Aprobación pendiente. Esta es la configuración predeterminada.</p> 
      <p>Cuando se selecciona esta opción:</p> 
       <ul> 
       <li>Todos los aprobadores (y cualquier otro usuario que tenga acceso para editar el formulario personalizado) pueden realizar cambios en el formulario personalizado cuando el objeto esté pendiente de aprobación, independientemente de la ruta de aprobación actual o del paso de aprobación.</li> 
       <li>Los cambios realizados en el formulario personalizado durante un proceso de aprobación no afectan a ninguna decisión de aprobación tomada antes del cambio.</li> 
       <li> <p>Cualquier cambio realizado en el proyecto, la tarea o el problema se rastrea de la misma manera, independientemente de esta configuración. </p> <p>Por ejemplo, si agregó campos de formulario personalizados para su seguimiento en el flujo de actualización, cualquier cambio en el formulario se rastreará en el flujo de actualización del objeto.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que los usuarios recuperen las solicitudes recién creadas con aprobación pendiente</td> 
      <td> <p>Seleccione esta opción para configurar si los usuarios pueden recuperar un problema o una solicitud pendiente de aprobación para su primer estado. Puede asociar el primer estado de un problema o una solicitud con un proceso de aprobación configurando las colas de solicitudes. </p> 
      <p>Para obtener más información acerca de las colas de solicitudes, vea <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitudes</a>.</p> 
      <p>Realice una de las siguientes acciones:</p> 
       <ul> 
       <li>Seleccione esta opción para permitir que los usuarios recuperen una aprobación para el primer estado de un problema o una solicitud. En este caso, puede ver un botón Recall&lt; en un nuevo problema o solicitud que está pendiente de aprobación. Cuando seleccionen recuperar el problema, recibirán un aviso de que el problema también se eliminará. El problema se elimina después de que hayan confirmado que lo han recuperado. </li> 
       <li> <p>Anule la selección de esta opción para evitar que los usuarios recuperen un problema o una solicitud cuyo primer estado sea pendiente de aprobación. No pueden ver el botón Recall&lt; en el nuevo problema o solicitud y se debe conceder la aprobación. Esta es la opción predeterminada.</p> 
       <p>Para obtener más información acerca de la revisión de elementos en espera de aprobación, vea <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Ver aprobaciones </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar cambios.**
