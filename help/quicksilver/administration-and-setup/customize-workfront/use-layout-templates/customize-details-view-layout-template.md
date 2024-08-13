---
title: Personalización de la vista de detalles mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador de Workfront, puede utilizar una plantilla de diseño para determinar qué información aparece cuando un usuario selecciona la sección Detalles en el panel izquierdo mientras ve una tarea, un problema, un documento, un programa o un portafolio.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# Personalización de la vista Detalles mediante una plantilla de diseño

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Como administrador de Adobe Workfront, puede usar una plantilla de diseño para determinar qué información aparece cuando un usuario hace clic en el icono Detalles ![](assets/project-details-icon.png) en el panel izquierdo mientras ve una tarea, un problema, un documento, un programa o un portafolio.

<!--
or billing record
-->

También puede cambiar el orden de la información en la que aparece. Por ejemplo, para todas las tareas que ven los usuarios, puede mover información de Forms personalizada a la parte superior de la vista Detalles para todas las tareas que vean los usuarios.

Para obtener información sobre cómo crear plantillas de diseño, consulte [Crear y administrar plantillas de diseño](../use-layout-templates/create-and-manage-layout-templates.md).

Para obtener información acerca de las plantillas de diseño para grupos, vea [Crear y modificar plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Después de configurar una plantilla de diseño, debe asignarla a usuarios para que los cambios que ha realizado sean visibles para otros. Para obtener información acerca de cómo asignar una plantilla de diseño a los usuarios, vea [Asignar usuarios a una plantilla de diseño](../use-layout-templates/assign-users-to-layout-template.md).

Los cambios que realice en la vista Detalles de un objeto también determinan la disponibilidad y el orden de los campos que ven los usuarios en las áreas siguientes:


* Cuadros &quot;Crear objeto&quot;, como Crear tarea

  ![](assets/new-task-dialog.png)


* Pantallas &quot;Editar objeto&quot; al editar un objeto, como Editar tarea, Editar problema y Editar proyecto

  ![](assets/edit-task-screen.png)


* Pantallas &quot;Editar objetos&quot; al editar objetos de forma masiva. Actualmente, esto es compatible con la edición de proyectos por lotes.

  ![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* Panel de resumen ![](assets/summary-panel-icon.png) para listas de tareas y problemas

  ![](assets/summary-area.png)

  >[!NOTE]
  >
  >Los cambios en las plantillas de diseño afectan al orden y la disponibilidad de los campos en el Panel de resumen solo para las tareas y problemas asignados al usuario que ha iniciado sesión.

* Cuadros de conversión, como los cuadros Convertir problema en tarea o Convertir problema en proyecto.

  ![Convertir problema en cuadro de tareas](assets/convert-issue-to-task-box.png)

Para obtener información acerca de las plantillas de diseño para grupos, vea [Crear y modificar plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.
Para realizarlos para un grupo, debe ser administrador de ese grupo</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Personalizar lo que los usuarios ven en la vista Detalles

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Haga clic en la flecha abajo ![](assets/dropdown-arrow-12x12.png) bajo **Personalizar lo que ven los usuarios** y, a continuación, haga clic en **Proyecto**, **Tarea**, **Problema**, **Programa** o **Portfolio.**
<!--
, or billing record
-->

1. En la sección **Detalles**, realice una de las acciones siguientes para personalizar lo que ven los usuarios en la vista Detalles:

   * Arrastre cualquier encabezado de sección ![](assets/move-icon---dots.png) para cambiar su orden.
   * Habilite o deshabilite las opciones en **Información general** y **Forms personalizado** para mostrarlas u ocultarlas.

     Si oculta todos los campos de una de estas secciones, se oculta toda la sección.

     Todos los campos están habilitados de forma predeterminada.

1. Siga personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **Guardar**.

   >[!TIP]
   >
   >Puede hacer clic en Guardar en cualquier momento para guardar el progreso y seguir modificando la plantilla más adelante.
