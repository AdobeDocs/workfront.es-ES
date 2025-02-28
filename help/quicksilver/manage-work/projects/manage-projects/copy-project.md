---
product-area: projects
navigation-topic: manage-projects
title: Copiar un proyecto
description: Puede copiar un proyecto en lugar de crear uno desde cero. Solo se puede copiar un proyecto a la vez. No puede copiar proyectos en lote.
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 92%

---

# Copiar un proyecto

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

Puede copiar un proyecto en lugar de crear uno desde cero. Solo se puede copiar un proyecto a la vez. No puede copiar proyectos en lote.

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
> Las fechas de las tareas originales de los proyectos se copian en el nuevo proyecto. Debe cambiar la fecha de inicio o finalización del proyecto (según su modo de programación) para actualizar las fechas de las tareas. Las restricciones de tareas pueden impedir que se cambien las fechas del proyecto.

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
   <td> <p>Plan de Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td> <p>Licencia de Adobe Workfront*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraciones del nivel de acceso*</strong> </td> 
   <td> <p>Acceso de edición a los proyectos con la posibilidad de crear <span>y copiar</span> proyectos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creación o modificación de niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Permisos de visualización o superiores del proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Copiar un solo proyecto

Al copiar un proyecto también se copia parte de la información del proyecto original en el nuevo proyecto. También puede especificar qué elementos no deben copiarse al nuevo proyecto durante el proceso de copia.

Para copiar un proyecto, haga lo siguiente:

1. Vaya al proyecto que desee copiar y haga clic en el icono **Más** ![Menú Más](assets/qs-more-menu.png) a la derecha del nombre del proyecto

   ![Más lista desplegable](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   O

   Vaya a una lista de proyectos o a un informe y seleccione un proyecto. Luego, haga clic en el icono **Más** ![Menú Más](assets/qs-more-menu.png) que se encuentra en la parte superior de la lista.

   ![Menú más expandido](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Haga clic en **Copiar**.

1. Actualice el nombre del nuevo proyecto.

   De manera predeterminada, el nuevo nombre es **Copia de `<Original project name>`.**

   ![Copiar cuadro de proyecto](assets/copy-project-box-nwe-350x276.png)

1. Seleccione **Estado** para el nuevo proyecto.

   De manera predeterminada, el **Estado** coincide con el proyecto original.

1. (Opcional) Anule la selección de los elementos que no quiera copiar en el nuevo proyecto. En la tabla siguiente se describe lo que sucede cuando se anula la selección de los elementos:


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seleccionar todo</td> 
      <td> <p>Selecciona todas las opciones y borra todos los campos y objetos enumerados del nuevo proyecto.</p> <p><b>Sugerencia</b>

   Al anular la selección de <strong>Seleccionar todo</strong>, se anulan todos los elementos. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Asignaciones</td> 
      <td>Elimina todas las asignaciones de proyectos y tareas</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progreso</td> 
      <td>Elimina el progreso de todas las tareas y se mostrarán como Nuevas. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Datos personalizados</td> 
      <td> <p>Elimina la información del formulario personalizado del proyecto, así como la información de los formularios personalizados asociados a los siguientes elementos:</p> 
       <ul> 
        <li>Tareas</li> 
        <li>Gastos</li> 
        <li> Documentos</li> 
       </ul> <p><b>NOTA</b>

   Los formularios personalizados permanecen adjuntos a las tareas, los gastos, los documentos y el proyecto, pero la información de los campos personalizados de los formularios no se copia en el nuevo proyecto. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Elimina todo lo que hay en la pestaña de documentos, incluidas las versiones de los documentos, los documentos vinculados y las carpetas.</p> <p>De forma predeterminada, las revisiones y aprobaciones de los documentos no se pueden copiar a otro proyecto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Todas las predecesoras</td> 
      <td> <p>Elimina todas las relaciones de las predecesoras entre las tareas del proyecto. </p> <p><b>Sugerencia</b>

   Las predecesoras entre proyectos nunca se transfieren al nuevo proyecto, independientemente de si está seleccionado o no. </p> </td>
   </tr>

<tr> 
      <td role="rowheader">Horas presupuestadas</td> 
      <td> <p>Elimina del proyecto copiado las horas presupuestadas en el área de Planificación de recursos del caso empresarial del proyecto.</p>

<b>NOTA</b>

Las horas presupuestadas con el Planificador de escenarios nunca se copian en el nuevo proyecto porque el nuevo proyecto no está vinculado a una iniciativa de dicho planificador. Para obtener más información, consulte <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">Recursos presupuestarios en el caso empresarial con el Planificador de escenarios</a>
</tr></td>
    <tr> 
      <td role="rowheader">Información financiera</td> 
      <td> <p>Elimina la información de las áreas siguientes: </p> 
       <ul> 
        <li>Subpestaña Finanzas del proyecto</li> 
        <li> Beneficio planificado en el caso empresarial</li> 
        <li>Información financiera de todas las tareas<br></li> 
       </ul> <p>Para obtener más información acerca de la subpestaña Finanzas del proyecto, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Administrar información en el área Finanzas del proyecto</a>.</p> </td> 
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

1. Haga clic en **Copiar** para crear una copia del proyecto.

   Esto crea un nuevo proyecto similar al proyecto que ha copiado.

   Puede empezar a realizar cambios en el nuevo proyecto copiado, como revisar asignaciones de tareas o ajustar líneas de tiempo.
