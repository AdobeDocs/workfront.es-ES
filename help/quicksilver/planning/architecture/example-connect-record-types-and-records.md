---
title: Ejemplo de conexión de tipos y registros
description: Este artículo describe un ejemplo de cómo crear una conexión entre un tipo de registro de Adobe Workfront Planning y un tipo de objeto de proyecto de Workfront. También se describe cómo conectar un registro de Workfront Planning con un proyecto individual.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 38509572-72a4-4fce-b3ec-2cb31bb4669a
source-git-commit: 52e8ce6dd5146d72f698583b531b3db6bc5dbf25
workflow-type: tm+mt
source-wordcount: '1801'
ht-degree: 0%

---

# Ejemplo de conexión de tipos y registros

{{planning-important-intro}}

Este artículo describe un ejemplo de lo siguiente:

* Cómo crear una conexión entre dos tipos de registros de Workfront Planning y dos registros.

* Cómo crear una conexión entre un tipo de registro de Workfront Planning y un tipo de objeto de proyecto de Workfront, así como una conexión entre un registro y un proyecto.

Para obtener más información, consulte los siguientes artículos:

* [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md)
* [Conectar registros](/help/quicksilver/planning/records/connect-records.md)

## Conectar dos tipos de registros y registros de Workfront Planning (ejemplo)

Por ejemplo, tiene un tipo de registro denominado Campaign como tipo de registro original.

También tiene otro tipo de registro llamado Producto, que tiene un campo de moneda denominado Presupuesto.

Desea crear un campo en el tipo de registro de Campaign en el que pueda mostrar los valores del campo Presupuesto del tipo de registro Producto.

Para ello:

1. Abra la vista de tabla del tipo de registro de campaña en un espacio de trabajo.
1. Haga clic en **+** en la esquina superior derecha de la vista de tabla para añadir un nuevo campo y haga clic en **Nueva conexión**, luego haga clic en **Product** en la sección del espacio de trabajo seleccionado.
1. Añada la siguiente información, por ejemplo:

   * **Tipo de registro**: producto <!--did they change the casing here?-->
   * **Nombre**: Asigne un nombre al nuevo campo. Por ejemplo, &quot;Información del producto&quot;. Es el nombre del campo de registro vinculado.
   * **Descripción**: Añada una descripción para el nuevo campo. Por ejemplo, &quot;Estos son los productos con los que quiero que se asocien mis campañas&quot;. La descripción del campo se muestra al pasar el ratón por encima del campo en el encabezado de la columna.
   * **Permitir varios registros**: Si deja seleccionada esta opción, los usuarios pueden seleccionar varios registros cuando el campo de tipo de registro vinculado (Información del producto) se muestra en los registros originales (Campañas). En este caso, los usuarios pueden seleccionar varios productos para conectarlos a una campaña.
   * **Seleccionar campos de búsqueda**: Si deja seleccionada esta opción, la variable **Agregar campos de búsqueda** se abre el cuadro de diálogo siguiente para permitirle vincular los campos de producto con el tipo de registro de Campaign. Puede hacer clic en **Omitir** para omitir este paso y añadir campos de producto más adelante.

   ![](assets/new-connection-with-product-record-type.png)

1. (Opcional) Anule la selección del **Título** alternar en **Registrar apariencia** para mostrar únicamente la imagen en miniatura del registro en los campos conectados. Si está activada, los registros muestran la miniatura y el título. La opción está activada de forma predeterminada.
1. (Condicional) Si seleccionó la variable **Seleccionar opción de campos de búsqueda** en el paso anterior, en la lista de campos asociados con el **Product** tipo de registro, haga clic en **+** para el **Presupuesto** y haga clic en **Añadir campos**. Esto crea un campo llamado **Presupuesto (de la información del producto)**, que es el nombre del campo vinculado. Cualquier información del presupuesto del producto se muestra en este campo para los registros de campaña.

   ![](assets/add-fields-for-budget-field-for-connector-with-record-type.png)

   >[!TIP]
   >
   >    Si desea ver el presupuesto de todos los productos seleccionados como un número total, seleccione **SUM** en el menú desplegable situado a la derecha del nombre del campo. Cuando los usuarios seleccionan varios productos en la **Información del producto** campo de registro vinculado, la variable **Presupuesto (de la información del producto)** El campo suma todos sus valores de Budget y muestra el total. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Si selecciona **Ninguno**, en lugar de **SUM**, los presupuestos individuales de los productos seleccionados se muestran separados por comas.

   Esto genera los campos siguientes:

   * En la vista de tabla Registro de campaña y en la página Registro de campaña de una campaña:

      * **Información del producto** (el campo de registro vinculado): muestra el nombre o los nombres de los productos cuando los agrega.
      * **Presupuesto (de la información del producto)** (el campo vinculado): esto muestra los presupuestos de los productos seleccionados en el campo Información del producto.

   * En la vista de tabla de registros de producto y en la página de registro de producto de un producto:

      * **Campaign**: esto indica que el tipo de registro de producto está vinculado desde el tipo de registro de campaña.

     ![](assets/example-campaign-information-relationship-fields-from-product-record-table.png)

   >[!TIP]
   >
   >    Los campos de registro vinculados van precedidos del icono de relación ![](assets/relationship-field-icon.png).

1. Desde el **Campaign** para crear una campaña agregando una fila nueva en la tabla de la página Tipo de registro de campaña.

1. Haga doble clic dentro de **Información del producto** de la nueva campaña.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Realice una de las siguientes acciones:

   * Haga clic en el nombre de un producto conectado de la lista para agregarlo al registro seleccionado. El producto se añade automáticamente.
   * Empiece a escribir el nombre de un producto y haga clic en él cuando se muestre en la lista. El producto se añade automáticamente.
   * Clic **Ver todo** para mostrar todos los productos.

1. (Condicional) Si hizo clic en **Ver todo** en el paso anterior, la variable **Conectar objetos** aparece el cuadro.

   ![](assets/connected-objects-table-for-records.png)

1. Comience a escribir el nombre de un producto en el cuadro de búsqueda y, a continuación, selecciónelo cuando se muestre en la lista

   O

   Seleccione los registros de producto que desea conectar con los registros de Campaign y haga clic en **Conectar objetos**.

   >[!TIP]
   >
   >    Puede abrir la página de registro de una campaña, buscar el campo de registro vinculado y hacer clic en **+** en el campo para añadir productos del tipo de registro de producto conectado.

   Las siguientes columnas se rellenan en la tabla de tipo de registro de Campaign:
   * El **Información del producto** El campo se rellena para el registro de Campaign con los productos seleccionados.
   * **El presupuesto (de la información del producto)** Este campo se rellena con el valor de Presupuesto para cada Producto seleccionado, o con un total de todos los presupuestos de los productos seleccionados (si ha seleccionado SUMA para el agregador).

   ![](assets/example-product-information-and-budget-relationship-fields-for-campaign-record-table.png)

   >[!TIP]
   >
   >Cuando no se selecciona un acumulador para varios valores, todos los valores de los productos seleccionados se muestran separados por comas.

1. Para rellenar el **Campaign** del campo **Product** vista de tabla, repita los pasos del 5 al 7 empezando por la vista de tabla Tipo de registro de producto y seleccionando información de campaña. Esto también actualiza el campo Product information en la tabla de la página Campaign record type. <!--ensure the step numbers remain correct-->


## Conectar un tipo de registro de Workfront Planning con un tipo de objeto de proyecto de Workfront y conectar un registro con proyectos individuales

>[!IMPORTANT]
>
>    Todas las personas con permisos de Vista o superiores en el espacio de trabajo pueden ver la información en los campos vinculados, independientemente de sus permisos o nivel de acceso en Workfront.

Por ejemplo, tiene un tipo de registro denominado Campaign como tipo de registro original.

También tiene proyectos en Workfront con un campo llamado &quot;Ingresos planificados&quot;.

Desea crear un campo de conexión en el tipo de registro de Campaign donde puede mostrar los valores del campo Ingresos planificados de los proyectos en Workfront que están conectados a campañas en Workfront Planning.

Para ello:

1. Vaya a una Workspace en la que desee conectar el tipo de registro de campaña con proyectos de Workfront.
1. Abra la vista de tabla del tipo de registro de campaña en el espacio de trabajo seleccionado.
1. Haga clic en **+** en la esquina superior derecha de la vista de tabla para añadir un nuevo campo y haga clic en **Nueva conexión**, luego haga clic en **Proyecto** en el **Tipos de objeto de Workfront** sección.
1. Añada la siguiente información, por ejemplo:

   * **Tipo de registro**: proyecto (desde la subsección de Workfront)
   * **Nombre**: Asigne un nombre al nuevo campo, por ejemplo, &quot;Información del proyecto&quot;.
   * **Descripción**: Añada una descripción para el nuevo campo. Por ejemplo, &quot;Estos son los proyectos a los que quiero asociar mis campañas&quot;. La descripción se muestra en la vista de tabla a medida que pasa el ratón por encima del nombre del campo en el encabezado de la columna.
   * 
      * **Permitir varios registros**: Si deja seleccionada esta opción, los usuarios pueden seleccionar varios proyectos cuando el campo de tipo de proyecto vinculado (Información del proyecto) se muestra en los registros originales (Campañas).
   * **Seleccionar campos de búsqueda**: Si deja seleccionada esta opción, la variable **Agregar campos de búsqueda** se abre el cuadro siguiente para permitirle vincular los campos de Project con el tipo de registro de Campaign. Puede hacer clic en **Omitir** para omitir este paso y agregar campos de proyecto más adelante.

   ![](assets/new-connection-tab-with-workfront-option.png)

1. (Condicional) Si seleccionó la variable **Seleccionar opción de campos de búsqueda** en el paso anterior, en la lista de campos asociados con el **Proyecto** tipo de objeto, haga clic en **+** para el **Ingresos planificados** y haga clic en **Añadir campos**. Esto crea un campo llamado **Ingresos planificados (de la información del proyecto)**, que es el nombre del campo vinculado. Cualquier información del campo Ingresos planificados del proyecto se mostrará automáticamente en este campo para los registros de campaña.

   >[!TIP]
   >
   >    Si desea ver los ingresos planificados de todos los proyectos seleccionados como un número total, seleccione **SUM** en el menú desplegable situado a la derecha del nombre del campo. Cuando los usuarios seleccionan varios proyectos en la **Información del proyecto** Campo de objeto vinculado, la variable **Ingresos planificados (de la información del producto)** Este campo suma todos sus valores y muestra el total. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Si selecciona **Ninguno**, en lugar de **SUM**, los ingresos planificados individuales se muestran separados por comas.

   ![](assets/add-planned-revenue-project-field-to-new-connection.png)

   Esto genera los campos siguientes:

   * En la vista de tabla de registros de Campaign y en la página de registros de Campaign:

      * **Información del proyecto** (el campo del objeto vinculado): Muestra el nombre o los nombres de los proyectos.
      * **Ingresos planificados (de la información del proyecto)** (el campo vinculado): Esto muestra los ingresos planificados de los proyectos seleccionados en el campo Información del proyecto.

   >[!TIP]
   >
   >    Los campos de objeto vinculados van precedidos del icono de relación ![](assets/relationship-field-icon.png).

1. Desde el **Campaign** tipo de registro vista de tabla, cree una campaña agregando una nueva fila en la tabla.

1. Haga doble clic dentro de la columna Información ** proyecto de la nueva campaña.

   ![](assets/connect-projects-smaller-box-in-table.png)

1. Realice una de las siguientes acciones:

   * Haga clic en el nombre de un proyecto de la lista para agregarlo al registro seleccionado. El proyecto se agrega automáticamente.
   * Empiece a escribir el nombre de un proyecto y haga clic en él cuando se muestre en la lista. El proyecto se agrega automáticamente.
   * Clic **Ver todo** para mostrar todos los proyectos.

1. (Condicional) Si hizo clic en **Ver todo** en el paso anterior, la variable **Conectar objetos** aparece el cuadro.

   ![](assets/connect-projects-larger-box.png)

1. Comience a escribir el nombre de un proyecto en el cuadro de búsqueda y, a continuación, selecciónelo cuando se muestre en la lista

   O

   Seleccione los registros de Project que desee conectar con los registros de Campaign y haga clic en **Conectar objetos**.

   >[!TIP]
   >
   >    Puede abrir la página de una campaña, buscar el campo del proyecto vinculado y hacer clic en **+** en el campo para añadir proyectos desde el tipo de registro de producto conectado.

   Esto añade lo siguiente al espacio de trabajo seleccionado:

   * En la tabla Tipo de registro de campaña:
      * El **Información del proyecto** Este campo se rellena para el registro de Campaign con los proyectos seleccionados.
      * El **Ingresos planificados (de la información del producto)** Este campo se rellena con el valor de Presupuesto para cada Producto seleccionado. Este es un campo de solo lectura.

   ![](assets/project-linked-field-and-planned-revenue-in-campaign-table-highlighted.png)

   >[!TIP]
   >
   >Cuando no se selecciona un agregador para los valores múltiples y se seleccionan varios objetos en el campo enlazado a objetos, todos los valores se muestran separados por comas.

1. Haga clic en el nombre de un proyecto en el campo de registro conectado.

   Esto abre el proyecto en Workfront si tiene al menos permisos de visualización en el proyecto.
1. (Opcional) Actualice la información sobre el proyecto en Workfront, si tiene permisos para hacerlo.

1. (Opcional) En la vista de tabla de Campaign, pase el ratón sobre la **Información del proyecto** encabezado de campo, haga clic en la flecha hacia abajo y, a continuación, haga clic en **Editar campos de búsqueda.**
1. Haga clic en **+** icono para cualquier campo de proyecto que desee agregar al registro de planificación de Workfront del proyecto en la **Campos no seleccionados** sección.
1. Haga clic en **-** icono para cualquier campo de proyecto que desee eliminar del registro de planificación de proyectos de Workfront en **Campos seleccionados** sección.
1. Haga clic en **Guardar**.

   Los campos vinculados adicionales se añaden al tipo de registro de campaña.
