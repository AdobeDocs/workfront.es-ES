---
title: Personalización de la vista Detalles mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador de Workfront, puede utilizar una plantilla de diseño para determinar qué información aparece cuando un usuario selecciona la sección Detalles del panel izquierdo mientras visualiza una tarea, un problema, un documento, un programa o un portafolio.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 92fb1ee0b641d2f4b527e17df272e4c37c0feaef
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Personalización de la vista Detalles mediante una plantilla de diseño

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Como administrador de Adobe Workfront, puede utilizar una plantilla de diseño para determinar qué información aparece cuando un usuario hace clic en el icono Detalles ![](assets/project-details-icon.png) en el panel izquierdo mientras ve una tarea, un problema, un documento, un programa o un portafolio.

<!--
or billing record
-->

También puede cambiar el orden de la información en la que aparece esta información. Por ejemplo, para todas las tareas que vean los usuarios, puede mover la información de Forms personalizada a la parte superior de la vista Detalles para todas las tareas que vean los usuarios.

Los cambios que realice en la vista Detalles de un objeto también determinan la disponibilidad y el orden de los campos que verán los usuarios en las siguientes áreas:

* Los cuadros &quot;Nuevo objeto&quot;, como Nueva tarea y Nuevo problema

   ![](assets/new-task-dialog.png)

* Pantallas &quot;Editar objeto&quot;, como Editar tarea, Editar problema y Editar proyecto

   ![](assets/edit-task-screen.png)


* Editar objetos cuando edita objetos de forma masiva. Actualmente, se admite para editar proyectos de forma masiva.

   ![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* Resumen ![](assets/summary-panel-icon.png) panel para listas de tareas y problemas

   ![](assets/summary-area.png)

   >[!NOTE]
   >
   >Los cambios en las plantillas de diseño afectan al orden y la disponibilidad de los campos en el panel Resumen solo para las tareas y los problemas que se asignan al usuario que ha iniciado sesión.

* Los cuadros de conversión, como Convertir problema a tarea o Convertir problema a cuadros de proyecto.

   ![Convertir problema en cuadro de tareas](assets/convert-issue-to-task-box.png)

Para obtener información sobre plantillas de diseño para grupos, consulte [Creación y modificación de las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
   <td> <p>Para realizar estos pasos a nivel de sistema, necesita el nivel de acceso del administrador del sistema.
Para realizarlos para un grupo, debe ser administrador de dicho grupo</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalice lo que ven los usuarios en la vista Detalles

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Haga clic en la flecha hacia abajo ![](assets/dropdown-arrow-12x12.png) under **Personalización de lo que ven los usuarios** y haga clic en **Proyecto**, **Tarea**, **Problema**, **Programa** o **Portfolio.**
<!--
, or billing record
-->

1. En el **Detalles** , realice una de las acciones siguientes para personalizar lo que ven los usuarios en la vista Detalles:

   * Arrastrar cualquier encabezado de sección ![](assets/move-icon---dots.png) para cambiar su orden.
   * Activar o desactivar opciones en **Información general** y **Forms personalizado** para mostrarlos u ocultarlos.

      Si oculta todos los campos de una de estas secciones, se oculta toda la sección.

      Todos los campos están habilitados de forma predeterminada.

1. Continúe personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **Guardar**.

   >[!TIP]
   >
   >Puede hacer clic en Guardar en cualquier momento para guardar el progreso y luego seguir modificando la plantilla más tarde.
