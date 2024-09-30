---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Resumen del trabajo delegado
description: Cuando planea estar fuera de la oficina por un corto período de tiempo, puede delegar temporalmente su trabajo a otros usuarios para asegurarse de que su ausencia no se convierta en un obstáculo para el trabajo que se está completando.
author: Lisa
feature: Work Management
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: 70e20df7c9738f33496e37b31b6e11caf0ac2f0f
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 1%

---

# Resumen del trabajo delegado

Cuando planea estar fuera de la oficina por un corto período de tiempo, puede delegar temporalmente su trabajo a otros usuarios para asegurarse de que su ausencia no se convierta en un obstáculo para el trabajo que se está completando.

Por ejemplo, si algunas tareas vencen antes de que regrese pero no tiene tiempo para completarlas antes de que se vaya, puede delegar las tareas a otro usuario para que pueda completarlas a tiempo y no retrasar la finalización del proyecto hasta después de que regrese.

Puede delegar los siguientes objetos en [!DNL Adobe Workfront]:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Tareas asignadas a usted
* Problemas asignados a usted
* Aprobaciones de proyectos, tareas o problemas asignadas a usted.

Este artículo contiene información general sobre la delegación de tareas y problemas.

Para obtener información sobre la delegación de aprobaciones de proyectos, tareas y problemas, consulte [Delegar solicitud de aprobación](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Para obtener información acerca de cómo delegar tareas y problemas, vea [Delegar tareas y problemas](../../manage-work/delegate-work/how-to-delegate-work.md).

## Resumen del trabajo delegado

Tenga en cuenta lo siguiente al delegar tareas y problemas:

* El administrador de [!DNL Workfront] o de grupo debe habilitar las preferencias de delegación en el área de [!UICONTROL Configuración] para poder delegar su trabajo a otros.

  Para obtener más información, consulte [Configurar las preferencias de tareas y problemas en todo el sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Solo puede delegar tareas y problemas desde el área [!UICONTROL Inicio].
* Existen excepciones para los siguientes tipos de licencia:

   * Puede delegar el trabajo a revisores o solicitantes, aunque [!DNL Workfront] no lo recomienda.
   * Los revisores pueden delegar el trabajo a otros. No pueden ver elementos de trabajo en su área [!UICONTROL Principal]. Solo pueden ver las aprobaciones.
   * Los solicitantes no pueden delegar el trabajo a otros. No pueden ver elementos de trabajo en su área [!UICONTROL Principal]
* Solo puede delegar las tareas y problemas que se le hayan asignado. No puede delegar tareas y problemas asignados a otros usuarios, equipos o roles.
* Solo puede delegar tareas y problemas que no se hayan completado antes de la fecha de inicio de la delegación.
* Si un elemento de trabajo se completa durante el lapso de tiempo de delegación, permanece en el área de Inicio del delegado y del usuario asignado durante 2 semanas antes de que [!DNL Workfront] lo elimine automáticamente.
* Los usuarios que seleccione como delegados reciben los mismos permisos que sus permisos en las tareas y problemas que delegue en ellos. Los permisos deben funcionar dentro de sus niveles de acceso y, a veces, sus niveles de acceso pueden ser inferiores a los suyos.

>[!NOTE]
>
>  Para los elementos que se asignan después de que la delegación ya haya comenzado, puede tardar hasta una hora después de que el elemento se haya asignado a [!DNL Workfront] en compartir los elementos recién asignados con el delegado.

* Si se le asignan tareas y problemas adicionales durante el tiempo que ha seleccionado para delegar su trabajo a otros usuarios, el nuevo trabajo asignado se delegará automáticamente a la misma persona durante el lapso de tiempo seleccionado si las fechas de la tarea o del problema se encuentran dentro de ese lapso de tiempo.
* Varios usuarios pueden seleccionar el mismo usuario como delegado.
* Las tareas y los problemas delegados no se muestran en las herramientas de administración de recursos, como [!UICONTROL Distribuidor de cargas de trabajo] o [!UICONTROL Planificador de recursos] para los usuarios delegados.
* Puede ver el trabajo delegado y los nombres delegados en varias áreas de [!DNL Workfront]. Para obtener más información, consulte la sección &quot;Localizar trabajo delegado e información de delegados&quot; en el artículo [Administrar la delegación de tareas y problemas](../delegate-work/how-to-delegate-work.md).


  >[!IMPORTANT]
  >
  >  Si un usuario solo tiene acceso de Vista a las tareas de su nivel de acceso y usted tiene permisos de Administración en las tareas que delega en él, recibirá permisos de Administración en las tareas que delega en él. Sin embargo, no podrán realizar las mismas acciones que usted en las tareas delegadas. Deben solicitar al administrador del sistema acceso de edición de tareas para poder actualizar las tareas en su ausencia.

* Al detener la delegación no se eliminan los permisos otorgados a los usuarios delegados en las tareas y problemas en los que se les ha delegado.
* Si un sistema o deshabilita la opción [!UICONTROL Permitir a los usuarios delegar sus tareas y problemas] en el área [!UICONTROL Configuración], los usuarios delegados actualmente se eliminarán de las tareas y problemas en los que se les haya delegado anteriormente. Sus permisos para las tareas o problemas no se eliminan.

## Diferencias y similitudes entre asignaciones y delegaciones

| Acción | Asignaciones | Delegaciones |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Un usuario asignado o delegado puede editar o eliminar el elemento de trabajo al que está asignado o delegado | Según permisos y nivel de acceso | Según permisos y nivel de acceso |
| Aparece un usuario asignado o delegado en el encabezado del elemento de trabajo | Sí | Sí |
| Las tareas o problemas asignados o delegados se muestran en el área de Inicio del usuario asignado o delegado | Sí, hasta que finalice el artículo | Sí, sólo para el período de tiempo de la delegación |
| Puede asignar o delegar trabajo a usuarios desde el área de Inicio | Sí | Sí |
| Puede asignar o delegar trabajo a usuarios mediante el | Sí | No |
| Puede asignar o delegar trabajo a usuarios de una lista o desde el encabezado de un elemento de trabajo | Sí | No |
| Cualquier usuario puede asignar o delegar otros usuarios con elementos de trabajo con los que no están asociados | Según permisos y nivel de acceso | No. Solo el usuario asignado puede delegar sus propios elementos. |
| Las horas planificadas, reales o presupuestadas para el trabajo asignado o delegado a un usuario se muestran para ese usuario en las herramientas de administración de recursos | Sí | No |
