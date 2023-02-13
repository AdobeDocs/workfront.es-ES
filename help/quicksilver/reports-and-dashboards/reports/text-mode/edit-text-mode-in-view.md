---
product-area: reporting
navigation-topic: text-mode-reporting
title: Edición de una vista mediante el modo de texto
description: '''NOTA: agregue una sección en este artículo: /Contenido/Informes y tableros/Informes/Informes/Informes Elements/create-customize-views.html *** También, borrador esta área en el artículo de información general del modo de texto)"'
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '1636'
ht-degree: 1%

---

# Edición de una vista mediante el modo de texto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

Puede editar una vista de una lista o informe mediante el modo de texto para acceder a los campos que no están disponibles en la interfaz estándar y crear vistas más complejas.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a filtros, vistas y grupos</p> <p>Editar acceso a informes, tableros y calendarios para editar elementos de informes en un informe</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe para editar vistas en un informe</p> <p>Administrar permisos en una vista para editarla</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de empezar a utilizar el modo de texto en un informe o lista, asegúrese siempre de que está familiarizado con la sintaxis del modo de texto de Workfront.

Para obtener más información, consulte:

* [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Información general sobre la sintaxis del modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Ejemplos de vista, filtro y agrupamiento personalizados](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Edición del modo de texto en una vista

La edición de una vista mediante el modo de texto es idéntica para los informes y las listas. El acceso a la vista desde un informe o desde una lista es distinto.

>[!TIP]
>
>Se recomienda generar la mayor cantidad posible de vista en modo estándar y luego convertirla al modo de texto para editarla.

Para obtener información sobre la creación de vistas, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Para obtener información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Realice una de las siguientes acciones:

   1. Para acceder a la vista desde un informe, vaya al informe y haga clic en **Acciones de informe** > **Editar** > **Columnas (Vista)** pestaña .
   1. Para acceder a la vista desde una lista, vaya a la lista y desde la **Ver** menú desplegable, pase el ratón sobre la vista que desee modificar y haga clic en la **Editar** icono ![](assets/edit-icon.png).

      Se abre el generador de vistas.

1. Seleccione una columna en la vista.

   O

   Seleccione el **Columnas (Vista)** del Creador de informes y, a continuación, seleccione una columna.

   >[!TIP]
   >
   >Para editar una vista mediante el modo de texto, debe editar una columna a la vez.

1. Haga clic en **Cambiar al modo de texto** en la esquina superior derecha del generador.

   >[!NOTE]
   >
   >Cuando edita una columna en modo de texto, Workfront agrega la variable `textmode=true` línea de código a la columna . Esto indica que la columna se modifica en el modo de texto.

   ![](assets/switch-to-text-mode-in-view-nwe-highlighted-350x447.png)

   En la tabla siguiente se describen las líneas clave de una vista de modo de texto:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Línea de muestra</th> 
      <th>Descripción</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>campo de valor</strong>=</p> </td> 
      <td> <p>Es el nombre del objeto o del campo tal como aparece en la base de datos. Para obtener más información sobre cómo aparecen los objetos y los campos en la base de datos, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>.</p> <p>Existen los siguientes escenarios:</p> 
       <ol> 
        <li value="1"> <p> Si el nombre del campo que muestra es una frase en lugar de un solo nombre, debe utilizar la sintaxis de mayúsculas y minúsculas para la variable <code>valuefield</code>. Por ejemplo, para la Fecha de inicio planeada de una tarea, el código es: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Si desea mostrar un campo personalizado, la variable <code>valuefield</code> es el nombre real del campo, tal como se ve en la interfaz. Por ejemplo, para un campo personalizado llamado "Más información", el código es:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Si desea mostrar objetos relacionados con otros objetos de una vista mediante el <code>valuefield</code> línea de código en la que los nombres y atributos de los objetos se separan con dos puntos. </p> <p>Por ejemplo, una columna de una vista de tarea que mostraría el nombre del propietario del Portfolio tiene el siguiente valor para la línea del campo de valor:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>Esto indica que, desde el objeto del informe (tarea), puede acceder al siguiente objeto relacionado (proyecto), desde allí puede acceder al siguiente objeto relacionado desde el proyecto (portafolio), luego el propietario del portafolio (propietario) y después su nombre (nombre). </p> </li> 
       </ol> <p>Para obtener información sobre cómo se conectan los objetos entre sí, consulte la sección <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependencia y jerarquía de objetos</a> en <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Explicación de los objetos en Adobe Workfront</a>.</p> <p>Nota: Si elige un campo en modo de texto que no es válido en la interfaz estándar, no puede volver a la interfaz estándar dentro de la columna .</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>Esta línea representa el formato utilizado para mostrar la variable <code>valuefield</code>. La variable <code>valueformat</code> identifica si un objeto o campo se muestra como texto, número, porcentaje o fecha.</p> <p>Se recomienda usar <code>HTML</code> para su <code>valueformat</code>, especialmente cuando se usa <code>valueexpression</code>, para garantizar la visualización más precisa de la información. </p> <p>Para obtener información sobre valores adicionales para esta línea, consulte <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Utilizar el formato condicional en modo de texto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>Puede añadir esta línea para reemplazar <code>valuefield</code>, si desea mostrar un campo calculado en la columna .</p> <p>Debe incluir el <code>valuefield</code> de los objetos entre llaves cada vez que los utilice en un <code>valueexpression</code>.</p> <p>Existen los siguientes escenarios: </p> 
       <ol> 
        <li value="1"> <p>Si desea mostrar un campo en una columna en mayúsculas, debe utilizar:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>La variable <code>valuefield</code> del objeto se escribe tal como aparece en el Explorador de API. </p> </li> 
        <li value="2">Si desea agregar varias <code>valuefields</code> al unirlos, hay que separarlos por punto.</li> 
        <li value="3"> <p>Por ejemplo, si desea mostrar el nombre del usuario asignado principal de una tarea mediante <code>valueexpression</code>, utilizaría:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>Si desea utilizar un campo personalizado en un <code>valueexpression</code> línea debe preceder al nombre del campo por <code>DE:</code> para indicar que es un campo personalizado. El nombre del campo se escribe tal como aparece en la interfaz. </p> <p>Importante: Cuando se utiliza un campo personalizado que se coloca en una sección de formulario personalizado que tiene permisos restringidos para algunos usuarios, el cálculo de la expresión de valor se deja en blanco cuando esos usuarios ven este cálculo en un informe. Para obtener información sobre el ajuste de permisos en secciones de formularios personalizados, consulte <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a></span>.</p> <p>Por ejemplo, si tiene un campo personalizado etiquetado como "Nombre del desarrollador" y desea mostrar este campo en mayúsculas en una columna, puede utilizar el siguiente <code>valueexpression</code> para indicar esto:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>Al hacer referencia a un campo personalizado de tipo Typeforward , utilice la siguiente expresión para hacer referencia al nombre del objeto seleccionado en un campo denominado "Nombre del desarrollador":</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>descriptionkey= / description=</strong> </p> </td> 
      <td> <p>Esta línea define el texto de la información del objeto mientras pasa el ratón sobre el nombre de la columna. En este caso, se utiliza una clave para traducir el valor del nombre en el texto de la descripción. Si desea modificar la descripción, cambie esta línea para que diga: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Esta línea define la etiqueta de columna. En este caso, utiliza el valor abreviado basado en la clave.</p> <p>Si desea modificar el nombre de la columna, puede cambiar este valor a: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> permite introducir cualquier texto para el nombre de la columna, mientras que<code>namekey</code> requiere que introduzca una clave que se utilice para traducir el nombre de una columna.</p> <p>Para cambiar el nombre de la columna, también puede agregar la variable <code>displayname </code>línea, si una no está presente.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>Puede agregar la siguiente línea para cambiar el nombre de una columna, que suspende el <code>namekey/name</code> valor:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
     <tr> 
      <td><strong>querysort=</strong> </td> 
      <td>Esta línea define cómo se ordenan los resultados cuando se hace clic en el encabezado de columna. Si no está presente, la columna no se puede ordenar después de ejecutar el informe.</td> 
     </tr> 
     <tr> 
      <td><strong>width=</strong> </td> 
      <td> <p>Esta línea representa el número de píxeles que se utilizan para la columna. Si se omite la línea o se establece en 0 (cero), la columna no aparece en la vista.</p> <p>Cuando modifique este campo manualmente en modo de texto, también debe agregar la variable <code>usewidths=true</code> a su columna.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>usewidths=true</strong> </td> 
      <td> <p>Debe utilizar esta línea además del <code>width=</code> al personalizar el ancho de una columna. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>makeFieldEditable=</strong> </td> 
      <td> <p>Esta línea define si el valor mostrado en una columna es editable en línea o no. Si esta línea es igual a <strong>true</strong>, el valor de la columna es editable en línea. Si esta línea es igual a <code>false</code>, el valor de la columna no se puede editar en línea.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueField=</strong> </td> 
      <td> <p>Inserte esta línea únicamente cuando desee que el valor mostrado en una columna vincule al objeto asociado a ella. El vínculo abre la página de detalles del objeto. Este valor debe coincidir con la variable <code>valuefield=</code> línea. Al insertar esto, también debe agregar la variable <code>link.valueformat=</code> línea. </p> <p> Por ejemplo, puede insertar <code>link.valuefield=priority</code> en una vista de problemas, y la prioridad del problema se muestra como vínculo. Al hacer clic en este vínculo, se abre la página Problema .</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.value.format=</strong> </td> 
      <td> <p>Inserte esta línea solo cuando haya insertado el <code>link.valuefield</code> para añadir un vínculo al valor en una columna. El vínculo abre la página de detalles del objeto. Este valor debe coincidir con la variable <code>valueformat=</code> línea e indica el formato utilizado para mostrar la variable <code>valuefield</code>. </p> <p>Importante: Al ver el modo de texto en una columna integrada que también incluye un vínculo, se observa una serie de líneas que hacen referencia al vínculo. Es posible que algunas de estas líneas ya no sean compatibles o que no sean necesarias al crear su propia columna personalizada en modo de texto y añadir las instrucciones de vínculo a ella. Las líneas que son obligatorias al añadir un valor vinculado son<code> link.valuefield</code> y <code>link.valueformat</code>. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>agregator.function=</strong> </td> 
      <td> <p>Esto hace referencia a cómo se resumen los valores de cada columna. Hay varias líneas que empiezan por <code>aggregator.</code> y todos hacen referencia al agregador que resume los resultados de la columna. </p> <p>Como regla general, la variable <code>aggregator.</code> las líneas coinciden con las del objeto column . </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>">
        <span class="autonumber"><span><b>Ejemplo: </b></span></span> 
        <p>La columna Horario planificado de un informe de tareas resumido por Suma puede tener un aspecto similar al siguiente: </p> 
        <div>
         <pre>textmode=true</pre>
         <pre>valueField=workRequired</pre>
         <pre>valueformat=compuesto</pre>
         <pre>aggregator.function=SUM</pre>
         <pre>aggregator.valuefield=workRequired</pre>
         <pre>aggregator.displayformat=minutesAsHoursString</pre>
         <pre>aggregator.valueformat=compound</pre>
         <pre>namekey=workRequired</pre>
         <pre>short-view=false</pre> 
        </div> 
       </div> 
       <div>
        La variable <code>aggregator. </code>las líneas pueden contener <code>valuefield </code>o <code>valueexpression</code>
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Aplicar** si desea guardar los cambios y seguir editando la vista.
1. Haga clic en **Guardar + Cerrar** para guardar el informe.

   O

   Haga clic en **Guardar vista** para guardar la vista en una lista.
