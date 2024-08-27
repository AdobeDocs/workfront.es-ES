---
title: Ejemplo de conexión de tipos de registros y registros
description: Este artículo describe un ejemplo de cómo crear una conexión entre un tipo de registro de Adobe Workfront Planning y un tipo de objeto de proyecto de Workfront. También se describe cómo conectar un registro de Workfront Planning con un proyecto individual.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 38509572-72a4-4fce-b3ec-2cb31bb4669a
source-git-commit: 83c716dea3815ed9a2ce4c3d0598ef42b128de87
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
1. Haga clic en el icono **+** en la esquina superior derecha de la vista de tabla para agregar un nuevo campo, luego haga clic en **Nueva conexión** y, a continuación, haga clic en **Producto** en la sección del área de trabajo seleccionada.
1. Añada la siguiente información, por ejemplo:

   * **Tipo de registro**: Producto <!--did they change the casing here?-->
   * **Nombre**: asigne un nombre al nuevo campo. Por ejemplo, &quot;Información del producto&quot;. Es el nombre del campo de registro vinculado.
   * **Descripción**: agregue una descripción para el nuevo campo. Por ejemplo, &quot;Estos son los productos con los que quiero que se asocien mis campañas&quot;. La descripción del campo se muestra al pasar el ratón por encima del campo en el encabezado de la columna.
   * **Permitir varios registros**: si deja seleccionada esta opción, los usuarios podrán seleccionar varios registros cuando el campo de tipo de registro vinculado (Información del producto) se muestre en los registros originales (Campañas). En este caso, los usuarios pueden seleccionar varios productos para conectarlos a una campaña.
   * **Seleccionar campos de búsqueda**: si deja seleccionada esta opción, se abrirá el cuadro **Agregar campos de búsqueda** a continuación para que pueda vincular los campos de producto con el tipo de registro de campaña. Puede hacer clic en **Omitir** para omitir este paso y agregar campos de producto más adelante.

   ![](assets/new-connection-with-product-record-type.png)

1. (Opcional) Anule la selección del botón de alternancia **Title** en la sección **Apariencia de registro** para mostrar solo la imagen en miniatura del registro en los campos conectados. Si está activada, los registros muestran la miniatura y el título. La opción está activada de forma predeterminada.
1. (Condicional) Si seleccionó la opción **Seleccionar campos de búsqueda** en el paso anterior, en la lista de campos asociados con el tipo de registro **Producto**, haga clic en el icono **+** para el campo **Presupuesto** y, a continuación, haga clic en **Agregar campos**. Esto crea un campo denominado **Presupuesto (a partir de la información del producto)**, que es el nombre del campo vinculado. Cualquier información del presupuesto del producto se muestra en este campo para los registros de campaña.

   ![](assets/add-fields-for-budget-field-for-connector-with-record-type.png)

   >[!TIP]
   >
   >    Si desea ver el presupuesto de todos los productos seleccionados como un número total, seleccione **SUM** en el menú desplegable situado a la derecha del nombre del campo. Cuando los usuarios seleccionan varios productos en el campo de registro vinculado **Información del producto**, el campo **Presupuesto (de Información del producto)** suma todos sus valores de presupuesto y muestra el total. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Si selecciona **Ninguno**, en lugar de **SUMA**, los presupuestos individuales de los productos seleccionados se mostrarán separados por comas.

   Esto genera los campos siguientes:

   * En la vista de tabla Registro de campaña y en la página Registro de campaña de una campaña:

      * **Información del producto** (el campo de registro vinculado): esto muestra el nombre o los nombres de los productos cuando los agrega.
      * **Presupuesto (de la información del producto)** (el campo vinculado): esto mostrará los presupuestos de los productos seleccionados en el campo Información del producto.

   * En la vista de tabla de registros de producto y en la página de registro de producto de un producto:

      * **Campaign**: Esto indica que el tipo de registro de producto está vinculado desde el tipo de registro de campaña.

     ![](assets/example-campaign-information-relationship-fields-from-product-record-table.png)

   >[!TIP]
   >
   >    Los campos de registros vinculados van precedidos del icono de relación ![](assets/relationship-field-icon.png).

1. Desde la vista de tabla de tipo de registro **Campaign**, cree una campaña agregando una nueva fila en la tabla de la página de tipo de registro de Campaign.

1. Haga doble clic dentro de la columna **Información del producto** de la nueva campaña.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Realice una de las siguientes acciones:

   * Haga clic en el nombre de un producto conectado de la lista para agregarlo al registro seleccionado. El producto se añade automáticamente.
   * Empiece a escribir el nombre de un producto y haga clic en él cuando se muestre en la lista. El producto se añade automáticamente.
   * Haga clic en **Ver todo** para mostrar todos los productos.

1. (Condicional) Si hizo clic en **Ver todo** en el paso anterior, se muestra el cuadro **Conectar objetos**.

   ![](assets/connected-objects-table-for-records.png)

1. Comience a escribir el nombre de un producto en el cuadro de búsqueda y, a continuación, selecciónelo cuando se muestre en la lista

   O

   Seleccione los registros de productos que desea conectar con los registros de Campaign y haga clic en **Conectar objetos**.

   >[!TIP]
   >
   >    Puede abrir la página de registro de una campaña, buscar el campo de registro vinculado y hacer clic en el icono **+** del campo para agregar productos del tipo de registro de producto conectado.

   Las siguientes columnas se rellenan en la tabla de tipo de registro de Campaign:
   * El campo **Información del producto** se rellena para el registro de campaña con los productos seleccionados.
   * **El campo Presupuesto (de la información del producto)** se rellena con el valor Presupuesto de cada producto seleccionado o con un total de todos los presupuestos de los productos seleccionados (si seleccionó SUMA para el agregador).

   ![](assets/example-product-information-and-budget-relationship-fields-for-campaign-record-table.png)

   >[!TIP]
   >
   >Cuando no se selecciona un acumulador para varios valores, todos los valores de los productos seleccionados se muestran separados por comas.

1. Para rellenar el campo **Campaign** desde la vista de tabla de **Product**, repita los pasos del 5 al 7 a partir de la vista de tabla Tipo de registro de producto y seleccionando información de campaña. Esto también actualiza el campo Product information en la tabla de la página Campaign record type. <!--ensure the step numbers remain correct-->


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
1. Haga clic en el icono **+** en la esquina superior derecha de la vista de tabla para agregar un nuevo campo, luego haga clic en **Nueva conexión** y, a continuación, haga clic en **Proyecto** en la sección **Tipos de objetos de Workfront**.
1. Añada la siguiente información, por ejemplo:

   * **Tipo de registro**: Proyecto (de la subsección de Workfront)
   * **Nombre**: asigne un nombre al nuevo campo, por ejemplo &quot;Información del proyecto&quot;.
   * **Descripción**: agregue una descripción para el nuevo campo. Por ejemplo, &quot;Estos son los proyectos a los que quiero asociar mis campañas&quot;. La descripción se muestra en la vista de tabla a medida que pasa el ratón por encima del nombre del campo en el encabezado de la columna.
   * 
      * **Permitir varios registros**: si deja seleccionada esta opción, los usuarios podrán seleccionar varios proyectos cuando el campo de tipo de proyecto vinculado (Información del proyecto) se muestre en los registros originales (Campañas).
   * **Seleccionar campos de búsqueda**: si deja seleccionada esta opción, se abrirá el cuadro **Agregar campos de búsqueda** a continuación para que pueda vincular los campos de Project con el tipo de registro de Campaign. Puede hacer clic en **Omitir** para omitir este paso y agregar campos de proyecto más adelante.

   ![](assets/new-connection-tab-with-workfront-option.png)

1. (Condicional) Si seleccionó la opción **Seleccionar campos de búsqueda** en el paso anterior, en la lista de campos asociados con el tipo de objeto **Proyecto**, haga clic en el icono **+** para el campo **Ingresos planificados** y, a continuación, haga clic en **Agregar campos**. Esto crea un campo denominado **Ingresos planificados (a partir de la información del proyecto)**, que es el nombre del campo vinculado. Cualquier información del campo Ingresos planificados del proyecto se mostrará automáticamente en este campo para los registros de campaña.

   >[!TIP]
   >
   >    Si desea ver los ingresos planificados de todos los proyectos seleccionados como un número total, seleccione **SUM** en el menú desplegable a la derecha del nombre del campo. Cuando los usuarios seleccionan varios proyectos en el campo de objeto vinculado **Información del proyecto**, el campo **Ingresos planificados (de Información del producto)** suma todos sus valores y muestra el total. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Si selecciona **Ninguno**, en lugar de **SUMA**, los ingresos planificados individuales se muestran separados por comas.

   ![](assets/add-planned-revenue-project-field-to-new-connection.png)

   Esto genera los campos siguientes:

   * En la vista de tabla de registros de Campaign y en la página de registros de Campaign:

      * **Información del proyecto** (el campo del objeto vinculado): esto muestra el nombre o nombres de los proyectos.
      * **Ingresos planificados (de la información del proyecto)** (el campo vinculado): esto mostrará los ingresos planificados de los proyectos seleccionados en el campo de información del proyecto.

   >[!TIP]
   >
   >    Los campos de objetos vinculados van precedidos del icono de relación ![](assets/relationship-field-icon.png).

1. Desde la vista de tabla de tipo de registro **Campaign**, cree una campaña agregando una nueva fila en la tabla.

1. Haga doble clic dentro de la columna Información ** proyecto de la nueva campaña.

   ![](assets/connect-projects-smaller-box-in-table.png)

1. Realice una de las siguientes acciones:

   * Haga clic en el nombre de un proyecto de la lista para agregarlo al registro seleccionado. El proyecto se agrega automáticamente.
   * Empiece a escribir el nombre de un proyecto y haga clic en él cuando se muestre en la lista. El proyecto se agrega automáticamente.
   * Haga clic en **Ver todos** para mostrar todos los proyectos.

1. (Condicional) Si hizo clic en **Ver todo** en el paso anterior, se muestra el cuadro **Conectar objetos**.

   ![](assets/connect-projects-larger-box.png)

1. Comience a escribir el nombre de un proyecto en el cuadro de búsqueda y, a continuación, selecciónelo cuando se muestre en la lista

   O

   Seleccione los registros de Project que desee conectar con los registros de Campaign y haga clic en **Conectar objetos**.

   >[!TIP]
   >
   >    Puede abrir la página de una campaña, buscar el campo de proyecto vinculado y hacer clic en el icono **+** del campo para agregar proyectos desde el tipo de registro de producto conectado.

   Esto añade lo siguiente al espacio de trabajo seleccionado:

   * En la tabla Tipo de registro de campaña:
      * El campo **Información del proyecto** se rellena para el registro de campaña con los proyectos seleccionados.
      * El campo **Ingresos planificados (de la información del producto)** se rellena con el valor de presupuesto de cada producto seleccionado. Este es un campo de solo lectura.

   ![](assets/project-linked-field-and-planned-revenue-in-campaign-table-highlighted.png)

   >[!TIP]
   >
   >Cuando no se selecciona un agregador para los valores múltiples y se seleccionan varios objetos en el campo enlazado a objetos, todos los valores se muestran separados por comas.

1. Haga clic en el nombre de un proyecto en el campo de registro conectado.

   Esto abre el proyecto en Workfront si tiene al menos permisos de visualización en el proyecto.
1. (Opcional) Actualice la información sobre el proyecto en Workfront, si tiene permisos para hacerlo.

1. (Opcional) En la vista de tabla de Campaign, pase el ratón sobre el encabezado del campo **Información del proyecto**, haga clic en la flecha hacia abajo y, a continuación, haga clic en **Editar campos de búsqueda.**
1. Haga clic en el icono **+** de cualquier campo de proyecto que desee agregar al registro de Workfront Planning del proyecto en la sección **Campos no seleccionados**.
1. Haga clic en el icono **-** de cualquier campo de proyecto que desee eliminar del registro de Workfront Project Planning en la sección **Campos seleccionados**.
1. Haga clic en **Guardar**.

   Los campos vinculados adicionales se añaden al tipo de registro de campaña.
