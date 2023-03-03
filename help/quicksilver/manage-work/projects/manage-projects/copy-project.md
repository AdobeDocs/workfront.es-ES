---
product-area: projects
navigation-topic: manage-projects
title: Copiar un proyecto
description: Puede copiar un proyecto en lugar de crear uno desde cero. Solo se puede copiar un proyecto a la vez. No puede copiar proyectos de forma masiva.
author: Alina
feature: Work Management
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 5%

---

# Copiar un proyecto

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

Puede copiar un proyecto en lugar de crear uno desde cero. Solo se puede copiar un proyecto a la vez. No puede copiar proyectos de forma masiva.

>[!IMPORTANT]
>
>Los siguientes elementos nunca se copian de un proyecto existente en uno nuevo:
>
>* Problemas
>* Tarifas de facturación
>* Registros de facturación
>* Notas
>* Horas
>* Predecesoras entre proyectos
>* Horas presupuestadas
>
>Los siguientes elementos siempre se copian de un proyecto existente a uno nuevo:
>
>* Tareas
>* Plantilla
>* Riesgos
>* Información de configuración de cola
>* Portfolio y programa
>* Tarjeta de puntuación
>* Información predeterminada de la tarea (Proceso de aprobación predeterminado de la tarea, Forms personalizado predeterminado de la tarea)
>


## Requisitos de acceso

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>View permissions or higher to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>plan Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td> <p>Licencia de Adobe Workfront*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Editar acceso a Proyectos con capacidad de Creación <span>y Copiar</span> proyectos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Ver permisos o superiores al proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Copiar un solo proyecto

Al copiar un proyecto también se copia parte de la información del proyecto original en el nuevo proyecto. También puede especificar qué elementos no deben copiarse al nuevo proyecto durante el proceso de copia.

Para copiar un proyecto:

1. Vaya al proyecto que desee copiar y haga clic en **Más** icono ![](assets/qs-more-menu.png) a la derecha del nombre del proyecto

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   O

   Vaya a una lista de proyectos o a un informe y seleccione un proyecto. A continuación, haga clic en **Más** icono ![](assets/qs-more-menu.png) al principio de la lista.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Clic **Copiar**.

1. Actualice el nombre del nuevo proyecto.

   De forma predeterminada, el nuevo nombre es **Copia de `<Original project name>`.**

   ![](assets/copy-project-box-nwe-350x276.png)

1. Seleccione el **Estado** para el nuevo proyecto.

   De forma predeterminada, la variable **Estado** coincide con el del proyecto original.

1. (Opcional) Anule la selección de los elementos que no quiera copiar en el nuevo proyecto. En la tabla siguiente se describe lo que sucede cuando se anula la selección de los elementos:


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seleccionar todo</td> 
      <td> <p>Selecciona todas las opciones y borra todos los campos y objetos enumerados del nuevo proyecto.</p> <p><b>SUGERENCIA</b>

   Anulando selección <strong>Seleccionar todo</strong> anula la selección de todos los elementos. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Asignaciones</td> 
      <td>Quita todas las asignaciones de proyectos y tareas</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progreso</td> 
      <td>Quita el progreso de todas las tareas y se mostrarán como Nuevas. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Datos personalizados</td> 
      <td> <p>Quita la información del formulario personalizado del proyecto, así como la información de los formularios personalizados asociados a los siguientes elementos:</p> 
       <ul> 
        <li>Tareas</li> 
        <li>Gastos</li> 
        <li> Documentos</li> 
       </ul> <p><b>NOTA</b>

   Los formularios personalizados permanecen adjuntos a las tareas, los gastos, los documentos y el proyecto, pero la información de los campos personalizados de los formularios no se copia en el nuevo proyecto. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Quita todo lo que hay en la ficha de documentos, incluidas las versiones de los documentos, los documentos vinculados y las carpetas.</p> <p>De forma predeterminada, las revisiones y aprobaciones de documentos no se pueden copiar en otro proyecto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Todas las predecesoras</td> 
      <td> <p>Quita todas las relaciones de predecesoras entre las tareas del proyecto. </p> <p><b>SUGERENCIA</b>

   Las tareas predecesoras entre proyectos nunca se transfieren al nuevo proyecto, independientemente de si está seleccionado o no. </p> </td>
   </tr>

<tr> 
      <td role="rowheader">Horas presupuestadas</td> 
      <td> <p>Quita del proyecto copiado las horas presupuestadas en el área de Planificación de recursos del caso comercial del proyecto.</p>

<b>NOTA</b>

Las horas presupuestadas con el Scenario Planner nunca se copian en el nuevo proyecto porque el nuevo proyecto no está vinculado a una iniciativa del Scenario Planner. Para obtener más información, consulte <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">Presupuestar recursos en el caso empresarial con el Scenario Planner</a>
</tr></td>
    <tr> 
      <td role="rowheader">Información financiera</td> 
      <td> <p>Quita la información de las áreas siguientes: </p> 
       <ul> 
        <li>Subpestaña Finanzas del proyecto</li> 
        <li> Beneficio planificado en el caso comercial</li> 
        <li>Información financiera de todas las tareas<br></li> 
       </ul> <p>Para obtener más información sobre la subpestaña Project Finance, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Administrar información en el área de finanzas del proyecto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proceso de aprobación</td> 
      <td>Elimina todas las aprobaciones asociadas con las tareas o el proyecto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td> Quita las notificaciones de recordatorio asociadas con las tareas o el proyecto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td>Quita los gastos asociados con las tareas o el proyecto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permisos</td> 
      <td> Quita los permisos a todos los usuarios de las tareas o del proyecto.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Copiar** para crear una copia del proyecto.

   Esto crea un nuevo proyecto similar al proyecto que ha copiado.

   Puede empezar a realizar cambios en el nuevo proyecto copiado, como revisar asignaciones de tareas o ajustar escalas de tiempo.
