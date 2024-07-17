---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Descripción general de la fecha real de inicio del proyecto
description: Los proyectos, las tareas y los problemas tienen una fecha de inicio real en Adobe Workfront. Para las tareas y problemas, esta es la fecha en la que se han marcado como En curso. En los proyectos, esta es la fecha en la que se marca la primera tarea del proyecto como En curso o se ha completado.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Descripción general de la fecha real de inicio del proyecto

Los proyectos, las tareas y los problemas tienen una fecha de inicio real en Adobe Workfront. Para las tareas y problemas, esta es la fecha en la que se han marcado como En curso. En los proyectos, esta es la fecha en la que se marca la primera tarea del proyecto como En curso o se ha completado.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de visualización o superior a Proyectos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos superiores a un proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones sobre las fechas de inicio reales en Workfront

* La fecha de inicio real se encuentra en la sección Detalles de proyectos, tareas y problemas. 
* La fecha real de inicio de un proyecto, tarea o problema no se rellena al crear estos elementos.
* La fecha real de inicio se rellena cuando el trabajo comienza realmente en el proyecto, tarea o problema.
* La Fecha real de inicio no aparece en la ficha Detalles del proyecto si el trabajo en el proyecto aún no ha comenzado.

  La Fecha real de inicio se muestra en blanco en las fichas Detalles de tarea y Detalles del problema si el trabajo aún no ha comenzado en ellas.

* Puede modificar manualmente la fecha de inicio real de una tarea o un problema, pero no puede modificar la fecha de inicio real de un proyecto.

## Consideraciones sobre las fechas de inicio reales de los proyectos

* Workfront establece automáticamente la fecha real de un proyecto cuando se produce cualquiera de las siguientes situaciones:

   * Un usuario asignado a una tarea cambia el estado de una tarea de *Nuevo* a cualquier otro estado que no sea igual a *Nuevo*.

   * Un usuario asignado a una tarea cambia el porcentaje completado de una tarea.

     >[!IMPORTANT]
     >
     >La fecha real de inicio del proyecto no se completa cuando el proyecto se marca como Actual. El trabajo real debe comenzar en las tareas del proyecto antes de que se rellene la Fecha real de inicio del proyecto.

     En estos casos, la fecha real de inicio del proyecto se establece en la fecha y hora en que se produjeron estas acciones para la primera tarea del proyecto. Esto indica que el proyecto comenzó realmente en esta fecha y hora.

## Buscar la fecha real de inicio de un proyecto

Puede localizar la fecha real de inicio de un proyecto en las áreas siguientes:

* En la sección Detalles de un proyecto.
* En un informe o vista de proyecto, cuando se agrega la fecha de inicio real del objeto Proyecto en el informe.

  Para obtener información sobre cómo crear informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para localizar la fecha de inicio real en la sección Detalles del proyecto:

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront y luego haga clic en **Proyectos**.
1. Haga clic en el proyecto cuya fecha real de inicio desee ver.
1. Haga clic en **Detalles del proyecto** en el panel izquierdo y, a continuación, vaya a la sección **Información general**.

   La Fecha real de inicio se muestra junto con otras fechas del proyecto

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
