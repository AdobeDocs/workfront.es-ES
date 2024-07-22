---
title: Creación de una trayectoria del hito
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Como administrador de Adobe Workfront, puede crear rutas de hitos que luego se pueden aplicar a cualquier proyecto del sistema. Los cambios que realice en las rutas de hitos en esta área afectarán a todo el sistema de Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: ed179058cfec1332384ef76cb04598278109291b
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 2%

---

# Creación de una trayectoria del hito

<!--Audited: 07/2024-->

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Como administrador de Adobe Workfront, puede crear rutas de hitos que luego se pueden aplicar a cualquier proyecto del sistema. Los cambios que realice en las rutas de hitos en esta área afectarán a todo el sistema de Workfront.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Hitos y rutas de hitos

Puede asociar las tareas clave de un proyecto con hitos predefinidos. Esta función puede proporcionar a los administradores y otras partes interesadas una visión general de alto nivel sobre el progreso de un proyecto.

La suma de todos los hitos predefinidos se denomina trayectoria del hito.

El primer paso para construir una trayectoria del hito es identificar cuáles son los pasos del hito y establecer los hitos. Dado que puede asociar una trayectoria del hito a varios proyectos, los pasos del hito deben ser fases o etapas generales de cualquier proyecto.

Para obtener más información sobre cómo asociar una ruta de hitos a un proyecto y un hito a una tarea, vea [Asociar hitos a tareas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Creación de una trayectoria del hito

{{step-1-to-setup}}

1. Haga clic en **Procesos** > **Rutas de hitos**.
1. Haga clic en **Nueva ruta de hitos.**
1. Especifique la siguiente información en el área **Información básica**:

   <table style="table-layout:auto">
    <tr>
      <td>Nombre de ruta de hitos</td>
       <td>Introduzca un nombre para la trayectoria del hito.</td>
    </tr>
    <tr>
      <td>Descripción</td>
      <td>Introduzca una descripción para definir la trayectoria del hito.</td>
    </tr>
    <tr>
       <td>Activo</td>
      <td>Seleccione esta casilla de verificación si desea que la trayectoria del hito esté activa. Otros usuarios pueden encontrar esta ruta y adjuntarla a proyectos al crear o editar proyectos. Las rutas de hitos inactivas no se pueden adjuntar a los proyectos. Esta opción está habilitada de forma predeterminada.</td>
    </tr>
    <tr>
      <td>Grupos</td>
      <td>Seleccione los grupos enumerados para permitir que los usuarios de estos grupos vean y apliquen esta ruta de hitos a sus proyectos. El grupo de inicio del usuario que entra en la trayectoria del hito se selecciona de forma predeterminada.</td>
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
      <td> <p>Elija un color que se asociará al hito. </p> <p>Si no se elige un color, el sistema elige el último color utilizado en una trayectoria del hito. Le recomendamos que elija un color único para cada hito. El color se utiliza con fines visuales y de creación de informes.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Agregar hito** y continúe agregando hitos según sea necesario hasta que finalice la ruta de acceso.
1. Haga clic en **Crear ruta de hitos** para guardar los cambios.

   La ruta de hitos está lista para asociarse a un proyecto.

   Para obtener más información sobre cómo asociar rutas de hitos a proyectos e hitos a tareas, vea [Asociar hitos a tareas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).
