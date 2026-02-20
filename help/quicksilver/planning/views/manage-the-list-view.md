---
title: Administrar la vista de lista en Adobe Workfront Planning
description: Puede mostrar objetos y sus campos en una vista de lista, al acceder a ellos en la página Registros conectados de un registro, en Adobe Workfront Planning. Este artículo describe cómo se puede crear o editar una vista de lista en la página Registros conectados de un registro.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: a5f33f914dabaa9368dea919510375bcb6ee03e2
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 2%

---


# Administrar la vista de lista en Adobe Workfront Planning

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Puede mostrar objetos y sus campos en una vista de lista, al acceder a ellos en la página Registros conectados de un registro, en Adobe Workfront Planning.

Este artículo describe cómo se puede crear o editar una vista de lista en la página Registros conectados de un registro y cómo se pueden editar los objetos de la vista.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier Workfront y cualquier paquete de Planning</p>
<p>Cualquier flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p> Estándar para crear y eliminar vistas</p>
   <p>Colaborador o superior para actualizar los elementos de vista</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración de una vista</p>  
   <p>Ver permisos en una vista para cambiar temporalmente la configuración de la vista o para duplicarla</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> A los usuarios con una licencia Light o Contributor se les debe asignar una plantilla de diseño que incluya Planning.
   <p>Los usuarios estándar y los administradores del sistema tienen las áreas de Planning habilitadas de forma predeterminada.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

## Consideraciones sobre las vistas de lista

* No puede ver registros en las páginas de tipo de registro en una vista de lista. Sólo se pueden mostrar los objetos siguientes en una vista de lista cuando se ven en la página Registros conectados de un registro:

   * Proyectos Workfront

  Para obtener información acerca de cómo crear una página de registros conectados, vea [Agregar una página de registros conectados a un registro](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
* Para poder ver una vista de lista en una página de registros conectada de un registro, debe conectar los proyectos de Workfront con los tipos de registros de Planning. Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).
* Las vistas de lista son similares a las listas mejoradas. Para obtener más información, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


## Administración de una vista de lista {#manage-a-list-view}

Para obtener más información sobre cómo administrar vistas de listas en Workfront, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

{{step1-to-planning}}

1. Haga clic en una tarjeta de espacio de trabajo y, a continuación, haga clic en una tarjeta de tipo de registro.
1. Desde cualquier vista, haga clic en el nombre de un registro para abrir la página de vista previa o de detalles del registro.
1. Agregue una **página Registros conectados** para proyectos conectados como se describe en el artículo [Agregar una página Registros conectados a un registro](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

   La página Registros conectados muestra los proyectos conectados al registro en la vista de lista.

   <!--add new screen shot when they release Row colors/ special formatting for rows-->

   ![Proyectos en la página de registros conectados en la vista de lista](assets/projects-on-connected-records-page-list-view.png)

1. (Opcional) Realice una de las siguientes acciones para modificar la vista de lista:

   1. Expanda el menú de vistas desplegables en la esquina superior derecha de la lista para seleccionar otra vista, o haga clic en **Nueva vista** y cree otra.

      Las vistas se comparten en todo el sistema. Si crea una vista Proyectos para un tipo de registro, puede verla en otros tipos de registro que muestran proyectos conectados.

   1. Pase el ratón sobre el nombre de una vista existente y haga clic en el menú **Más** ![Menú más](assets/more-menu.png); a continuación, haga clic en una de las siguientes opciones:
      * **Cambiar nombre**, para asignar un nuevo nombre a la vista
      * **Compartir**, para compartir la vista con otros
      * **Eliminar**, para eliminar la vista.

      >[!NOTE]
      >
      >* Debe tener permisos de administración en una vista para poder editarla, compartirla o eliminarla.
      >
      >* No puede modificar Vistas del sistema.
      >
      <!--* <span class="preview">You can reset a view that was shared with you after you modified it to restore its original preferences, or you can copy it with your changes and share the copy. For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
        -->
   1. Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png) para agregar un filtro a la vista. Los resultados se filtran inmediatamente en la lista. No puede guardar los filtros de nombre. Los filtros se recuerdan cuando acceda a la página en el futuro y forman parte de vistas compartidas.
   1. Haga clic en el icono **Columnas** ![Icono de columnas](assets/columns-icon.png) para seleccionar qué columnas mostrar u ocultar en la vista.
   1. Pase el ratón sobre el nombre de una columna, haga clic en la flecha hacia abajo situada a la izquierda del nombre de la columna y, a continuación, haga clic en una de las siguientes opciones:
      * **Cambiar nombre**, para agregar una **etiqueta personalizada** para la columna. El nombre del campo original en Workfront no cambia.
      * **Ordenar**, para ordenar la lista por el campo seleccionado. Se agrega un icono de ordenación que indica la dirección de la ordenación al encabezado de la columna.
   1. Haga clic en el icono **+** en la esquina superior derecha de la lista para agregar o quitar columnas y, a continuación, haga clic en **Guardar**.

      Se abre **Administrador de columnas**.

      Solo se pueden agregar campos existentes a la vista de lista.
No se puede quitar el campo principal en la vista de lista que aparece en la primera columna.


   <!--
    1. <span class="preview">Click **Row colors** <!-insert icon and edit the name of the icon if they changed it->. The **Format** box opens. <!-change the name of the box when they update it-></span>
        <span class="preview">Do the following: </span>
        <div class="preview">
        1. Define the formatting conditions in the **If** area by clicking **Add condition**, then select a field you want to format by and choose a field value. 
            >[!TIP]
            >
            >Only field visible in the list view are available for conditional formatting.
        1. (Optional) Click **Add condition** in the If area to add more conditions. 
        1. Click the **Or** connector between conditions to change to **And**. **Or** is the default connector.  
        1. In the **Format** area, select a field to indicate which column will be formatted. <!-edit this area, if it changes names???->
        1. Click on the color circle to expand and choose another color.
        1. Turn on the **Apply to row** setting to apply the formatting to the entire row that meets the conditions. 
        1. (Optional) Click **Clear all** to remove all formatting.
            The formatting is applies immediately.
        1. Click outside the **Format** box to close it. 
            This returns you to the list view. There is a blue dot next to the **Row colors** icon to indicate that the view has special formatting applied. <!-might need to edit the icon name and get a screen shot of the icon with the dot and insert it here->
        </div>
    -->

1. (Opcional) Agregue una palabra clave al cuadro de búsqueda en la esquina superior derecha de la lista para buscar un elemento.


   Los elementos que coincidan con el término de búsqueda se resaltarán en la lista.
1. (Opcional) Para agregar más elementos a la lista y conectarlos automáticamente al registro seleccionado, realice una de las siguientes acciones:

   * Haga clic en **Conectar registros** en la esquina superior derecha de la lista para agregar los elementos existentes.
   * Haga clic en **Nueva fila** al final de la lista para agregar nuevos elementos.
1. Haga clic en el nombre de un elemento conectado en la lista para abrirlo en otra ficha del explorador.
1. Haga doble clic dentro de una celda de la lista para editar la información de un campo y, a continuación, pulse Intro para guardar los cambios.

   Algunos campos son de solo lectura. Por ejemplo, el porcentaje completado de un proyecto es un campo calculado por el sistema y no se puede editar manualmente.

1. Pase el ratón sobre el nombre de un elemento en la lista y haga clic en el menú **Más** [Menú más](assets/more-menu.png) y luego haga clic en **Ver** para abrir el proyecto en otra pestaña

   O

   Seleccione uno o varios elementos, observe la barra de acciones situada en la parte inferior de la lista y, a continuación, haga clic en una de las siguientes opciones:

   * **Eliminar** para eliminar el proyecto. Al eliminar un proyecto, se desconecta del registro y se mueve a la papelera de reciclaje de Workfront. Los administradores de Workfront pueden recuperar los proyectos eliminados hasta 30 días después de haberlos eliminado.
   * **Desconectar** para desconectar el proyecto del registro. Al desconectar un proyecto, éste y todos los valores de sus campos de búsqueda se eliminan del registro actual.

   ![Barra de acciones en la vista Lista de páginas de registros conectados](assets/actions-bar-connected-records-page-list-view.png)

