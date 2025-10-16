---
product-area: projects
navigation-topic: manage-projects
title: Copiar un proyecto
description: Puede copiar un proyecto en lugar de crear uno desde cero. Solo se puede copiar un proyecto a la vez. No puede copiar proyectos en lote.
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 62%

---

# Copiar un proyecto

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

<!-- Audited: 5/2025 -->

Puede copiar un proyecto de uno existente en lugar de crear uno desde cero, lo que le ayuda a ahorrar tiempo.

Tenga en cuenta que no puede copiar proyectos de forma masiva.

>[!IMPORTANT]
>
>Los siguientes elementos nunca se copian de un proyecto existente a uno nuevo:
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
>* Portafolio y programa
>* Tarjeta de puntuación
>* Información predeterminada de la tarea (Proceso de aprobación predeterminado de la tarea, Formularios personalizados predeterminados de la tarea)
>
> Las fechas de las tareas del proyecto original se copiarán en el nuevo proyecto. Debe cambiar la fecha de inicio o finalización del proyecto (según su modo de programación) para actualizar las fechas de las tareas. Las restricciones de tareas pueden impedir que se cambien las fechas del proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.
Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>paquete de Adobe Workfront</p> </td>  
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td> <p>Licencia de Adobe Workfront</p> </td> 
   <td> <p>Estándar</p> 
   <p>Plan</p>
      </td> 
  </tr> 
     <td>Configuraciones de nivel de acceso </td> 
   <td> <p>Editar el acceso a los proyectos con capacidad para crear y copiar proyectos</p> </td> 
  </tr>

<td> <p>Permisos de objeto </p> </td> 
   <td> <p>Permisos de visualización o superiores del proyecto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license</p> </td> 
   <td> <p>New: Standard </p> 
   <p>Or</p>
   <p>Current: Plan </p>
   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configurations </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>View permissions or higher to the project</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Copiar un solo proyecto

Al copiar un proyecto también se copia parte de la información del proyecto original en el nuevo proyecto. También puede especificar qué elementos no deben copiarse al nuevo proyecto durante el proceso de copia.

Para copiar un proyecto, haga lo siguiente:

{{step1-to-projects}}

1. Seleccione el proyecto que desea copiar de la lista de proyectos y luego haga clic en el icono **Más** ![Menú Más](assets/more-icon.png) a la derecha del nombre del proyecto.

   O

   Vaya a una lista de proyectos o a un informe y seleccione un proyecto. Luego, haga clic en el icono **Más** ![Menú Más](assets/more-icon.png) que se encuentra en la parte superior de la lista.

1. En el menú desplegable **Más**, haga clic en **Copiar**. Aparece el cuadro de diálogo **Copia de [Nombre del proyecto]**.

1. (Opcional) Actualice **Nombre de proyecto**. De manera predeterminada, el nuevo nombre es **Copia de [nombre del proyecto original]**.

   ![Copiar cuadro de proyecto](assets/copy-of-project-box.png)

1. Seleccione un **estado**. De forma predeterminada, se selecciona el estado del proyecto original.

1. (Opcional) Anule la selección de los elementos que no quiera copiar en el nuevo proyecto. En la tabla siguiente se describe lo que sucede cuando se anula la selección de los elementos:


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seleccionar todo</td> 
      <td> <p>Selecciona todas las opciones y borra todos los campos y objetos enumerados del nuevo proyecto. </p>

   <p> Al anular la selección de esta opción, se anulan todos los elementos. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Asignaciones</td> 
      <td>Quita todas las asignaciones de proyectos y tareas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progreso</td> 
      <td>Quita el progreso de todas las tareas y las muestra como Nuevas. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Datos personalizados</td> 
      <td> <p>Elimina la información del formulario personalizado del proyecto, así como la información de los formularios personalizados asociados a los siguientes elementos:</p> 
       <ul> 
        <li>Tareas</li> 
        <li>Gastos</li> 
        <li> Documentos</li> 
       </ul> 
      <p>Los formularios personalizados permanecen adjuntos a las tareas, los gastos, los documentos y el proyecto, pero la información de los campos personalizados del formulario no se copia en el nuevo proyecto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Quita todo lo que hay en la ficha Documentos, incluidas las versiones de los documentos, los documentos vinculados y las carpetas.</p> <p>De forma predeterminada, las revisiones y aprobaciones de los documentos no se pueden copiar a otro proyecto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Todas las predecesoras</td> 
      <td> <p>Elimina todas las relaciones de las predecesoras entre las tareas del proyecto. </p> <p>

   Las predecesoras entre proyectos nunca se transfieren al nuevo proyecto, independientemente de si está seleccionado o no. </p> </td>
   </tr>

<tr> 
      <td role="rowheader">Horas presupuestadas</td> 
      <td> <p>Elimina del proyecto copiado las horas presupuestadas en el área de Planificación de recursos del caso empresarial del proyecto.</p> 
    <p>
   Las horas presupuestadas con el Planificador de escenarios nunca se copian en el nuevo proyecto porque el nuevo proyecto no está vinculado a una iniciativa de dicho planificador. Para obtener más información, consulte <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">Recursos presupuestarios en el caso empresarial con el Planificador de escenarios</a></p>
   </tr></td>
    <tr> 
      <td role="rowheader">Información financiera</td> 
      <td> <p>Elimina la información de las áreas siguientes: </p> 
       <ul> 
        <li>Subpestaña Finanzas del proyecto</li> 
        <li> Beneficio planificado en el caso empresarial</li> 
        <li>Información financiera de todas las tareas<br></li> 
       </ul> <p>Para obtener más información acerca de la subficha Finanzas del proyecto, vea <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Administrar información en el área Finanzas del proyecto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proceso de aprobación</td> 
      <td>Elimina todas las aprobaciones asociadas con las tareas o el proyecto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td> Elimina las notificaciones de recordatorio asociadas con las tareas o el proyecto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td>Elimina los gastos asociados con las tareas o el proyecto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permisos</td> 
      <td> Elimina los permisos a todos los usuarios de las tareas o del proyecto.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Copiar proyecto**. Se crea el proyecto copiado.
