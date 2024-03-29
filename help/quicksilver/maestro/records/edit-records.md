---
title: Edición de registros
description: Puede editar la información de los registros en Adobe Workfront Planning. Debe crear tipos de registros antes de empezar a crear y editar registros.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Edición de registros

{{maestro-important-intro}}

Puede editar la información de los registros en Adobe Workfront Planning editando los valores de los campos asociados a los registros.

Debe crear tipos de registros antes de empezar a crear y editar registros.

Para obtener más información, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

Para obtener información sobre la creación de registros, consulte [Creación de registros](/help/quicksilver/maestro/records/create-records.md).

&lt;!— mencione aquí que los campos de la vista Detalles son los mismos que los de la vista de tabla — este artículo está vinculado desde Administrar vistas de registros a hacer referencia a esta información—>

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en el programa beta de planificación de Adobe Workfront. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <p>Nuevo: claro o superior</p>
   O
   <p>Actual: Trabajo o superior</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de acceso para la planificación de Adobe Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Permisos de contribución o superiores en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Consideraciones acerca de la edición de registros

* Puede editar los registros que haya creado o los creados por otros usuarios si dispone de permisos para el espacio de trabajo.
* Puede editar los campos de registro desde las siguientes áreas:

   * El cuadro Detalles de un registro de una vista de registros.
   * La página Detalles de un registro.
   * En línea, en una vista de tabla.

* Los siguientes tipos de campos se actualizan automáticamente y no se pueden editar sus valores manualmente:
   * Campos vinculados de otros registros
   * Campos de tipo fórmula
   * Campos del sistema (Creado por, Fecha de creación, Última modificación por, Fecha de última modificación)
* Si los registros que muestra están vinculados a otros registros, la nueva información de los registros que está modificando se reflejará en los registros vinculados.
* No puede editar registros de forma masiva. <!--this will probably change-->
* Las direcciones URL se reconocen como vínculos en tipos de campo de texto de una sola línea solo cuando comienzan con lo siguiente: http://, https://, ftp:// o www. .

## Edición de registros

Puede editar un registro desde las siguientes áreas:

* [Desde la vista de tabla de un tipo de registro](#edit-a-record-from-the-table-view-of-a-record-type)
* [Desde la página Detalles de un registro](#edit-a-record-from-the-records-details-page)

### Editar un registro en línea en la vista de tabla de un tipo de registro

{#step1-to-maestro}

Se abre el espacio de trabajo al que accedió por última vez.

1. (Opcional) Haga clic en la flecha hacia abajo situada a la derecha del nombre del área de trabajo para seleccionar el área de trabajo cuyos registros desea actualizar.
1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. (Condicional) Haga clic en la pestaña de una vista de tabla o en **+ Ver** para crear una vista de tabla. La vista de tabla debe ser la vista predeterminada, a menos que haya visto el tipo de registro en otro tipo de vista cuando accedió por última vez.

   Los registros asociados al tipo de registro seleccionado se muestran en la vista de tabla.
1. Haga clic dentro de la fila de un registro para empezar a editar la información sobre el registro en línea.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!NOTE]
   >
   >  No puede editar la información de los siguientes campos, ya que son de solo lectura y Workfront los actualiza automáticamente:
   >  
   >  * Campos vinculados que se crean conectando tipos de registro. Para obtener más información, consulte [Conectar tipos de registros](../architecture/connect-record-types.md).
   >  * Campos de los siguientes tipos: Creado por, Fecha de creación, Última modificación por, Fecha de última modificación, Campos de fórmula.

1. (Opcional y condicional) Cuando edite un campo de tipo Párrafo, utilice el siguiente **Texto enriquecido** opciones de formato:

   * Negrita
   * Cursiva
   * Subrayado
   * Añadir un vínculo
   * Agregar una lista con viñetas
   * Añadir una lista numerada

   ![](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Opcional) Haga doble clic en un campo de registro conectado para agregar registros u objetos conectados a otro registro. Para obtener más información, consulte [Conectar registros](/help/quicksilver/maestro/records/connect-records.md).
1. Prensa **Entrar** en el teclado o haga clic fuera de una fila para guardar los cambios. Los cambios se guardan automáticamente. A **Guardado** Este indicador se muestra brevemente en la esquina superior derecha de la vista de tabla para mostrar que los cambios se han guardado.


1. (Opcional) Para copiar y pegar información de un campo a otro, siga uno de estos procedimientos:

   * Copie uno o varios valores existentes de un campo y péguelos en un campo del mismo tipo en otro registro
   * Haga clic en el encabezado de una columna para seleccionarla y copiarla. A continuación, haga clic en el encabezado de otra columna y pegue el contenido de la columna copiada. Las columnas deben contener tipos de campo similares.
   * Con la tecla Mayús pulsada, haga clic en para seleccionar varias filas de una tabla, copie la información de las filas seleccionadas y, a continuación, haga clic en una fila diferente y pegue la información seleccionada en la nueva fila y en las filas siguientes.

   >[!NOTE]
   >
   >Tenga en cuenta lo siguiente:
   >
   >* Utilice los siguientes métodos abreviados del teclado para copiar y pegar información:
   >   * Copiar: CTRL + C (⌘ + C para Mac)
   >   * Pegar: CTRL + V (⌘ + V para Mac)
   >* No puede copiar información de otro origen que no sea un campo de registro del mismo tipo que el campo en el que pega la información.
   >
   >* No se pueden copiar y pegar valores de campo en el área de Detalles de un registro. Esta funcionalidad solo se admite en la vista de tabla de un tipo de registro.
   >* No puede copiar y pegar valores de campo para los siguientes tipos de campo:
   >
   >
   >    * Campos vinculados que se crean conectando tipos de registro. Puede copiar y pegar campos de registro vinculados. Para obtener más información, consulte [Conectar tipos de registros](../architecture/connect-record-types.md).
   >    * Campos de los siguientes tipos: Creado por, Fecha de creación, Última modificación por, Fecha de última modificación

1. (Opcional) Utilice los siguientes métodos abreviados del teclado para deshacer o rehacer la edición o copiar y pegar la información de los registros:

   * CTRL + Z (⌘ + Z para Mac) para deshacer un cambio
   * CTRL + Mayús + Z (⌘ + Mayús + Z para Mac) para rehacer un cambio

   >[!TIP]
   >
   >    Puede utilizar los métodos abreviados de teclado varias veces seguidas para deshacer varios cambios.

1. (Opcional) Agregue una miniatura a un registro. Para obtener más información, consulte [Añadir una miniatura en un registro](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

### Editar un registro desde el cuadro Detalles del registro en una vista

Puede editar un registro desde el cuadro Detalles de cualquier vista.

{{step1-to-maestro}}

El espacio de trabajo al que se accede por última vez se abre.

1. (Opcional) Haga clic en la flecha hacia abajo situada a la derecha del nombre del área de trabajo para seleccionar el área de trabajo cuyos registros desea actualizar.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. Desde cualquier vista, haga clic en el nombre de un registro

   O

   En la vista de tabla de tabla, haga clic en **Abrir detalles** icono ![](assets/open-details-icon-in-table-name-field.png) a la izquierda del nombre de un registro o haga clic en un nombre de registro. El **Detalles** se abre en la vista.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Puede ver el **Abrir detalles** a la izquierda del campo Nombre de un registro en una vista de tabla sólo cuando el campo Nombre es un campo principal.

1. Comience a editar la información del campo en **Detalles** cuadro. Workfront guarda automáticamente los cambios.

1. (Opcional) Haga clic en **Abrir en ficha nueva** icono ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> en la esquina superior derecha de la **Detalles** para abrir el cuadro de diálogo del registro **Detalles** en una nueva pestaña. Siga editando el registro como se describe en [Editar un registro desde la página de detalles del registro](#edit-a-record-from-the-records-details-page) de este artículo.

### Editar un registro desde la página de detalles del registro

Puede editar un registro desde la página Detalles.

{{step1-to-maestro}}

El espacio de trabajo al que se accede por última vez se abre.

1. (Opcional) Haga clic en la flecha hacia abajo situada a la derecha del nombre del área de trabajo para seleccionar el área de trabajo cuyos registros desea actualizar.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. Realice una de las siguientes acciones:

   * Desde cualquier vista, acceda al cuadro Detalles, tal como se describe en la [Editar un registro desde el cuadro Detalles del registro en una vista](#edit-a-record-from-the-records-details-box-in-a-view)de este artículo. A continuación, haga clic en **Abrir en ficha nueva** icono ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> en la esquina superior derecha de la **Detalles** para abrir el cuadro de diálogo del registro **Detalles** en una nueva pestaña.

   * Desde el **Tabla** , pase el ratón sobre el nombre de un registro y haga clic en el botón **Más** menú ![](assets/more-menu.png), luego haga clic en **Ver**

     ![](assets/contextual-menu-for-record-row.png)

     El registro **Detalles** se abre la página.

     ![](assets/details-page.png)

1. Haga clic en **Más** menú ![](assets/more-menu.png) a la derecha del nombre del registro y haga clic en **Editar**

   O

   Haga clic dentro de cualquier campo editable de la página Detalles para editar la información.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Clic **Guardar cambios**.