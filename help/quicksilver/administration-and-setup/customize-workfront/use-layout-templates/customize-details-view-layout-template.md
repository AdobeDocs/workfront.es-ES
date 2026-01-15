---
title: Personalizar la vista de detalles con una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador de Workfront, puede utilizar una plantilla de diseño para determinar qué información aparece cuando un usuario selecciona la sección Detalles en el panel izquierdo mientras ve una tarea, un problema, un documento, un programa o un portafolio.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: c037b4f9e5530d8dd796bed25021f7073f16061f
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 70%

---

# Personalizar la vista de detalles con una plantilla de diseño

Como administrador de Adobe Workfront, puede usar una plantilla de diseño para determinar qué información aparece cuando un usuario hace clic en el icono de detalles ![icono de detalles](assets/project-details-icon.png) en el panel izquierdo mientras ve una tarea, un problema, un documento, un programa o un portafolio.

También puede cambiar el orden en que aparece esta información. Por ejemplo, para todas las tareas que ven sus usuarios, puede mover la información de los formularios personalizados a la parte superior de la vista Detalles para todas las tareas que ven sus usuarios.

Para obtener información sobre cómo crear plantillas de diseño, consulte [Crear y administrar plantillas de diseño](../use-layout-templates/create-and-manage-layout-templates.md).

Para obtener información acerca de las plantillas de diseño para grupos, consulte [Creación y modificación de las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Después de configurar una plantilla de diseño, debe asignarla a usuarios para que los cambios que ha realizado sean visibles para otros. Para obtener información acerca de cómo asignar una plantilla de diseño a los usuarios, consulte [Asignar usuarios a una plantilla de diseño](../use-layout-templates/assign-users-to-layout-template.md).

Los cambios que realice en la vista Detalles de un objeto también determinan la disponibilidad y el orden de los campos que los usuarios ven en las siguientes áreas:


* Cuadros “Crear objeto”, como Crear tarea

  ![Cuadro de diálogo Nueva tarea](assets/new-task-dialog.png)


* Pantallas “Editar objeto” al editar un objeto, como Editar tarea, Editar problema y Editar proyecto

  ![Editar pantalla de tareas](assets/edit-task-screen.png)


* Pantallas “Editar objetos” al editar objetos en lotes. Actualmente, esto es compatible con la edición de proyectos en lotes.

  ![Personalizar y editar proyectos](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* Panel de resumen ![Panel de resumen](assets/summary-panel-icon.png) para listas de tareas y problemas

  ![Área de resumen](assets/summary-area.png)

  >[!NOTE]
  >
  >Los cambios en las plantillas de diseño afectan al orden y la disponibilidad de los campos en el panel de resumen solo para las tareas y problemas asignados al usuario que ha iniciado sesión.

* Cuadros de conversión, como los cuadros Convertir problema en tarea o Convertir problema en proyecto.

  ![Convertir problema en cuadro de tareas](assets/convert-issue-to-task-box.png)

Para obtener información sobre las plantillas de diseño para grupos, consulte [Creación y modificación de las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.</p>
        <p>Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar lo que ven los usuarios en la vista Detalles

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Haga clic en la flecha abajo ![Flecha abajo](assets/dropdown-arrow-12x12.png) bajo **Personalizar lo que ven los usuarios**, luego haga clic en **Proyecto**, **Tarea**, **Problema**, **Programa** o **Portfolio.**<!--, or billing record-->
1. En la sección **Detalles**, realice una de las acciones siguientes para personalizar lo que ven los usuarios en la vista Detalles:

   * Arrastre cualquier encabezado de sección ![Icono de mover](assets/move-icon---dots.png) para cambiar su orden.
   * Habilite o deshabilite las opciones en las diversas áreas (como **Información general**, **Finanzas** y **Forms personalizado**) para mostrarlas u ocultarlas.

     Si oculta todos los campos de una de estas secciones, se oculta toda la sección.

     Todos los campos están habilitados de forma predeterminada. Puede activar o desactivar la casilla de verificación **Seleccionar todo** de un área para mostrar u ocultar todos los campos de dicha área.

     ![Vista de detalles en la plantilla de diseño](assets/layout-template-details-view-updated-save-buttons.png)

1. Siga personalizando la plantilla de diseño. Puede hacer clic en **Aplicar** en cualquier momento para guardar el progreso.

   O

   Si ha terminado de personalizar, haga clic en **Guardar y cerrar**.

