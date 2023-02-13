---
user-type: administrator
product-area: system-administration;user-management
keywords: inicio rápido,inicio inicial,inicio rápido,inicio inicial
navigation-topic: use-kick-starts
title: 'Escenario de inicio rápido: Importar campos personalizados de varias opciones en Workfront'''
description: Puede importar campos personalizados con varias opciones en Adobe Workfront mediante la funcionalidad Inicio rápido .
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 80ad604330e8b55037f1607b754cc8bb34f6a3ec
workflow-type: tm+mt
source-wordcount: '2126'
ht-degree: 0%

---


# Caso Kick-Starts : Importar campos personalizados de varias opciones en Workfront

Puede importar campos personalizados con varias opciones en Adobe Workfront mediante la funcionalidad Inicio rápido .

Algunos ejemplos de campos personalizados con varias opciones son:

* Lista desplegable de selección múltiple
* Lista desplegable
* Casillas de verificación
* Botones de radio

Estos campos a veces pueden tener muchas opciones (a veces cientos). Importarlos con la funcionalidad Inicio rápido puede ahorrarle, como administrador de Workfront, mucho tiempo y asegurarse de evitar errores.

>[!IMPORTANT]
>
>Debe seguir los pasos descritos en las secciones siguientes, en este orden, para importar campos personalizados con varias opciones mediante un inicio inicial:
>
>1. Exportar datos personalizados existentes desde Workfront (paso opcional)
>1. Exportar la plantilla de inicio rápido para datos personalizados
>1. Rellenar la hoja de cálculo de Excel Kick-Starts
>1. Cargar la hoja de cálculo de Excel a Workfront



## Exportar datos personalizados existentes desde Workfront (paso opcional)

Si no está familiarizado con la estructura de la base de datos de Workfront o si no está familiarizado con el archivo de inicio que Workfront requiere para importar información, le recomendamos que exporte primero un archivo de inicio desde Workfront con información existente, similar a la de los campos que desea importar.

Por ejemplo, si desea importar formularios personalizados o campos personalizados, primero debe exportar un archivo de inicio inicial con datos personalizados existentes.

La exportación de los datos existentes primero le permite analizarlos y ver cómo se debe dar formato a los nuevos datos.

Si conoce bien los objetos y la estructura de la base de datos de Workfront, puede continuar con la sección siguiente.

Para exportar datos existentes desde Workfront:

1. Haga clic en **Menú principal > Configuración** en la esquina superior derecha de la interfaz de Workfront.
1. Expanda el **Sistema** a la izquierda, haga clic en **Exportar datos (inicio rápido)**.

   ![](assets/export-data-kick-starts-link-in-setup.png)

1. Select **Datos personalizados** en el **Qué incluir** para obtener más información.

   ![](assets/existing-custom-data-box-checked-kick-starts.png)

1. Choose **Archivo .xlsx** en el **Formato de descarga** para obtener más información.

   >[!TIP]
   >
   >    Dependiendo de la cantidad de datos personalizados que tenga en su sistema, esto puede tardar mucho tiempo.

   ![](assets/download-button-for-kick-starts.png)

1. Haga clic en **Descargar**. Se descarga un archivo .xlsx en el equipo. Desplácese hasta y ábrala.

   ![](assets/existing-data-excel-parameter-sheet.png)

1. Examine el archivo descargado y tenga en cuenta los siguientes detalles:

   * El archivo contiene varias hojas. Es posible que no necesite conocer la información de cada hoja, pero utilizará algunas hojas para importar la información. Tómese algún tiempo para familiarizarse con su contenido y especialmente con el formato del contenido de cada hoja.
   * Preste especial atención a los nombres de las columnas y al formato en el que se muestran los datos de cada columna.
   * No debe cambiar los nombres ni el orden de las columnas en ninguna de las hojas. Los encabezados de columna indican los campos que debe rellenar con su información, en cada fila. Si el encabezado de la columna aparece en negrita, se trata de un campo obligatorio, por lo que debe tener información en esa columna.
   >[!IMPORTANT]
   >
   >Es posible que algunos encabezados de columna no se muestren en negrita, pero es posible que sigan siendo obligatorios.

   * Mantenga el archivo descargado para referencia futura y continúe con la siguiente sección.


## Exportación de la plantilla Inicio rápido para datos personalizados

Después de analizar la información sobre los campos personalizados existentes en el sistema, puede descargar una nueva plantilla de inicio para la importación.

1. Haga clic en **Menú principal > Configuración** en la esquina superior derecha de la interfaz de Workfront.

1. Expanda el **Sistema** a la izquierda.

1. Haga clic en **Importar datos (inicio rápido)**.

   ![](assets/import-data-kick-starts-link-in-setup.png)

1. En el **Descargar una hoja de cálculo de inicio rápido en blanco** , elija la **Datos personalizados** casilla de verificación y haga clic en **Descargar**.

   ![](assets/blank-custom-data-option-checked-kick-starts.png)

   Se descarga en el equipo un archivo de inicio en blanco.

   >[!NOTE]
   >
   >El número de hojas del archivo, sus nombres y el número y los nombres de las columnas de cada hoja deben ser idénticos a los del inicio descargado en la sección anterior que contenían los datos personalizados existentes.

## Rellenar la hoja de cálculo de Excel Kick-Starts

Antes de rellenar la hoja de cálculo de excel, descargue la plantilla de inicio tal como se describe en la sección anterior.

>[!IMPORTANT]
>
>No intente importar información mediante una hoja de cálculo de Excel ad-hoc. Todas las hojas de cálculo para importar información a Workfront mediante la funcionalidad de inicio deben coincidir con el contenido de los archivos que descargue de Workfront y que se describe en este artículo.

Para rellenar la hoja de cálculo de Excel con información para los nuevos campos personalizados:

1. Abra la hoja de cálculo de Excel que descargó en la sección anterior y observe varias hojas. Cada hoja representa un objeto en la aplicación.

   >[!INFO]
   >
   >Por ejemplo, **Parámetro** (que hace referencia a Campo personalizado), **Opción de parámetro**(que hace referencia a la opción Campo personalizado ), **Categoría** (que hace referencia al formulario personalizado).
   >
   >Debe escribir los nombres de los objetos y sus atributos en el formato admitido por la base de datos de Workfront.
   >
   >Para obtener información sobre el significado de estos objetos, consulte la [Glosario de Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
   >
   >Para obtener información sobre los nombres de los objetos de la base de datos de Workfront, consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).
   >
   >![](assets/sheets-included-in-custom-data-export-kick-start-file.png)





1. Asegúrese de que la siguiente información tenga el formato correcto:

   * La primera fila de cada hoja debe permanecer vacía; de lo contrario, la importación genera un error.
   * Los encabezados de columna de cada hoja representan atributos de los objetos que se pueden configurar durante una importación. Todos los encabezados de columna deben permanecer en el mismo orden en el que se encuentran al exportar la hoja y no se puede cambiar su nombre.
   * Los encabezados de columna en negrita son campos obligatorios y deben tener un valor.

      >[!TIP]
      >
      >Algunas columnas son necesarias aunque no estén en negrita. Por ejemplo, la variable `isNew` y `ID` las columnas no están en negrita, pero son campos obligatorios.

1. Seleccione el `**PARAM Parameter`** hoja y añada información sobre los nuevos campos personalizados en las siguientes columnas requeridas:

   * **`isNew`** = enter **`TRUE`** en esta columna para cada línea que represente un nuevo campo personalizado. Esto indica que el campo es nuevo y no existe en Workfront.

      >[!TIP]
      >
      >    Si una línea representa un campo existente ya en Workfront, debe introducir **`isNew`** = **`FALSE`**.

   * **`ID`** = debe ser un número único para cada línea que represente un nuevo campo. Puede utilizar cualquier número que comience por 1, siempre que cada nuevo campo tenga un número único.
   * **`setDataType`** = para cada línea que representa un nuevo campo, introduzca el tipo de datos que admite el campo. Se debe introducir el tipo de datos tal como aparecería en la base de datos. Seleccione entre los siguientes tipos de datos:
      * **`NMBR`** para número
      * **`CURC`** para moneda
      * **`TEXT`** para texto
   * `**setDisplaySize**`= el tamaño de visualización (&#39;**setDisplaySize**&#39;) para cualquier opción, los campos personalizados siempre son 0.
   * **`setDisplayType`** = para cada línea que represente un nuevo campo, introduzca el tipo de visualización del campo. Se debe introducir el tipo de visualización tal como aparecería en la base de datos.

      Para campos personalizados con varias opciones, seleccione una de las siguientes opciones:

      * **`MULT`** para Selección múltiple, menú desplegable
      * **`SLCT`** para menú desplegable
      * **`RDIO`** para botones de opción
      * **`CHCK`** para casillas de verificación
      >[!TIP]
      >
      >Para buscar la información de Tipo de datos y Tipo de visualización, consulte la [Explorador de API](../../../wf-api/general/api-explorer.md), expanda el **Parámetro** y busque estos atributos en la sección **campos** pestaña .

   * **`setName`** = introduzca el nombre de los campos personalizados tal como desea que se muestren en Workfront.

      >[!INFO]
      >
      >Por ejemplo, podemos importar dos campos personalizados, llamados _Marca_, un campo de casilla de verificación y _Medios_, un campo de botón de radio.

   * La variable **`setName`** y **`setValue`** normalmente contienen la misma información y deben reflejar los nombres deseados en la interfaz de Workfront para el nuevo campo.
   El valor de un campo es el nombre que aparece en los informes, por ejemplo, mientras que el nombre aparece en los formularios personalizados adjuntos a los objetos.

   Para obtener más información, consulte [Añadir un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).

   ![](assets/parameter-sheet-filled-out-kick-starts.png)

1. Seleccione el **`POPT Parameter Options`** hoja y agregue información sobre las opciones de cada campo personalizado en las siguientes columnas requeridas:

   * **`isNew`** = enter **`TRUE`** en esta columna para cada línea que represente una nueva opción de campo.

      >[!TIP]
      >
      >    Si una línea representa una opción existente, debe introducir **`isNew`** = **`FALSE`**.

   * **`ID`** = debe ser un número único para cada línea que represente una nueva opción. Puede utilizar cualquier número que comience por 1, siempre que cada nueva opción tenga un número único.
   * **`setIsDefault`** = enter `TRUE` para las opciones que desea mostrar de forma predeterminada, y `FALSE` para todas las demás opciones, para cada campo.  Por ejemplo, queremos _Nike_ para que sea la opción predeterminada de _Marca_ y _Imprimir_ para que sea la opción predeterminada de _Medios_.

      >[!TIP]
      >
      >Solo puede tener una opción predeterminada para cada campo.

   * **`setParameterID`** = las opciones correspondientes a la variable _Marca_ el campo personalizado tiene un **`setParameterID`** de 1 y las opciones correspondientes a la variable _Medios_ tienen un **`setParameterID`**de 2. La variable `PARAM` y `POPT` las hojas se hacen referencias cruzadas entre sí para indicar qué opciones pertenecen a cada campo personalizado.
   * **`setDisplayOrder`**= la columna orden de visualización indica el orden en que se mostrarán las opciones en el campo personalizado. Puede empezar con 1 y continuar en orden ascendente para todas las opciones, independientemente de los campos a los que pertenezcan. Lo importante aquí es tener números únicos para cada opción.
   * La variable **`setLabel`** y `**setValue`** las columnas suelen contener la misma información y deben reflejar los nombres deseados en la interfaz de usuario de Workfront. El valor de una opción es el nombre que se muestra en los informes, por ejemplo, mientras que la etiqueta aparece en los formularios personalizados cuando se adjunta a un objeto. Para obtener más información, consulte [Añadir un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
   * **`setIsHidden`** = enter `TRUE` si desea que cualquiera de las opciones se oculte.
   ![](assets/parameter-option-sheet-filled-out-kick-starts.png)


1. (Opcional) Si también desea crear un formulario personalizado en el que posteriormente pueda agregar los campos nuevos, seleccione la opción  **`CTGY Category`** y actualice las siguientes columnas requeridas para la información del formulario personalizado:

   * **`isNew`** = enter **`TRUE`** en esta columna para cada línea que represente un nuevo formulario personalizado.
   * **`ID`** = introduzca un número único para cada línea que represente un formulario nuevo. Puede utilizar cualquier número que comience por 1, siempre que cada nueva opción o línea tenga un número único.
   * **`setGroupID`** = agregue el ID de grupo para su grupo principal o cualquier otro grupo del sistema cuyos miembros desee tener acceso a este formulario. Este campo es obligatorio.
   Para averiguar la `ID` de un grupo, puede crear un informe de grupo y agregar la variable `ID` en la vista o desplácese a un grupo y busque la dirección URL del grupo. El ID de grupo se encuentra en la dirección URL de la página del grupo. Por ejemplo, si la dirección URL del grupo es `https://companyName.my.workfront.com/group/575b000800467a6f66e747932c807464/members`, el ID del grupo es `575b000800467a6f66e747932c807464`.

   * **`setCatObjCode` **= es el código de objeto para el tipo de objeto para el que desea crear el formulario. Introduzca un código de las siguientes opciones:
      * **`CMPY`** para Empresa
      * **`TASK`** para la tarea
      * **`PROJ`** para proyecto
      * **`PORT`** para Portfolio
      * **`PRGM`** para el programa
      * **`USER`** para el usuario
      * **`DOCU`** para documento
      * **`OPTASK`** para problemas
      * **`EXPNS`** para gastos
      * **`ITRN`** para iteración
      * **`BILL`** para registros de facturación
      * **`GROUP`** para grupo
      >[!NOTE]
      >
      >Para los formularios de varios objetos, introduzca el primer objeto que seleccionaría al crear un formulario en la interfaz de usuario. Por ejemplo, establezca la variable `setCatObjCode` a `TASK`, si selecciona Tarea en la interfaz de Workfront y, a continuación, Problema, Portfolio, etc., pero no desea que el formulario esté disponible para Proyectos.

   * **`setName`** = es el nombre del formulario personalizado tal como desea que aparezca en la interfaz de Workfront.

      ![](assets/category-sheet-filled-out-kick-starts.png)



1. Guarde la hoja de cálculo como archivo .xls o .xlsx en el equipo. La hoja de cálculo de Excel se ha rellenado y ya está lista para su importación en Workfront.


## Cargar la hoja de cálculo de Excel a Workfront

Después de realizar los pasos descritos en las secciones anteriores, siga con lo siguiente para cargar los nuevos campos y formularios en Workfront:

1. Haga clic en **Importar datos** **(Inicio de marca) **en el **Menú principal > Configuración > Sistema** para abrir el Navegador.

1. Haga clic en **Elegir archivo** en la sección **Carga de datos con la hoja de cálculo Kick-Start**.

1. Busque la hoja de cálculo de Excel que ha preparado en el equipo y selecciónela cuando la encuentre.  Cuando Workfront reconoce el archivo, el botón Upload se vuelve azul.
1. Haga clic en **Cargar.**

   ![](assets/kick-start-file-selected-and-upload-blue-button.png)

1. Se muestra una notificación de que la importación se ha realizado correctamente. En función de la cantidad de información que importe, este paso puede tardar entre unos segundos y un minuto.

   ![](assets/kick-start-successful.png)

   Los nuevos campos y formularios personalizados se encuentran ahora en el sistema Workfront. Puede encontrarlos en el área Forms personalizado de Configuración.

   >[!NOTE]
   >
   >Los nuevos formularios y los campos importados aún no están conectados. El formulario se importa sin campos personalizados. Debe agregar manualmente los campos al nuevo formulario personalizado o a otro formulario personalizado existente.


   Para obtener información sobre cómo agregar campos a formularios personalizados, consulte [Añadir un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).

1. (Condicional) Si la importación no se ha realizado correctamente, recibirá un mensaje de error con el problema. Intente identificar el campo, la hoja y el número de fila en el que se encontró el problema, corregir la información del archivo de Excel y, a continuación, intente importar el archivo una vez más.

   ![](assets/kick-start-error.png)

1. (Condicional) Según el problema, como se indica en el mensaje de error, es posible que ya se haya importado parte de la información. Debe realizar una de las siguientes acciones antes de volver a importar la hoja:

   * Elimine la información que se importó correctamente desde Workfront del área de Forms personalizado y, a continuación, realice la corrección indicada por el mensaje de error.
   * Indique que ya hay un campo o un formulario en el sistema para los campos o formularios que ya se han importado y realice la corrección.
Para indicar que un campo o un formulario personalizado ya está en Workfront, debe asegurarse de que la variable `inNew` el campo está marcado como `FALSE` en hojas que contienen información sobre el formulario (`CTGY`) o el campo (`PARAM`) en la hoja de importación inicial.
