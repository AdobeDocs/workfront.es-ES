---
title: Crear tipos de registro
description: Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear tipos de registros personalizados que ilustren los elementos de trabajo necesarios en el ciclo de vida de su organización.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 0da877936ba8f52341a5b151f76710c979ce9294
workflow-type: tm+mt
source-wordcount: '1453'
ht-degree: 1%

---


<!--this is linked to the UI in an empty workspace screen-->

# Creación de tipos de registros

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede crear tipos de registros personalizados que ilustran los elementos relacionados con el trabajo necesarios en el ciclo de vida de su organización.

Para obtener más información acerca de los tipos de registros, vea [Información general sobre los tipos de registros](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Productos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planificación de Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>plan Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia Adobe unificado para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiencia unificada de Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Estándar</p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administrar permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Consideraciones sobre la creación de tipos de registros

* Puede crear tipos de registros en un espacio de trabajo de las siguientes maneras:

   * Automáticamente:
      * Cuando se crea un espacio de trabajo mediante una plantilla.

        Para obtener más información, consulte [Crear espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

      * <span class="preview">Al importarlos mediante un archivo de Excel o CSV. </span>

     >[!TIP]
     >
     ><span class="preview">Al importar un tipo de registro desde un archivo de Excel o CSV, también se pueden importar registros y campos.</span>

   * Manualmente:

      * Desde cero.

        Este artículo describe cómo crear tipos de registros desde cero.

* Puede mover tipos de registros dentro de una sección y de una sección de un espacio de trabajo a otra. No se pueden mover tipos de registros de un espacio de trabajo a otro.

## Creación de tipos de registros con una plantilla de Workspace

Puede crear tipos de registros automáticamente al crear un espacio de trabajo con una plantilla de Workfront Planning. Cada plantilla contiene tipos de registro de ejemplo.

Al crear un espacio de trabajo a partir de una plantilla, los tipos de registro se agrupan en las siguientes secciones:

* Tipos de registros operativos
* Taxonomías

Puede añadir manualmente tipos de registros en las secciones Tipos de registros operativos y Taxonomías.

Para obtener información acerca de cómo crear espacios de trabajo, vea [Crear espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

Para obtener información sobre los tipos de registros que se incluyen en cada plantilla, vea [Lista de plantillas de área de trabajo](/help/quicksilver/planning/architecture/workspace-templates.md).

## Crear un tipo de registro desde cero

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee crear un tipo de registro,

   O

   Desde un espacio de trabajo, expanda la flecha hacia abajo a la derecha del nombre de un espacio de trabajo existente, busque un espacio de trabajo y selecciónelo cuando se muestre en la lista.
1. (Opcional) Haga clic en **Agregar sección** para agregar una nueva sección al área de trabajo.
1. Haga clic en **Agregar tipo de registro** y luego en <span class="preview">**Nuevo**</span>.

   Se abre el cuadro Agregar tipo de registro.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Actualice la siguiente información:

   * Sustituya &quot;Tipo de registro sin título&quot; por el nombre del tipo de registro futuro. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Descripción**: Agregue más información sobre el tipo de registro.
   * Seleccione un color y una forma para el icono asociado al tipo de registro. Haga lo siguiente:
      * Seleccione un color para identificar el nuevo tipo de registro. Es el color del icono de tipo de registro. Gris está seleccionado de forma predeterminada.
      * Seleccione un icono de la lista o empiece a escribir el nombre de un icono para describir lo que representa y, a continuación, selecciónelo cuando se muestre. Este es el icono del tipo de registro. De forma predeterminada, se selecciona un icono de archivo.

1. Haga clic en **Crear**.

   La tarjeta de tipo de registro se añade a la sección y al espacio de trabajo seleccionado.
La descripción del tipo de registro se muestra en la tarjeta.

   ![](assets/record-type-card-with-description.png)

1. (Opcional) Pase el ratón sobre la tarjeta de tipo de registro, haga clic en el icono **Más** ![](assets/more-menu.png) en la esquina superior derecha y, a continuación, haga clic en **Editar** para modificar la información sobre el tipo de registro.
1. (Opcional) Haga clic en la tarjeta de tipo de registro para abrir la página de tipo de registro.

   ![](assets/operational-record-type-blank.png)

   La página de tipo de registro se muestra en la vista de tabla de forma predeterminada. Las columnas de la tabla son campos asociados al nuevo tipo de registro. Cada fila es un registro único que debe agregar.

   De forma predeterminada, los campos siguientes se muestran en las columnas de la vista de tabla de un tipo de registro operativo:

   * Nombre
   * Descripción
   * Fecha de inicio
   * Fecha de finalización
   * Estado

1. (Opcional) Actualice el nombre del tipo de registro en el encabezado de la página

   O

   Haga clic en el icono **Más** ![](assets/more-menu.png) a la derecha del nombre del tipo de registro y haga clic en **Editar** para cambiarle el nombre o cambiar la información sobre él. Para obtener más información, vea [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Opcional) Haga clic en **+ Nuevo registro** para agregar registros del tipo de registro seleccionado. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).
1. (Opcional) Haga clic en el icono **+** en la esquina superior derecha de la tabla para agregar más campos al tipo de registro.

   Para obtener más información sobre cómo crear campos, vea [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

1. (Opcional) Haga clic en la flecha que señala a la izquierda del nombre del tipo de registro, en el encabezado, para volver al espacio de trabajo seleccionado.

1. (Opcional) En el espacio de trabajo, haga clic y mantenga pulsada una tarjeta de tipo de registro para arrastrar y soltar el tipo de registro en un punto deseado o para moverlo a otra sección.

   Los cambios se guardan automáticamente.

   Para obtener información adicional sobre cómo agregar registros, eliminar o editar tipos de registros, o actualizar la vista en la página de tipo de registro, vea los siguientes artículos:

   * [Creación de registros](/help/quicksilver/planning/records/create-records.md)
   * [Eliminar tipos de registros](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md)

<div class="preview">

## Creación de tipos de registros importando un archivo CSV o de Excel

Tenga en cuenta lo siguiente al importar tipos de registros mediante un archivo CSV o de Excel:

* Cada hoja del archivo de Excel se convierte en un tipo de registro. El nombre de la hoja se convierte en el nombre del tipo de registro.
* Si sólo hay una hoja o si importa un archivo CSV, el nombre del archivo se convierte en el nombre del tipo de registro.
* Los encabezados de columna de cada hoja se convierten en los campos asociados a cada tipo de registro.
* Los campos son únicos para sus respectivos tipos de registros.
* Cada fila de cada hoja se convierte en un registro único asociado a su tipo de registro respectivo.
* Cada hoja del archivo de Excel no debe superar lo siguiente:
   * 10 000 filas
   * 500 columnas
* El archivo de Excel no debe tener más de 5 MB.
* No se admiten hojas vacías.

Para importar tipos de registros mediante un archivo CSV o de Excel:

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo donde desee crear los tipos de registro,

   O

   Desde un espacio de trabajo, expanda la flecha hacia abajo a la derecha del nombre de un espacio de trabajo existente, busque un espacio de trabajo y selecciónelo cuando se muestre en la lista.
1. Haga clic en **Agregar tipo de registro**.
1. Haga clic en **Desde el archivo**.
1. Arrastre y suelte un archivo de Excel o CSV guardado anteriormente en el equipo, o haga clic en **Seleccione un archivo CSV o de Excel** para buscar uno.
1. Haz clic en **Vista previa y edita**.

   Se muestra el cuadro **Previsualizar y editar** con la siguiente información:

   * Los nombres de las hojas o de los futuros tipos de registros se muestran en el panel izquierdo. De forma predeterminada, Workfront Planning selecciona un icono y un color para cada nuevo tipo de registro.
   * Se selecciona el primer tipo de hoja o registro y los nombres de los campos asociados a él se muestran como encabezados de columna. El tipo de cada campo está seleccionado de forma predeterminada.
   * Cada fila representa un nuevo registro. Solo se muestran los 10 primeros registros en el cuadro Vista previa y edición.

   ![](assets/preview-and-edit-box.png)

1. (Opcional) Haga clic en el nombre de cada hoja en el panel izquierdo para revisar la información que contiene.

   >[!NOTE]
   >
   >Las hojas vacías no son compatibles y aparecen atenuadas.

1. (Opcional) Anule la selección de las hojas que no quiera importar del panel izquierdo.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Las hojas que no haya seleccionado se muestran con un fondo gris.

1. (Opcional) Haga clic en la flecha hacia abajo situada a la derecha del encabezado de la columna para realizar una de las siguientes acciones:

   * Cambie el nombre de uno de los campos
   * Cambiar **tipo de campo**
   * Actualizar el campo **Descripción**

1. (Condicional) Después de actualizar la información del campo, haga clic en **Guardar**.

1. Haga clic en **Importar** cuando esté listo para importar el archivo.

   La siguiente información se importa en Workfront Planning:

   * Nuevos tipos de registros
   * Nuevos campos asociados a cada tipo de registro
   * Nuevos registros asociados a cada tipo de registro

   Puede empezar a administrar campos y registros en las páginas de tipos de registros.

   Todas las personas con acceso a Workfront Planning ahora pueden ver y editar los tipos de registro importados y su información.

</div>

