---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Creación de tareas personales
description: Las tareas personales son solicitudes de trabajo ad hoc que se envían a un usuario, a sí mismo o elementos pendientes que crea para sí mismo en el área de Inicio. Workfront guarda las solicitudes de trabajo ad hoc y las tareas pendientes como tareas personales.
author: Becky
feature: Get Started with Workfront
exl-id: b40d6b10-19c7-4e11-a74f-a8af3ebafb65
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 5%

---

# Crear tareas personales

<!--Audited: 10/2024-->

Las tareas personales son solicitudes de trabajo ad hoc que se envían a un usuario o que se agregan o se envían por sí mismos.

Adobe Workfront guarda las solicitudes de trabajo ad hoc y las tareas pendientes como tareas personales en un proyecto personal del usuario que Wprfront crea automáticamente para cada usuario.

Las siguientes son características del proyecto personal de un usuario:

* Todos los usuarios de Workfront tienen un proyecto personal llamado &quot;Tareas de &lt; nombre completo del usuario>&quot;. Por ejemplo, &quot;Tareas de John Smith&quot;.
* El proyecto personal de cada usuario no se muestra en las búsquedas y está oculto.
* Un proyecto personal no se puede eliminar aunque se hayan desactivado los usuarios.
* El estado de un proyecto personal siempre es Actual. Los proyectos personales no se pueden completar ni cancelar.
* Todas las tareas personales se almacenan en el proyecto personal del usuario.
* Si es necesario, puede mover tareas personales a otro proyecto.

Puede crear tareas personales de las siguientes maneras:

* Crear un elemento pendiente en el área de Inicio

  Para obtener más información, vea [Crear elementos de trabajo y proyectos desde el área de inicio](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Crear y enviar una solicitud de trabajo personal a otro usuario desde la página de perfil de usuario
* Cree y envíe una solicitud de trabajo personal a usted mismo desde la página de perfil de usuario

Este artículo describe cómo crear una solicitud de trabajo personal para un usuario o para usted mismo desde la página de perfil de usuario.

Independientemente de cómo agregue una tarea personal, puede encontrarla en las mismas áreas de Workfront. Para obtener más información, consulte la sección [Buscar tarea personal](#locate-personal-tasks) en este artículo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>paquete de Adobe Workfront</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront</strong></td> 
   <td> 
   <p>Estándar<p>
   <p>Plan</p>
   <p>Esta es la licencia necesaria para enviar solicitudes a otros usuarios. Todos los usuarios pueden crear una solicitud de trabajo por sí mismos.</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>Edite el acceso a los usuarios para crear una solicitud de trabajo para ellos. Ver el acceso para crear una solicitud de trabajo personal para usted. </p>
   </td> 
  </tr>

</tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> 
   <p>New: Standard to send requests to other users. All users can create a work request for themselves.</p> 
   <p>Current: Plan to send requests to other users. All users can create a work request for themselves.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>Edit access to Users to create a work request for them. View access to create a personal work request for yourself. </p>
   </td> 
  </tr> 
 
 </tbody> 
</table>-->


## Crear una solicitud de trabajo personal

1. Vaya a la página de perfil del usuario o a la página de perfil de otro usuario que tenga acceso para ver.

   >[!TIP]
   >
   >Es posible que el administrador de Workfront le impida ver a determinados usuarios cuando configuren su nivel de acceso.

1. Haga clic en el **menú Más** ![](assets/more-menu.png) que se encuentra a la derecha del nombre del usuario en el encabezado.
1. Haga clic en **Enviar solicitud de trabajo**.
Aparece el cuadro **Enviar al usuario una solicitud de trabajo**.

   ![](assets/personal-task-box.png)
1. Actualice la siguiente información:

   * **Nombre de tarea**: Este es el nombre de la solicitud de trabajo ad hoc para la tarea personal.
   * **Descripción**: agregue una descripción para la tarea.
   * **Asignar a**: el nombre del usuario seleccionado se muestra de forma predeterminada. Puede agregar más usuarios o equipos.
   * **Fecha de vencimiento**: Es la fecha en la que desea completar esta tarea. De forma predeterminada, es la fecha de hoy. No se puede seleccionar una fecha del pasado
   * **Hora**: Este es el tiempo en que desea que se complete esta tarea. De forma predeterminada, es la hora actual.

1. Haga clic en **Enviar solicitud** para guardar la solicitud de trabajo.

   La solicitud de trabajo se guarda como una tarea personal en Workfront y se agrega al widget Tareas pendientes del usuario en el área de Inicio. Si se envía la solicitud de trabajo a sí mismo, se mostrará en el widget Tareas pendientes en Inicio.


## Localizar tareas personales

Puede localizar tareas personales en las siguientes áreas:

* El widget Tareas pendientes en el área de Inicio del usuario al que se envió la solicitud personal.

  Para obtener más información, vea [Crear elementos de trabajo y proyectos desde el área de inicio](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Informe o lista de tareas personales. Puede generar y aplicar un filtro de tareas personales a un informe o lista de tareas para mostrar solo las tareas personales y excluir las tareas de proyecto.

  Para obtener más información, vea [Filtro: tareas personales](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md).
