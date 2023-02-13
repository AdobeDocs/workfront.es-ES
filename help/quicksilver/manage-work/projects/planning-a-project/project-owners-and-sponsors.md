---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: Descripción general de los propietarios y patrocinadores del proyecto
description: Puede designar un propietario del proyecto y un patrocinador del proyecto para un proyecto.
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Descripción general de los propietarios y patrocinadores del proyecto

Puede designar un propietario del proyecto y un patrocinador del proyecto para un proyecto.

El propietario del proyecto es la persona responsable de la finalización del proyecto a tiempo y con cargo al presupuesto.

El Patrocinador del Proyecto es una parte importante del proyecto que tiene recursos invertidos en él. La finalización del proyecto suele beneficiar al patrocinador del proyecto.

Para obtener información sobre cómo actualizar el propietario o el patrocinador del proyecto de un proyecto, consulte [Actualizar propietarios y patrocinadores de proyectos](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## Propietarios de proyectos

Puede designar el administrador de un proyecto especificando un Propietario del proyecto en un proyecto o una plantilla.

Solo puede definir un propietario del proyecto para un proyecto.

Las siguientes opciones son posibles mediante el campo Propietario del proyecto :

* Solo puede designar un usuario como Propietario del proyecto.
* Puede designar Propietarios del proyecto como aprobadores de horas para el proyecto.
* Puede designar al propietario del proyecto como aprobador genérico al definir procesos de aprobación de proyectos, tareas o problemas. Para obtener información sobre las aprobaciones, consulte [Editar un proceso de aprobación](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >Cuando se asigna una aprobación al propietario del proyecto y no se designa a nadie como propietario de un proyecto, la aprobación se reasigna al administrador principal de Workfront, tal como se indica en la sección Información del cliente del área Configuración . Para obtener más información, consulte [Configurar información básica para el sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).


* Puede activar ciertas notificaciones que se entregan únicamente al propietario del proyecto.

   Para obtener más información sobre las notificaciones por correo electrónico, consulte la sección [Configurar notificaciones de eventos para todos los miembros del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) en el artículo [Configurar notificaciones de eventos para todos los miembros del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Puede mostrar el campo Propietario del proyecto en un informe o una lista.

   También puede mostrar el campo Propietario del proyecto en una vista, agrupación o solicitud.

   Por ejemplo, puede copiar la siguiente expresión de modo de texto en un filtro para mostrar los proyectos que sean propiedad del usuario que ha iniciado sesión: 

   ```
   ownerID=$$USER.ID
   ```

Para obtener más información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE:&nbsp;drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Patrocinadores de proyectos

Puede designar cualquier usuario del sistema como patrocinador del proyecto. El patrocinador del proyecto es normalmente un administrador, ejecutivo o parte interesada que necesita saber qué está pasando con el proyecto.

Tenga en cuenta lo siguiente al asignar un patrocinador de proyecto:

* El patrocinador del proyecto no obtiene acceso adicional al proyecto, pero se añade a las notificaciones por correo electrónico del proyecto. Para obtener información sobre las notificaciones, consulte el artículo [Configurar notificaciones de eventos para todos los miembros del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Solo puede designar un patrocinador de proyecto.
* Puede designar el Patrocinador del proyecto como aprobador genérico al definir los procesos de aprobación de proyectos, tareas o problemas. Para obtener información sobre las aprobaciones, consulte [Editar un proceso de aprobación](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >Cuando se asigna una aprobación al Patrocinador del proyecto y no se designa a nadie como patrocinador de un proyecto, la aprobación se reasigna al Propietario del proyecto. Si no se designa a nadie como propietario del proyecto, la aprobación se asigna al administrador de Workfront.

* Puede mostrar el campo Patrocinador del proyecto en un informe o una lista.

   También puede mostrar el campo Patrocinador del proyecto en una vista, agrupación o solicitud.

   Por ejemplo, puede copiar la siguiente expresión de modo de texto en un filtro para mostrar los proyectos patrocinados por el usuario que ha iniciado sesión:

   ```
   sponsorID=$$USER.ID
   ```

    

   Para obtener más información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->
