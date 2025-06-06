---
title: Crear una ruta de hitos
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Como administrador de Adobe Workfront, puede crear rutas de hitos que luego se pueden aplicar a cualquier proyecto del sistema. Los cambios que realice en las rutas de hitos en esta área afectarán a todo el sistema de Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: 6e2e337969fccba88ea7089fe9a6d9db605343f7
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 64%

---

# Crear ruta de hitos

<!--Audited: 07/2024-->

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Como administrador de Adobe Workfront, puede crear rutas de hitos que luego se pueden aplicar a cualquier proyecto del sistema. Los cambios que realice en las rutas de hitos en esta área afectarán a todo el sistema de Workfront.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Hitos y rutas de hitos

Puede asociar las tareas clave de un proyecto con hitos predefinidos. Esta función puede proporcionar a los administradores y otras partes interesadas información general de alto nivel sobre el progreso de un proyecto.

La suma de todos los hitos predefinidos se denomina ruta de hitos.

El primer paso para construir una ruta de hitos es identificar cuáles son los pasos del hito y establecer los hitos. Dado que puede asociar una ruta de hitos a varios proyectos, los pasos del hito deben ser fases o etapas generales de cualquier proyecto.

Para obtener más información sobre cómo asociar una ruta de hitos a un proyecto y un hito a una tarea, consulte [Asociar hitos con tareas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Crear ruta de hitos

{{step-1-to-setup}}

1. Haga clic en **Procesos** > **Rutas de hitos**.
1. Haga clic en **Nueva ruta de hitos.**
1. Especifique la siguiente información en el área **Información básica**:

   <table style="table-layout:auto">
    <tr>
      <td>Nombre de ruta de hitos</td>
       <td>Introduzca un nombre para la ruta de hitos.</td>
    </tr>
    <tr>
      <td>Descripción</td>
      <td>Introduzca una descripción para definir la ruta de hitos.</td>
    </tr>
    <tr>
       <td>Activo</td>
      <td>Seleccione esta casilla de verificación si desea que la ruta de hitos esté activa. Otros usuarios pueden encontrar esta ruta y adjuntarla a proyectos al crearlos o editarlos. Las rutas de hitos inactivas no se pueden adjuntar a los proyectos. Esta opción está activada de forma predeterminada.</td>
    </tr>
    <tr>
      <td>Grupos</td>
      <td>Seleccione los grupos enumerados para permitir a los usuarios de estos grupos ver y aplicar esta ruta de hitos a sus proyectos. El grupo de inicio del usuario que entra en la ruta de hitos se selecciona de forma predeterminada.</td>
    </tr>
   </table>

1. Especifique la siguiente información en el área **Hitos**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td>Escriba nombres descriptivos para cada hito.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba una descripción para el hito.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Color</td> 
      <td> <p>Elija un color que se asociará al hito. </p> <p>Si no se elige un color, el sistema elige el último color utilizado en una ruta de hitos. Le recomendamos que elija un color único para cada hito. El color se utiliza con fines visuales y de creación de informes.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Añadir hito** y continúe añadiendo hitos según sea necesario hasta que finalice la ruta.

1. Haga clic en **Crear ruta de hitos** para guardar los cambios.

   La ruta de hitos está lista para asociarse a un proyecto.

   Para obtener más información sobre cómo asociar rutas de hitos a proyectos e hitos a tareas, consulte [Asociar hitos a tareas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).


1. (Opcional) Haga clic en el icono **Exportar** ![Icono de exportar](assets/export-icon.png) y, a continuación, seleccione uno de los siguientes formatos para exportar la lista de rutas de hitos a un archivo:

   * PDF
   * Excel
   * Excel (xlsx)
   * Delimitado por tabulaciones

1. (Opcional) Seleccione un hito en la lista de hitos y, a continuación, haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png) para editar la información del hito.
1. (Opcional) Seleccione un hito en la lista de hitos y, a continuación, haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete-icon.png) para eliminarlo.
1. Haga clic en **Sí, eliminarlo**.
El hito se elimina y no se puede recuperar. También se elimina cualquier información de proyecto asociada al hito y cualquier información de tarea asociada a las rutas de hitos.


## Ver detalles de ruta de hitos en un informe de proyecto

Puede ver los detalles de una trayectoria del hito en un informe de proyecto.

Debe asociar una trayectoria del hito a un proyecto para poder ver sus detalles en un informe de proyecto.

Para obtener información sobre cómo asociar rutas de hitos a proyectos, vea [Editar proyectos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

{{step1-to-reports}}

1. Haga clic en **Nuevo informe** y luego haga clic en **Proyecto**.
1. Haga clic en **Añadir columna**.
1. En el área **Mostrar en esta columna**, empiece a escribir **Ruta de hitos** y, a continuación, haga clic en **Nombre de ruta de hitos** cuando aparezca.
1. (Opcional) Haga clic en **Filtros** y agregue el siguiente filtro al informe: **El Id. de ruta de hitos del proyecto no está en blanco**.

   El filtro garantiza que en el informe solo se muestren los proyectos asociados a una trayectoria del hito.

1. Haga clic en **Guardar + Cerrar**.
1. Agregue un nombre al informe y haga clic en **Aplicar**.

   Se muestra el informe del proyecto. Las rutas de hitos asociadas a cada proyecto se muestran en la última columna del informe.
1. Haga clic en el nombre de una trayectoria del hito en la última columna del informe.

   Se muestran los detalles de la trayectoria del hito.

   ![Detalles de ruta de hitos del informe de proyecto](assets/milestone-details-from-project-report.png)

   La página de detalles de la trayectoria del hito muestra la siguiente información:

   * Nombre, ID y descripción de la ruta del hito
   * Grupos de rutas de hitos
   * Nombres, descripciones, colores e iconos de color de hitos

1. (Opcional) Haga clic en **Atrás** para volver al informe del proyecto.



