---
title: Crear una ruta de hitos
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Como administrador de Adobe Workfront, puede crear rutas de hitos que luego se pueden aplicar a cualquier proyecto del sistema. Los cambios que realice en las rutas de hitos de esta área afectarán a todo el sistema de Workfront.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 2%

---

# Crear una ruta de hitos

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Como administrador de Adobe Workfront, puede crear rutas de hitos que luego se pueden aplicar a cualquier proyecto del sistema. Los cambios que realice en las rutas de hitos de esta área afectarán a todo el sistema de Workfront.

## Requisitos de acceso

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
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Hitos y rutas de hitos

Puede asociar las tareas clave de un proyecto con hitos predefinidos. Esta función puede proporcionar a los administradores y a otros interesados una visión general de alto nivel sobre el progreso de un proyecto.

La suma de todos los hitos predefinidos se denomina ruta de hitos.

El primer paso para construir una ruta de hitos es identificar cuáles son los pasos de hitos y establecer los hitos. Dado que puede asociar una ruta de hitos a varios proyectos, los pasos de hitos deben ser fases generales o etapas de cualquier proyecto.

Para obtener más información sobre cómo asociar una ruta de hitos a un proyecto y un hito a una tarea, consulte [Asociar hitos con tareas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Crear una ruta de hitos

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Procesos** > **Rutas de Milestone**.
1. Haga clic en **Nueva ruta de Milestone.**
1. Especifique la siguiente información en la **Información básica** área:

   <table style="table-layout:auto">
    <tr>
      <td>Nombre de ruta de hitos</td>
       <td>Escriba un nombre para la ruta de hitos.</td>
    </tr>
    <tr>
      <td>Descripción</td>
      <td>Introduzca una descripción para definir la ruta del hito.</td>
    </tr>
    <tr>
       <td>Activo</td>
      <td>Seleccione esta casilla si desea que la ruta de hitos esté activa. Otros usuarios pueden encontrar esta ruta y adjuntarla a los proyectos al crear o editar proyectos. Las rutas de hitos inactivas no se pueden adjuntar a los proyectos. Esta opción está activada de forma predeterminada.</td>
    </tr>
    <tr>
      <td>Grupos</td>
      <td>Seleccione los grupos enumerados para permitir a los usuarios de estos grupos ver y aplicar esta ruta de hitos a sus proyectos. El grupo principal del usuario que entra en la ruta de hitos está seleccionado de forma predeterminada.</td>
    </tr>
   </table>

1. Especifique la siguiente información en la **Hitos** área:

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
      <td> <p>Elija un color para asociarlo al hito. </p> <p>Si no elige un color, el sistema elige el último color utilizado en una ruta de hitos. Le recomendamos que elija un color único para cada hito. El color se utiliza para fines visuales y de informes.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Agregar Milestone** y siga agregando hitos según sea necesario hasta que se complete la ruta.
1. Haga clic en **Crear ruta de Milestone** para guardar los cambios.

   La ruta de hito está lista para asociarse con un proyecto.

   Para obtener más información sobre cómo asociar rutas de hitos a proyectos e hitos a tareas, consulte [Asociar hitos con tareas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).
