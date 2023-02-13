---
title: Personalización de encabezados de objeto mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador de Adobe Workfront o de grupo , puede utilizar una plantilla de diseño para configurar los campos que los usuarios ven en el encabezado del objeto cuando abren la página de un objeto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: a1ffec0d8a50ff7f025ff23370afa746cf0d6d3f
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Personalización de encabezados de objeto mediante una plantilla de diseño

Como administrador de Adobe Workfront o de grupo, puede utilizar una plantilla de diseño para configurar los campos que los usuarios ven en el encabezado del objeto cuando abren la página de un objeto.

>[!IMPORTANT]
>
>La personalización de encabezados de objeto está disponible actualmente para proyectos, tareas y problemas.


Para obtener información sobre plantillas de diseño para grupos, consulte [Creación y modificación de las plantillas de diseño de un grupo](../../manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

![](assets/object-header-fields.png)

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:


<table>
  <tr>
   <td><strong>plan de Adobe Workfront</strong>
   </td>
   <td>Cualquiera
   </td>
  </tr>
  <tr>
   <td><strong>Licencia de Adobe Workfront</strong>
   </td>
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong>Configuraciones de nivel de acceso</strong>
   </td>
   <td>Debe ser administrador de Workfront o de grupo.
<p>
   </td>
  </tr>
</table>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte [Crear o modificar niveles de acceso personalizados](../../add-users/configure-and-grant-access/create-modify-access-levels.md).

## Personalizar encabezados de objeto

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Creación y administración de plantillas de diseño](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. En el **Personalización de lo que ven los usuarios** menú desplegable, seleccione **Proyectos**, **Tareas** o **Problemas**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. En el [!UICONTROL Campos de encabezado] , pase el ratón sobre los campos mostrados y realice una de las siguientes acciones:
   * Haga clic en el **x** icono para quitar un campo

      O

   * Haga clic y mantenga presionada la tecla **take** para arrastrar y soltar el campo en una nueva ubicación.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. Puede tener hasta cinco campos en el encabezado de un objeto.
Si ya tiene cinco campos seleccionados, debe quitar un campo antes de agregar uno nuevo.
1. En el **Añadir campo** , empiece a escribir el nombre de un campo Workfront no editable que desee agregar y, a continuación, selecciónelo cuando aparezca en la lista. El campo se agrega a la derecha inmediata del cuadro Agregar campo y se muestra como el primer campo en la esquina superior izquierda del encabezado del objeto.

   >[!TIP]
   >
   >* Solo se pueden añadir campos que se muestren en el área Información general de la sección Detalles del objeto y que no se puedan editar. Los campos no editables son campos que los usuarios no pueden editar manualmente. Workfront los calcula automáticamente.
   >
   >* Puede agregar campos editables que ya formen parte de los encabezados predeterminados (por ejemplo, Propietario del proyecto, Estado, Porcentaje completado, Asignaciones).
   >
   >* Cuando agrega el campo &quot;Resuelto por&quot; al encabezado de un problema, el campo cambia a &quot;Resolver problema, tarea o proyecto&quot;, cuando hay un objeto de resolución asociado al problema.



   ![](assets/add-field-to-header-in-lt-list.png)


1. (Opcional) Arrastre y suelte los campos añadidos en un orden diferente.

1. Continúe personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **Guardar**.

   >[!TIP]
   >
   >Puede hacer clic en Guardar en cualquier momento para guardar el progreso y luego seguir modificando la plantilla más tarde.
