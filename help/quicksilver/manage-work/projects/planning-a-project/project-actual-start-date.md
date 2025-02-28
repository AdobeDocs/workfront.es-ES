---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Información general sobre la fecha real de inicio del proyecto
description: Los proyectos, las tareas y los problemas tienen una fecha de inicio real en Adobe Workfront. En el caso de las tareas y los problemas, es la fecha en la que se han marcado como En curso. En el caso de los proyectos, es la fecha en la que la primera tarea del proyecto se marca como En curso o que se ha completado.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 97%

---

# Información general sobre la fecha real de inicio del proyecto

Los proyectos, las tareas y los problemas tienen una fecha de inicio real en Adobe Workfront. En el caso de las tareas y los problemas, es la fecha en la que se han marcado como En curso. En el caso de los proyectos, es la fecha en la que la primera tarea del proyecto se marca como En curso o que se ha completado.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisión o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de visualización o superior a los proyectos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos Ver o superiores para un proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones sobre las fechas de inicio reales en Workfront

* La fecha de inicio real se encuentra en la sección Detalles de proyectos, tareas y problemas. 
* La fecha de inicio real de un proyecto, tarea o problema no se rellena al crear estos elementos.
* La fecha de inicio real se rellena cuando el trabajo comienza realmente en el proyecto, la tarea o el problema.
* La fecha de inicio real no aparece en la pestaña Detalles del proyecto si el trabajo en el proyecto aún no ha comenzado.

  La fecha de inicio real se muestra en blanco en las pestañas Detalles de tarea y Detalles del problema si el trabajo aún no ha comenzado en ellas.

* Puede modificar manualmente la fecha de inicio real de una tarea o un problema, pero no puede modificar la fecha de inicio real de un proyecto.

## Consideraciones sobre las fechas de inicio reales de los proyectos

* Workfront establece automáticamente la fecha real de un proyecto cuando se produce cualquiera de las siguientes situaciones:

   * Una persona asignada a una tarea cambia el estado de una tarea de *Nuevo* a cualquier otro estado que no sea igual a *Nuevo*.

   * Una persona asignada a una tarea cambia el porcentaje completado de una tarea.

     >[!IMPORTANT]
     >
     >La fecha de inicio real del proyecto no se completa cuando el proyecto se marca como Actual.El trabajo real debe comenzar en las tareas del proyecto antes de que se rellene la fecha de inicio real del proyecto.

     En estos casos, la fecha de inicio real del proyecto se establece en la fecha y la hora en que se produjeron estas acciones para la primera tarea del proyecto. Esto indica que el proyecto comenzó realmente en esta fecha y a esta hora.

## Localización de la fecha de inicio real de un proyecto

Puede localizar la fecha de inicio real de un proyecto en las áreas siguientes:

* En la sección Detalles de un proyecto.
* En un informe o vista de proyecto, cuando se añade la fecha de inicio real del objeto Proyecto en el informe.

  Para obtener información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para localizar la fecha de inicio real en la sección Detalles del proyecto:

1. Haga clic en el icono **Menú principal** ![Menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Workfront y, a continuación, haga clic en **Proyectos**.
1. Haga clic en el proyecto cuya fecha de inicio real desea ver.
1. Haga clic en **Detalles del proyecto** en el panel izquierdo y, a continuación, vaya a la sección **Información general**.

   La fecha de inicio real se muestra junto con otras fechas del proyecto.

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
