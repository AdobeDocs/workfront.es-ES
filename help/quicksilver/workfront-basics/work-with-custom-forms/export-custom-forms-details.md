---
title: Exportar formularios personalizados y detalles de objetos
description: Exportar formularios personalizados y detalles de objetos
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1670edf153e57152e51adcfbda052eb74541d931
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 1%

---

# Exportar formularios personalizados y detalles de objetos

Puede exportar la Información general y la información de formulario personalizada desde la sección Detalles de un objeto a un archivo de PDF. A continuación, puede imprimir o compartir el PDF con otros usuarios.

Esta funcionalidad se admite en los siguientes objetos:

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
>Los campos de la sección Detalles que el administrador de Workfront o del grupo ha eliminado mediante una plantilla de diseño no se muestran.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>plan de Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licencia de Adobe Workfront*</p> </td> 
   <td> <p>Solicitar o superior para problemas</p> <p>Revisión o posterior para proyectos y tareas</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Ver o superior para proyectos, tareas y problemas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Permisos de objeto</p> </td> 
   <td> <p>Ver o conceder permisos superiores al proyecto, la tarea o el problema cuyo formulario desee exportar</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de comenzar, debe tener todo lo siguiente:

1. Pida que se cree un formulario personalizado para un objeto específico desde el que desea exportarlo.
1. Incluir el formulario personalizado en el objeto

   O

   Tenga el acceso correcto para adjuntar un formulario personalizado y editar la información del formulario.

Para obtener información sobre la creación de formularios personalizados, consulte [Crear o editar un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

Para obtener información sobre cómo adjuntar formularios a objetos, consulte [Adición de un formulario personalizado a un objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Exportar información en la sección Detalles

La exportación de información desde la sección Detalles de un objeto es idéntica para todos los objetos admitidos.

1. Vaya a un proyecto, tarea, portafolio, programa o problema para el que tenga al menos permisos de visualización.
1. Haga clic en el **Elemento &quot;Detalles&quot;** en el panel izquierdo, como **Detalles de la tarea**.
1. (Opcional) Si no hay ningún formulario personalizado adjunto al objeto, empiece a escribir el nombre de un formulario personalizado en el **Agregar campo de formulario personalizado** y haga clic en ella cuando aparezca en la lista.

   Se pueden agregar hasta 10 formularios.

1. (Opcional) Actualice la información en la sección Detalles y haga clic en **Guardar cambios**.
1. Haga clic en el **Exportar** menú desplegable en la esquina superior derecha, seleccione **Información general** o los formularios que desea exportar y, a continuación, haga clic en **Exportar**.

   También puede seleccionar **Seleccionar todo** si desea exportar el área Información general y todos los formularios personalizados.

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Pueden darse los siguientes escenarios:
   >
   >   
   >   
   >   * Cuando el administrador del grupo o de Workfront anula la selección de todos los campos del área Información general y el objeto tiene formularios personalizados adjuntos, no se muestra la sección Información general .
   >   * Cuando el administrador del grupo o de Workfront anula la selección de todos los campos del área Información general y el objeto no tiene formularios personalizados adjuntos, el menú desplegable Exportar no está visible.
   >   * Si el objeto no tiene formularios personalizados adjuntos, solo puede exportar el área Información general .
   >   * Los campos personalizados que están detrás de la lógica y no son visibles en el formulario no se exportan. Para obtener información sobre cómo agregar lógica a un formulario personalizado, consulte [Agregar lógica de visualización y de omisión de lógica a un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md).


   Se genera y descarga un archivo PDF en el equipo. El archivo PDF contiene la siguiente información:

   * Nombre del objeto al que está adjunto el formulario
   * Nombre del usuario que exportó el PDF
   * Fecha y hora en que se produjo el PDF
   * Nombre de los formularios exportados
   * Información de los campos completados en el formulario
