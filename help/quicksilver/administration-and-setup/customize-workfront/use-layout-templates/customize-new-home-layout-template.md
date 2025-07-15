---
title: Personalizar inicio mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Puede utilizar una plantilla de diseño para configurar lo que ven los usuarios al abrir Inicio en Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 39%

---

# Personalizar la página de inicio mediante una plantilla de diseño

Puede utilizar una plantilla de diseño para configurar lo que ven los usuarios la primera vez que abren Inicio.

Puede configurar lo siguiente:

* Qué widgets se muestran en el espacio de trabajo de forma predeterminada
* Qué fondo se selecciona
* Configuración de widgets específicos, incluidos los filtros y grupos disponibles para los widgets Mis proyectos, Mis tareas y Mis problemas, así como sus valores predeterminados

>[!IMPORTANT]
>
>Los usuarios finales pueden cambiar su fondo y reordenar los widgets de la página después de aplicar la plantilla de diseño. No pueden eliminar los widgets incluidos por un administrador de Workfront.
> 
>Los administradores tienen la capacidad de añadir nuevos widgets para los usuarios. Sin embargo, si un usuario final ya ha personalizado el orden de los widgets o la selección del fondo, esas personalizaciones específicas no se modifican.

Para obtener información sobre Inicio, consulte [Introducción a Inicio](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

Para obtener información sobre cómo crear plantillas de diseño, consulte [Crear y administrar plantillas de diseño](../use-layout-templates/create-and-manage-layout-templates.md).

Para obtener información acerca de las plantillas de diseño para grupos, consulte [Creación y modificación de las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Después de configurar una plantilla de diseño, debe asignarla a usuarios para que los cambios que ha realizado sean visibles para otros. Para obtener información acerca de cómo asignar una plantilla de diseño a los usuarios, consulte [Asignar usuarios a una plantilla de diseño](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
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

## Personalizar el Inicio con una plantilla de diseño

Para personalizar la página de inicio mediante una plantilla de diseño:

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Haga clic en la flecha abajo ![Flecha abajo](assets/dropdown-arrow.png) bajo **Personalizar lo que ven los usuarios** y, a continuación, haga clic en **Workspace doméstico**.

1. En las pestañas de la derecha, haga clic en una de las siguientes opciones:

   * **Diseño**: selecciona para elegir y organizar los widgets y el fondo
   * **Configuración del widget**: selecciónelo para administrar la configuración de widgets individuales, como los filtros y grupos disponibles.

   La siguiente tabla contiene detalles sobre cada pestaña:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Diseño y disposición</td> 
      <td>
      <p>Seleccione los widgets que se mostrarán en los espacios de trabajo de los usuarios, su posición y elija un fondo.</p> 
      <p>Tenga en cuenta que, aunque los usuarios no pueden eliminar los widgets seleccionados, pueden moverlos y cambiarles el tamaño libremente. También pueden agregar más widgets.</p>
      <p>Esta pestaña funciona esencialmente como una previsualización del espacio de trabajo de Inicio real que experimentarán los usuarios con esta plantilla de diseño.</p> 
      <p> Realice una de las siguientes acciones: </p>
      <ul><li>Personalice esta ficha según los pasos descritos en <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Agregar, editar o quitar widgets en Inicio</a>. </li>
      <li>Seleccione los widgets y organice el espacio de trabajo tal como desea que aparezca para los usuarios.</li>
      <li>Para cambiar el fondo, sigue los pasos de <b>Personalización del fondo</b> en <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">Introducción a la página principal</a>.</li></p>
      <p>

   >[!NOTE]
   >
   >Al mover o cambiar el tamaño de los widgets en la plantilla de diseño, las páginas de inicio de los usuarios no se almacenan en déclencheur para actualizar su diseño. Sin embargo, añadir o eliminar un widget almacenará activará una actualización de las páginas de los usuarios.

   </p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuración del widget</td> 
      <td>
      <p>Cambie la configuración de los widgets individuales.</p> 
      <p>

   >[!NOTE]
   >
   >Estas opciones no se extienden al panel Resumen. Debe configurar esa área en la pestaña Resumen de la plantilla de diseño.

   </p>
      <p> Seleccione entre los siguientes widgets de la lista a la izquierda:</p>
      <ul>
        <li>Mis proyectos</li>
        <li>Mis tareas</li>
        <li>Mis problemas</li>
      </ul>
      <p>Después de seleccionar el widget que desea editar, seleccione los <b>Filtros</b>, <b>Columnas</b> y <b>Grupos</b> que desea poner a disposición de Inicio a la derecha.</p>
      <p> Puede:</p>
      <ul>
      <li><p>Seleccione y ordene los filtros, columnas o grupos disponibles para los usuarios marcando la casilla junto a las opciones de la lista. Las opciones no seleccionadas no aparecerán para los usuarios.</p></li>
      <li> <p>Arrastre y suelte las opciones de la lista para establecer un orden.</p></li>
      <p>

   >[!IMPORTANT]
   >
   >* Las opciones Filtro, Columnas y Grupo están vinculadas a las opciones de personalización de la lista de la plantilla de diseño. Los cambios realizados aquí también se aplicarán a esa configuración.
   >* Los usuarios deben tener al menos acceso de creación a vistas para que la configuración de la columna del administrador se aplique correctamente a sus páginas de inicio.

   </p>
      <li><p>Defina un filtro o un grupo predeterminado para el widget pasando el puntero sobre una opción y haciendo clic en <b>Establecer como predeterminado</b>. El valor predeterminado actual muestra un distintivo <b>Default</b> azul a la derecha.</p></li>
      <li><p>Agregue un filtro, columna o grupo existente a la lista de opciones disponibles haciendo clic en el botón del signo más situado en la parte inferior de cada lista para agregar una opción a esa lista. Tenga en cuenta que solo los Filtros, Campos (para columnas) o Grupos existentes se pueden agregar de esta manera.</p></li>
      </ul>
      <p>

   >[!NOTE]
   >
   >Como resultado, si establece un filtro o una agrupación predeterminados para un widget específico mediante una plantilla de diseño, es posible que no surta efecto inmediatamente debido a las preferencias de usuario existentes. Para aplicar el nuevo filtro o agrupación inmediatamente, es posible que usted o el usuario tengan que restablecer sus preferencias de usuario añadiendo &quot;/resetUser&quot; al final de su URL.

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
   >Los usuarios deben actualizar su página de inicio para ver las personalizaciones de la plantilla de diseño.
