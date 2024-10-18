---
title: Personalizar una nueva página de inicio mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Puede utilizar una plantilla de diseño para configurar lo que ven los usuarios cuando abren una nueva página de inicio.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 1426f806b72d740712eba5e337c8424f8af6c9dc
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 1%

---

# Personalizar una nueva página de inicio con una plantilla de diseño

Puede utilizar una plantilla de diseño para configurar lo que ven los usuarios la primera vez que abren una nueva página de inicio.

Puede configurar lo siguiente:

* Qué widgets se muestran en el espacio de trabajo de forma predeterminada
* Qué fondo se selecciona
* Configuración de widgets específicos, incluidos los filtros y grupos disponibles para los widgets Mis proyectos, Mis tareas y Mis problemas, así como sus valores predeterminados

>[!IMPORTANT]
>
>Los usuarios finales pueden cambiar su fondo y reordenar los widgets de la página después de aplicar la plantilla de diseño. No pueden eliminar los widgets incluidos por un administrador de Workfront.
> <br>
>Los administradores tienen la capacidad de añadir nuevos widgets para los usuarios. Sin embargo, si un usuario final ya ha personalizado el orden de los widgets o la selección del fondo, esas personalizaciones específicas no se modifican.



Para obtener información sobre la nueva página de inicio, consulte [Introducción a la página de inicio](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

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

## Personalizar una nueva página de inicio con una plantilla de diseño

Para personalizar el nuevo directorio raíz mediante una plantilla de diseño:

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Haga clic en la flecha abajo ![](assets/dropdown-arrow.png) bajo **Personalizar lo que ven los usuarios** y, a continuación, haga clic en **Workspace particular**.

1. En las pestañas que aparecen a la derecha, haz clic en **Diseño y diseño** para elegir y organizar los widgets y el fondo, o en **Configuración de los widgets** para administrar la configuración de widgets individuales como filtros y grupos disponibles.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Diseño y disposición</td> 
      <td>
      <p>Seleccione los widgets que estarán presentes en los espacios de trabajo de los usuarios, su posición y elija un fondo. Tenga en cuenta que, aunque los usuarios no pueden eliminar los widgets seleccionados, pueden moverlos y cambiarles el tamaño libremente, así como agregar widgets adicionales.</p>
      <p>Esta ficha funciona esencialmente como un pequeño espacio de trabajo de Inicio; como tal, se puede personalizar según los pasos descritos en <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Agregar, editar o quitar widgets en Inicio</a>. Seleccione los widgets y organice el espacio de trabajo tal como desea que aparezca para los usuarios.</p>
      <p>Para cambiar el fondo, sigue los pasos de <b>Personalización del fondo</b> en <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">Introducción a la página principal</a>.</p>
      <p>

>[!NOTE]
>
>Al mover o cambiar el tamaño de los widgets en la plantilla de diseño, no se almacenarán en déclencheur las nuevas páginas de inicio de los usuarios para actualizar su diseño. Sin embargo, añadir o eliminar un widget almacenará en déclencheur una actualización de las páginas de los usuarios.

</p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuración del widget</td> 
      <td>
      <p>Cambie la configuración de los widgets individuales. Actualmente, solo se admiten tres widgets:</p>
      <ul>
        <li>Mis proyectos</li>
        <li>Mis tareas</li>
        <li>Mis problemas</li>
      </ul>
      <p>Una vez que haya seleccionado el widget que desea editar, las opciones disponibles se mostrarán a la derecha. Estas opciones incluyen <b>Filtros</b>, <b>Columnas</b> y <b>Grupos</b>. Puede:</p>
      <ul>
      <li><p><b>Seleccione y ordene los filtros, columnas o grupos disponibles para los usuarios:</b></p>
      <p>Marque la casilla junto a todas las opciones de la lista que desee que los usuarios puedan utilizar. Estas opciones no se extienden al panel Resumen. Debe configurar esa área en la pestaña Resumen de la plantilla de diseño. Las opciones no seleccionadas no aparecerán para los usuarios. Arrastre y suelte las opciones de la lista para establecer un orden.</li></p>
      <p>

>[!IMPORTANT]
>
>Los usuarios deben tener al menos acceso de creación a vistas para que la configuración de la columna del administrador se aplique correctamente a sus nuevas páginas de inicio.

</p>
      <li><p><b>Establezca un filtro o un grupo predeterminado para el widget:</b></p>
      <p>Pase el ratón sobre una opción y aparecerá un botón que le permitirá establecer esa opción como predeterminada para los usuarios. El valor predeterminado actual tendrá un distintivo predeterminado azul a su derecha.</li></p>
      <li><p><b>Agregue un filtro, una columna o un grupo existentes a la lista de opciones disponibles:</b></p>
      <p>Haga clic en el botón del signo más situado en la parte inferior de cada lista para agregar una opción a esa lista. Tenga en cuenta que solo los filtros, campos (para columnas) o grupos existentes se pueden agregar de esta manera.</p></li>
      </ul>
      <p>

>[!NOTE]
>
>Si establece un filtro o una agrupación predeterminados para un widget específico mediante una plantilla de diseño, es posible que no surta efecto inmediatamente debido a las preferencias de usuario existentes. Para aplicar el nuevo filtro o agrupación inmediatamente, es posible que usted o el usuario tengan que restablecer sus preferencias de usuario añadiendo &quot;/resetUser&quot; al final de su URL.

</p>
  </td> 
  </tr>
  </tbody> 
  </table>

1. Siga personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **Guardar** en la esquina inferior izquierda.

>[!IMPORTANT]
>
>Debe actualizar la nueva página de inicio para ver las personalizaciones de la plantilla de diseño.
