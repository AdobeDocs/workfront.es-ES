---
title: Ejemplo de conexión de tipos de registros y registros
description: Este artículo describe un ejemplo de cómo crear una conexión entre un tipo de registro de Adobe Workfront Planning y un tipo de objeto de proyecto de Workfront. También se describe cómo conectar un registro de Workfront Planning con un proyecto individual.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 38509572-72a4-4fce-b3ec-2cb31bb4669a
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '2047'
ht-degree: 81%

---

# Ejemplo de conexión de tipos de registro y registros

{{planning-important-intro}}

Este artículo describe un ejemplo de lo siguiente:

* Cómo crear una conexión entre dos tipos de registros de Workfront Planning y dos registros.

* Cómo crear una conexión entre un tipo de registro de Workfront Planning y un tipo de objeto de proyecto de Workfront, así como una conexión entre un registro y un proyecto.

Para obtener más información, consulte los siguientes artículos:

* [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md)
* [Conectar registros](/help/quicksilver/planning/records/connect-records.md)

## Conectar dos tipos de registros de Workfront Planning y registros de Workfront Planning (ejemplo)

Por ejemplo, tiene un tipo de registro denominado Campaña como tipo de registro original.

También tiene otro tipo de registro llamado Producto, que tiene un campo de moneda denominado Presupuesto.

Desea crear un campo en el tipo de registro de Campaña en el que pueda mostrar los valores del campo Presupuesto del tipo de registro Producto.

Para ello:

1. Abra la vista de tabla del tipo de registro de Campaña en un espacio de trabajo.
1. Haga clic en el icono **+** en la esquina superior derecha de la vista de tabla para añadir un nuevo campo, luego haga clic en **Nueva conexión** y, a continuación, haga clic en **Producto** en la sección del área de trabajo seleccionada.
1. Añada la siguiente información, por ejemplo:

   * **Tipo de registro**: producto <!--did they change the casing here?-->
   * **Nombre**: asigne un nombre al nuevo campo. Por ejemplo, “Información del producto”. Es el nombre del campo de registro vinculado.
   * **Descripción**: añada una descripción para el nuevo campo. Por ejemplo, &quot;Estos son los productos con los que quiero que se asocien mis campañas&quot;. La descripción del campo se muestra al pasar el puntero por encima del campo en el encabezado de la columna.
   * **Tipo de conexión**: seleccione una de las siguientes opciones:
      * **Muchos a muchos**: Los usuarios pueden conectar una campaña a varios productos y un producto a varias campañas.
      * **De uno a varios**: los usuarios pueden conectar una campaña a varios productos y un producto a una campaña.
      * **Muchas a una**: los usuarios pueden conectar una campaña a un producto y un producto a varias campañas.
      * **Uno a uno**: los usuarios pueden conectar una campaña a un producto y un producto a una campaña.

     >[!NOTE]
     >
     >La opción **Tipo de conexión** no está disponible al conectar registros de diferentes espacios de trabajo o al conectar recursos de Experience Manager. Para obtener más información, vea [Información general sobre los tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

   * **Apariencia del registro**: elija entre las siguientes opciones:
      * **Nombre e imagen**: muestra el nombre y la miniatura o el icono de los registros conectados. Esta opción está seleccionada de forma predeterminada.
      * **Nombre**: muestra solamente el nombre de los registros conectados.
      * **Imagen**: muestra solamente la miniatura o el icono de los registros conectados.
   * **Seleccionar campos de búsqueda**: si deja seleccionada esta opción, se abrirá el cuadro **Añadir campos de búsqueda** a continuación para que pueda vincular los campos de producto con el tipo de registro de campaña. Puede hacer clic en **Omitir** para omitir este paso y añadir campos de producto más adelante.

     ![Nueva conexión con tipo de registro de producto](assets/new-connection-with-product-record-type.png)

1. (Condicional) Si ha seleccionado la opción **Seleccionar campos de búsqueda** en el paso anterior, en la lista de campos asociados con el tipo de registro **Producto**, haga clic en el icono **+** para el campo **Presupuesto** y, a continuación, haga clic en **Añadir campos**. Esto crea un campo denominado **Presupuesto (a partir de la información del producto)**, que es el nombre del campo vinculado. Cualquier información del presupuesto del producto se muestra en este campo para los registros de campaña.

   ![Agregar campos para el campo de presupuesto para la conexión con el tipo de registro](assets/add-fields-for-budget-field-for-connector-with-record-type.png)

   >[!TIP]
   >
   >    Si desea ver el presupuesto de todos los productos seleccionados como un número total, seleccione **SUM** en el menú desplegable situado a la derecha del nombre del campo. Cuando los usuarios seleccionan varios productos en el campo de registro vinculado **Información del producto**, el campo **Presupuesto (de Información del producto)** suma todos sus valores de presupuesto y muestra el total. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Si selecciona **Ninguno**, en lugar de **SUM**, los presupuestos individuales de los productos seleccionados se mostrarán separados por comas.

   Esto genera los campos siguientes:

   * En la vista de la tabla del registro de Campaña y en la página de registro de Campaña de una campaña:

      * **Información del producto** (el campo de registro vinculado): esto muestra el nombre o los nombres de los productos cuando los añade.
      * **Presupuesto (de la información del producto)** (el campo vinculado): esto mostrará los presupuestos de los productos seleccionados en el campo Información del producto.

   * En la vista de la tabla de registros de producto y en la página de registros de productos de un producto:

      * **Campaña**: esto indica que el tipo de registro de Producto está vinculado desde el tipo de registro de Campaign.

     ![Ejemplo de campos de relación de información de campaña de la tabla de registros de productos](assets/example-campaign-information-relationship-fields-from-product-record-table.png)

   >[!TIP]
   >
   >    Los campos de registros vinculados están precedidos por el icono de relación ![Icono de campo de relación](assets/relationship-field-icon.png).

1. Desde la vista de tabla del tipo de registro **Campaña**, cree una campaña añadiendo una nueva fila en la tabla de la página de tipo de registro de Campaña.

1. Haga doble clic dentro de la columna **Información del producto** de la nueva campaña.

   ![Conectar otro cuadro más pequeño de registros en la vista de tabla](assets/connect-other-records-smaller-box-in-table-view.png)

1. Realice una de las siguientes acciones:

   * Haga clic en el nombre de un producto conectado de la lista para añadirlo al registro seleccionado. El producto se añadirá automáticamente.
   * Empiece a escribir el nombre de un producto y haga clic en él cuando se muestre en la lista. El producto se añadirá automáticamente.
   * Haga clic en **Ver todo** para mostrar todos los productos.

1. (Condicional) Si hizo clic en **Ver todo** en el paso anterior, se mostrará el cuadro **Conectar objetos**.

   ![Tabla de objetos conectados para registros](assets/connected-objects-table-for-records.png)

1. Empiece a escribir el nombre de un producto en el cuadro de búsqueda y, a continuación, selecciónelo cuando se muestre en la lista

   O

   Seleccione los registros de productos que desea conectar a los registros de Campaña y a continuación, haga clic en **Conectar objetos**.

   >[!TIP]
   >
   >    Puede abrir la página de registro de una campaña, buscar el campo de registro vinculado y hacer clic en el icono **+** del campo para añadir productos del tipo de registro de producto conectado.

   Las siguientes columnas se rellenan en la tabla del tipo de registro de Campaña:
   * El campo **Información del producto** se rellena para el registro de Campaña con los productos seleccionados.
   * El campo **Presupuesto (de Información del producto)** se rellena con el valor de presupuesto de cada producto seleccionado o con un total de todos los presupuestos de los productos seleccionados (si seleccionó SUM para el agregador).

   ![Ejemplo de información de producto y campos de relación de presupuesto para la tabla de registro de campaña](assets/example-product-information-and-budget-relationship-fields-for-campaign-record-table.png)

   >[!TIP]
   >
   >Cuando no se selecciona un agregador para varios valores, todos los valores de los productos seleccionados se muestran separados por comas.

1. Para rellenar el campo **Campaña** desde la vista de tabla **Producto**, repita los pasos del 5 al 7 empezando por la vista de la tabla del tipo de registro de Producto y seleccione la información de campaña. Se actualizará también el campo Información del producto en la tabla del tipo de registro de Campaña. <!--ensure the step numbers remain correct-->


## Conexión de un tipo de registro de Workfront Planning a un tipo de objeto de proyecto de Workfront y conexión de un registro a proyectos individuales

>[!IMPORTANT]
>
>    Todas las personas con permisos de visualización o superiores en el espacio de trabajo pueden ver la información en los campos vinculados, independientemente de sus permisos o nivel de acceso en Workfront.

Por ejemplo, tiene un tipo de registro denominado Campaña como tipo de registro original.

También tiene proyectos en Workfront con un campo llamado &quot;Ingresos planificados&quot;.

Desea crear un campo de conexión en el tipo de registro de Campaña donde puede mostrar los valores del campo Ingresos planificados de los proyectos en Workfront que están conectados a campañas en Workfront Planning.

Para ello:

1. Vaya a un espacio de trabajo en el que desee conectar el tipo de registro de Campaña a proyectos de Workfront.
1. Abra la vista de tabla del tipo de registro de Campaña en el espacio de trabajo seleccionado.
1. Haga clic en el icono **+** en la esquina superior derecha de la vista de tabla para añadir un nuevo campo, luego haga clic en **Nueva conexión** y, a continuación, haga clic en **Proyecto** en la sección **Tipos de objetos de Workfront**.
1. Añada la siguiente información, por ejemplo:

   * **Tipo de registro**: proyecto (de la subsección de Workfront)
   * **Nombre**: asigne un nombre al nuevo campo, por ejemplo &quot;Información del proyecto&quot;.
   * **Descripción**: añada una descripción para el nuevo campo. Por ejemplo, &quot;Estos son los proyectos a los que quiero asociar mis campañas&quot;. La descripción se muestra en la vista de tabla al pasar el puntero por encima del nombre del campo en el encabezado de la columna.
   * **Tipo de conexión**: seleccione una de las siguientes opciones:
      * **Muchos a muchos**: Los usuarios pueden conectar una campaña a varios productos y un producto a varias campañas.
      * **De uno a varios**: los usuarios pueden conectar una campaña a varios productos y un producto a una campaña.
      * **Muchas a una**: los usuarios pueden conectar una campaña a un producto y un producto a varias campañas.
      * **Uno a uno**: los usuarios pueden conectar una campaña a un producto y un producto a una campaña.
   * **Vincular solo objetos que cumplan estos criterios**: seleccione un formulario personalizado en el menú desplegable **Formulario personalizado**. Solo los proyectos asociados con los formularios especificados están disponibles para conectarse a campañas. Puede seleccionar varios formularios.
   * **Seleccionar campos de búsqueda**: si deja seleccionada esta opción, se abrirá a continuación el cuadro **Añadir campos de búsqueda** para que pueda vincular los campos de Proyecto al tipo de registro de Campaña. Puede hacer clic en **Omitir** para omitir este paso y añadir campos de proyecto más adelante.

   ![Nueva pestaña de conexión con la opción Workfront](assets/new-connection-tab-with-workfront-option.png)

1. (Condicional) Si seleccionó la opción **Seleccionar campos de búsqueda** en el paso anterior, en la lista de campos asociados al tipo de objeto **Proyecto**, haga clic en el icono **+** para el campo **Ingresos planificados** y, a continuación, haga clic en **Añadir campos**. Se creará un campo denominado **Ingresos planificados (de Información del proyecto)**, que es el nombre del campo vinculado. Cualquier información del campo Ingresos planificados del proyecto se mostrará automáticamente en este campo para los registros de Campaña.

   >[!TIP]
   >
   >    Si desea ver los ingresos planificados de todos los proyectos seleccionados como un número total, seleccione **SUM** en el menú desplegable a la derecha del nombre del campo. Cuando los usuarios seleccionan varios proyectos en el campo de objeto vinculado **Información del proyecto**, el campo **Ingresos planificados (de Información del producto)** suma todos sus valores y muestra el total. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Si selecciona **Ninguno**, en lugar de **SUM**, los ingresos planificados individuales se muestran separados por comas.

   ![Agregar campo de proyecto de ingresos planificados a una nueva conexión](assets/add-planned-revenue-project-field-to-new-connection.png)

   Esto genera los campos siguientes:

   * En la vista de tabla del registro de Campaña y en la página del registro de Campaña:

      * **Información del proyecto** (el campo del objeto vinculado): muestra el nombre o nombres de los proyectos.
      * **Ingresos planificados (de Información del proyecto)** (el campo vinculado): se mostrarán los ingresos planificados de los proyectos seleccionados en el campo Información del proyecto.

   >[!TIP]
   >
   >    Los campos de objetos vinculados están precedidos por el icono de relación ![Icono de campo de relación](assets/relationship-field-icon.png).

1. En la vista de tabla de tipo de registro **Campaña**, cree una campaña añadiendo una nueva fila en la tabla.

1. Haga doble clic dentro de la columna Información del proyecto** de la nueva campaña.

   ![Conectar proyectos en un cuadro más pequeño de la tabla](assets/connect-projects-smaller-box-in-table.png)

1. Realice una de las siguientes acciones:

   * Haga clic en el nombre de un proyecto de la lista para añadirlo al registro seleccionado. El proyecto se añade automáticamente.
   * Empiece a escribir el nombre de un proyecto y haga clic en él cuando se muestre en la lista. El proyecto se añade automáticamente.
   * Haga clic en **Ver todos** para mostrar todos los proyectos.

1. (Condicional) Si hizo clic en **Ver todos** en el paso anterior, se muestra el cuadro **Conectar objetos**.

   ![Conectar proyectos con cuadro más grande](assets/connect-projects-larger-box.png)

1. Comience a escribir el nombre de un proyecto en el cuadro de búsqueda y, a continuación, selecciónelo cuando se muestre en la lista

   O

   Seleccione los registros de proyectos que desee conectar con los registros de campañas y haga clic en **Conectar objetos**.

   >[!TIP]
   >
   >    Puede abrir la página de una campaña, buscar el campo de proyecto vinculado y hacer clic en el icono **+** del campo para añadir proyectos del tipo de registro de producto conectado.

   Esto añade lo siguiente al espacio de trabajo seleccionado:

   * En la tabla de tipo de registro de campaña:
      * El campo **Información del proyecto** se rellena para el registro de campaña con los proyectos seleccionados.
      * El campo **Ingresos planificados (de la información del producto)** se rellena con el valor de presupuesto de cada producto seleccionado. Este campo es de solo lectura.

   ![Campo vinculado al proyecto e ingresos planificados resaltados en la tabla de la campaña](assets/project-linked-field-and-planned-revenue-in-campaign-table-highlighted.png)

   >[!TIP]
   >
   >Cuando no se selecciona una agregación para los valores múltiples y se seleccionan varios objetos en el campo vinculado al objeto, todos los valores se muestran separados por comas.

1. Haga clic en el nombre de un proyecto en el campo de registro conectado.

   Se abre el proyecto en Workfront si tiene al menos permisos de visualización sobre el proyecto.
1. (Opcional) Actualice la información sobre el proyecto en Workfront, si tiene permisos para hacerlo.

1. (Opcional) En la vista de tabla de la campaña, pase el puntero por encima del encabezado del campo **Información del proyecto**, haga clic en la flecha que apunta hacia abajo y, a continuación, haga clic en **Editar campos de búsqueda.**
1. Haga clic en el icono **+** de los campos de cualquier proyecto que desee añadir al registro de Planificación de Workfront del proyecto en la sección **Campos no seleccionados**.
1. Haga clic en el icono **-** de los campos de cualquier proyecto que desee quitar del registro de Planificación de Workfront del proyecto en la sección **Campos seleccionados**.
1. Haga clic en **Guardar**.

   Los campos vinculados adicionales se añaden al tipo de registro de campaña.
