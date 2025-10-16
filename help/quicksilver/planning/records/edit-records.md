---
title: Editar registros
description: Puede editar la información de los registros en Adobe Workfront Planning. Debe crear tipos de registros antes de empezar a crear y editar registros.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '2732'
ht-degree: 9%

---


# Editar registros

<!--keep the choice values information in yellow till Jan 2026-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Puede editar la información de los registros en Adobe Workfront Planning editando los valores de los campos asociados a los registros.

Debe crear tipos de registros antes de empezar a crear y editar registros.

Para obtener más información, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

Para obtener información sobre cómo crear registros, vea [Crear registros](/help/quicksilver/planning/records/create-records.md).

&lt;!— mencione aquí que los campos de la vista Detalles son los mismos que los de la vista de tabla — este artículo está vinculado desde Administrar vistas de registros a hacer referencia a esta información—>

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
   <td role="rowheader"><p>paquete de Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Cualquier Workfront y cualquier paquete de Planning</p></li>
O
<li><p>Cualquier flujo de trabajo y cualquier paquete de Planning</p></li></ul>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de contribución o superiores para un espacio de trabajo y tipo de registro  </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> </td> 
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
   <td> <p>Standard</p> 
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
   <td>  <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> -->

## Consideraciones acerca de la edición de registros

* Puede editar los registros que haya creado o los creados por otros usuarios si dispone de permisos para el espacio de trabajo.
* Puede editar los campos de registro desde las siguientes áreas:

   * Vista previa del registro en una vista de registros
   * La página de detalles del registro
   * En línea, en una vista de tabla.
   * La vista de calendario y de escala de tiempo, al cambiar el tamaño o arrastrar y soltar los registros. Esto actualiza las fechas de los registros.

* Cuando un usuario edita un registro en una vista, los cambios son visibles inmediatamente en todas las vistas y las páginas de registros para todos los demás usuarios.

* Los siguientes tipos de campos se actualizan automáticamente y no se pueden editar sus valores manualmente:
   * Campos vinculados de otros registros
   * Campos de tipo fórmula
   * Campos del sistema (Creado por, Fecha de creación, Última modificación por, Fecha de última modificación)
* Si los registros que muestra están vinculados a otros registros, la nueva información de los registros que está modificando se reflejará en los registros vinculados.
* No puede editar registros de forma masiva. <!--this will probably change-->
* Las direcciones URL se reconocen como vínculos en tipos de campo de texto de una sola línea solo cuando comienzan con lo siguiente: http://, https://, ftp:// o www. .
* Puede agregar una imagen de portada a cada registro. La imagen es única para cada registro y no se aplica a todos los registros del mismo tiempo.
* Puede editar el orden de los campos en una página de registro y agregar una imagen de portada para un registro. Para obtener más información, consulte [Administrar el diseño de la página de registros](/help/quicksilver/planning/records/manage-the-record-page.md).

## Editar registros

Puede editar un registro desde las siguientes áreas:

* [La vista de tabla](#edit-a-record-inline-in-the-table-view-of-a-record-type)
* [La vista de cronología](#edit-a-record-in-the-timeline-view-of-a-record-type)
* [La vista de calendario](#edit-a-record-in-the-calendar-view-of-a-record-type)
* [Vista previa del registro en una vista](#edit-a-record-from-the-records-preview-in-a-view)
* [La página del registro](#edit-a-record-from-the-records-page)
* [Un objeto Workfront en la sección Planning](#edit-a-record-from-a-workfront-object-in-the-planning-section)

Para editar las fechas de los registros, haga lo siguiente:

* [Cambiar el tamaño de las barras de los registros en la vista de calendario y escala de tiempo]

### Editar un registro en línea en la vista de tabla de un tipo de registro

Cuando edita registros desde la vista de tabla, existe una indicación de qué campo están editando otros usuarios en el momento en que está viendo el registro.

Para obtener más información, consulte [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

Cuando se agrega un nuevo registro después del último registro de una agrupación o subagrupación, Workfront actualiza automáticamente los campos incluidos en las agrupaciones para los registros nuevos. Puede editar manualmente estos campos, si es necesario, y los registros pueden eliminarse de la agrupación.

Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos registros desee editar

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.
1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. (Condicional) Haga clic en la ficha de una vista de tabla o haga clic en **+ Ver** para crear una vista de tabla. La vista de tabla debe ser la vista predeterminada, a menos que haya visto el tipo de registro en otro tipo de vista cuando accedió por última vez.

   Los registros asociados al tipo de registro seleccionado se muestran en la vista de tabla.
1. Haga clic dentro de la fila de un registro para empezar a editar la información sobre el registro en línea.

   ![Editar campo de párrafo de registro con vista de tabla de formato](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!TIP]
   >
   >  No puede editar la información de los siguientes campos, ya que son de solo lectura y Workfront los actualiza automáticamente:
   >  
   >  * Campos vinculados que se crean conectando tipos de registro. Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Campos de los siguientes tipos: Creado por, Fecha de creación, Última modificación por, Fecha de última modificación, Campos de fórmula.

1. (Opcional y condicional) Cuando edite un campo de tipo Párrafo, utilice las siguientes opciones de formato de **Texto enriquecido**:

   * Negrita
   * Cursiva
   * Subrayado
   * Añadir un vínculo
   * Agregar una lista con viñetas
   * Añadir una lista numerada

   ![Barra de herramientas de texto enriquecido en el campo de párrafo](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Opcional) Haga doble clic en un campo de registro conectado para agregar registros u objetos conectados a otro registro. Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. Presione **Enter** en el teclado o haga clic fuera de una fila para guardar los cambios. Los cambios se guardan automáticamente. Un indicador **Guardado** aparece brevemente en la esquina superior derecha de la vista de tabla para mostrar que los cambios se han guardado.


1. (Opcional) Para copiar y pegar información de un campo a otro, siga uno de estos procedimientos:

   * Copie uno o varios valores existentes de un campo y péguelos en un campo del mismo tipo en otro registro
   * Haga clic en el encabezado de una columna para seleccionarla y copiarla. A continuación, haga clic en el encabezado de otra columna y pegue el contenido de la columna copiada. Las columnas deben contener tipos de campo similares.
   * Con la tecla Mayús pulsada, haga clic en para seleccionar varias filas de una tabla, copie la información de las filas seleccionadas y, a continuación, haga clic en una fila diferente y pegue la información seleccionada en la nueva fila y en las filas siguientes.
   * Copie la información de una celda, seleccione varias celdas y pegue la misma información en varias celdas. Puede seleccionar varias celdas y pegar la misma información en varias celdas de filas y columnas adyacentes.
   * Seleccione la esquina inferior derecha de una celda existente que contiene la información que desea copiar y, a continuación, arrástrela y suéltela sobre las celdas adyacentes en las que desee pegar la misma información. Todas las celdas deben contener el mismo tipo de información.

     ![Esquina inferior derecha arrastrable para copiar y pegar en la vista de tabla](assets/dragable-lower-right-corner-for-copy-paste-in-table-view.png)


   * Copie una o varias celdas de un origen externo (por ejemplo, un archivo de Excel) y péguelas en uno de los siguientes tipos de campos:

      * Campos de conexión de Workfront Planning.
      * Campos de personas. Solo se admiten campos con un valor.

     No se puede copiar información de un origen externo y pegarla en ningún otro tipo de campo, incluidos los campos de conexión de Workfront o de AEM Assets.

   >[!NOTE]
   >
   >Tenga en cuenta lo siguiente:
   >
   >* Utilice los siguientes métodos abreviados del teclado para copiar y pegar información:
   >   * Copiar: CTRL + C (⌘ + C para Mac)
   >   * Pegar: CTRL + V (⌘ + V para Mac)
   >
   >* No se pueden copiar y pegar valores de campo en la página de registro. Esta funcionalidad solo se admite en la vista de tabla de un tipo de registro.
   >* No puede copiar y pegar valores de campo para los siguientes tipos de campo:
   >
   >    * Campos de búsqueda que se crean al conectar tipos de registros. Puede copiar y pegar campos de registro vinculados. Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).
   >    * Campos de los siguientes tipos: Creado por, Fecha de creación, Última modificación por, Fecha de última modificación

1. (Opcional) Utilice los siguientes métodos abreviados del teclado para deshacer o rehacer la edición o copiar y pegar la información de los registros:

   * CTRL + Z (⌘ + Z para Mac) para deshacer un cambio
   * CTRL + Mayús + Z (⌘ + Mayús + Z para Mac) para rehacer un cambio

   >[!TIP]
   >
   >    Puede utilizar los métodos abreviados de teclado varias veces seguidas para deshacer varios cambios.

1. (Opcional) Agregue una miniatura a un registro. Para obtener más información, consulte [Añadir una miniatura a un registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).


### Editar un registro en la vista de cronología de un tipo de registro

<!--add another step about drag and drop here when that is available-->

1. Abra la página de tipo de registro en una vista de cronología. Para obtener más información, consulte [Administrar la vista de línea de tiempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

1. Pase el ratón sobre los extremos de la barra de un registro, haga clic, arrastre y suelte su margen en otra fecha. Esto actualiza automáticamente la fecha de inicio o de finalización del registro.

   ![Barra izquierda en la vista de escala de tiempo para cambiar el tamaño](assets/left-end-bar-handle-to-resize-timeline-view.png)

1. Haga clic y mantenga presionada una barra de registro y, a continuación, arrástrela y suéltela en otra posición para actualizar su escala de tiempo y sus fechas. Las fechas de inicio y finalización del registro se actualizan automáticamente.

1. Haga clic en la barra de un registro para abrir su área de detalles y editar todos los campos.

   Para obtener más información, consulte la sección [Editar un registro desde la vista previa del registro en una vista](#edit-a-record-from-the-records-preview-in-a-view) de este artículo.

### Editar un registro en la vista de calendario de un tipo de registro

<!--add another step about drag and drop here when that is available-->

1. Abra la página de tipo de registro en una vista de calendario. Para obtener más información, vea [Administrar la vista de calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).
1. (Condicional) Pase el ratón sobre los extremos de la barra de un registro en la vista de calendario y, a continuación, haga clic en sus márgenes, arrástrelos y suéltelos en otra fecha. Esto actualiza automáticamente la fecha de inicio o de finalización del registro.

   ![Barra izquierda en la vista de calendario para cambiar el tamaño](assets/left-end-bar-handle-to-resize-calendar-monthly-view.png)

1. Haga clic y mantenga presionada una barra de registro y, a continuación, arrástrela y suéltela en otra posición para actualizar su escala de tiempo y sus fechas. Las fechas de inicio y finalización del registro se actualizan automáticamente.

1. Haga clic en la barra de un registro para abrir su área de detalles y editar todos los campos.

   Para obtener más información, consulte la sección [Editar un registro desde la vista previa del registro en una vista](#edit-a-record-from-the-records-preview-in-a-view) de este artículo.

### Editar un registro desde la vista previa del registro en una vista

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos registros desee editar

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. Desde cualquier vista, haga clic en el registro

   O

   En la vista de tabla, haga clic en el icono **Abrir detalles** ![Abrir detalles en el campo de nombre de tabla](assets/open-details-icon-in-table-name-field.png) de la primera columna. La vista previa del registro se abrirá en la vista.

   ![Cuadro de detalles](assets/details-box.png)

1. (Opcional) Haga clic en el menú **Más** a la derecha del título del registro y, a continuación, haga clic en **Cambiar nombre**. Se actualiza el campo que se muestra como título del registro.

   El título del registro es el campo principal del registro cuando se ve en una vista de tabla. Para obtener más información, vea [Información general del campo primario](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Comience a editar la información del campo en la vista previa del registro.

   >[!TIP]
   >
   >  No puede editar la información de los siguientes campos, ya que son de solo lectura y Workfront los actualiza automáticamente:
   >  
   >  * Campos de búsqueda de otros registros creados conectando tipos de registros. Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Campos de los siguientes tipos: Creado por, Fecha de creación, Última modificación por, Fecha de última modificación, Campos de fórmula.

1. (Opcional) Haga clic en **Agregar portada** para agregar una imagen de portada al registro. Para obtener más información, vea [Agregar una imagen de portada a un registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

1. (Opcional) Pase el ratón sobre el icono de la miniatura y luego haga clic en **Más** ![Menú más](assets/more-menu.png) > **Editar miniatura** para agregar una imagen en miniatura. Para obtener más información, consulte [Añadir una miniatura a un registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   Workfront guardará automáticamente los cambios.

1. (Opcional) Haga clic en el **indicador en tiempo real** ![icono de indicador en tiempo real](assets/real-time-indicator-icon.png) en la esquina superior derecha del cuadro de vista previa del registro y, a continuación, habilite la opción **Mostrar colaboradores** para resaltar los campos que otros están editando en tiempo real.

   En esta área se muestran los nombres y avatares de todos los usuarios que acceden al registro al mismo tiempo.

   Cuando la configuración está desactivada, los avatares y los nombres se enumeran en el área del indicador en tiempo real y los campos que se están editando no están resaltados.

   ![Cuadro de vista previa de registro expandido con indicador de tiempo real](assets/real-time-indicator-expanded-record-preview-box.png)

1. (Opcional) Haga clic en el icono **Exportar** del menú ![Exportar en la página de detalles del registro](assets/export-icon-in-record-details-page.png) para exportar los detalles del registro. Para obtener más información, vea [Exportar los detalles de un registro](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Opcional) Haga clic en el icono **Abrir en ficha nueva** ![Abrir detalles en un icono de ficha nueva](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> en la esquina superior derecha de la vista previa del registro para abrir la página del registro en una ficha nueva. Continúe editando el registro como se describe en [Edite un registro desde la sección de la página del registro](#edit-a-record-from-the-records-page) en este artículo.

### Editar un registro desde la página del registro

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos registros desee editar

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. Realice una de las siguientes acciones:

   * Desde cualquier vista, acceda a la vista previa del registro, tal como se describe en la sección [Editar un registro de la vista previa del registro en una vista](#edit-a-record-from-the-records-preview-in-a-view) de este artículo y, a continuación, haga clic en el icono **Abrir en ficha nueva** ![Abrir detalles en un nuevo icono de ficha](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> en la esquina superior derecha de la vista previa del registro para abrir la página del registro en una nueva pestaña.

   * En la vista **Tabla**, pase el ratón sobre el nombre de un registro, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Ver**

     ![Menú contextual para la fila de registros](assets/contextual-menu-for-record-row.png)

     Se abre la página de registro.

     ![Página de detalles](assets/details-page.png)

1. (Opcional) Haga clic en el menú **Más** a la derecha del título del registro y, a continuación, haga clic en **Cambiar nombre**. Se actualiza el campo que se muestra como título del registro.

   El título del registro es el campo principal del registro cuando se ve en una vista de tabla. Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

1. Haga clic en cualquier campo editable de la página de registro para editarlo.

   >[!TIP]
   >
   >  No puede editar la información de los siguientes campos, ya que son de solo lectura y Workfront los actualiza automáticamente:
   >  
   >  * Campos vinculados que se crean conectando tipos de registro. Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Campos de los siguientes tipos: Creado por, Fecha de creación, Última modificación por, Fecha de última modificación, Campos de fórmula.

1. (Opcional) Haga clic en el icono de información a la derecha de cualquier campo que lo muestre para ver la descripción de un campo.
1. (Opcional) Haga clic en **Agregar portada** para agregar una imagen de portada al registro

   O

   Pase el ratón sobre la imagen de portada existente y luego haga clic en el menú **Más** ![Menú más](assets/more-menu.png) > **Cargar** para agregar una nueva imagen de portada para el registro.

   Para obtener más información, vea [Agregar una imagen de portada a un registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

1. (Opcional) Pase el ratón sobre una miniatura existente o sobre el **icono de miniatura** ![Grabar icono de miniatura en la página de detalles](assets/record-thumbnail-icon-on-details-page.png) y, a continuación, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) > **Editar miniatura** para agregar una miniatura para el registro.

   Para obtener más información, consulte [Añadir una miniatura a un registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   Workfront guardará automáticamente los cambios.

1. (Opcional) Haga clic en el **indicador en tiempo real** ![icono del indicador en tiempo real](assets/real-time-indicator-icon.png) en la esquina superior derecha de la página del registro y, a continuación, habilite la opción **Mostrar colaboradores** para resaltar los campos que otros están editando en tiempo real.

   En esta área se muestran los nombres y avatares de todos los usuarios que acceden al registro al mismo tiempo.

   Cuando la configuración está desactivada, los avatares y los nombres se enumeran en el área del indicador en tiempo real y los campos que se están editando no están resaltados.

   ![Cuadro de vista previa de registro expandido de indicador de tiempo real](assets/real-time-indicator-expanded-record-preview-box.png)

1. (Opcional) Haga clic en el icono **Exportar** del menú ![Exportar en la página de detalles del registro](assets/export-icon-in-record-details-page.png) para exportar los detalles del registro. Para obtener más información, vea [Exportar los detalles de un registro](/help/quicksilver/planning/records/export-the-record-page.md).


## Edición de un registro de un objeto de Workfront en la sección Planificación

Después de conectar registros con objetos de Workfront, puede editar los registros de Workfront Planning en Workfront desde la sección Planificación del objeto.

Para obtener más información, consulte [Administrar conexiones de registro desde objetos de Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

## Editar la configuración de campos de selección única o múltiple al actualizar sus valores

<!--some of this information is also available in Edit fields article - update both when necessary-->

Cuando se actualiza la información en un campo de selección única o múltiple, se pueden agregar nuevas opciones al campo sin tener que editarlo.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta sección solo está disponible en la vista de tabla. No está disponible en ninguna otra área en la que se muestren campos de selección única o múltiple.

**EJEMPLO**

Puede tener un campo de selección único llamado Estado que tiene las opciones Nuevo y Cerrado, y desea agregar una opción para un estado En curso. Puede agregar la opción realizando una de las siguientes acciones:

* Edición del campo. Para obtener más información, consulte [Editar campos](/help/quicksilver/planning/fields/edit-fields.md)
* Agregar una nueva opción mientras se edita el registro en la vista de tabla, como se describe a continuación.

Para agregar una nueva opción a un campo de selección existente al editar un registro:

1. Vaya a una página de tipo de registro y abra la vista de tabla.
1. Agregue el campo de selección única o múltiple al que desee agregar una opción en la vista de tabla como una nueva columna. Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).
1. Comience a editar el campo en línea haciendo doble clic en la celda del campo.
1. Escriba el nombre de la opción que desea agregar y haga clic en **Agregar opción**.

   ![Agregar opción en un campo de selección única en la vista de tabla](assets/add-choice-in-table-view-for-single-select-field.png)

   La nueva opción se agrega inmediatamente al campo de selección única.

   <span class="preview">También se agrega un nuevo valor de opción a cada opción. Puede utilizar los valores de opción en llamadas a la API u otras integraciones. Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md). </span>

