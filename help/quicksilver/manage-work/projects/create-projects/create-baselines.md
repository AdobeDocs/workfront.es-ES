---
product-area: projects
navigation-topic: create-projects
title: Crear líneas base del proyecto
description: Una línea de base es una instantánea del proyecto que representa información clave incluida en el plan inicial del proyecto o en cualquier momento dado durante la duración del proyecto.
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Crear líneas base del proyecto

<!-- Audited: 12/2023 -->

Una línea de base es una instantánea del proyecto que representa información clave incluida en el plan inicial del proyecto o en cualquier momento dado durante la duración del proyecto.

Puede utilizar la línea de base para comparar la información del plan actual con el plan original o con cualquier otro momento, para identificar las tareas problemáticas, la evolución del ámbito y otras tendencias en el tiempo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<!--
drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
    <td><p>Nuevo: estándar</p>
        <p>o</p>
        <p>Actual: plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso</td> 
   <td> <p>Editar acceso a Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos del proyecto o superior para ver líneas de base</p> <p>Administrar permisos del proyecto para crear líneas de base</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones para trabajar con líneas de base

* Puede capturar una instantánea del progreso de un proyecto varias veces durante su duración y crear varias líneas de base.
* Puede ver la información incluida en las líneas de base de un proyecto creando una línea de base o un informe de Línea de base.
* Cuando se crea una línea de base, la información de la tarea también se captura en las tareas de línea de base de esa línea de base.
* Puede ver la información de las tareas de línea de base creando un informe de Tarea de línea de base.

>[!IMPORTANT]
>
>Una línea base toma una instantánea del nombre, las fechas y la información financiera del proyecto. La línea de base no incluye los valores de los campos personalizados del proyecto. Para obtener información sobre la información financiera incluida en la línea de base, consulte [Finanzas del proyecto incluidas en las bases de referencia del proyecto](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Crear una línea base

Se puede crear una instantánea de las siguientes maneras:

* **Automáticamente**: el administrador de Workfront o de un grupo establece la preferencia de proyecto para que Workfront cree automáticamente una línea de base cuando un proyecto se convierta en Actual. Si se habilita esta configuración, se crea una línea de base cuando el estado del proyecto pasa a ser Actual. Cuando esta configuración no está habilitada, debe crear manualmente las líneas de base.

  Para obtener más información sobre la configuración de las preferencias del proyecto y la creación automática de líneas de base, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  >[!CAUTION]
  >
  >Al habilitar esta configuración, se crea automáticamente una línea de base para un proyecto cada vez que el estado de un proyecto cambia a Actual. La primera línea base creada es la predeterminada. Debe crear manualmente todas las demás líneas de base durante la duración del proyecto

* **Manualmente**: puede crear nuevas líneas de base para el proyecto según sea necesario a medida que avance el proyecto. A continuación, puede comparar las líneas de base para ver el progreso del proyecto a lo largo del tiempo.

Para crear una línea base:

1. Vaya a un proyecto.
1. En el panel izquierdo, haga clic en **Líneas bases**.

   O

   Clic **Mostrar más**, luego haga clic en **Líneas bases**.

   ![Sección de líneas de base del proyecto](assets/baselines-section-on-project-with-header.png)

1. Clic **Nueva línea base.**
1. Especifique el nombre de la instantánea.
1. (Opcional) Si esta es la primera línea de base, es posible que desee elegirla como predeterminada.
1. Haga clic en **Guardar**.

   De forma predeterminada, se muestra la siguiente información sobre la línea base creada:

   * Nombre de línea base
   * Fecha de entrada prevista
   * Fecha planificada de inicio del proyecto en la que se creó la línea base
   * Fecha proyectada de inicio del proyecto en que se creó la línea base
   * Duración real del proyecto cuando se creó la línea de base
   * % Finalizado del proyecto cuando se creó la línea base
   * Indicador de línea de base predeterminada que muestra si una línea de base es la línea de base predeterminada del proyecto

     >[!TIP]
     >
     >No se puede ver información de dos líneas base al mismo tiempo en la misma vista o informe. Sólo se puede ver información de una línea base determinada y de la línea base predeterminada en el mismo informe. Puede modificar la línea base que considere como predeterminada en cualquier momento durante la duración del proyecto.

1. (Opcional) Haga clic en **Ver** y, a continuación, cree una vista nueva o edite la vista actual para añadir campos a la vista y comparar información adicional entre líneas base. Para obtener más información, consulte [Creación o edición de vistas en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Crear un informe de Línea base o de Tarea de línea base

Para ver la información de línea de base, también puede crear un informe de línea de base o de tarea de línea de base. Esto le permite mostrar cualquier número de campos acerca de las líneas de base o tareas de línea de base para compararlos en una vista.

>[!TIP]
>
>Debe crear una línea base antes de crear un informe de Línea base o de Tarea de línea base.

Para obtener información sobre cómo crear un informe, consulte [Creación de un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Se recomienda agregar una agrupación Nombre del proyecto al informe Línea de base o Tarea de línea de base para facilitar la lectura.

Para obtener información sobre cómo crear una agrupación, consulte [Creación de agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).
