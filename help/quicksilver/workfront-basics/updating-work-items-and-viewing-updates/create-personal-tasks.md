---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Crear tareas personales
description: Las tareas personales son anuncios solicitudes de trabajo hoc que envía a un usuario, a usted mismo o a los elementos de tareas que crea para usted en el área de su hogar. Workfront ahorra solicitudes de trabajo anuncios hoc y tareas como tareas personales.
author: Lisa
feature: Get Started with Workfront
exl-id: b40d6b10-19c7-4e11-a74f-a8af3ebafb65
source-git-commit: a1081b7ce0877b08f9546ab57cfac3f2a580ea76
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 7%

---

# Crear tareas personales

<!--Audited: 10/2024-->

Las tareas personales son anuncios solicitudes de trabajo hoc que envía a un usuario o envía o agrega para usted.

Adobe Systems Workfront guarda solicitudes de trabajo anuncios hoc y hace elementos como tareas personales en el proyecto personal de un usuario que Wprfront crea automáticamente para cada usuario.

Las siguientes son características del proyecto personal de un usuario:

* Todos los usuarios de Workfront tienen un proyecto personal denominado &quot;&lt; User&#39;s full name>&#39;s Tasks&quot;. Por ejemplo, &quot;Las tareas de John Smith&quot;.
* El proyecto personal de cada usuario no se muestra en las búsquedas y es oculta.
* Un proyecto personal no se puede eliminar, igualado si se han desactivado los usuarios.
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

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plan de Adobe Workfront</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> 
   <p>Nuevo: Estándar para enviar solicitudes a otros usuarios. Todos los usuarios pueden crear una solicitud de trabajo por sí mismos.</p> 
   <p>Actual: plan para enviar solicitudes a otros usuarios. Todos los usuarios pueden crear una solicitud de trabajo por sí mismos.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>Editar acceso a los Usuarios para crear una solicitud de trabajo para ellos. Ver acceso para crear un solicitud de trabajo personal para usted. </p>
   </td> 
  </tr>

</tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Crear una solicitud de trabajo personal

1. Vaya a la página de perfil del usuario o a la página de perfil de otro usuario que tenga acceso para ver.

   >[!TIP]
   >
   >Es posible que el administrador de Workfront le impida ver a determinados usuarios cuando configuren su nivel de acceso.

1. Haga clic en el **menú Más** ![](assets/more-menu.png) que se encuentra a la derecha del nombre del usuario en el encabezado.
1. Haga clic en **Enviar solicitud de trabajo**.
Se muestra el **cuadro Enviar usuario una solicitud** de trabajo.

   ![](assets/personal-task-box.png)
1. Actualice la siguiente información:

   * **Nombre de tarea**: Este es el nombre de la solicitud de trabajo ad hoc para la tarea personal.
   * **Descripción**: agregue una descripción para la tarea.
   * **Asignar a**: el nombre del usuario seleccionado se muestra de forma predeterminada. Puede agregar más usuarios o equipos.
   * **Fecha** de vencimiento: Esta es la fecha en la que gustar que se completara este tarea. De forma predeterminada, es la fecha de hoy. No se puede seleccionar una fecha que ya haya pasado
   * **Tiempo**: Este es el tiempo en el que gustar que se completara este tarea. De forma predeterminada, es la hora actual.

1. Haga clic en **Enviar solicitud** para guardar el trabajo solicitud.

   El solicitud trabajo se guarda como un tarea personal en Workfront y se agrega al widget de tareas pendientes del usuario en su área Inicio. Si te envías el solicitud de trabajo a ti mismo, se muestra en el widget Tareas pendientes de Inicio.


## Localizar tareas personales

Puede localizar tareas personales en las siguientes áreas:

* El widget Tareas pendientes en el área de Inicio del usuario al que se envió la solicitud personal.

  Para obtener más información, vea [Crear elementos de trabajo y proyectos desde el área de inicio](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Informe o lista de tareas personales. Puede generar y aplicar un filtro de tareas personales a un informe o lista de tareas para mostrar solo las tareas personales y excluir las tareas de proyecto.

  Para obtener más información, vea [Filtro: tareas personales](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md).
