---
title: Crear campos
description: En Adobe Workfront Planning, puede crear campos personalizados para cada tipo de registro. A continuación, puede asociar el campo con los registros de Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '4129'
ht-degree: 1%

---


<!--Should the structure of this article be like this other one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

<!--Do we need this for FORMULAS: when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula - not sure is needed??-->

# Creación de campos

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

En Adobe Workfront Planning, puede crear campos personalizados para los tipos de registro. A continuación, puede asociar los campos con los registros de Workfront Planning para mejorar la información de los registros.

Debe crear tipos de registros antes de poder crear campos que se asocien a ellos. Para obtener más información, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

Puede crear campos de las siguientes maneras en Workfront Planning:

* Desde cero
* Conectando tipos de registros
* Creando un tipo de registro
* Al crear un espacio de trabajo a partir de una plantilla
  <!--* By importing record types using an Excel or CSV file-->

Para obtener más información acerca de los campos de Workfront Planning, vea [Información general de los campos](/help/quicksilver/planning/fields/fields-overview.md).

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
   <td><p> Estándar </p>
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
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
OLD:

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
   <td> <p>There are no access level control for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->


## Crear campos desde cero {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos registros desee crear campos.

   Se abre el espacio de trabajo y se muestran los tipos de registro.

1. Haga clic en la tarjeta de un tipo de registro.

   Todos los registros existentes asociados al tipo de registro se muestran en las filas de la vista de tabla.

   >[!TIP]
   >
   >    Si no se muestra ningún registro, es posible que aún no tenga ningún registro, o que tenga aplicado un filtro que limite lo que ve en la pantalla.

   Todos los campos existentes asociados al tipo de registro se muestran en las columnas de la vista de tabla.

   >[!TIP]
   >
   >    Algunos campos pueden estar ocultos. Haga clic en Campos y active la opción de los campos que desee ver como columnas en la vista de tabla.

1. Haga clic en el icono **+** en la esquina superior derecha de la vista de tabla

   O

   Pase el ratón sobre el encabezado de cualquier columna, haga clic en la flecha hacia abajo después del nombre del campo y, a continuación, haga clic en **Insertar a la izquierda** o **Insertar a la derecha** para agregar el nuevo campo.
1. En la ficha **Nuevo campo**, busque un tipo de campo en el cuadro **Tipo de campo** o seleccione uno de los siguientes tipos de campo:

   En la ficha **Nuevo campo**, busque un tipo de campo en el cuadro **Tipo de campo** <!--using any related keyword--> o seleccione uno de los tipos de campo que se enumeran a continuación.


   * [Texto de línea única](#single-line-text)
   * [Párrafo](#paragraph)
   * [Selección múltiple](#multi-select)
   * [Selección única](#single-select)
   * [Fecha](#date)
   * [Número](#number)
   * [Porcentaje](#percentage)
   * [Divisa](#currency)
   * [Casilla de verificación](#checkbox)
   * [Fórmula](#formula)
   * [Personas](#people)
   * [Creado por](#created-by)
   * [Fecha de creación](#created-date)
   * [Última modificación realizada por](#last-modified-by)
   * [Fecha de la última modificación](#last-modified-date)

   >[!IMPORTANT]
   >
   >    No se puede cambiar el tipo de campo después de guardarlo.

   <!--Add this to the IMPORTANT above and make it a NOTE - should do directly to Prod:
    * You can use any keyword that might be related to any of the field type names. For example, a search for "Budget" will display the Number or Currency field type.-->

1. Siga agregando cada campo, tal como se describe en las secciones siguientes.

### Texto de línea única {#single-line-text}

Los campos de texto de una sola línea capturan información alfanumérica limitada. Por ejemplo, puede capturar la información del propietario, la parte interesada, el equipo o la unidad organizativa en un campo de texto de una sola línea. El contenido de un campo de texto de una sola línea puede tener hasta 1000 caracteres. <!-- used to be 250 but just tested with 1000 and it allowed this as a maximum. -->

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Texto de una sola línea**.

   ![](assets/single-line-text-field-type.png)

1. Agregue la siguiente información en la ficha **Nuevo campo**:
   * **Nombre**: El nombre del tipo de campo, tal como aparecerá en una tabla o en la página Detalles del registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre el encabezado de columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>
1. Haga clic en **Crear**.

   El nuevo campo de una sola línea se agrega como una columna al tipo de registro y sus valores se pueden asociar con registros.


### Párrafo {#paragraph}

Los campos de párrafo capturan información alfanumérica adicional sobre un registro, similar al campo Descripción.

>[!TIP]
>
>* Puede tener un máximo de 20 campos de párrafo para un tipo de registro.
>
>* El contenido de un campo de párrafo puede tener hasta 10 000 caracteres.
>* Puede utilizar el formato de texto enriquecido para mejorar el contenido de los campos de párrafo cuando se muestran en la vista de tabla o en la página Detalles de un registro. Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).
>


1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Párrafo**.

   ![](assets/paragraph-field-type.png)


1. Agregue la siguiente información en la ficha **Nuevo campo**:
   * **Nombre**: El nombre del tipo de campo, tal como aparecerá en una tabla o en la página Detalles del registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>
1. Haga clic en **Crear**.

   El nuevo campo de párrafo se agrega como una columna al tipo de registro y sus valores se pueden asociar con registros.


### Selección múltiple {#multi-select}

Puede utilizar un campo de selección múltiple para capturar información adicional en cualquier formato seleccionando más de una opción en un menú desplegable.

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Selección múltiple**.

   ![](assets/multi-select-field-type.png)


1. Agregue la siguiente información en la ficha **Nuevo campo**:
   * **Nombre**: El nombre del tipo de campo, tal como aparecerá en una tabla o en la página Detalles del registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>
   * **Opciones**: las opciones que los usuarios pueden seleccionar al actualizar este campo. Puede utilizar números y letras para el nombre de cada opción.
1. Haga clic en **Agregar opción** para agregar más opciones. No hay límite en la cantidad de opciones que se pueden agregar a un campo de selección múltiple.
1. (Opcional) Arrastre y suelte manualmente cada opción en el orden deseado o seleccione la
   **Ordenar opciones A-Z** opción si desea que las opciones se enumeran automáticamente en orden alfabético. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. (Opcional) Para quitar una opción, haga clic en el icono **x** a su derecha.
1. Haga clic en la muestra de color a la izquierda de la opción para expandir el selector de color y personalizar el color de cada opción.
1. Haga clic en **Crear**.

   El nuevo campo de selección múltiple se agrega como una columna al tipo de registro y sus valores se pueden asociar con registros.

### Selección única {#single-select}

Los campos de selección única capturan información adicional en cualquier formato seleccionando una opción en un menú desplegable.

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Selección única**.

   ![](assets/single-select-field-type.png)


1. Agregue la siguiente información en la ficha **Nuevo campo**:
   * **Nombre**: El nombre del tipo de campo, tal como aparecerá en una tabla o en la página Detalles del registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>
   * **Opciones**: opciones disponibles para seleccionar en el menú desplegable después de guardar el campo. Puede tener números y letras para el nombre de cada opción.

1. Haga clic en **Agregar opción** para agregar más opciones. No hay límite en la cantidad de opciones que se pueden agregar a un campo de selección única.
1. (Opcional) Arrastre y suelte manualmente cada opción en el orden deseado o seleccione la opción **Ordenar opciones A-Z** si desea que las opciones se muestren automáticamente en orden alfabético. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. (Opcional) Para quitar una opción, haga clic en el icono **x** a su derecha.
1. Haga clic en la muestra de color a la izquierda de la opción para expandir el selector de color y personalizar el color de cada opción.
1. Haga clic en **Crear**.

   El nuevo campo de selección única se agrega como una columna al tipo de registro y sus valores se pueden asociar con registros.

### Fecha {#date}

Puede utilizar un campo de fecha para capturar información adicional en formato de fecha y hora.

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Fecha**.

   ![](assets/date-field-type.png)


1. Agregue la siguiente información en la ficha **Nuevo campo**:
   * **Nombre**: nombre del tipo de campo, tal como aparecerá en una tabla o en la página de registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>
   * **Formato de fecha**: El tipo de formato de fecha que desea mostrar en este campo. <!--update this casing - submitted bug for it-->

     Seleccione entre los siguientes formatos:
      * **Configuración regional**: Coincide con la configuración regional del explorador.
      * **Estándar**: 16/05/2023
      * **Long**: 16 de mayo de 2023
      * **Europeo**: 16/05/2023
      * **ISO**: 16-05-2023
      * **Incluir un campo de hora**: seleccione esta opción si desea incluir una marca de hora. De forma predeterminada, esta opción no está seleccionada. <!--update this setting name - submitted bug for it to be changed-->

     Seleccione entre las siguientes opciones:

      * **24hr**: Por ejemplo: 18:00
      * **12hr**: Por ejemplo: 6:00 PM

1. Haga clic en **Crear**.

   El nuevo campo de fecha se agrega como una columna al tipo de registro y sus valores se pueden asociar con registros.

### Número {#number}

Los tipos de campos de número capturan información en formato numérico.

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Número**.

   ![](assets/number-field-type.png)
1. Agregue la siguiente información en la ficha **Nuevo campo**:

   * **Nombre**: nombre del tipo de campo, tal como aparecerá en una tabla o en la página de registro.
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>
   * **Precisión**: El número de decimales que desea registrar para el campo. Se pueden mostrar hasta 6 decimales.
   * **Permitir números negativos**: seleccione esta opción si desea permitir números negativos en este campo. Esta opción está desactivada de forma predeterminada.

   >[!NOTE]
   >
   >    Si selecciona Permitir números negativos y los valores negativos se almacenan en los registros a los que está adjunto el campo, ya no podrá anular la selección de la configuración en el futuro.

1. Haga clic en **Crear**.

   El nuevo campo de número se agrega como una columna al tipo de registro y sus valores se pueden asociar con registros.

### Porcentaje {#percentage}

Los tipos de campo de porcentaje capturan información en un formato numérico seguido de un signo de porcentaje.

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Porcentaje**. <!--change screen shot for preview-->

   ![](assets/percentage-field-type.png)

1. Agregue la siguiente información en la ficha **Nuevo campo**:
   * **Nombre**: nombre del tipo de campo, tal como aparecerá en una tabla o en la página de registro.
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>
   * **Precisión**: El número de decimales que desea registrar para el campo. Se pueden mostrar hasta 6 decimales.
   * **Permitir números negativos**: seleccione esta opción si desea permitir valores de porcentaje negativos en este campo. Esta opción está desactivada de forma predeterminada.

     >[!NOTE]
     >
     >Si selecciona Permitir números negativos y los valores negativos se almacenan en los registros a los que está adjunto el campo, ya no podrá anular la selección de la configuración en el futuro.

   <div class="preview">

   * **Mostrar como**: en el menú desplegable, elija cómo desea que se muestren los valores de porcentaje en la vista de tabla. Seleccione entre las siguientes opciones:
      * **Número**: el valor porcentual se muestra como un número seguido del signo de porcentaje.
      * **Barra**: El valor porcentual se muestra como una barra junto al número de porcentaje. El color de relleno de la barra indica el valor porcentual. Esta es la selección predeterminada.
      * **Círculo**: el valor porcentual se muestra como el contorno de un círculo junto al número porcentual. El color de relleno del contorno del círculo indica el valor porcentual.

   >[!NOTE]
   >
   >* La selección que realice en el campo Mostrar como solo se aplica al valor porcentual visible en la vista de tabla. El valor porcentual del campo se muestra como un número seguido del signo de porcentaje en cualquier otra parte de Workfront Planning. Esto también se aplica al campo de tipo porcentual cuando se muestra como un campo de búsqueda en las vistas de tabla de otros registros.
   >* Puede cambiar la selección Mostrar como cuando edite el campo más adelante.
   </div>

1. Haga clic en **Crear**.

   El nuevo campo de porcentaje se agrega como una columna al tipo de registro y sus valores se pueden asociar con registros.

### Divisa {#currency}

Los tipos de campo Moneda capturan información en un formato de número precedido por un símbolo de moneda.

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Moneda**.

   ![](assets/currency-field-type.png)

1. Agregue la siguiente información en la ficha **Nuevo campo**:
   * **Nombre**: nombre del tipo de campo, tal como aparecerá en una tabla o en la página de registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>
   * **Moneda**: El tipo de moneda que desea mostrar en este campo. Esta es una lista de monedas según la Organización Internacional de Normalización (ISO).
   * **Precisión**: El número de decimales que desea registrar para el campo. Se pueden mostrar hasta 6 decimales.
   * **Permitir números negativos**: seleccione esta opción si desea permitir valores de moneda negativos en este campo. Esta opción está desactivada de forma predeterminada.

   >[!NOTE]
   >
   >    Si selecciona Permitir números negativos y los valores negativos se almacenan en los registros a los que está adjunto el campo, ya no podrá anular la selección de la configuración en el futuro.

1. Haga clic en **Crear**.

   El nuevo campo de moneda se agrega como una columna al tipo de registro y sus valores se pueden asociar con registros.

### Casilla de verificación

Puede utilizar el tipo de campo Casilla de verificación para agregar una sola opción de casilla de verificación a un registro. Puede utilizar este campo para indicar un atributo o estado específico para ese registro en particular. Por ejemplo, puede utilizarlo como indicador para rastrear la finalización, la aprobación o cualquier otro atributo binario de cada registro.

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Casilla de verificación**.

   ![](assets/checkbox-field-type.png)

1. Agregue la siguiente información en la ficha **Nuevo campo**:
   * **Nombre**: nombre del tipo de campo, tal como aparecerá en una tabla o en la página de registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>
1. Haga clic en **Crear**.

   El nuevo campo de casilla de verificación se agrega como una columna al tipo de registro y sus valores se pueden asociar con registros.

### Fórmula

Los campos de fórmula generan un nuevo valor utilizando valores existentes de otros campos en un tipo de registro y una función que indica cómo se deben calcular los valores existentes.

Para obtener más información, vea [Información general sobre los campos de fórmula](/help/quicksilver/planning/fields/formula-fields.md).

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Fórmula**.

   ![](assets/new-formula-field-with-list-of-expressions.png)

1. Agregue la siguiente información en la ficha **Nuevo campo**:

   * **Nombre**: escriba un nombre para el nuevo campo.
   * **Descripción**: agregue información sobre el nuevo campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>
   * **Fórmula**: Empiece a escribir al menos un carácter para tener acceso a una expresión y selecciónela cuando se muestre en la lista.

1. Haga clic en la expresión seleccionada para mostrar la definición y ver su formato.

   ![](assets/description-of-formula-expression.png)

   Para obtener más información acerca de las expresiones admitidas, vea [Información general sobre los campos de fórmula](/help/quicksilver/planning/fields/formula-fields.md).

1. Agregue nombres de campo tal y como se muestran en Workfront Planning para hacer referencia a ellos en una fórmula.

   >[!NOTE]
   >
   >* No se pueden agregar campos de tipo Selección múltiple en una fórmula.
   >
   >* Puede hacer referencia a un campo que esté hasta 4 campos (y objetos) fuera del tipo de registro actual. Por ejemplo, si está creando un campo de fórmula para un tipo de registro Actividad (1) y la actividad está conectada al tipo de registro Campaña (2) que está conectado a un proyecto Workfront (3), puede hacer referencia al campo Presupuesto del proyecto (4) en la fórmula que está creando para el tipo de registro Actividad.
   >
   >![](assets/formula-example-project-budget-four-fields-removed.png)
   >

1. En el campo **Formato**, seleccione entre las siguientes opciones para identificar el formato del resultado mostrado en el campo de tipo de fórmula:

   * **Texto**: el resultado del campo de fórmula se muestra como texto sin formato.
   * **Número**: el resultado del campo de fórmula se muestra como un número.
   * **Porcentaje**: el resultado del campo de fórmula se muestra como un número seguido de un símbolo de porcentaje.
   * **Moneda**: el resultado del campo de fórmula se muestra como un número precedido o seguido por un símbolo de moneda.
   * **Etiquetas**: el resultado del campo de fórmula se muestra como una etiqueta con el nombre del objeto.

     >[!TIP]
     >
     >Recomendamos las etiquetas para los campos que muestran matrices. En este caso, cada miembro de la matriz se muestra como una etiqueta independiente.

     ![](assets/formula-field-formats-list-with-tag-selected-highlighted.png)

   * **Fecha**: el resultado del campo de fórmula se muestra como una fecha.

     Se muestra una vista previa del aspecto que tendrá el resultado en el campo **Formato**.

     >[!WARNING]
     >
     >Si el resultado de la fórmula no coincide con el formato seleccionado, el campo mostrará un mensaje de error donde se muestra.

1. Haga clic en **Crear**.

   El nuevo campo de fórmula se agrega como una columna al tipo de registro y sus valores se pueden asociar a registros.

### Personas

Puede usar el tipo de campo Personas para agregar un usuario <!--, job role, or team--> a un registro. Este es un campo de escritura anticipada y solamente puede agregar usuarios <!--, roles, or teams--> que ya existen en su instancia de Workfront.

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Personas**.

   ![](assets/people-field-type.png)

1. Agregue la siguiente información en la ficha **Nuevo campo**:
   * **Nombre**: nombre del tipo de campo, tal como aparecerá en una tabla o en la página de registro.
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>
   * **Permitir varios valores**: seleccione esta opción si desea permitir que los usuarios agreguen más de un usuario en este campo. Esta opción está desactivada de forma predeterminada.

   >[!NOTE]
   >
   >    Si selecciona Permitir varios valores y se almacenan varios usuarios en los registros a los que está adjunto el campo, ya no podrá anular la selección de la configuración en el futuro al editar este campo.

1. Haga clic en **Crear**.

   El nuevo campo de tipo Personas se agrega como una columna al tipo de registro y sus valores se pueden asociar con registros.

### Creado por

Puede utilizar el tipo de campo Creado por para agregar el usuario que creó el registro a un registro. Este es un campo de solo lectura y se rellena automáticamente con el nombre del usuario que había iniciado sesión cuando se creó el registro.

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Creado por**.

   ![](assets/created-by-field-type.png)

1. Agregue la siguiente información en la ficha **Nuevo campo**:

   * **Nombre**: nombre del tipo de campo, tal como aparecerá en una tabla o en la página de registro. <!--this might change and they might prepopulate it with "Created by"-->
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>

1. Haga clic en **Crear**.

   El nuevo campo Creado por tipo se agrega como una columna al tipo de registro y sus valores se rellenan previamente con el nombre del usuario que creó cada registro.


### Fecha de creación

Puede utilizar el tipo de campo Fecha de creación para agregar la fecha en la que se creó el registro a un registro. Este es un campo de solo lectura y se rellena automáticamente con la fecha (y opcionalmente con la hora) en que se creó el registro.

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Fecha de creación**.

   ![](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Agregue la siguiente información en la ficha **Nuevo campo**:

   * **Nombre**: nombre del tipo de campo, tal como aparecerá en una tabla o en la página de registro. <!--this might change and they might prepopulate it with "Created date"-->
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>
   * **Formato de fecha**: seleccione uno de los siguientes formatos:

      * **Configuración regional**: Coincide con la configuración regional del explorador.
      * **Estándar**: 16/05/2023
      * **Long**: 16 de mayo de 2023
      * **Europeo**: 16/05/2023
      * **ISO**: 16-05-2023
   * **Incluir un campo de hora**: seleccione esta opción si desea incluir una marca de hora. De forma predeterminada, esta opción no está seleccionada. <!--submitted a UI text change for this - check the UI-->

     Seleccione entre las siguientes opciones:

      * **24hr**: Por ejemplo: 18:00
      * **12hr**: Por ejemplo: 6:00 PM

1. Haga clic en **Crear**.

   El nuevo campo de tipo Fecha de creación se agrega como una columna al tipo de registro y sus valores se rellenan previamente con la fecha (o fecha y hora) en que se creó el registro.


### Última modificación realizada por

Puede utilizar el tipo de campo Última modificación realizada por para agregar a un registro al usuario que modificó el registro por última vez. Este es un campo de solo lectura y se rellena automáticamente con el nombre del usuario que inició sesión cuando se actualizó el registro por última vez.

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Última modificación realizada por**.

   ![](assets/last-modified-by-field-type.png)

1. Agregue la siguiente información en la ficha **Nuevo campo**:

   * **Nombre**: nombre del tipo de campo, tal como aparecerá en una tabla o en la página de registro. <!--this might change and they might prepopulate it with "Created by"-->
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>

1. Haga clic en **Crear**.

   El nuevo campo Última modificación por tipo se agrega como una columna al tipo de registro y sus valores se rellenan previamente con el nombre del usuario que modificó cada registro por última vez.


### Fecha de la última modificación

Puede utilizar el tipo de campo Fecha de la última modificación para agregar la fecha en la que se modificó por última vez un registro a un registro. Este es un campo de solo lectura y se rellena automáticamente con la fecha (y opcionalmente con la hora) en que se modificó el registro por última vez.

1. Comience a crear un campo como se describe en la sección [Crear campos desde cero](#create-fields-from-scratch) de este artículo y, a continuación, seleccione el tipo de campo **Fecha de creación**.

   ![](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Agregue la siguiente información en la ficha **Nuevo campo**:

   * **Nombre**: nombre del tipo de campo, tal como aparecerá en una tabla o en la página de registro. <!--this might change and they might prepopulate it with "Created date"-->
   * **Descripción**: Información adicional sobre el campo. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo en una tabla o <span class="preview"> cuando hace clic en el icono de información situado junto al nombre del campo en la página de detalles del registro.</span>
   * **Formato de fecha**: seleccione uno de los siguientes formatos:

      * **Configuración regional**: Coincide con la configuración regional del explorador.
      * **Estándar**: 16/05/2023
      * **Long**: 16 de mayo de 2023
      * **Europeo**: 16/05/2023
      * **ISO**: 16-05-2023

   * **Incluir un campo de hora**: seleccione esta opción si desea incluir una marca de hora. De forma predeterminada, esta opción no está seleccionada. <!--submitted a UI text change for this - check the UI-->

     Seleccione entre las siguientes opciones:

      * **24hr**: Por ejemplo: 18:00
      * **12hr**: Por ejemplo: 6:00 PM

1. Haga clic en **Crear**.

   El nuevo campo de tipo Fecha de la última modificación se agrega como una columna al tipo de registro y sus valores se rellenan previamente con la fecha (o fecha y hora) en que se modificó por última vez el registro.

## Creación de campos conectando tipos de registro

Puede crear campos de registro vinculados al agregar una nueva conexión entre dos tipos de registro o un tipo de registro y un tipo de objeto de otras aplicaciones.

Para obtener información acerca de cómo conectar tipos de registros de Workfront Planning, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

<!--## Create fields by importing record types using an Excel or CSV file

For more information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).-->

## Creación de campos creando un tipo de registro

Al crear un tipo de registro, también se crean de forma predeterminada varios campos asociados al nuevo tipo de registro. Para obtener más información, vea [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

## Creación de campos creando un espacio de trabajo a partir de una plantilla

Adobe Workfront Planning crea campos para los tipos de registro al crear un espacio de trabajo a partir de una plantilla.

Para obtener más información, consulte [Crear espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).
