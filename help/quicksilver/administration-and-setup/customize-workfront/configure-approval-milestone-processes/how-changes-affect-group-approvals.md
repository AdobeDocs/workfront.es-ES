---
title: Cómo afectan los cambios de grupos y procesos de aprobación a los procesos de aprobación asignados
user-type: administrator
content-type: reference
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: En este artículo se explica qué sucede cuando un proceso de aprobación ya está en uso cuando un administrador de Workfront (o un usuario con acceso administrativo a procesos de aprobación) cambia su asociación con un grupo.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 77b2dce2-1523-4262-a659-0d301059a54c
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 1%

---

# Cómo afectan los cambios en los procesos de aprobación y de grupo a los procesos de aprobación asignados

En este artículo se explica qué sucede cuando un proceso de aprobación ya está asociado con tareas, problemas, proyectos, plantillas o tareas de plantilla y un administrador de Workfront (o un usuario con acceso administrativo a los procesos de aprobación) realiza una de las siguientes acciones:

* Cambia el proceso de aprobación (nivel de grupo) de un grupo a otro
* Cambia el grupo asociado con el proyecto
* Cambia el proceso de aprobación de nivel de grupo a nivel de sistema
* Cambia el proceso de aprobación de nivel de sistema a nivel de grupo

El artículo también describe lo que sucede cuando se mueven o copian tareas o problemas asociados con un proceso de aprobación de nivel de grupo entre dos proyectos de diferentes grupos.

Para obtener información acerca de los tres tipos de procesos de aprobación que se pueden usar en Workfront, vea [Resumen del proceso de aprobación](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

>[!NOTE]
>
>Si el proyecto, sus tareas o problemas ya están asociados a un proceso de aprobación de nivel de grupo mediante estados personalizados de nivel de grupo, cambiar el grupo podría crear un conflicto entre los estados de aprobación del grupo anterior y los existentes en el nivel de sistema.
>
>Por ejemplo, si un proceso de aprobación contiene dos rutas, una para un estado de nivel de sistema y otra para un estado de nivel de grupo que equivale al mismo estado de nivel de sistema, cambiar el grupo del proyecto original hará que Workfront tenga problemas para comprender el estado específico del grupo que podría no existir en el segundo grupo. En este caso, se producirá un error.
>
>Considere la posibilidad de eliminar los procesos de aprobación de nivel de grupo en el proyecto, o sus tareas o problemas antes de actualizar el grupo del proyecto.
>
>Para obtener información acerca de cómo crear procesos de aprobación de nivel de grupo, vea [Procesos de aprobación de nivel de grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).
>
>Para obtener información sobre cómo crear un estado personalizado de nivel de grupo, vea [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)

## Cambio de un proceso de aprobación específico de un grupo de un grupo a otro

Los siguientes escenarios ocurren cuando ya se está usando un proceso de aprobación específico de un grupo en un objeto y alguien lo reasigna a un grupo diferente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Área u objeto donde se adjuntó el proceso de aprobación</th> 
   <th>Objeto de aprobación</th> 
   <th>Cambio en el proceso de aprobación del objeto o área</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aprobación de proyecto o plantilla </td> 
   <td>Proyecto</td> 
   <td>Se convierte en un proceso de aprobación de un solo uso</td> 
  </tr> 
  <tr> 
   <td>Aprobación de tarea o plantilla de tarea </td> 
   <td>Tarea</td> 
   <td>Se convierte en un proceso de aprobación de un solo uso </td> 
  </tr> 
  <tr> 
   <td>Aprobación del problema</td> 
   <td>Problema</td> 
   <td>Se convierte en un proceso de aprobación de un solo uso</td> 
  </tr> 
  <tr> 
   <td>Área Tareas en el cuadro Editar proyecto o Editar plantilla</td> 
   <td>Tarea</td> 
   <td> <p>El campo Proceso de aprobación predeterminado de la tarea se restablece a N/D.</p> <p>De forma predeterminada, no hay procesos de aprobación asociados con las nuevas tareas del proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>Sección Detalles de cola de un proyecto o plantilla</td> 
   <td>Problema</td> 
   <td> <p>El campo Aprobación predeterminada se restablece a N/D.</p> <p>De forma predeterminada, no hay procesos de aprobación asociados con nuevos problemas o solicitudes en el proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>Sección Tema de cola de un proyecto o plantilla</td> 
   <td>Problema</td> 
   <td> <p>El campo Aprobación predeterminada se restablece a N/D.</p> <p>De forma predeterminada, no hay procesos de aprobación asociados a nuevos problemas o solicitudes en el proyecto.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modificación del grupo asociado a un proyecto

Cuando alguien cambia el grupo asociado con un proyecto a otro grupo, ocurre lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Área u objeto que tiene el proceso de aprobación ya adjunto</th> 
   <th>Objeto de aprobación</th> 
   <th>Cambio en el proceso de aprobación del objeto o área</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aprobación de proyecto o plantilla </td> 
   <td>Proyecto</td> 
   <td>Se convierte en un proceso de aprobación de un solo uso y el estado asociado a él se actualiza para que coincida con un estado similar para el nuevo grupo.</td> 
  </tr> 
  <tr> 
   <td>Aprobación de tarea o plantilla de tarea </td> 
   <td>Tarea</td> 
   <td>Se convierte en un proceso de aprobación de un solo uso y el estado asociado a él se actualiza para que coincida con un estado similar para el nuevo grupo.</td> 
  </tr> 
  <tr> 
   <td>Aprobación del problema</td> 
   <td>Problema</td> 
   <td>Se convierte en un proceso de aprobación de un solo uso y el estado asociado a él se actualiza para que coincida con un estado similar para el nuevo grupo.</td> 
  </tr> 
  <tr> 
   <td>Área Tareas en el cuadro Editar proyecto o Editar plantilla</td> 
   <td>Tarea</td> 
   <td> <p>El campo Proceso de aprobación predeterminado de la tarea se restablece a N/D</p> <p>De forma predeterminada, no hay procesos de aprobación asociados con las nuevas tareas del proyecto</p> </td> 
  </tr> 
  <tr> 
   <td>Sección Detalles de cola de un proyecto o plantilla</td> 
   <td>Problema</td> 
   <td> <p>El campo Proceso de aprobación predeterminado se restablece a N/D</p> <p>De forma predeterminada, no hay procesos de aprobación asociados con nuevos problemas o solicitudes en el proyecto</p> </td> 
  </tr> 
  <tr> 
   <td>Sección Tema de cola de un proyecto o plantilla</td> 
   <td>Problema</td> 
   <td> <p>El campo Proceso de aprobación predeterminado se restablece a N/D</p> <p>De forma predeterminada, no hay procesos de aprobación asociados con nuevos problemas o solicitudes en el proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

## Cambio de un proceso de aprobación de nivel de grupo a nivel de sistema

Cuando alguien cambia la opción Group en un proceso de aprobación específico del grupo a All groups, el proceso de aprobación pasa a ser de todo el sistema y ocurre lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Área u objeto donde se adjuntó el proceso de aprobación</th> 
   <th>Objeto de aprobación</th> 
   <th>Cambio en el proceso de aprobación del objeto o área</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aprobación de proyecto o plantilla </td> 
   <td>Proyecto</td> 
   <td>Sin cambios</td> 
  </tr> 
  <tr> 
   <td>Aprobación de tarea o plantilla de tarea </td> 
   <td>Tarea</td> 
   <td>Sin cambios</td> 
  </tr> 
  <tr> 
   <td>Aprobación del problema</td> 
   <td>Problema</td> 
   <td>Sin cambios</td> 
  </tr> 
  <tr> 
   <td>Área Tareas en el cuadro Editar proyecto o Editar plantilla</td> 
   <td>Tarea</td> 
   <td> <p>No hay cambios en el proceso de aprobación, pero, de forma predeterminada, está asociado con nuevas tareas del proyecto</p> </td> 
  </tr> 
  <tr> 
   <td>Sección Detalles de cola de un proyecto o plantilla</td> 
   <td>Problema</td> 
   <td> <p>No hay cambios en el proceso de aprobación, pero de forma predeterminada está asociado con nuevos problemas o solicitudes en el proyecto</p> </td> 
  </tr> 
  <tr> 
   <td>Sección Tema de cola de un proyecto o plantilla</td> 
   <td>Problema</td> 
   <td> <p>No hay cambios en el proceso de aprobación, pero de forma predeterminada está asociado con nuevos problemas o solicitudes en el proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

## Cambio de un proceso de aprobación de nivel de sistema a nivel de grupo

Cuando alguien cambia la disponibilidad de un proceso de aprobación de todo el sistema de &quot;Todos los grupos&quot; a un grupo específico, el proceso de aprobación se vuelve específico del grupo y ocurre lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Área u objeto donde se adjuntó el proceso de aprobación</th> 
   <th>Objeto de aprobación</th> 
   <th>Cambio en el proceso de aprobación del objeto o área</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Proyecto, tarea, problema, plantilla o tarea de plantilla que pertenece al grupo del proceso de aprobación</td> 
   <td> <p>Proyecto, tarea o problema</p> </td> 
   <td>Sin cambios</td> 
  </tr> 
  <tr> 
   <td>Área Tareas en el cuadro Editar proyecto o Editar plantilla de un proyecto o plantilla que pertenece al grupo del proceso de aprobación</td> 
   <td>Tarea</td> 
   <td> <p>No hay cambios en el proceso de aprobación, pero, de forma predeterminada, está asociado con nuevas tareas del proyecto</p> </td> 
  </tr> 
  <tr> 
   <td>Detalles de cola para un proyecto o plantilla que pertenece al grupo del proceso de aprobación</td> 
   <td>Problema</td> 
   <td> <p>No hay cambios en el proceso de aprobación, pero de forma predeterminada está asociado con nuevos problemas o solicitudes en el proyecto</p> </td> 
  </tr> 
  <tr> 
   <td>Sección Tema de cola para un proyecto o plantilla que pertenece al grupo del proceso de aprobación</td> 
   <td>Problema</td> 
   <td> <p>No hay cambios en el proceso de aprobación, pero de forma predeterminada está asociado con nuevos problemas o solicitudes en el proyecto</p> </td> 
  </tr> 
  <tr> 
   <td>Proyecto, tarea, problema, plantilla o tarea de plantilla que pertenece a un grupo que no sea el grupo del proceso de aprobación</td> 
   <td> <p>Proyectos</p> <p>Tareas</p> <p>Problemas</p> </td> 
   <td>Se convierte en un proceso de aprobación de un solo uso</td> 
  </tr> 
  <tr> 
   <td>Área Tareas en el cuadro Editar proyecto o Editar plantilla de un proyecto o plantilla que pertenece a un grupo que no es el grupo del proceso de aprobación</td> 
   <td>Tareas</td> 
   <td> <p>El campo Proceso de aprobación predeterminado de la tarea se restablece a N/D.</p> <p>De forma predeterminada, no hay procesos de aprobación asociados con las nuevas tareas del proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>Detalles de cola para un proyecto o plantilla que pertenece a un grupo que no es el grupo del proceso de aprobación</td> 
   <td>Problemas</td> 
   <td> <p>El campo Aprobación predeterminada se restablece a N/D.</p> <p>De forma predeterminada, no hay procesos de aprobación asociados con nuevos problemas o solicitudes en el proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td>Sección Tema de cola para un proyecto o plantilla que pertenece a un grupo que no es el grupo del proceso de aprobación</td> 
   <td>Problemas</td> 
   <td> <p>El campo Aprobación predeterminada se restablece a N/D.</p> <p>De forma predeterminada, no hay procesos de aprobación asociados con nuevos problemas o solicitudes en el proyecto.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Mover o copiar una tarea o un problema a un proyecto con un grupo diferente al del proceso de aprobación

Mover o copiar una tarea o un problema de un proyecto a otro puede afectar los procesos de aprobación existentes en la tarea o el problema según los grupos de los dos proyectos. La siguiente tabla ilustra los escenarios que podrían existir:

| Proceso de aprobación de tarea o problema original | Grupos de los dos proyectos | Cambios en el proceso de aprobación después de mover la tarea o el problema a otro proyecto |
|---|---|---|
| Proceso de aprobación de un solo uso asociado a un estado de todo el sistema | Los proyectos están en el mismo grupo o en diferentes grupos | Sin cambios |
| Proceso de aprobación de un solo uso asociado a un estado específico de grupo | Los proyectos están en diferentes grupos | La aprobación sigue siendo un proceso de aprobación de un solo uso y el estado asociado con las actualizaciones de aprobación para que coincidan con un estado similar para el nuevo grupo. |
| Proceso de aprobación en todo el sistema | Los proyectos están en el mismo grupo o en diferentes grupos | Sin cambios |
| Proceso de aprobación específico del grupo | Los proyectos están en el mismo grupo | Sin cambios |
| Proceso de aprobación específico del grupo | Los proyectos están en diferentes grupos y los grupos tienen diferentes estados específicos de grupos | La aprobación se convierte en un proceso de aprobación de un solo uso y el estado asociado con las actualizaciones de aprobación se actualiza para que coincidan con un estado similar para el nuevo grupo. |
| Proceso de aprobación específico del grupo | Los proyectos están en grupos diferentes y hay un estado con la misma clave en el nuevo grupo que el estado asociado al proceso de aprobación del primer grupo | Sin cambios |
