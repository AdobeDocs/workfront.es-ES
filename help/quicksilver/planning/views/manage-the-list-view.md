---
title: Administrar la vista de lista en Adobe Workfront Planning
description: Puede mostrar objetos y sus campos en una vista de lista, al acceder a ellos en la página Registros conectados de un registro, en Adobe Workfront Planning. Este artículo describe cómo se puede crear o editar una vista de lista en la página Registros conectados de un registro.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: 973a095e8ff08e382010247d9ed38e48d4b2c564
workflow-type: tm+mt
source-wordcount: '1342'
ht-degree: 1%

---


# Administrar la vista de lista en Adobe Workfront Planning

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

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

   <!--add new screen shot when they release Conditional formatting MVP -->

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
      >* <span class="preview">Puede restablecer una vista que se compartió con usted después de modificarla para restaurar sus preferencias originales, o bien puede copiarla con sus cambios y compartir la copia. Para obtener más información, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>

   1. Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png) para agregar un filtro a la vista. Los resultados se filtran inmediatamente en la lista. No puede guardar los filtros de nombre. Los filtros se recuerdan cuando acceda a la página en el futuro y forman parte de vistas compartidas.
   1. Haga clic en el icono **Columnas** ![Icono de columnas](assets/columns-icon.png) para seleccionar qué columnas mostrar u ocultar en la vista.
   1. Pase el ratón sobre el nombre de una columna, haga clic en la flecha hacia abajo situada a la izquierda del nombre de la columna y, a continuación, haga clic en una de las siguientes opciones:
      * **Cambiar nombre**, para agregar una **etiqueta personalizada** para la columna. El nombre del campo original en Workfront no cambia.
      * **Ordenar**, para ordenar la lista por el campo seleccionado. Se agrega un icono de ordenación que indica la dirección de la ordenación al encabezado de la columna.
   1. Haga clic en el icono **+** en la esquina superior derecha de la lista para agregar o quitar columnas y, a continuación, haga clic en **Guardar**.

      Se abre **Administrador de columnas**.

      Solo se pueden agregar campos existentes a la vista de lista.
No se puede quitar el campo principal en la vista de lista que aparece en la primera columna.


   1. <span class="preview">Haga clic en el icono **Formato de celdas** ![Formato de celdas](assets/format-cells-icon.png). Se abre el cuadro **Formato**.</span> <!--change the name of the box when they update it-->
      <span class="preview">Haga lo siguiente: </span>

      <div class="preview">

      1. En la línea **If**, haga clic en **Agregar condición**, seleccione un campo al que desee dar formato y elija un valor de campo.

         >[!TIP]
         >
         >Solo los campos visibles en la vista de lista están disponibles para el formato condicional.

      1. (Opcional) Haga clic en **Agregar condición** en la línea **If** para agregar más condiciones a la misma regla.

         >[!TIP]
         >
         >Puede agregar hasta 10 condiciones en una regla de condicionamiento y hasta 20 reglas para un campo.

      1. Haga clic en el conector **Or** entre condiciones para cambiar a **And** e indicar que se deben cumplir varias condiciones al mismo tiempo. **Or** es el conector predeterminado.
      1. En la línea **Format**, seleccione un campo para indicar a qué columna se dará formato. <!--edit this area, if it changes names??-->
      1. (Opcional) Haga clic en el icono **círculo de color** ![icono de círculo de color](assets/color-circle.png) junto al campo seleccionado, para expandirlo y elegir otro color.
      1. Active la opción **Aplicar a fila** para aplicar el formato a toda la fila del campo que cumpla las condiciones.
      1. (Opcional) Haga clic en **Agregar condición** en el cuadro **Formato** para agregar otra regla para otro campo y, a continuación, repita los pasos anteriores.
      1. (Opcional) Haga clic en **Borrar todo** para quitar todo el formato.
      1. Haga clic fuera del cuadro **Formato** para cerrarlo.

         Esto le devuelve a la vista de lista.
El formato se aplica inmediatamente a la vista de lista.
Hay un punto azul al lado del icono **Formato de celdas** para indicar que la vista tiene un formato especial aplicado.

      </div>

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

