---
title: Administrar la vista de lista en Adobe Workfront Planning
description: Puede mostrar objetos y sus campos en una vista de lista, al acceder a ellos en la página Registros conectados de un registro, en Adobe Workfront Planning. Este artículo describe cómo se puede crear o editar una vista de lista en la página Registros conectados de un registro.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: a6c2bc4127a52fad209004995ea2262fa64c240d
workflow-type: tm+mt
source-wordcount: '1791'
ht-degree: 1%

---


# Administrar la vista de lista en Adobe Workfront Planning

<!--
although list views in Planning are very similar to Workfront enhanced lists, keep this one separate with all the information, because of Planning standalone; some information here is also duplicated in this main Glist article: help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md
-->

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Puede ver objetos en la vista de lista en las siguientes áreas de Workfront Planning:

* Página de registros conectada para proyectos en el área de detalles de un registro

  ![Proyectos en la página de registros conectados en la vista de lista](assets/projects-on-connected-records-page-list-view.png)

* Una lista de formularios de solicitud en el nivel de tipo de registro

  ![Solicitar formularios en la vista de lista](assets/request-forms-in-list-view.png)

En este artículo se describe cómo desplazarse, crear o editar una vista de lista en Workfront Planning.

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

* Tenga en cuenta lo siguiente para la vista de lista de páginas de registros conectados:

   * Sólo se pueden ver proyectos en la vista de lista de la página de registros conectados de un registro. La vista de lista no está disponible para ningún otro tipo de objeto o registro de una página de registros conectada.

  Para obtener información acerca de cómo crear una página de registros conectados, vea [Agregar una página de registros conectados a un registro](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
   * Para poder ver una vista de lista en una página de registros conectada de un registro, debe conectar los proyectos de Workfront con los tipos de registros de Planning. Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).
   * Puede crear varias vistas de lista para proyectos en la página de registros conectados de un registro.

* Tenga en cuenta lo siguiente para la vista de lista de formularios de solicitud:

   * No se pueden crear ni editar vistas de lista adicionales para formularios de solicitud de Planning. Workfront crea una vista de lista para los formularios de solicitud. <!--this will change-->

     Para obtener información acerca de los formularios de solicitud, vea [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* Dependiendo de dónde se muestre, no todas las vistas de lista tienen todos los elementos descritos en este artículo.

## Administración de una vista de lista {#manage-a-list-view}

Las vistas de lista de Workfront Planning son similares a las listas mejoradas de Workfront. La mayoría de los elementos de las vistas mejoradas también existen en las vistas de lista de Workfront Planning.

Para obtener más información, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!--
Removed - more direct steps below: 
{{step1-to-planning}}

1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card. 
    1. From any view, click the name of a record to open the record's preview or details page. 
    1. Add a **Connected records page** for connected projects as described in the article [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

    The Connected records page displays projects connected to the record in the list view. 

    ![Projects on connected records page in list view](assets/projects-on-connected-records-page-list-view.png)

1. (Conditional) To access a list of request forms, do the following: 

    1. {{step1-to-planning}}

    1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card.
    1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the header, then click **Manage request forms**.

        A list of request forms displays.

-->

1. Vaya a una vista de lista en una de las siguientes áreas:

   * Página de registros conectada para proyectos en el área de detalles de un registro
   * La página Formularios de solicitud de un tipo de registro

1. (Condicional) Cuando esté disponible, realice una de las siguientes acciones para modificar la vista de la lista:

   1. Expanda el menú de vistas desplegables en la esquina superior izquierda de la lista para seleccionar otra vista, o haga clic en **Nueva vista** y cree otra.

      >[!TIP]
      >
      >Las vistas se comparten en todo el sistema. Si crea una vista Proyectos para un tipo de registro, puede verla en otros tipos de registro que muestran proyectos conectados.

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
      >* Puede restablecer una vista que se haya compartido con usted y para la que solo tenga permisos de Vista, después de modificarla para restaurar sus preferencias originales, o puede copiarla con los cambios y compartir la copia. Para obtener más información, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

   1. Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png) para agregar un filtro a la vista. Los resultados se filtran inmediatamente en la lista. No puede guardar los filtros de nombre. Los filtros se recuerdan cuando acceda a la página en el futuro y forman parte de vistas compartidas.

      >[!TIP]
      >
      >Para aplicar un filtro personalizado, seleccione una de las siguientes opciones para un valor de campo:
      >
      >* **Yo (usuario conectado)** para hacer referencia al usuario conectado en los campos que hacen referencia a los usuarios.
      >
      >* **Mis equipos** o **Mi equipo de inicio** para hacer referencia a sus equipos en campos que hacen referencia a equipos.
      >
      >* **Mis grupos** o **Mi grupo de inicio** para hacer referencia a sus grupos en campos que hacen referencia a grupos.
      >
      >* **Mi compañía** para hacer referencia a su compañía en campos que hacen referencia a compañías.
      > 
      >* **Mis roles** o **Mi rol principal** para hacer referencia a sus roles en los campos que hacen referencia a los roles.

   1. Haga clic en el icono **Columnas** ![Icono de columnas](assets/columns-icon.png) para seleccionar qué columnas mostrar u ocultar en la vista.
   1. Pase el ratón sobre el nombre de una columna, haga clic en la flecha hacia abajo situada a la izquierda del nombre de la columna y, a continuación, haga clic en una de las siguientes opciones:
      * **Cambiar nombre**, para agregar una **etiqueta personalizada** para la columna. El nombre del campo original en Workfront no cambia.
      * **Ordenar**, para ordenar la lista por el campo seleccionado. Se agrega un icono de ordenación que indica la dirección de la ordenación al encabezado de la columna.
   1. Haga clic en el icono **+** en la esquina superior derecha de la lista para agregar o quitar columnas y, a continuación, haga clic en **Guardar**.

      Se abre **Administrador de columnas**.

      Solo se pueden agregar campos existentes a la vista de lista.
No se puede quitar el campo principal en la vista de lista que aparece en la primera columna.

   1. Haga clic en el icono **Formato de celdas** ![Formato de celdas](assets/format-cells-icon.png). Se abre el cuadro **Formato**. <!--change the name of the box when they update it-->
Haga lo siguiente:

      1. Haga clic en **Agregar condición**.
      1. En la línea **If**, seleccione un campo, elija un valor de campo y agregue un modificador. Los modificadores cambian según el tipo de campo elegido.

         >[!TIP]
         >
         >Solo los campos visibles en la vista de lista están disponibles para el formato condicional.

      1. (Opcional) En lugar de agregar un valor de campo, haga clic en el icono **Comparar con otro campo** ![Comparar con otro campo](assets/compare-to-another-field-icon.png) y elija un campo cuyo valor desee comparar con el valor del campo seleccionado. Por ejemplo, puede comparar los campos Propietario del proyecto y Patrocinador del proyecto.

         >[!TIP]
         >
         >Solo los campos visibles en la vista de lista están disponibles para el formato condicional. Los campos que compare deben ser del mismo tipo.

      1. (Opcional) Haga clic en **Agregar condición** en la línea **If** para agregar más condiciones a la misma regla.

         >[!TIP]
         >
         >Puede agregar hasta 10 condiciones en una regla de condicionamiento y hasta 20 reglas para un campo.

      1. Haga clic en el conector **Or** entre condiciones para cambiar a **And** e indicar que se deben cumplir varias condiciones al mismo tiempo. **Or** es el conector predeterminado.
      1. En la línea **Format**, seleccione un campo para indicar a qué columna se dará formato. <!--edit this area, if it changes names??-->
      1. (Opcional) Haga clic en el icono **círculo de color** ![icono de círculo de color](assets/color-circle.png) junto al campo seleccionado, para expandirlo y elegir otro color en el área **Relleno de celda** para cambiar el color del fondo de una celda o elegir un color del área **Color de texto** para cambiar el color del texto de una celda.
      1. Haga clic en el icono **Formato de texto** ![Icono de formato de texto](assets/text-format-icon.png) y seleccione una de las siguientes opciones para dar formato al texto en una celda:
         * Negrita
         * Cursiva

      1. Active la opción **Aplicar a fila** para aplicar el formato a toda la fila del campo que cumpla las condiciones.
      1. (Opcional) Haga clic en **Agregar condición** en el cuadro **Formato** para agregar otra regla para otro campo y, a continuación, repita los pasos anteriores.
      1. (Opcional) Haga clic en **Borrar todo** para quitar todo el formato.
      1. Haga clic fuera del cuadro **Formato** para cerrarlo.

         Esto le devuelve a la vista de lista.
El formato se aplica inmediatamente a la vista de lista.
Hay un punto azul al lado del icono **Formato de celdas** para indicar que la vista tiene un formato especial aplicado.

   1. (Opcional) Haga clic en el icono **Agrupación** ![Icono de agrupación](assets/grouping-icon.png) <!--have they updated this to "Grouping"??--> para agrupar los elementos de la lista por un campo común. Seleccione una de las opciones o utilice la barra de búsqueda para buscar un campo.

      El campo debe ser una columna de la lista para poder agrupar por él. No todos los tipos de campo se pueden usar para agrupaciones.

   1. Haga clic en el icono **Alto de fila** ![Icono de alto de fila](assets/row-height-icon.png) para actualizar la longitud vertical de una fila. Elija entre las siguientes opciones:

      * Baja
      * Estándar. Esta es la opción predeterminada.
      * Media
      * Alta

   <!--leave these here, although they duplicate for Enhanced lists in Workfront-->

1. (Opcional) Agregue una palabra clave al cuadro de búsqueda en la esquina superior derecha de la lista para buscar un elemento.

   Los elementos que coincidan con el término de búsqueda se resaltarán en la lista.

1. (Opcional y condicional) En la página conectada de los proyectos <!--change projects to items here when more items will display in the Glist-->, para agregar más elementos a la lista y conectarlos automáticamente al registro seleccionado, realice una de las siguientes acciones:

   * Haga clic en **Conectar registros** en la esquina superior derecha de la lista para agregar los elementos existentes.
   * Haga clic en **Nueva fila** al final de la lista para agregar nuevos elementos.
1. Haga clic en el nombre de un elemento conectado en la lista para abrirlo en otra ficha del explorador.
1. Haga doble clic dentro de una celda de la lista para editar la información de un campo y, a continuación, pulse Intro para guardar los cambios.

   Algunos campos son de solo lectura. Por ejemplo, el porcentaje completado de un proyecto es un campo calculado por el sistema y no se puede editar manualmente.

1. Pase el ratón sobre el nombre de un elemento en la lista y haga clic en el menú **Más** [Menú más](assets/more-menu.png) y luego haga clic en **Ver** para abrir el proyecto en otra pestaña

   O

   Seleccione uno o varios elementos, observe la barra de acciones situada en la parte inferior de la lista y, a continuación, haga clic en uno de los siguientes, cuando esté disponible. Según el área desde la que acceda a la vista de lista, haga clic en una de las siguientes opciones:

   * **Eliminar** para eliminar el elemento. Al eliminar un proyecto, se desconecta del registro y se mueve a la papelera de reciclaje de Workfront. Los administradores de Workfront pueden recuperar los proyectos eliminados hasta 30 días después de haberlos eliminado. Al eliminar un formulario, no se eliminan las solicitudes ni los registros creados cuando se envió el formulario.
   * **Desconectar** para desconectar el proyecto del registro. Al desconectar un proyecto, éste y todos los valores de sus campos de búsqueda se eliminan del registro actual.

     <!--update screen shot at preview release-->

     ![Barra de acciones en la vista Lista de páginas de registros conectados](assets/actions-bar-connected-records-page-list-view.png)

   * **Editar formulario**: abre un formulario de solicitud de Planning y le permite editarlo.
   * **Cancelar publicación**: cancela la publicación de un formulario de solicitud. Esto quita el formulario del área de solicitudes y los usuarios ya no pueden agregar solicitudes a este tipo de registro.
   * **Compartir**: abre el cuadro Compartir de un formulario de solicitud donde puede compartir con otros usuarios.
   * **Copiar vínculo**: copia un vínculo a un formulario de solicitud de Planning para que pueda compartirlo con otros usuarios. Si el formulario se comparte públicamente, puede compartir el vínculo con usuarios que no pertenezcan a Workfront Planning.

     ![Barra de acciones en la lista de solicitudes de Planning](assets/actions-bar-in-inake-forms-list.png)



