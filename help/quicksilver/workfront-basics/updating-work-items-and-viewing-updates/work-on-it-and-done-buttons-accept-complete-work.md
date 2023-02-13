---
content-type: o
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Información general sobre el botón Trabajar en él y Hecho
description: Cuando se le asigna una tarea o un problema, puede utilizar un botón contextual que cambie los nombres y las funciones en función de su participación en el elemento de trabajo.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: cfda6702-1a9a-4645-b031-8b2f201ac0af
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 0%

---

# Información general sobre el botón Trabajar en él y Hecho

Cuando se le asigna una tarea o un problema, puede utilizar un botón contextual que cambie los nombres y las funciones en función de su participación en el elemento de trabajo.

Con el botón contextual para aceptar o completar elementos de trabajo, puede dejar que Adobe Workfront actualice varios campos de los elementos sin tener que actualizarlos manualmente.

## Trabaje en él y haga clic en los nombres de botón Listo

En función del área de Workfront desde la que acceda a su tarea o problema, el botón Trabajar en ella o Hecho puede cambiar los nombres, como se describe en los siguientes casos: 

* Cuando la tarea o el problema se le asigna por primera vez y el estado es Nuevo, el botón aparece como Trabajar en él.

   ![](assets/nwe-work-on-it-button.png)

   >[!TIP]
   >
   >Puede reemplazar el botón Trabajar en él con un botón Inicio . Para obtener información sobre cómo reemplazar el botón Trabajar en él por un botón Inicio, consulte  [Reemplazar el botón Trabajar en él con un botón Inicio](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md) .

* Después de hacer clic en Trabajar en él para aceptar, el botón cambia a Marcar como hecho o Hecho , según desde dónde acceda a la tarea o el problema en Workfront. Para obtener información sobre dónde puede acceder al botón Trabajar en él, consulte la sección [Busque el botón Trabajar en él y Hecho .](#locate-the-work-on-it-and-done-button) en este artículo.

   ![](assets/nwe-mark-as-done-button-350x122.png)

* Si no es el único asignado a la tarea o al problema y accede al elemento de trabajo desde la lista de trabajos del área principal, el botón cambia a Hecho con mi parte.

   ![](assets/home-left-done-with-my-part-button-350x184.png)

## Busque el botón Trabajar en él y Hecho . {#locate-the-work-on-it-and-done-button}

Puede localizar el botón Trabajar en él y Hecho en las siguientes áreas de Workfront:

* El área principal, tanto en la lista de trabajo como en el panel de detalles

   Para obtener información sobre cómo marcar un elemento como Hecho en el área principal, consulte [Marcar un elemento como Hecho en el área de inicio](../../workfront-basics/using-home/using-the-home-area/mark-item-done-in-home.md).

* En el encabezado de la tarea o problema

   Para obtener información sobre los encabezados de objeto, consulte [Nuevos encabezados de objeto](../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

* En el panel Resumen de tarea o problema de una lista o en el equilibrador de carga de trabajo

   Para obtener información sobre el uso del panel Resumen, consulte [Resumen](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

## Información general de los campos que se actualizan automáticamente al hacer clic en el botón Trabajar en él y Hecho

La ventaja de utilizar los botones Trabajar en él y Hecho es que puede permitir que Workfront actualice automáticamente la información sobre el elemento de trabajo asignado a usted.

* [Botón Trabajar en él](#work-on-it-button)
* [Botón Inicio](#start-button)
* [Botón Listo](#the-done-button)

### Botón Trabajar en él {#work-on-it-button}

Al hacer clic en Trabajar en él, también se actualizan los siguientes elementos:

* Actualizaciones del estado de asignación de Solicitado a Trabajo

   >[!TIP]
   >
   >El campo Estado de asignación solo está visible en informes y listas. Para obtener información sobre el campo Estado de asignación , consulte la [Glosario de terminología de Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Fecha de confirmación

   Para obtener información sobre la fecha de confirmación, consulte [Resumen de la fecha de confirmación](../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

### Botón Inicio {#start-button}

Si tiene acceso para editar equipos, puede reemplazar el botón Trabajar en él con un botón Iniciar para un equipo. Cuando los usuarios con ese equipo como su equipo de origen hacen clic en el botón Inicio de los elementos asignados, los campos adicionales de sus elementos de trabajo se actualizan automáticamente. Para obtener información sobre cómo reemplazar el botón Trabajar en él por un botón Inicio, consulte [Reemplazar el botón Trabajar en él con un botón Inicio](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Además de los campos que se actualizan al hacer clic en el botón Trabajar en él , los siguientes campos se actualizan automáticamente en una tarea o problema al hacer clic en el botón Inicio :

* Estado
* Fecha de inicio real

   Para obtener información sobre la fecha de inicio real, consulte [Descripción general de la fecha de inicio real del proyecto](../../manage-work/projects/planning-a-project/project-actual-start-date.md).

* Fecha de finalización real si el botón Inicio está asociado con un estado igual a Complete o Closed.

   Para obtener información sobre la fecha de finalización real, consulte [Descripción general de la fecha de finalización real del proyecto](../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

>[!NOTE]
>
>Al hacer clic en el botón Deshacer se devuelve el elemento de trabajo al estado original y se elimina la Fecha de inicio real.
>
>El botón Deshacer no está disponible en las siguientes áreas:
>
>* Solicitudes de equipo
>* Encabezado de tarea
>


### Botón Listo {#the-done-button}

Si tiene acceso para editar equipos, puede configurar el botón Listo para que un equipo actualice los estados de la tarea o del problema cuando marque un elemento como completado. Cuando los usuarios con ese equipo como su equipo principal hagan clic en el botón Listo de sus elementos, los siguientes campos se actualizarán automáticamente en una tarea o problema:

* Estado
* Actualizaciones del estado de asignación de Trabajo a Hecho
* Fecha de finalización real

Para obtener información sobre la configuración del botón Listo para un equipo, consulte los siguientes artículos:

* [Configuración del botón Listo para tareas](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
* [Configuración del botón Listo para problemas](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)
