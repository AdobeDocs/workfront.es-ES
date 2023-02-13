---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Resumen del trabajo de los delegados
description: Cuando planee estar fuera de la oficina durante un breve período de tiempo, puede delegar temporalmente su trabajo a otros usuarios para asegurarse de que su ausencia no se convierta en un obstáculo para el trabajo que se está completando.
author: Alina
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: f3ae487f53f7c4f8c389cf0d35323f21e76ece35
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 1%

---

# Resumen del trabajo de los delegados

Cuando planee estar fuera de la oficina durante un breve período de tiempo, puede delegar temporalmente su trabajo a otros usuarios para asegurarse de que su ausencia no se convierta en un obstáculo para el trabajo que se está completando.

Por ejemplo, si determinadas tareas están pendientes antes de regresar pero no tiene tiempo de completarlas antes de irse, puede delegar las tareas a otro usuario para que pueda completarlas a tiempo y no retrasar la finalización del proyecto hasta después de volver.

Puede delegar los siguientes objetos en [!DNL Adobe Workfront]:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Tareas asignadas
* Problemas asignados
* Proyecto, tarea, problema, aprobaciones de documento asignadas a usted.

Este artículo contiene información general sobre la delegación de tareas y problemas.

Para obtener información sobre la delegación de aprobaciones de proyecto, tarea, problema y documento, consulte [Delegar solicitud de aprobación](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Para obtener información sobre cómo delegar tareas y problemas, consulte [Delegación de tareas y problemas](../../manage-work/delegate-work/how-to-delegate-work.md).

## Resumen del trabajo de los delegados

Tenga en cuenta lo siguiente cuando delegue tareas y problemas:

* Su [!DNL Workfront] o el administrador del grupo debe habilitar las preferencias de Delegación en la variable [!UICONTROL Configuración] para poder delegar el trabajo a otros.

   Para obtener más información, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Solo se pueden delegar tareas y problemas desde el [!UICONTROL Página principal] .
* Existen excepciones para los siguientes tipos de licencia:

   * Puede delegar el trabajo a revisores o solicitantes, aunque [!DNL Workfront] no lo recomienda.
   * Los revisores pueden delegar el trabajo a otros. No pueden ver los elementos de trabajo en su [!UICONTROL Página principal] . Solo pueden ver las aprobaciones.
   * Los solicitantes no pueden delegar el trabajo a otros. No pueden ver los elementos de trabajo en su [!UICONTROL Página principal] area
* Solo puede delegar las tareas y los problemas asignados a usted. No puede delegar tareas y problemas asignados a otros usuarios, equipos o funciones de trabajo.
* Solo puede delegar tareas y problemas que no se hayan completado antes de la fecha de inicio de la delegación.
* Si un elemento de trabajo se completa durante el período de tiempo de delegación, el elemento permanecerá en la zona de origen del delegado y del cesionario durante dos semanas antes [!DNL Workfront] automáticamente lo elimina.
* Los usuarios que seleccione como delegados reciben los mismos permisos que sus permisos en las tareas y problemas que delega en ellos. Los permisos deben funcionar dentro de sus niveles de acceso y, a veces, sus niveles de acceso pueden ser inferiores a los suyos.

>[!NOTE]
>
>  Para los elementos que se asignan después de que la delegación ya se haya iniciado, puede tardar hasta una hora después de que se haya asignado el elemento [!DNL Workfront] para compartir los elementos recién asignados con el delegado.

* Si se le asignan tareas y problemas adicionales durante el tiempo seleccionado para delegar su trabajo a otros usuarios, el nuevo trabajo asignado se delega automáticamente a la misma persona durante el lapso de tiempo seleccionado si las fechas de la tarea o del problema se encuentran dentro de ese lapso de tiempo.
* El mismo usuario puede ser seleccionado como delegado por varios usuarios.
* Las tareas y los problemas delegados no se muestran en las herramientas de administración de recursos, como el [!UICONTROL Equilibrador de carga de trabajo] o [!UICONTROL Planificador de recursos] para los usuarios delegados.
* Puede ver los nombres de delegados y trabajos delegados en varias áreas de [!DNL Workfront]. Para obtener más información, consulte la sección &quot;Localización de trabajo delegado e información sobre los delegados&quot; en el artículo [Administrar delegación de tareas y problemas](../delegate-work/how-to-delegate-work.md).


   >[!IMPORTANT]
   >
   >  Si un usuario solo tiene acceso de vista a tareas en su nivel de acceso y tiene permisos de administración en las tareas que delega en ellas, recibirá permisos de administración para las tareas que delegue en ellas. Sin embargo, no podrán realizar las mismas acciones que usted en las tareas delegadas. Deben solicitar el acceso de edición a Tareas al administrador del sistema para poder actualizar las tareas en su ausencia.

* Al detener la delegación, no se eliminan los permisos otorgados a los usuarios delegados sobre las tareas y los problemas en los que se han delegado.
* Si un sistema o deshabilita la variable [!UICONTROL Permitir que los usuarios deleguen sus tareas y problemas] en la [!UICONTROL Configuración] , los usuarios delegados actualmente se eliminan de las tareas y problemas a los que se han delegado previamente. Sus permisos para las tareas o los problemas no se eliminan.

## Diferencias y similitudes entre asignaciones y delegaciones

| Acción | Asignaciones | Delegaciones |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Un usuario asignado o delegado puede editar o eliminar el elemento de trabajo al que está asignado o delegado | Basado en permisos y nivel de acceso | Basado en permisos y nivel de acceso |
| Se muestra un usuario asignado o delegado en el encabezado del elemento de trabajo | Sí | Sí |
| Las tareas o problemas asignados o delegados se muestran en el área de inicio del usuario asignado o delegado | Sí, hasta que se complete el artículo | Sí, sólo para el período de tiempo de la delegación |
| Puede asignar o delegar trabajo a usuarios del área principal | Sí | Sí |
| Puede asignar o delegar el trabajo a los usuarios mediante la variable | Sí | No |
| Puede asignar o delegar trabajo a usuarios de una lista o del encabezado de un elemento de trabajo | Sí | No |
| Cualquier usuario puede asignar o delegar otros usuarios con elementos de trabajo que no estén asociados a | Basado en permisos y nivel de acceso | No. Solo el usuario asignado puede delegar sus propios elementos. |
| Horario planificado, real o presupuestado para el trabajo asignado o delegado a un usuario se muestra para ese usuario en las herramientas de administración de recursos | Sí | No |
