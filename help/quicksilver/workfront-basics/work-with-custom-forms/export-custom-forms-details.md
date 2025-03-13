---
title: Exportar formularios personalizados y detalles de objetos
description: Exportar formularios personalizados y detalles de objetos
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: c21029e098f6b4f51f8698155e2b8a2e789c8bfc
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 95%

---

# Exportar formularios personalizados y detalles de objetos

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

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Plan de Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licencia de Adobe Workfront*</p> </td> 
   <td> <p>Permiso de solicitud o superior para los problemas</p> <p>Revisar o superior para proyectos y tareas</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configuraciones del nivel de acceso*</strong> </td> 
   <td> <p>Permisos de visualización o superiores para proyectos, tareas y problemas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Permisos de objeto</p> </td> 
   <td> <p>Permisos de visualización o superiores para el proyecto, tarea o problema cuyo formulario desea exportar</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

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

   ![](assets/export-custom-form-button-menu.png)

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
