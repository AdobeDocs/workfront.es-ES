---
title: Crear tipos de registro
description: Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear tipos de registros personalizados que ilustren los elementos de trabajo necesarios en el ciclo de vida de su organización.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 476e10f2962f19fd17705cb5f20619d3b636aaa4
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 13%

---


<!--this is linked to the UI in an empty workspace screen-->

<!--keep the yellow for cross-workspace functionality till Jan 2026-->

# Crear tipos de registro

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear tipos de registros personalizados que ilustran los elementos relacionados con el trabajo necesarios en el ciclo de vida de su organización.

Para obtener más información acerca de los tipos de registros, vea [Información general sobre los tipos de registros](/help/quicksilver/planning/architecture/overview-of-record-types.md).

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
<p>Cualquier paquete de Workfront y Planning</p>
<p>Cualquier paquete de flujo de trabajo y planificación</p>
<p><b>NOTA</b></p>
<p>Para configurar tipos de registros conectables: </p>
<ul> 
<li><p>Cualquier paquete Workfront y cualquier paquete Planning</p></li>
O
<li><p>Cualquier flujo de trabajo y un paquete de Planning Prime o Ultimate</p></li></ul>

<div class="preview">
<p>Para configurar tipos de registros globales:</p>

<ul> 
<li><p>Cualquier paquete Workfront y un paquete Planning Plus</p></li>
O
<li><p>Cualquier flujo de trabajo y un paquete de Planning Prime o Ultimate</p></li></ul>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p>

</div>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administración de permisos en un espacio de trabajo</p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
</tbody> 
</table> -->

## Consideraciones sobre la creación de tipos de registros

* Puede crear tipos de registros en un espacio de trabajo de las siguientes maneras:

   * Automáticamente:
      * Cuando se crea un espacio de trabajo mediante una plantilla.

        Para obtener más información, consulte [Crear espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Al importarlos mediante un archivo CSV o de Excel.

        Para obtener más información, vea [Crear tipos de registros importando información desde un archivo CSV o de Excel](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

     >[!TIP]
     >
     >Al importar un tipo de registro desde un archivo CSV o de Excel, también puede importar registros y campos.

   * Manualmente:

      * Desde cero

        Este artículo describe cómo crear tipos de registros desde cero.

      * <span class="preview">Agregándolos desde otro espacio de trabajo</span>
        <span class="preview">Para obtener más información, vea [Agregar tipos de registros existentes desde otro área de trabajo](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md). </span>


* Puede mover tipos de registros dentro de una sección y de una sección de un espacio de trabajo a otra. No se pueden mover tipos de registros de un espacio de trabajo a otro.

## Creación de tipos de registros con una plantilla de Workspace

Puede crear tipos de registros automáticamente al crear un espacio de trabajo con una plantilla de Workfront Planning. Cada plantilla contiene tipos de registro de ejemplo.

Para obtener información acerca de cómo crear espacios de trabajo, vea [Crear espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

Para obtener información sobre los tipos de registros que se incluyen en cada plantilla, vea [Lista de plantillas de área de trabajo](/help/quicksilver/planning/architecture/workspace-templates.md).

Al crear un espacio de trabajo a partir de una plantilla, los tipos de registro se agrupan en las siguientes secciones:

* Tipos de registros operativos
* Taxonomías

Puede añadir manualmente tipos de registros en las secciones Tipos de registros operativos y Taxonomías. Para obtener más información, vea la sección [Crear un registro desde cero](#create-a-record-type-from-scratch) en este artículo.

## Crear un tipo de registro desde cero

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee crear un tipo de registro,

   O

   Desde un espacio de trabajo, expanda la flecha hacia abajo situada a la derecha del nombre de un espacio de trabajo existente, busque un espacio de trabajo y, a continuación, selecciónelo cuando se muestre en la lista.
1. (Opcional) Haga clic en **Agregar sección** para agregar una nueva sección al área de trabajo.
1. Haga clic en **Agregar tipo de registro** y luego en **Agregar manualmente**.

   Se abre el cuadro Agregar tipo de registro.

   ![Agregar cuadro de tipo de registro con opciones de apariencia](assets/add-record-type-box-with-appearance-options.png)

1. Actualice la siguiente información en la ficha **Apariencia**:

   * Sustituya &quot;Tipo de registro sin título&quot; por el nombre del tipo de registro futuro. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Descripción**: Agregue más información sobre el tipo de registro.
   * Seleccione un color y una forma para el icono asociado al tipo de registro. Haga lo siguiente:
      * Seleccione un color para identificar el nuevo tipo de registro. Este es el color del icono de tipo de registro. Gris está seleccionado de forma predeterminada.
      * Seleccione un icono de la lista o empiece a escribir el nombre de un icono en el campo de búsqueda para describir lo que representa y, a continuación, selecciónelo cuando se muestre. Este es el icono del tipo de registro. De forma predeterminada, se selecciona un icono de archivo.

1. (Opcional y condicional) Si es administrador del sistema, haga clic en la pestaña **Configuración avanzada** <span class="preview">o **Configuración en todo el espacio de trabajo**</span> y <span class="preview">actualice la información sobre las capacidades en todo el espacio de trabajo del tipo de registro.

   ![Editar cuadro de tipo de registro con ficha de configuración avanzada](assets/edit-record-type-box-advanced-settings-tab.png) </span>

   Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

1. Haga clic en **Guardar**.

   La tarjeta de tipo de registro se añade a la sección y al espacio de trabajo seleccionado.
La descripción del tipo de registro se muestra en la tarjeta.

   ![Tarjeta de tipo de registro con descripción](assets/record-type-card-with-description.png)

   Si seleccionó conectar este registro desde otros espacios de trabajo, se mostrará el icono **Registro conectable** ![Conectarse desde otros espacios](assets/connect-from-other-workspaces-icon.png) en la tarjeta de registro.

   <span class="preview">Si ha seleccionado permitir la adición de este registro a otros espacios de trabajo, se muestra el icono **Registro global** ![Icono de tipo de registro global](assets/global-icon.png) en la tarjeta de registro. </span>

1. (Opcional) Pase el ratón sobre la tarjeta de tipo de registro, haga clic en el icono **Más** ![Menú más](assets/more-menu.png) en la esquina superior derecha y, a continuación, haga clic en **Editar** o <span class="preview">**Configuración**</span> para modificar la información sobre el tipo de registro.

   Para obtener más información, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Opcional) Haga clic en la tarjeta de tipo de registro para abrir la página de tipo de registro.

   ![Tipo de registro operativo en blanco](assets/operational-record-type-blank.png)

   La página de tipo de registro se muestra en la vista de tabla de forma predeterminada. Las columnas de la tabla son campos asociados al nuevo tipo de registro. Cada fila es un registro único que debe agregar.

   De forma predeterminada, los campos siguientes se muestran en las columnas de la vista de tabla de un tipo de registro operativo:

   * Nombre
   * Descripción
   * Fecha de inicio
   * Fecha de finalización
   * Estado

1. (Opcional) Actualice el nombre del tipo de registro en el encabezado de la página

   O

   Haga clic en el icono **Más** ![Menú más](assets/more-menu.png) a la derecha del nombre del tipo de registro y haga clic en **Editar** para cambiarle el nombre o cambiar la información sobre él. Para obtener más información, vea [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Opcional) Haga clic en **+ Nuevo registro** para agregar registros del tipo de registro seleccionado. Para obtener más información, consulte [Creación de registros](/help/quicksilver/planning/records/create-records.md).
1. (Opcional) Haga clic en el icono **+** en la esquina superior derecha de la tabla para agregar más campos al tipo de registro.

   Para obtener más información sobre cómo crear campos, vea [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

1. (Opcional) Haga clic en la flecha que señala a la izquierda del nombre del tipo de registro, en el encabezado, para volver al espacio de trabajo seleccionado.

1. (Opcional) En el espacio de trabajo, haga clic y mantenga pulsada una tarjeta de tipo de registro para arrastrar y soltar el tipo de registro en un punto deseado o para moverlo a otra sección.

   Los cambios se guardan automáticamente.

   Para obtener información adicional sobre cómo agregar registros, eliminar o editar tipos de registros, o actualizar la vista en la página de tipo de registro, vea los siguientes artículos:

   * [Crear registros](/help/quicksilver/planning/records/create-records.md)
   * [Eliminar tipos de registro](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Editar tipos de registro](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md)

## Crear tipos de registros importando información desde un archivo CSV o de Excel

Al importar información desde un archivo CSV o de Excel, puede importar lo siguiente:

* Tipos de registro
* Registros
* Campos de registro

Para obtener más información, vea [Crear tipos de registros importando información desde un archivo CSV o de Excel](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

<div class="preview">

## Crear tipos de registros agregando los existentes de otro espacio de trabajo

Puede agregar tipos de registros a un espacio de trabajo agregando los existentes desde otro espacio de trabajo. Sólo se pueden agregar tipos de registros que se hayan configurado como tipos de registros globales.

Para obtener más información, vea [Agregar tipos de registros existentes desde otro área de trabajo](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

</div>