---
product-area: projects
navigation-topic: manage-tasks
title: Conversión de una tarea en un proyecto
description: Cuando una tarea de un proyecto requiere un esfuerzo mayor que el planeado originalmente, puede convertirla en un proyecto.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Conversión de una tarea en un proyecto

Cuando una tarea de un proyecto requiere un esfuerzo mayor que el planeado originalmente, puede convertirla en un proyecto.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y proyectos</p> <p>Ver o tener más acceso a las plantillas, al convertir en un proyecto mediante una plantilla</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en una tarea</p> <p>Ver permisos de una plantilla, si se convierte a un proyecto mediante una plantilla</p> <p>Después de crear el proyecto, tiene permisos de administración para el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones para convertir tareas en proyectos

* Se elimina la tarea original.
* Se eliminan las aprobaciones de tareas.
* Todas las subtareas, problemas y notas se resumen en el nuevo proyecto.
* Los documentos, las versiones del documento y las pruebas se mueven al nuevo proyecto.
* Se conservan el estado y el porcentaje completado de todas las subtareas y problemas.
* Los usuarios compartidos de la tarea pasan a ser usuarios compartidos en el proyecto.
* La fecha de inicio del proyecto se establece en la fecha de inicio de la tarea.
* Si el estado de la tarea es &quot;Nuevo&quot;, el estado del proyecto se establece en &quot;Planificación&quot;.
* Si el estado de la tarea es &quot;En curso&quot;, el estado del proyecto se establece en &quot;Actual&quot;.
* Si el estado de la tarea es &quot;Completado&quot;, el estado del proyecto se establece en &quot;Completado&quot;.

## Conversión de una tarea en un proyecto

1. Vaya a la tarea que desea convertir en un proyecto.
1. Haga clic en el **Más** icono ![](assets/more-icon.png), luego **Convertir en proyecto**.
1. Elija las siguientes opciones:

   * **Nuevo proyecto**
   * Una plantilla en la variable **Seleccionar de plantillas** sección

      ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Haga clic en **Continuar** en la notificación que aparece.
1. En el **Convertir en proyecto** especifique lo siguiente:

   * **Nombre**: Asigne un nombre al proyecto. El nombre predeterminado es el nombre de la tarea.
   * (Opcional) **Descripción**: Describa el propósito de este proyecto.
   * (Opcional y condicional) Si ha seleccionado crear un proyecto a partir de una plantilla, actualice los campos disponibles en la variable **Convertir en proyecto** para abrir el Navegador.

      Para obtener más información sobre la edición de campos en proyectos, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >Para actualizar los campos de la sección Finanzas del cuadro Convertir a proyecto debe tener acceso de edición a datos financieros en el nivel de acceso. Si tiene acceso de vista a datos financieros en el nivel de acceso, toda la información financiera de la plantilla se transfiere al nuevo proyecto y no puede editarse mientras convierte el problema. Para obtener más información, consulte [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) y [Compartir una plantilla](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Opcional) Agregue **Forms personalizado** al nuevo proyecto.

      >[!TIP]
      Si un formulario personalizado de varios objetos adjunto a la tarea está configurado para su uso con tareas y proyectos, toda la información guardada en el formulario se conserva al realizar la conversión.
      Si utiliza una plantilla para la conversión y un formulario personalizado adjunto a la plantilla contiene un campo personalizado que también se encuentra en un formulario personalizado adjunto a la tarea, el valor del campo de la tarea se utiliza para el nuevo proyecto. Sin embargo, si el campo personalizado está vacío en la tarea, se utiliza el valor de la plantilla.

1. Haga clic en **Guardar cambios**.
