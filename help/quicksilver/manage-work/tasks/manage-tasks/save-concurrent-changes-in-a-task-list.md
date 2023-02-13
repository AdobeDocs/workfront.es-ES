---
product-area: projects
navigation-topic: manage-tasks
title: Información general sobre cómo guardar cambios simultáneos en una lista de tareas
description: Al editar tareas en una lista, puede utilizar la configuración de guardado independiente para indicar si desea que los cambios se guarden automáticamente en forma manual al editar tareas en una lista.
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Información general sobre cómo guardar cambios simultáneos en una lista de tareas

Al editar tareas en una lista, puede utilizar la configuración de guardado independiente para indicar si desea que los cambios se guarden automáticamente en forma manual al editar tareas en una lista.

Para obtener información sobre la edición de tareas en una lista de tareas, consulte el artículo [Editar tareas en una lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

A veces, pueden aparecer conflictos si dos usuarios realizan cambios en las mismas tareas.

Tenga en cuenta lo siguiente al editar tareas en una lista de tareas:

* Adobe Workfront guarda los cambios realizados en las tareas inmediatamente cuando selecciona guardar los cambios automáticamente si el tipo de actualización del proyecto es automático o automático o si está activado. Para obtener información sobre el tipo de actualización del proyecto, consulte [Seleccione el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
* Workfront actualiza la información de la lista en la que está trabajando cada minuto con los cambios que otros usuarios podrían realizar en cualquier otro lugar del sistema. Esto garantiza que siempre obtenga la información más reciente sobre las tareas.

Los siguientes escenarios existen cuando varios usuarios están editando las mismas tareas:

* **Un usuario guarda automáticamente los cambios en una lista de tareas y otro manualmente**: Si un usuario (usuario A) guarda los cambios manualmente mientras el usuario B edita las mismas tareas pero guarda sus cambios automáticamente, los cambios realizados por el usuario B se actualizan en la lista para el usuario A cada minuto. Si hay conflictos entre los cambios realizados por los dos usuarios, el usuario que guarda manualmente (usuario A) verá un mensaje de advertencia antes de poder guardar sus cambios. El mensaje de advertencia muestra los elementos que tienen los cambios conflictivos. En este momento, el usuario A puede elegir si debe conservar los cambios (que sobrescriben los cambios realizados por el usuario B) o descartarlos (que mantiene los cambios realizados por el usuario B).

>[!NOTE]
>
>Cuando selecciona descartar los cambios realizados, esto se aplica a todos los cambios y no solo a aquellos que tienen conflictos con las ediciones realizadas por otro usuario.

* **Varios usuarios guardan manualmente los cambios en una lista de tareas**: Si varios usuarios que realizan cambios en las tareas de una lista se guardan manualmente al mismo tiempo, Workfront guarda los cambios realizados por el usuario que guarda primero. Guardar estos cambios no debería encontrar ningún conflicto. Workfrontthen compara los cambios realizados por todos los demás usuarios con la información que ya ha guardado y muestra una advertencia a los demás usuarios sobre los cambios conflictivos antes de que puedan guardar su información.

>[!IMPORTANT]
>
>Cuando selecciona conservar los cambios sobre todos los demás cambios, se guardan todos los cambios, a menos que otro usuario elimine las tareas a las que realizó cambios. En este caso, el mensaje de advertencia le informa de que se pierden los cambios realizados en las tareas eliminadas.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - when replaced with the above live section; does it need an edit??) </p>
<div>
<p>When editing tasks in a list, you can select whether you want each change to be saved automatically or if you want to manually save multiple changes at one time by clicking the Save button. This depends on whether you enable the Autosave setting in the task list or not. </p>
<p>For information about editing tasks in a task list, see the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref" xrefformat="{para}">Edit tasks</a>. </p>
<p>Sometimes, conflicts might appear if two users are making changes on the same tasks. </p>
<p>Consider the following when editing tasks in a task list: </p>
<ul>
<li>Workfront saves the changes you make to tasks immediately when you have enabled the Autosave setting. </li>
<li>Workfront updates the information on the list you are working on every minute with changes that other users might make anywhere else in the system. This ensures that you always get the latest information on the tasks. </li>
</ul>
<p>The following scenarios exist when multiple users are editing the same tasks:</p>
<ul>
<li>One user has Autosave disabled and another has it enabled: If a user (User A) has disabled the Autosave setting and is editing the task list while User B is editing the same tasks but they have enabled the Autosave setting, the live changes made by User B are updated on the list for User A every minute. If there are conflicts between the changes made by the two users, the user with the Autosave setting disabled (User A) sees a warning message before they can save their changes, that shows the items that have those conflicting changes. At this time, User A can choose whether they should keep their changes (which overwrites the changes made by User B), or discard them (which keeps the changes made by User B.) </li>
</ul> <note type="note">
When you select to discard the changes you made, this applies to all the changes and not just to those that have conflicts with the edits made by another user.
</note>
<ul>
<li>Several users have disabled the Autosave setting: If several users that have disabled the Autosave setting are making changes at the same time, Workfront saves the changes made by the user who saves first. Saving these changes should not encounter any conflicts. Workfrontthen compares the changes made by all the other users with the information that it already saved and displays a warning about the conflicting changes to the other users before they can save their information. </li>
</ul> <note type="important">
When you select to keep your changes over all other changes, your changes are saved, unless the tasks you made changes to were deleted by another user. In this case, the warning message informs you that the changes you made to the deleted tasks are lost.
</note>
</div>
</div>
-->
