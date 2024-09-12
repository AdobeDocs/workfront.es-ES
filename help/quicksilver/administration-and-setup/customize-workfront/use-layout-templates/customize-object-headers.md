---
title: Personalización de encabezados de objeto mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador de Adobe Workfront o de un grupo, puede utilizar una plantilla de diseño para configurar los campos que ven los usuarios en el encabezado del objeto cuando abren la página de un objeto.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Personalización de encabezados de objeto mediante una plantilla de diseño

Como administrador de Adobe Workfront o de un grupo, puede utilizar una plantilla de diseño para configurar los campos que ven los usuarios en el encabezado del objeto cuando abren la página de un objeto.

>[!IMPORTANT]
>
>Actualmente, la personalización de encabezados de objeto está disponible para proyectos, tareas y problemas.

![](assets/object-header-fields.png)

Para obtener información sobre cómo crear plantillas de diseño, consulte [Crear y administrar plantillas de diseño](../use-layout-templates/create-and-manage-layout-templates.md).

Para obtener información acerca de las plantillas de diseño para grupos, vea [Crear y modificar plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Después de configurar una plantilla de diseño, debe asignarla a usuarios para que los cambios que ha realizado sean visibles para otros. Para obtener información acerca de cómo asignar una plantilla de diseño a los usuarios, vea [Asignar usuarios a una plantilla de diseño](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td><p>Nuevo: estándar</p>
  <p> Actual: plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.
Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar encabezados de objeto

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. En el menú desplegable **Personalizar lo que ven los usuarios**, seleccione **Proyectos**, **Tareas** o **Problemas**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. En la sección [!UICONTROL Campos de encabezado], pase el ratón sobre los campos mostrados y realice una de las siguientes acciones:
   * Haga clic en el icono **x** para quitar un campo

     O

   * Mantenga presionado el icono **asir** para arrastrar y soltar el campo en una nueva ubicación.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. Se pueden incluir hasta cinco campos en el encabezado de un objeto.
Si ya tiene cinco campos seleccionados, debe quitar un campo para poder agregar uno nuevo.
1. En el cuadro **Agregar campo**, empiece a escribir el nombre del campo de Workfront no editable que desea agregar y, a continuación, selecciónelo cuando se muestre en la lista. El campo se añade inmediatamente a la derecha del cuadro Agregar campo y se muestra como el primer campo en la esquina superior izquierda del encabezado del objeto.

   >[!TIP]
   >
   >* Solo puede añadir campos que se muestren en el área de Información general de la sección Detalles del objeto y que no se puedan editar. Los campos no editables son campos que los usuarios no pueden editar manualmente. Workfront los calcula automáticamente.
   >
   >* Puede agregar campos editables que ya formen parte de los encabezados predeterminados (por ejemplo, Propietario del proyecto, Estado, Porcentaje completado, Asignaciones).
   >
   >* Cuando agrega el campo &quot;Resuelto por&quot; al encabezado de un problema, el campo cambia a &quot;Resolviendo problema, tarea o proyecto&quot;, cuando hay un objeto de resolución asociado al problema.


   ![](assets/add-field-to-header-in-lt-list.png)


1. (Opcional) Arrastre y suelte los campos agregados en un orden diferente.

1. Siga personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **Guardar**.

   >[!TIP]
   >
   >Puede hacer clic en Guardar en cualquier momento para guardar el progreso y seguir modificando la plantilla más adelante.
