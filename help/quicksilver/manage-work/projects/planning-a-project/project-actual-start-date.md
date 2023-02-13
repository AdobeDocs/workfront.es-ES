---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Descripción general de la fecha de inicio real del proyecto
description: Los proyectos, las tareas y los problemas tienen una Fecha de inicio real en Adobe Workfront. Para las tareas y los problemas, esta es la fecha en la que se han marcado como En curso. Para los proyectos, esta es la fecha en la que la primera tarea del proyecto se marca como En curso o se ha completado.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Descripción general de la fecha de inicio real del proyecto

Los proyectos, las tareas y los problemas tienen una Fecha de inicio real en Adobe Workfront. Para las tareas y los problemas, esta es la fecha en la que se han marcado como En curso. Para los proyectos, esta es la fecha en la que la primera tarea del proyecto se marca como En curso o se ha completado.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver o acceder más a Proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores de un proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones sobre las fechas de inicio reales en Workfront

* La fecha de inicio real se encuentra en la sección Detalles de proyectos, tareas y problemas. 
* La fecha de inicio real de un proyecto, tarea o problema no se rellena cuando se crean estos elementos.
* La fecha de inicio real se rellena cuando se inicia el trabajo en el proyecto, la tarea o el problema.
* La fecha de inicio real no se muestra en la ficha Detalles del proyecto si el trabajo del proyecto aún no se ha iniciado.

   La Fecha de inicio real aparece en blanco en las pestañas Tarea y Detalles del problema si el trabajo aún no se ha iniciado en ellas.

* Puede modificar manualmente la fecha de inicio real de una tarea o un problema, pero no puede modificar la fecha de inicio real de un proyecto.

## Consideraciones sobre las fechas de inicio reales para los proyectos

* Workfront establece automáticamente la fecha real de un proyecto cuando se produce cualquiera de las siguientes situaciones:

   * Un usuario asignado de tareas cambia el estado de una tarea de *Nuevo* a cualquier otro estado que no sea igual a *Nuevo*.

   * El usuario asignado cambia el porcentaje de finalización de una tarea.

      >[!IMPORTANT]
      >
      >La fecha de inicio real del proyecto no se rellena cuando el proyecto está marcado como Actual. El trabajo real debe comenzar en las tareas del proyecto antes de que se complete la Fecha de inicio real del proyecto.

      En estos casos, la Fecha de inicio real del proyecto se establece en la fecha y hora en que se produjeron estas acciones para la tarea más temprana del proyecto. Esto indica que el proyecto se inició realmente en esta fecha y hora.

## Localizar la fecha de inicio real de un proyecto

Puede localizar la fecha de inicio real de un proyecto en las siguientes áreas:

* En la sección Detalles de un proyecto.
* En un informe o vista de proyecto, cuando se agrega la Fecha de inicio real para el objeto Proyecto en el informe.

   Para obtener información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para localizar la fecha de inicio real en la sección Detalles del proyecto:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Proyectos**.
1. Haga clic en el proyecto para el que desee ver la fecha de inicio real.
1. Haga clic en **Detalles del proyecto** en el panel izquierdo y, a continuación, vaya a la **Información general** para obtener más información.

   La Fecha de inicio real se muestra junto con otras fechas del proyecto .

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
