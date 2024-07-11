---
title: Conectar tipos de registros
description: Una manera de indicar cómo se relacionan los tipos de registros individuales entre sí es conectarlos. Además, puede conectar tipos de registros de Adobe Workfront Planning con tipos de objetos de otras aplicaciones para mejorar la experiencia de los usuarios y mantener el enfoque en una aplicación.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '2515'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Adobe Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# Conectar tipos de registros

{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

Puede conectar tipos de registros entre sí o tipos de registros con tipos de objetos de otras aplicaciones.

En este artículo se describe cómo conectar dos tipos de registros de Workfront Planning a un tipo de registro de Workfront Planning con un objeto de otra aplicación.

Después de establecer la conexión entre registros o tipos de objeto, puede conectar registros individuales entre sí y mostrar campos de los registros vinculados o tipos de objeto en un registro de Workfront Planning.

Para obtener información acerca de cómo conectar un registro de Workfront Planning a un objeto desde otra aplicación, vea [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

Para ver un ejemplo de conexión de tipos de registros y registros, consulte [Ejemplo de conexión de tipos y registros](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## Requisitos de acceso

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>Para conectar los tipos de registros de Adobe Workfront Planning con Experience Manager Assets, debe tener una licencia de Adobe Experience Manager Assets y la instancia de Workfront de su organización debe estar integrada en la experiencia unificada de Adobe. Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiencia unificada de Adobe para Workfront</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en la fase de acceso anticipado para Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plan de Adobe Workfront</p></td>
   <td>
<p>Cualquiera</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Nuevo: estándar</p> 
   <p>Actual: plan</p>
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon.
</td>
  </tr>
 </tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but planing is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## Consideraciones sobre la conexión de tipos de registros

* Puede conectar las siguientes entidades en Adobe Workfront Planning:

   * Dos tipos de registros

     Los tipos de registro deben pertenecer al mismo espacio de trabajo.
   * Tipo de registro y tipo de objeto de otra aplicación.

* Puede conectar los tipos de registros de Workfront Planning con los siguientes tipos de objetos desde las siguientes aplicaciones:

   * Adobe Workfront:

      * Proyectos
      * Portafolios
      * Programas
      * Compañías
      * Grupos

   * Adobe Experience Manager Assets:

      * Imágenes
      * Carpetas

     >[!IMPORTANT]
     >
     >Debe tener una licencia de Adobe Experience Manager Assets y la instancia de Workfront de su organización debe incorporarse a Adobe Business Platform o a Adobe Admin Console para conectar los registros de Workfront Planning a Adobe Experience Manager Assets.
     >
     >Si tiene alguna pregunta acerca de la incorporación a Adobe Admin Console, consulte la [Preguntas frecuentes sobre Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Después de crear registros individuales para un tipo de registro, puede seleccionar los registros a los que se conecta desde el campo tipo de registro vinculado. Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

* Después de conectar un tipo de registro con otro tipo de registro o con un tipo de objeto de otra aplicación, existen los siguientes escenarios:

   * **Cuando conecta dos tipos de registros**: se crea un campo de registro vinculado en el tipo de registro desde el que se conecta. Se crea un campo de registro vinculado similar en el tipo de registro al que se conecta.

     Por ejemplo, si conecta el tipo de registro &quot;Campaña&quot; con el tipo de registro &quot;Producto&quot;, se crea un campo de registro vinculado denominado &quot;Producto vinculado&quot; en el tipo de registro de Campaña y se crea un tipo de registro vinculado denominado automáticamente &quot;Campaña&quot; en el tipo de registro de Producto.

   * **Cuando conecta un tipo de registro con un tipo de objeto de otra aplicación**:

      * Se crea un campo de registro vinculado en el tipo de registro desde el que se conecta. No se crea automáticamente ningún campo de registro vinculado en el tipo de objeto de la otra aplicación.

      * No se puede acceder a los campos de registros de Planning desde objetos de Workfront.
      * Se puede acceder a los campos de registro de planificación desde los recursos del Experience Manager cuando el administrador de Workfront configura la asignación de metadatos mediante la integración entre Workfront y Adobe Experience Manager Assets. Para obtener más información, consulte [Configuración de la asignación de metadatos de recursos entre Adobe Workfront y Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

   * **Al agregar campos vinculados (o de búsqueda) del registro u objeto al que se conecta**: puede conectar campos del objeto de la otra aplicación al tipo de registro de Workfront Planning. Los campos vinculados son de sólo lectura y muestran automáticamente información de registros u objetos conectados al conectar los registros o los objetos.

     Por ejemplo, si conecta el tipo de registro &quot;Campaña&quot; con un proyecto de Workfront y selecciona llevar el campo Fecha planificada de finalización del proyecto al registro de Workfront Planning, se crea automáticamente un campo vinculado llamado Fecha planificada de finalización (desde proyecto) para la campaña. Este campo vinculado no se puede editar manualmente. El campo Fecha planificada de finalización (del proyecto) muestra la fecha planificada de finalización de los proyectos vinculados.

     >[!IMPORTANT]
     >
     >    Todas las personas con permisos de Vista o superiores en el espacio de trabajo pueden ver la información en los campos vinculados, independientemente de sus permisos o nivel de acceso en la aplicación de los tipos de objetos vinculados.

* Los campos de registro vinculados van precedidos de un icono de relación ![](assets/relationship-field-icon.png).

  Los campos vinculados van precedidos de un icono que identifica el tipo de campo. Por ejemplo, los campos vinculados (o de búsqueda) van precedidos de iconos que indican que un campo es un número, un párrafo o una fecha.


## Conectar tipos de registros

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registros desee conectar,

   O

   Desde un espacio de trabajo, expanda la flecha hacia abajo a la derecha del nombre de un espacio de trabajo existente, busque un espacio de trabajo y selecciónelo cuando se muestre en la lista.
1. Haga clic en la tarjeta de un tipo de registro para abrir la página del tipo de registro.
1. Haga clic en **+** en la esquina superior derecha de la vista de tabla y, a continuación, haga clic en el icono **Nueva conexión** pestaña.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. En el **Tipo de registro** , busque un tipo de registro o seleccione una de las siguientes opciones:

   * Otro tipo de registro de la sección del espacio de trabajo seleccionado

     ![](assets/new-connection-tab-fields-with-another-record-selected.png)

     >[!TIP]
     >
     >Solo están disponibles para la conexión los tipos de registro del espacio de trabajo seleccionado.
     > 
     >Si no tiene otros tipos de registro en el espacio de trabajo seleccionado, la sección del espacio de trabajo no se muestra.

   * A **Proyecto, Portfolio, Programa, Empresa**, o **Grupo** desde el **Tipos de objetos Workfront** sección.

     ![](assets/workfront-project-connection-selection.png)

   * **Experience Manager Assets** desde el **Aplicaciones de Adobe** sección.

     ![](assets/aem-assets-connection-selection.png)

1. Actualice la siguiente información:

   * **Nombre**: Nombre del campo conectado, tal como aparecerá en la vista de tabla o en la página de registro del tipo de registro original. Esto crea la columna de registro vinculado en la vista de tabla del tipo de registro original o el campo de registro vinculado para los registros originales. De forma predeterminada, el nombre del campo es el nombre del registro u objeto al que se conecta.

   >[!TIP]
   >
   >Puede tener varias conexiones al mismo registro o tipo de objeto. Si no edita el nombre del campo conectado, Workfront agrega un número después del nombre del registro conectado para indicar el número de tipos de registros conectados con el mismo nombre.

   * **Descripción**: Información adicional sobre el campo de registro conectado. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo de una tabla.
   * **Permitir varios registros**: seleccione esta opción para indicar que permite que los usuarios puedan agregar varios registros cuando el campo de tipo de registro vinculado aparece en los registros originales. Esta opción está seleccionada de forma predeterminada.
   * **Seleccionar campos de búsqueda**: seleccione esta opción para agregar campos del tipo de registro seleccionado. Los campos de búsqueda son campos asociados al tipo de registro u objeto al que está vinculando. Al vincularlos, se muestra información del registro u objeto al que se está vinculando en el registro desde el que se está estableciendo el vínculo. Esta opción está seleccionada de forma predeterminada.

     >[!TIP]
     >
     > No puede agregar los siguientes tipos de campo como campos de búsqueda:
     >
     >    * Personas
     >    * Creado por
     >    * Última modificación realizada por
     >    * Campos de escritura anticipada de Workfront (incluidos campos como Propietario del proyecto o Patrocinador del proyecto)

1. (Condicional y opcional) Si ha seleccionado conectar un objeto de Workfront, seleccione un **Formulario personalizado** desde el **Vincular solo objetos que cumplan estos criterios** sección. Solo los objetos que tienen los formularios personalizados seleccionados adjuntos pueden vincularse al tipo de registro seleccionado. Puede seleccionar varios formularios.

   >[!NOTE]
   >
   > Debe crear formularios personalizados en Workfront para los objetos seleccionados antes de que se muestren en esta lista.

1. (Condicional) Si ha seleccionado conectarse a Experience Manager Assets, seleccione un repositorio en la **repositorio del Experience Manager** menú desplegable en el **Vincular recursos del siguiente repositorio** sección. Este campo es obligatorio. En este campo solo se muestran los repositorios a los que tiene acceso en Experience Manager Assets.

   >[!NOTE]
   >
   >El administrador de Workfront puede asignar campos de Workfront Planning a campos de Experience Manager Assets a través de la asignación de metadatos en Workfront. Para obtener más información, consulte [Configuración de la asignación de metadatos de recursos entre Adobe Workfront y Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

1. (Condicional) Si seleccionó conectarse a Experience Manager Assets o a un tipo de registro de Workfront Planning, deshabilite la variable **Título** alternar en **Registrar apariencia** , si no desea que el título de los registros o recursos conectados se muestre en el campo vinculado. Cuando está desactivado, solo se muestran las miniaturas de los registros en los campos vinculados. Los registros sin imagen en miniatura muestran un icono de imagen en su lugar. La opción está activada de forma predeterminada. Un ejemplo de cómo se mostrarán los registros conectados en la **Registrar apariencia** área.

   >[!TIP]
   >
   >    Cuando permite vincular varios registros, la visualización de sólo la miniatura puede ahorrar espacio en áreas más pequeñas, como las vistas de registros.
   >
   >El título de un registro es el campo principal del registro. Para obtener más información, consulte [Resumen del campo principal](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Haga clic en **Crear**.

1. (Condicional) Si seleccionó la variable **Seleccionar campo de búsqueda** configuración, la **Agregar campos de búsqueda** se abre el cuadro.

   Haga clic en **+** para añadir campos desde el **Campos no seleccionados** área.

   O

   Haga clic en **-** para eliminar campos de la **Campos seleccionados** área

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   Los valores de los campos conectados se rellenan automáticamente después de vincular registros u objetos.

   >[!IMPORTANT]
   >
   >    Todas las personas con permisos de Vista o superiores en el espacio de trabajo pueden ver la información en los campos vinculados, independientemente de sus permisos o nivel de acceso en la aplicación de los tipos de objetos vinculados.


1. (Opcional) Haga clic en **Omitir** para omitir agregar campos del registro vinculado o tipo de objeto. El **Nombre** o el **Título** del registro vinculado es el único campo visible en la vista de tabla del tipo de registro desde el que se conecta.

1. (Opcional y condicional) Si selecciona vincular un campo de número, moneda, porcentaje o tipo de fecha, seleccione también un valor de acumulador para resumir varios valores. Los valores de los campos vinculados se muestran separados por comas o como un valor resumido según el agregador que elija, cuando los usuarios seleccionan más de un registro vinculado en el campo de registro vinculado.

   Si el campo de búsqueda contiene varios valores que no están resumidos, tenga en cuenta lo siguiente al utilizar el campo en la ordenación o agrupación de una vista:

   * La ordenación se realiza mediante el primer valor

   * Los registros se agrupan por cada combinación única de valores de campo

   * La vista de cronología se crea en función del primer valor de fecha.

   >[!IMPORTANT]
   >
   >    Debe seleccionar un valor de agregado al agregar campos de fecha de búsqueda si desea que los campos estén disponibles para agregarlos como fechas de inicio y finalización en las vistas de calendario y escala de tiempo. Por ejemplo, puede seleccionar el agregador MAX o MIN para un campo de fecha de búsqueda.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Los acumuladores no están disponibles al conectar tipos de registros a Experience Manager Assets.

   Seleccione una de las siguientes opciones:

   * **Ninguno**: Muestra los valores procedentes de varios registros separados por comas. Esta es la selección predeterminada.
   * **MAX**: Muestra el valor más alto de todos los valores procedentes de varios registros seleccionados en el campo de registro vinculado.
   * **MIN**: Muestra el valor más bajo de todos los valores procedentes de varios registros seleccionados en el campo de registro vinculado.
   * **SUM**: Muestra el total de todos los valores procedentes de varios registros seleccionados en el campo de registro vinculado.
   * **AVG**: Muestra el promedio de todos los valores procedentes de varios registros seleccionados en el campo de registro vinculado.
   * **ÚNICO**: elimina los duplicados de los valores de los campos de búsqueda y solo muestra los valores únicos. Esto no está disponible para los siguientes tipos de campo:
      * Párrafo
      * Casilla de verificación
      * Personas

   >[!NOTE]
   >
   >Por ejemplo, puede vincular el registro de producto (registro vinculado) desde el registro de campaña (registro original) y asignarle el nombre &quot;Campo de producto&quot;. También puede vincular el campo Presupuesto del registro de producto del registro de campaña y llamarlo &quot;Presupuesto de producto&quot;. Si se le permite seleccionar varios registros en el &quot;Campo de producto&quot;, puede seleccionar el Producto 1 con un Presupuesto de 100 000 $ y el Producto 2 con un Presupuesto de 110 000 $, y el Producto 3 con un Presupuesto de 100 000 $. Puede ver la siguiente información de presupuesto en el campo vinculado desde el registro original, en función del agregador que elija:
   >
   >* **Ninguno**: 100 000 $, 110 000 $, 100 000 $
   >* **MAX**: 110 000 $
   >* **MIN**: 100 000 $
   >* **SUM**: 310 000 $
   >* **AVG**: 103.000,33 $
   >* **ÚNICO**: 100 000 $
   >

1. (Opcional) Utilice la variable **búsqueda** icono ![](assets/search-icon.png) para buscar un campo.

1. Clic **Añadir campos** para guardar los cambios.

   Se añaden los elementos siguientes:

   * Un campo de registro vinculado en el tipo de registro desde el que está vinculando. El campo de registro vinculado mostrará registros individuales del tipo de registro vinculado, después de agregarlos manualmente. Para obtener información sobre cómo agregar registros, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md). El nombre del campo de registro vinculado es el nombre seleccionado en el paso 7. <!--accurate-->

   * Campo (o campos) vinculado (o de búsqueda) que muestra información sobre el registro vinculado o los tipos de objeto después de agregar manualmente los registros u objetos en el campo de registro vinculado. Los campos de búsqueda solo se crean cuando **Seleccionar campos de búsqueda** La configuración se selecciona al crear la conexión. Los campos de búsqueda se nombran automáticamente según este patrón:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Por ejemplo, si ha vinculado un tipo de registro de campaña con un tipo de registro de programa y asigna al campo de registro vinculado de programa el nombre &quot;Información del programa&quot;, seleccione para mostrar también el campo Presupuesto del programa en la vista de tabla de la campaña, el campo vinculado se llamará automáticamente `Budget (from Program information)` en la vista de tabla de la campaña.

   * Cuando se vinculan tipos de registros entre sí, también se agrega un campo de registro vinculado en el tipo de registro al que se está vinculando. El nombre del campo de registro vinculado en el tipo de registro vinculado es el nombre del tipo de registro desde el que se establece el vínculo.

     Por ejemplo, si vincula el tipo de registro &quot;Producto&quot; desde el tipo de registro &quot;Campaña&quot; y asigna al campo conectado de la campaña el nombre &quot;Producto vinculado&quot;, se crea un campo de registro vinculado &quot;Campaña&quot; para el tipo de registro Producto.

     >[!TIP]
     >
     > No se crea un campo de registro vinculado para los objetos de otra aplicación con el tipo de registro desde el que se está vinculando en Workfront Planning.

1. (Opcional y condicional) Desde el tipo de registro original o la vista de tabla del tipo de registro vinculado, haga clic en la flecha hacia abajo en el encabezado de los campos de registro vinculados y, a continuación, haga clic en una de las siguientes opciones:

   * **Editar campo**: Puede actualizar el **Nombre** y el **Descripción** información del campo.
   * **Editar campos de búsqueda**: agregue o quite cualquiera de los campos del registro vinculado.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Para agregar o quitar campos de búsqueda, siga las instrucciones de los pasos 10 a 14 anteriores. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > No se pueden agregar campos de búsqueda que pertenezcan a tipos de registro que esté vinculando a tipos de objeto de otra aplicación.
   >
   > Por ejemplo, no puede agregar el campo de búsqueda &quot;Estado de campaña&quot; a un proyecto de Workfront al que esté vinculando desde las campañas.

1. (Opcional) Haga clic en la flecha hacia abajo situada en el encabezado de un campo de registro vinculado o en el encabezado de un campo de búsqueda desde el tipo de registro desde el que está vinculando y, a continuación, haga clic en **Eliminar**.

   Se eliminan el campo de registro o el campo de búsqueda. Si elimina un campo de registro, también se eliminarán todos los campos de búsqueda asociados al registro vinculado.
