---
title: Exportar Forms personalizado y detalles del objeto
description: Puede exportar la Información general y la información del formulario personalizado desde la sección Detalles de un objeto a un archivo PDF. A continuación, puede imprimir o compartir el PDF con otros usuarios.
author: Alina
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 90%

---

# Exportar formularios personalizados y detalles de objetos

<!--Audited: 10/2025-->

Puede exportar la Información general y la información del formulario personalizado desde la sección Detalles de un objeto a un archivo PDF. A continuación, puede imprimir o compartir el PDF con otros usuarios.

Esta funcionalidad es compatible con los siguientes objetos:

* Proyectos
* Tareas
* Problemas
* Portafolio
* Programas

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>No se muestran los campos de la sección Detalles que su administrador de grupos o de Workfront ha eliminado mediante una plantilla de diseño.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Paquete de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licencia de Adobe Workfront</p> </td> 
   <td><p>Para problemas:</p>
   <ul><li><p>Colaborador o superior</p></li>
   <li><p>Solicitante o superior</p> </li></ul>
   <p>Para proyectos y tareas:</p>
   <ul><li><p>Ligero o superior</p></li>
   <li><p>Revisor o superior</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Permisos de visualización o superiores para proyectos, tareas y problemas</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Permisos de objeto</p> </td> 
   <td> <p>Permisos de visualización o superiores para el proyecto, tarea o problema cuyo formulario desea exportar</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Request or higher for issues</p> <p>Review or higher for projects and tasks</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Access level configurations*</strong> </td> 
   <td> <p>View or higher for Projects, Tasks, and Issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> <p>View or higher permissions to the project, task, or issue whose form you want to export</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Requisitos previos

Antes de comenzar, debe disponer de todos los elementos siguientes:

1. Cree un formulario personalizado para un objeto específico desde el que desee exportarlo.
1. Adjunte el formulario personalizado al objeto

   O

   Debe disponer del acceso correcto para adjuntar un formulario personalizado y editar la información del formulario.

Para obtener información sobre cómo crear formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Para obtener información acerca de cómo adjuntar formularios a objetos, consulte [Añadir un formulario personalizado a un objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Exportar información en la sección Detalles

La exportación de información desde la sección Detalles de un objeto es idéntica para todos los objetos en los que es compatible.

1. Vaya a un proyecto, tarea, portafolios, programa o problema para el cual tenga al menos permisos de visualización.
1. Haga clic en el elemento **“Detalles”** del panel izquierdo, como **Detalles de la tarea**.
1. (Opcional) Si no hay ningún formulario personalizado adjunto al objeto, empiece a escribir el nombre de un formulario personalizado en **Añadir campo de formulario personalizado**, y a continuación, haga clic sobre él cuando aparezca en la lista.

   Se pueden añadir hasta 10 formularios.

1. (Opcional) Actualice la información en la sección Detalles y, a continuación, haga clic en **Guardar cambios**.
1. Haga clic en el menú desplegable **Exportar** en la esquina superior derecha, seleccione **Información general** o los formularios que desee exportar y, a continuación, haga clic en **Exportar**.

   También puede seleccionar **Seleccionar todo** si desea exportar el área Información general y todos los formularios personalizados.

   ![Botón Exportar formulario personalizado](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Pueden darse los siguientes escenarios:
   >
   >   * Cuando el administrador del grupo o de Workfront anula la selección de todos los campos del área Información general y el objeto tiene adjuntos formularios personalizados, la sección Información general no se muestra.
   >   * Cuando el administrador del grupo o de Workfront anula la selección de todos los campos del área Información general y el objeto no tiene adjuntos formularios personalizados, el menú desplegable Exportar no está visible.
   >   * Cuando el objeto no tiene formularios personalizados adjuntos, solo puede exportar el área Información general.
   >   * Los campos personalizados que están detrás de la lógica y no son visibles en el formulario no se exportan. Para obtener información sobre cómo agregar lógica a un formulario personalizado, consulte [Agregar reglas lógicas a formularios y campos personalizados](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

   Se genera un archivo de PDF y se descarga en el equipo. El archivo PDF contiene la siguiente información:

   * Nombre del objeto al que está adjunto el formulario
   * El nombre del usuario que exportó el PDF
   * La fecha y la hora en que se produjo el PDF
   * El nombre de los formularios exportados
   * Información de los campos rellenados en el formulario
