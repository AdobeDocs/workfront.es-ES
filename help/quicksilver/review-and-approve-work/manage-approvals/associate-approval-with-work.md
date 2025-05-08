---
product-area: projects
navigation-topic: approvals
title: Asociar un proceso de aprobación nuevo o existente con el trabajo
description: Este artículo describe cómo asociar procesos de aprobación con elementos de trabajo. Para obtener información sobre cómo asociar aprobaciones con pruebas o documentos, consulte los siguientes artículos.
author: Courtney and Alina
feature: Work Management, Digital Content and Documents
sexl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: 06e42fa713bc9b0c1e308feb2b84ca62dafa416c
workflow-type: tm+mt
source-wordcount: '1891'
ht-degree: 95%

---

# Asociar un proceso de aprobación nuevo o existente con el trabajo

Este artículo describe cómo asociar procesos de aprobación con elementos de trabajo. Para obtener información sobre cómo asociar aprobaciones con pruebas o documentos, consulte los siguientes artículos:

* [Crear una prueba avanzada con un flujo de trabajo automatizado](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Solicitar aprobaciones de documentos](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

Puede asociar un proceso de aprobación global o de un solo uso con un elemento de trabajo en Adobe Workfront. Se dan los siguientes escenarios:

* Asociar un proceso de aprobación global existente a un proyecto, tarea, problema, plantilla o tarea de plantilla. Algunos procesos de aprobación globales están disponibles para todos los grupos del sistema. Los procesos de aprobación globales de nivel de grupo solo están disponibles para determinados grupos.
* Cree un proceso de aprobación de un solo uso y asócielo a un proyecto, tarea, problema, plantilla o tarea de plantilla existente.

>[!NOTE]
>
>En este artículo se utiliza el término &quot;proceso de aprobación global&quot; para diferenciarlo del término &quot;proceso de aprobación de un solo uso&quot;. Un proceso de aprobación global se puede utilizar repetidamente.
>
>El término &quot;proceso de aprobación global de nivel de grupo&quot; hace referencia a un proceso de aprobación que puede utilizarse repetidamente para elementos y con estados asociados únicamente a un grupo específico.

Para obtener información más general acerca de los procesos de aprobación, consulte [Introducción al proceso de aprobación](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Para obtener información acerca de cómo crear un proceso de aprobación global, consulte [Crear un proceso de aprobación para elementos de trabajo](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Editar el acceso o superior a Proyectos, Tareas, Problemas o Plantillas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el proyecto, tarea, problema o plantilla</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Consideraciones acerca de la asociación de procesos de aprobación con elementos de trabajo

Además de las consideraciones que se describen a continuación, le recomendamos que vuelva a examinar las consideraciones generales sobre los procesos de aprobación en Workfront. Para más información, consulte [Información general sobre el proceso de aprobación](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* Debe crear el proyecto, la tarea, el problema, la plantilla o la tarea de plantilla antes de que el proceso de aprobación se pueda asociar a ellos.
* Al adjuntar un proceso de aprobación a un elemento para un estado que ha pasado y en el que el elemento se encuentra actualmente, el proceso de aprobación no se activa y no se envían notificaciones a los aprobadores.

  **Ejemplo:** Si una tarea está en estado Completo y se adjunta un proceso de aprobación asociado con el estado Completo, la aprobación no se activa.

* Al adjuntar un proceso de aprobación al primer estado de un elemento (mediante el uso de una plantilla para tareas y proyectos, el uso de los ajustes de la configuración de la cola para problemas o la definición de la configuración de la tarea de un proyecto para nuevas tareas), los procesos de aprobación se omiten si se recupera la aprobación enviada. En este caso, los aprobadores no reciben ninguna notificación.

  Para obtener más información sobre cómo recuperar aprobaciones, consulte [Ver aprobaciones](../../review-and-approve-work/manage-approvals/view-approvals.md).

  >[!TIP]
  >
  >El primer estado de una tarea o problema es Nuevo. El primer estado de un proyecto es el estado seleccionado por el administrador de Workfront en las Preferencias de proyecto del sistema. Para obtener más información, consulte [Configurar las preferencias de proyecto en todo el sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* La asociación de procesos de aprobación con un objeto no se registra en el área Actualizaciones del objeto.
* No puede asociar un proceso de aprobación con una tarea principal.
* Añadir un usuario, equipo o función como aprobador no les otorga automáticamente permisos para el objeto asociado con esa aprobación. Reciben permisos para el objeto cuando se activa el paso de aprobación. De lo contrario, los objetos deben compartirse con ellos antes de que puedan tomar una decisión de aprobación.

En las secciones siguientes se describen los diferentes métodos para asociar un proceso de aprobación a un proyecto, tarea o problema.

## Asociar un proceso de aprobación global a un elemento de trabajo {#associate-a-global-approval-process-with-a-work-item}

Puede asociar un proceso de aprobación global a un elemento de trabajo (proyecto, tarea, problema, plantilla, tarea de plantilla).

Puede acceder a cualquier proceso de aprobación global siempre y cuando se comparta con un grupo al que pertenezca o con todos los grupos del sistema.

<!--The global approval process must be available to the group associated with the work item or to all groups in the system.-->

>[!NOTE]
>
>Puede adjuntar procesos de aprobación de proyectos a una plantilla y procesos de aprobación de tareas a una tarea de plantilla. Después de hacer esto, cuando alguien usa la plantilla para crear un proyecto, el proceso de aprobación se convierte en un proceso de aprobación de proyecto o tarea, respectivamente. Un proceso de aprobación de un solo uso adjunto a una plantilla o tarea de plantilla sigue siendo un proceso de aprobación de un solo uso para proyectos y tareas.

Para obtener información sobre cómo los administradores de Workfront pueden configurar un proceso de aprobación global para todos los grupos del sistema y cómo los administradores de grupos pueden crear aprobaciones para un grupo, consulte [Crear un proceso de aprobación para elementos de trabajo](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>También puede modificar un proceso de aprobación global para satisfacer sus necesidades específicas. Para obtener más información, vea la sección [Modificar un proceso de aprobación global para utilizarlo en un objeto específico](#modify-a-global-approval-process-for-use-on-a-specific-object) en este artículo.

Para asociar un proceso de aprobación global existente a un proyecto, tarea, problema, plantilla o tarea de plantilla:

1. Vaya al elemento de trabajo donde desea asociar un proceso de aprobación.
1. Haga clic en **Aprobaciones** en el panel izquierdo.

   ![Sección de aprobaciones en la tarea](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![Use las aprobaciones existentes o cree aprobaciones de un solo uso](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   Se muestra el proceso de aprobación seleccionado.

1. Expanda el menú desplegable **Usar existente** y seleccione un proceso de aprobación existente.

   ![Menú de aprobaciones](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   Se muestra el proceso de aprobación seleccionado.

   ![Aprobación existente adjunta a la tarea](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. Haga clic en **Guardar**.
1. (Opcional) Haga clic en Editar proceso de aprobación si desea modificar la aprobación existente que adjuntó al elemento. Esto cambia el proceso de aprobación global a un proceso de aprobación de un solo uso. Para obtener más información, consulte la sección [Modificar un proceso de aprobación global para utilizarlo en un objeto específico](#modify-a-global-approval-process-for-use-on-a-specific-object) en este artículo.

## Modificar un proceso de aprobación global para su uso en un objeto específico {#modify-a-global-approval-process-for-use-on-a-specific-object}

Su administrador de Workfront o de grupo crea procesos de aprobación globales para que los use, tal como se describe en [Crear un proceso de aprobación para elementos de trabajo](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Modificar un proceso de aprobación global adjunto a un elemento es idéntico a modificar un proceso de aprobación de un solo uso.

Puede modificar un proceso de aprobación global para adaptarlo a cualquier necesidad específica del proyecto, tarea o problema que asocie con él.

>[!IMPORTANT]
>
>Al modificar un proceso de aprobación global, se convierte en un proceso de aprobación de un solo uso que solo se puede utilizar en el objeto en el que se ha modificado. El proceso de aprobación global permanece sin cambios.
>
>Tenga en cuenta las siguientes limitaciones al modificar un proceso de aprobación global:
>
>* El proceso de aprobación solo se modifica para el proyecto, la tarea o el problema con el que esté asociando el proceso de aprobación.
>* Cualquier cambio futuro realizado por un administrador en el proceso de aprobación global original no se reflejará en el proceso de aprobación global que haya modificado.
>

Para modificar un proceso de aprobación ya asociado a un elemento:

1. Añada un proceso de aprobación global al proyecto, tarea o problema.

   Para obtener instrucciones, consulte la sección [Asociar un proceso de aprobación global con un elemento de trabajo](#associate-a-global-approval-process-with-a-work-item) en este artículo.

   >[!IMPORTANT]
   >
   >Asegúrese de hacer clic en **Guardar** al añadir la aprobación.

1. Una vez agregado el proceso de aprobación global, haga clic en el icono **Editar** icono ![Editar icono](assets/edit-icon.png) en la esquina superior derecha de la página de aprobación. Esta acción convierte el proceso de aprobación global o de nivel de grupo en un proceso de aprobación de un solo uso.
1. Realice los cambios necesarios en el proceso de aprobación existente. Para obtener más información, vea la sección [Asociar un proceso de aprobación de un solo uso a un proyecto, tarea, problema, plantilla o tarea de plantilla](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) en este artículo.
1. Haga clic en **Guardar** y, a continuación, haga clic en **Guardar** de nuevo para confirmar que desea convertir el proceso de aprobación global en un proceso de aprobación de un solo uso que solo está disponible en este objeto.

## Asociar un proceso de aprobación de un solo uso a un proyecto, tarea, problema, plantilla o tarea de plantilla {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

Puede crear un proceso de aprobación de un solo uso para utilizarlo solo en un proyecto, tarea o problema específico.

También puede asociar un proceso de aprobación de un solo uso con una plantilla o tarea de plantilla para que esté disponible en proyectos y tareas creados a partir de la plantilla.

>[!NOTE]
>
>Puede asociar un proceso de aprobación de un solo uso con cualquier estado de nivel de sistema o de grupo para un proyecto, tarea, problema, plantilla o tarea de plantilla. Para obtener información acerca de los estados de Workfront, consulte [Crear o editar un estado](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

La creación de un proceso de aprobación de esta manera le permite crear un proceso de aprobación personalizado para satisfacer sus necesidades. Sin embargo, el proceso de aprobación no se puede asociar con otros elementos de trabajo en el futuro.

Como alternativa, puede modificar un proceso de aprobación global para un elemento específico y que también se convierte en un proceso de aprobación de un solo uso. Para obtener más información, consulte la sección [Modificar un proceso de aprobación global para utilizarlo en un objeto específico](#modify-a-global-approval-process-for-use-on-a-specific-object) en este artículo.

Crear proceso de aprobación de un solo uso:

1. Vaya al proyecto, tarea, problema, plantilla o tarea de plantilla donde desea asociar un proceso de aprobación.
1. Haga clic en **Aprobaciones** en el panel izquierdo.

   ![Sección de aprobaciones en la tarea](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Haga clic en **Crear un solo uso**.

   ![Menú de aprobaciones](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. Complete los pasos que comienzan con el paso 6 de la sección &quot;Crear un proceso de aprobación global de nivel de sistema o de grupo para los elementos de trabajo&quot; del artículo [Crear un proceso de aprobación para los elementos de trabajo](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   >
   >Después de adjuntar el proceso de aprobación de un solo uso, se muestra como &quot;`<Custom>`&quot; en el campo Proceso de aprobación dentro del cuadro Editar de plantillas y tareas de plantilla. Para obtener información sobre la edición de plantillas o tareas de plantilla, consulte los siguientes artículos:
   >
   >* [Editar plantillas de proyecto](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   >* [Editar una tarea de plantilla](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)

   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## Quitar o eliminar un proceso de aprobación de un elemento de trabajo

Puede quitar un proceso de aprobación global o de nivel de grupo, o bien eliminar un proceso de aprobación de un solo uso de un proyecto, tarea o problema asociado anteriormente a él.

Se dan los siguientes escenarios: 

* Al eliminar el proceso de aprobación global o de nivel de grupo, no se elimina la aprobación. La aprobación permanece disponible para uso futuro.
* Al eliminar un proceso de aprobación de un solo usuario, se elimina de Workfront y no se puede recuperar.

Para quitar o eliminar un proceso de aprobación de un elemento de trabajo:

1. Vaya al proyecto, tarea, problema, plantilla o tarea de plantilla en el que desea eliminar un proceso de aprobación que haya añadido anteriormente.
1. Haga clic en **Aprobaciones** en el panel izquierdo.

   ![Sección de aprobaciones en la tarea](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Haga clic en uno de los siguientes iconos en la esquina superior derecha de la sección Aprobaciones, según el tipo de aprobación asociado con el elemento:

   * **El icono Remove** icon ![Remove icon](assets/remove-icon---x-in-circle.png) para las aprobaciones globales o de nivel de grupo.
   * **El icono Eliminar** Icono ![Eliminar icono](assets/delete.png) para aprobaciones de un solo uso.

1. Haga clic en **Eliminar** o **Eliminar** para confirmar.

   El proceso de aprobación se quita del elemento de trabajo.

## Asociar automáticamente un proceso de aprobación con elementos de trabajo

Puede asociar automáticamente un proceso de aprobación con elementos de trabajo mediante los siguientes flujos de trabajo:

* Para los proyectos y las tareas, puede asociar un proceso de aprobación mediante una plantilla. Puede adjuntar un proceso de aprobación existente a la pestaña Aprobaciones de plantilla o Aprobaciones de tarea de plantilla. Para obtener información acerca de cómo asociar una aprobación existente con un elemento de trabajo, consulte [Asociar un proceso de aprobación global con un elemento de trabajo](#associate-a-global-approval-process-with-a-work-item) en este artículo.
* Para las tareas nuevas de un proyecto existente, puede asociar un proceso de aprobación global o un proceso de aprobación global de nivel de grupo en el área Configuración de tarea del cuadro Editar proyecto. Para obtener más información, consulte la sección “Configuración de tareas” en el artículo [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).
* En el caso de los problemas, puede asociar una aprobación a cada problema nuevo que se añada a un proyecto asociando un proceso de aprobación existente con una cola de solicitudes. Para obtener información acerca de cómo configurar colas de solicitudes, consulte [Crear una cola de solicitudes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
