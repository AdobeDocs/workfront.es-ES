---
title: Conectar tipos de registro
description: Una manera de indicar cómo se relacionan los tipos de registros individuales entre sí es conectarlos. Además, puede conectar tipos de registros de Adobe Workfront Planning con tipos de objetos de otras aplicaciones para mejorar la experiencia de los usuarios y mantener el enfoque en una aplicación.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 7b5441b2aa17b22f0fd54cfe4921aa5dab2e0461
workflow-type: tm+mt
source-wordcount: '2222'
ht-degree: 1%

---


# Conectar tipos de registros

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>

{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

Puede conectar tipos de registros entre sí o conectar tipos de registros con tipos de objetos de otras aplicaciones.

En este artículo se describe cómo conectar dos tipos de registros de Workfront Planning o un tipo de registro de Workfront Planning con un objeto de otra aplicación.

Después de establecer la conexión entre registros o tipos de objeto, puede conectar registros individuales entre sí y mostrar campos de los registros vinculados o tipos de objeto en un registro de Workfront Planning.

Para obtener información general acerca de los tipos de conexión, vea [Información general sobre los tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

Para obtener información acerca de cómo conectar registros o registros con objetos de otras aplicaciones, vea [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

Para ver un ejemplo de conexión de tipos de registros y registros, vea [Ejemplo de conexión de tipos de registros y registros](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

Debe tener lo siguiente para poder acceder a Workfront Planning:

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
   <td role="rowheader"><p>Plan de planificación de Adobe Workfront*</p></td> 
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
   <td> <p>Estándar</p> 
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
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>Todos los usuarios, incluidos los administradores de Workfront, deben tener asignada una plantilla de diseño que incluya el área de Planning en el menú principal </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!-- OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p> Adobe Workfront Planning</p>
   <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p> 
   <p>Current: Plan</p>
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++


## Conectar tipos de registros

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registros desee conectar,

   O

   Desde un espacio de trabajo, expanda la flecha hacia abajo a la derecha del nombre de un espacio de trabajo existente, busque un espacio de trabajo y selecciónelo cuando se muestre en la lista.
1. Haga clic en la tarjeta de un tipo de registro para abrir la página del tipo de registro.
1. Haga clic en el icono **+** en la esquina superior derecha de la vista de tabla y, a continuación, haga clic en la ficha **Nueva conexión**.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. En el campo **Tipo de registro**, busque un tipo de registro o seleccione una de las siguientes opciones:

   * Otro tipo de registro del espacio de trabajo actual

     <span class="preview">![](assets/many-to-many-connection-picker.png)</span>
     >[!TIP]
     >
     > 
     >Si no tiene otros tipos de registro en el espacio de trabajo seleccionado, la sección del espacio de trabajo no se muestra.


   * Un tipo de registro de otro espacio de trabajo configurado para conectarse desde otros espacios de trabajo. Para obtener más información, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

     <span class="preview">![](assets/new-connection-allow-multiple-records-box.png)</span>

     >[!TIP]
     >
     >Si no hay ningún tipo de registro configurado para conectarse desde otros espacios de trabajo, la sección del espacio de trabajo no se muestra.


   * Un **proyecto, Portfolio, programa, compañía** o **grupo** de la sección **Tipos de objetos de Workfront**.

     ![](assets/workfront-project-connection-selection.png)

   * **Experience Manager Assets** de la sección **Aplicaciones de Adobe**.

     <span class="preview">![](assets/aem-assets-connection-selection.png)</span>

1. Actualice la siguiente información:

   * **Nombre**: nombre del campo conectado, tal como aparecerá en la vista de tabla o en la página de registro del tipo de registro original. Esto crea la columna de registro vinculado en la vista de tabla del tipo de registro original o el campo de registro vinculado para los registros originales. De forma predeterminada, el nombre del campo es el nombre del registro u objeto al que se conecta.

   >[!TIP]
   >
   >Puede tener varias conexiones al mismo registro o tipo de objeto. Si no edita el nombre del campo conectado, Workfront agrega un número después del nombre del registro conectado para indicar el número de tipos de registros conectados con el mismo nombre.

   * **Descripción**: Información adicional acerca del campo de registro conectado. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo de una tabla.
   * **Permitir varios registros**: seleccione esta opción para indicar que permite a los usuarios agregar varios registros cuando el campo de tipo de registro vinculado se muestra en los registros originales. Esta opción está seleccionada de forma predeterminada.

     Esta opción solo está disponible cuando se conectan registros de dos espacios de trabajo diferentes o un registro y un objeto de recurso de Adobe Experience Manager.

     <span class="preview">![](assets/new-connection-allow-multiple-records-box.png)</span>

   * **Tipo de conexión**: seleccione una de las siguientes opciones para indicar cuántos registros pueden conectar con y desde:

      * Muchos a muchos
      * Uno a muchos
      * Muchos a uno
      * Uno a uno

     Esta opción sólo está disponible cuando se conectan registros del mismo espacio de trabajo o un registro y un tipo de objeto de Workfront.

     <span class="preview">![](assets/many-to-many-connection-picker.png)</span>

     Para obtener más información acerca de los tipos de conexión, vea [Información general sobre los tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

   * **Seleccionar campos de búsqueda**: seleccione esta opción para agregar campos desde el tipo de registro seleccionado. Los campos de búsqueda son campos asociados al tipo de registro u objeto al que está vinculando. Al vincularlos, se muestra información del registro u objeto con el que se está vinculando en el registro desde el que se está vinculando. Esta opción está seleccionada de forma predeterminada.

     >[!TIP]
     >
     > No puede agregar los siguientes tipos de campo como campos de búsqueda:
     >
     >    * Personas
     >    * Creado por
     >    * Última modificación realizada por
     >    * Campos de escritura anticipada de Workfront (incluidos campos como Propietario del proyecto o Patrocinador del proyecto)

1. (Condicional y opcional) Si seleccionó conectar un objeto de Workfront, seleccione un **formulario personalizado** de la sección **Vincular solo objetos que coincidan con estos criterios**. Solo los objetos que tienen los formularios personalizados seleccionados adjuntos pueden vincularse al tipo de registro seleccionado. Puede seleccionar varios formularios.

   >[!NOTE]
   >
   > Debe crear formularios personalizados en Workfront para los objetos seleccionados antes de que se muestren en esta lista.

1. (Condicional) Si ha seleccionado conectarse a Experience Manager Assets, seleccione un repositorio en el menú desplegable **Repositorio de Experience Manager** de la sección **Vincular recursos del siguiente repositorio**. Este campo es obligatorio. En este campo solo se muestran los repositorios a los que tiene acceso en Experience Manager Assets.

   >[!NOTE]
   >
   >El administrador de Workfront puede asignar campos de Workfront Planning a campos de Experience Manager Assets a través de la asignación de metadatos en Workfront. Para obtener más información, consulte [Configuración de la asignación de metadatos de recursos entre Adobe Workfront y Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

1. (Condicional) Si ha seleccionado conectarse a Experience Manager Assets o a un tipo de registro de Workfront Planning, seleccione una de las siguientes opciones en el área **Apariencia del registro**:

   * <span class="preview">**Nombre e imagen**: tanto el nombre como la miniatura o el icono de los registros conectados se mostrarán en el campo de registro conectado. Esta es la opción predeterminada. </span>
   * <span class="preview">**Nombre**: solo se mostrará el nombre de los registros conectados en el campo de registro conectado.</span>
   * <span class="preview">**Imagen**: solo se mostrará la miniatura o el icono de los registros conectados en el campo de registro conectado.</span>

   Los registros sin imagen en miniatura muestran el icono de tipo de registro en su lugar. Se mostrará un ejemplo de cómo se mostrarán los registros conectados en el área **Apariencia del registro**.

   >[!NOTE]
   >
   >* Cuando permite vincular varios registros, la visualización de sólo la miniatura puede ahorrar espacio en áreas más pequeñas, como las vistas de registros.
   >
   >* El nombre de un registro es el campo principal del registro. Para obtener más información, vea [Información general del campo primario](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >* La selección de una apariencia de registro no está disponible al seleccionar tipos de objetos de Workfront.
   >
   >* Lo que seleccione en el área de Apariencia del registro determina cómo se muestran los registros en las conexiones de cualquier parte del sistema, incluidas todas las vistas y páginas de detalles.

1. Haga clic en **Crear**.

1. (Condicional) Si seleccionó la opción **Seleccionar campo de búsqueda**, se abrirá el cuadro **Agregar campos de búsqueda**.

   Haga clic en el icono **+** para agregar campos del área **Campos no seleccionados**.

   O

   Haga clic en el icono **-** para quitar campos del área **Campos seleccionados**

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   Los valores de los campos conectados se rellenan automáticamente después de vincular registros u objetos.

   >[!IMPORTANT]
   >
   >    Todas las personas con permisos de Vista o superiores en el espacio de trabajo pueden ver la información en los campos vinculados, independientemente de sus permisos o nivel de acceso en la aplicación de los tipos de objetos vinculados.


1. (Opcional) Haga clic en **Omitir** para omitir la adición de campos del registro u tipo de objeto vinculado. El nombre o el campo Principal del registro vinculado es el único campo visible en la vista de tabla del tipo de registro desde el que se conecta.

1. (Opcional y condicional) Si selecciona vincular un campo de número, moneda, porcentaje o tipo de fecha, seleccione también un valor de acumulador para resumir varios valores. Los valores de los campos vinculados se muestran separados por comas o como un valor resumido según el agregador que elija, cuando los usuarios seleccionan más de un registro vinculado en el campo de registro vinculado.

   Si el campo de búsqueda contiene varios valores que no están resumidos, tenga en cuenta lo siguiente al utilizar el campo en la ordenación o agrupación de una vista:

   * La ordenación se realiza mediante el primer valor

   * Los registros se agrupan por cada combinación única de valores de campo

   * La vista de cronología se crea en función del primer valor de fecha

   >[!IMPORTANT]
   >
   >    Debe seleccionar un valor de agregado al agregar campos de fecha de búsqueda si desea que los campos estén disponibles para agregarlos como fechas de inicio y finalización en las vistas de calendario y escala de tiempo. Por ejemplo, puede seleccionar el agregador MAX o MIN para un campo de fecha de búsqueda.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Los acumuladores no están disponibles al conectar tipos de registros a Experience Manager Assets.

   Seleccione una de las siguientes opciones:

   * **Ninguno**: Muestra los valores que provienen de varios registros separados por comas. Esta es la selección predeterminada.
   * **MAX**: muestra el valor más alto de todos los valores procedentes de varios registros seleccionados en el campo de registro vinculado.
   * **MIN**: muestra el valor más bajo de todos los valores que provienen de varios registros seleccionados en el campo de registro vinculado.
   * **SUM**: Muestra el total de todos los valores que provienen de varios registros seleccionados en el campo de registro vinculado.
   * **AVG**: Muestra el promedio de todos los valores que provienen de varios registros seleccionados en el campo de registro vinculado.
   * **ÚNICO**: quita los duplicados de los valores de los campos de búsqueda y solo muestra los valores únicos. Esto no está disponible para los siguientes tipos de campo:
      * Párrafo
      * Casilla de verificación
      * Personas

   >[!NOTE]
   >
   >Por ejemplo, puede vincular el registro de producto (registro vinculado) desde el registro de campaña (registro original) y asignarle el nombre &quot;campo de producto&quot;. También puede vincular el campo Presupuesto del registro de producto del registro de campaña y llamarlo &quot;Presupuesto de producto&quot;. Si se le permite seleccionar varios registros en el &quot;Campo de producto&quot;, puede seleccionar el Producto 1 con un Presupuesto de 100 000 $ y el Producto 2 con un Presupuesto de 110 000 $, y el Producto 3 con un Presupuesto de 100 000 $. Puede ver la siguiente información de presupuesto en el campo vinculado desde el registro original, en función del agregador que elija:
   >
   >* **Ninguno**: 100.000, 110.000, 100.000 $
   >* **MAX**: $110,000
   >* **MIN**: $100,000
   >* **SUMA**: $310,000
   >* **PROMEDIO**: 103.000,33 $
   >* **ÚNICO**: $100,000
   >

1. (Opcional) Use el icono **search** ![](assets/search-icon.png) para buscar un campo.

1. Haga clic en **Agregar campos** para guardar los cambios.

   Se añaden los elementos siguientes:

   * Un campo de registro vinculado en el tipo de registro desde el que está vinculando. El campo de registro vinculado mostrará registros individuales del tipo de registro vinculado, después de agregarlos manualmente. Para obtener información sobre cómo agregar registros, vea [Conectar registros](/help/quicksilver/planning/records/connect-records.md). El nombre del campo de registro vinculado es el nombre seleccionado en el paso 6. <!--accurate-->

   * Campo (o campos) vinculado (o de búsqueda) que muestra información sobre el registro vinculado o los tipos de objeto después de agregar manualmente los registros u objetos en el campo de registro vinculado. Los campos de búsqueda solo se crean cuando la opción **Seleccionar campos de búsqueda** está seleccionada al crear la conexión. Los campos de búsqueda se nombran automáticamente según este patrón:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Por ejemplo, si ha vinculado un tipo de registro de campaña con un tipo de registro de programa y ha asignado al campo de registro vinculado de programa el nombre &quot;Información del programa&quot;, seleccionado a continuación para mostrar también el campo Presupuesto del programa en la vista de tabla de la campaña, el campo vinculado se denomina automáticamente `Budget (from Program information)` en la vista de tabla de la campaña.

   * Cuando se vinculan tipos de registros entre sí, también se agrega un campo de registro vinculado en el tipo de registro al que se está vinculando. El nombre del campo de registro vinculado en el tipo de registro vinculado es el nombre del tipo de registro desde el que se establece el vínculo.

     Por ejemplo, si vincula el tipo de registro &quot;Producto&quot; desde el tipo de registro &quot;Campaña&quot; y asigna al campo conectado de la campaña el nombre &quot;Producto vinculado&quot;, se crea un campo de registro vinculado &quot;Campaña&quot; para el tipo de registro Producto.

     >[!TIP]
     >
     > No se crea un campo de registro vinculado para los objetos de otra aplicación con el tipo de registro desde el que se está vinculando en Workfront Planning.

1. (Opcional y condicional) Desde el tipo de registro original o la vista de tabla del tipo de registro vinculado, haga clic en la flecha hacia abajo en el encabezado de los campos de registro vinculados y, a continuación, haga clic en una de las siguientes opciones:

   * **Editar campo**: Actualice la información de **Nombre** y **Descripción** del campo.
   * **Editar campos de búsqueda**: agregue o quite cualquiera de los campos del registro vinculado.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Para agregar o quitar campos de búsqueda, siga las instrucciones de los pasos 16-17 anteriores. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > No se pueden agregar campos de búsqueda que pertenezcan a tipos de registro que esté vinculando a tipos de objeto de otra aplicación.
   >
   > Por ejemplo, no puede agregar el campo de búsqueda &quot;Estado de campaña&quot; a un proyecto de Workfront al que esté vinculando desde las campañas.

1. (Opcional) Haga clic en la flecha hacia abajo en el encabezado de un campo de registro vinculado o en el encabezado de un campo de búsqueda desde el tipo de registro desde el que está vinculando y, a continuación, haga clic en **Eliminar**.

   Se eliminan el campo de registro o el campo de búsqueda. Si elimina un campo de registro, también se eliminarán todos los campos de búsqueda asociados al registro vinculado.
