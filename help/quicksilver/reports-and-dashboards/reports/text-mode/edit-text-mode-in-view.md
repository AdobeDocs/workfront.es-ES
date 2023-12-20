---
product-area: reporting
navigation-topic: text-mode-reporting
title: Edición de una vista mediante el modo de texto
description: "NOTA: añada una sección en este artículo: /Contenido/Informes y paneles/Informes/Informes Elements/create-customize-views.html *** Además, redacte esta área en el artículo Información general sobre el modo de texto"
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1639'
ht-degree: 1%

---

# Edición de una vista mediante el modo de texto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

Puede editar una vista de una lista o informe utilizando el modo de texto para acceder a campos que no están disponibles en la interfaz estándar y crear vistas más complejas.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Editar el acceso a los informes, paneles y calendarios para editar los elementos de un informe</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe para editar vistas en un informe</p> <p>Administrar permisos a una vista para editarla</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Requisitos previos

Antes de empezar a utilizar el modo de texto en un informe o una lista, asegúrese siempre de estar familiarizado con la sintaxis del modo de texto de Workfront.

Para obtener más información, consulte:

* [Introducción al modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Resumen de sintaxis de modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Ejemplos de vistas, filtros y agrupaciones personalizadas: índice de artículos](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Edición del modo de texto en una vista

La edición de una vista mediante el modo de texto es idéntica para los informes y las listas. El acceso a la vista desde un informe o desde una lista es distinto.

>[!TIP]
>
>Le recomendamos que genere la mayor parte posible de la vista en el modo estándar y luego la convierta al modo de texto para editarla.

Para obtener información sobre la creación de vistas, consulte [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Para obtener información sobre cómo crear un informe, consulte [Creación de un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Realice una de las siguientes acciones:

   1. Para acceder a la vista desde un informe, vaya al informe y haga clic en **Acciones de informe** > **Editar** > **Columnas (vista)** pestaña.
   1. Para acceder a la vista desde una lista, vaya a la lista y, desde **Ver** , pase el ratón sobre la vista que desee modificar y haga clic en el icono **Editar** icono ![](assets/edit-icon.png).

      Se abre el generador de vistas.

1. Seleccione una columna en la vista.

   O

   Seleccione el **Columnas (vista)** de report builder y, a continuación, seleccione una columna.

   >[!TIP]
   >
   >Para editar una vista con el modo de texto, debe editar las columnas de una en una.

1. Clic **Cambiar a modo de texto** en la esquina superior derecha del generador.

   >[!NOTE]
   >
   >Cuando edita una columna en modo de texto, Workfront agrega la variable `textmode=true` línea de código a la columna. Esto indica que la columna se modifica en modo de texto.

   ![](assets/switch-to-text-mode-in-view-nwe-highlighted-350x447.png)

   En la tabla siguiente se describen las líneas clave en una vista de modo de texto:

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
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>Es el nombre del objeto o del campo tal como aparece en la base de datos. Para obtener más información sobre cómo aparecen los objetos y campos en la base de datos, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>.</p> <p>Existen los siguientes escenarios:</p> 
       <ol> 
        <li value="1"> <p> Si el nombre del campo que se muestra es una frase en lugar de un nombre único, se debe utilizar la sintaxis en minúscula para el campo <code>valuefield</code>. Por ejemplo, para la fecha planificada de inicio de una tarea, el código es: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Si desea mostrar un campo personalizado, la variable <code>valuefield</code> value es el nombre real del campo, tal como lo ve en la interfaz. Por ejemplo, para un campo personalizado llamado "Más información", el código es:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Si desea mostrar objetos relacionados con otros objetos de una vista utilizando <code>valuefield</code> línea de código los nombres de objeto y atributos están separados por dos puntos. </p> <p>Por ejemplo, una columna en una vista de tareas que mostraría el nombre del Propietario del Portfolio tiene el siguiente valor para la línea de campo de valor:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>Esto indica que desde el objeto del informe (tarea) puede acceder al siguiente objeto relacionado (proyecto); desde allí, puede acceder al siguiente objeto relacionado desde proyecto (portafolio), luego al propietario del portafolio (propietario) y por último a su nombre (nombre). </p> </li> 
       </ol> <p>Para obtener información acerca de cómo se conectan los objetos entre sí, vea la sección <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependencia y jerarquía de objetos</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Explicación de los objetos en Adobe Workfront</a>.</p> <p>Nota: Si elige un campo en modo de texto que no es válido en la interfaz estándar, no puede volver a la interfaz estándar dentro de la columna.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>Esta línea representa el formato utilizado para mostrar el <code>valuefield</code>. El <code>valueformat</code> identifica si un objeto o campo se muestra como texto, número, porcentaje o fecha.</p> <p>Se recomienda utilizar <code>HTML</code> para su <code>valueformat</code>, especialmente al utilizar <code>valueexpression</code>, para garantizar la visualización más precisa de su información. </p> <p>Para obtener más información sobre los valores adicionales de esta línea, consulte <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Uso del formato condicional en el modo Texto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>Puede agregar esta línea para reemplazar <code>valuefield</code>, si desea mostrar un campo calculado en la columna.</p> <p>Debe adjuntar el <code>valuefield</code> de los objetos entre llaves cada vez que los utilice en una <code>valueexpression</code>.</p> <p>Existen los siguientes escenarios: </p> 
       <ol> 
        <li value="1"> <p>Si desea mostrar un campo en una columna en mayúsculas, debe utilizar:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>El <code>valuefield</code> del objeto se escribe tal como aparece en el Explorador de API. </p> </li> 
        <li value="2">Si desea agregar varias <code>valuefields</code> al unirlos, debe separarlos por un punto.</li> 
        <li value="3"> <p>Por ejemplo, si desea mostrar el nombre de la persona asignada principal de una tarea utilizando <code>valueexpression</code>, utilizaría:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>Si desea utilizar un campo personalizado en una <code>valueexpression</code> línea debe preceder el nombre del campo por <code>DE:</code> para indicar que es un campo personalizado. El nombre del campo se escribe tal y como aparece en la interfaz. </p> <p>Importante: Cuando se utiliza un campo personalizado que se coloca en una sección de formulario personalizada que tiene permisos restringidos para algunos usuarios, el cálculo de la expresión de valor está en blanco cuando esos usuarios ven este cálculo en un informe. Para obtener información sobre el ajuste de permisos en secciones de formularios personalizados, consulte <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a></span>.</p> <p>Por ejemplo, si tiene un campo personalizado etiquetado como "Nombre del desarrollador" y desea mostrar este campo en mayúsculas en una columna, puede utilizar lo siguiente <code>valueexpression</code> para indicar esto:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>Al hacer referencia a un campo personalizado de tipo Escritura anticipada, utilice la siguiente expresión para hacer referencia al nombre del objeto seleccionado en un campo denominado "Nombre del desarrollador":</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>descriptionkey= / description=</strong> </p> </td> 
      <td> <p>Esta línea define el texto de la información del objeto al pasar el ratón por encima del nombre de la columna. En este caso, se utiliza una clave para traducir el valor del nombre en el texto de la descripción. Si desea modificar la descripción, cambie esta línea para que diga: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>name= / name=</strong> </td> 
      <td> <p>Esta línea define la etiqueta de columna. En este caso, se utiliza el valor abreviado basado en la clave.</p> <p>Si desea modificar el nombre de la columna, puede cambiar este valor a: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> permite introducir cualquier texto para el nombre de la columna, mientras que<code>namekey</code> requiere que escriba una clave que se utilice para traducir el nombre de una columna.</p> <p>Para cambiar el nombre de la columna, también puede añadir la variable <code>displayname </code>línea, si no hay ninguna.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>Puede agregar la línea siguiente para cambiar el nombre de una columna, lo que suspende el <code>namekey/name</code> valor:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
     <tr> 
      <td><strong>querysort=</strong> </td> 
      <td>Esta línea define cómo se ordenan los resultados cuando se hace clic en el encabezado de la columna. Si no está presente, la columna no se puede ordenar después de ejecutar el informe.</td> 
     </tr> 
     <tr> 
      <td><strong>width=</strong> </td> 
      <td> <p>Esta línea representa el número de píxeles que se utilizan para la columna. Si la línea se omite o se establece en 0 (cero), la columna no aparecerá en la vista.</p> <p>Cuando modifique este campo manualmente en el modo de texto, también debe añadir la variable <code>usewidths=true</code> a su columna.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>usewidths=true</strong> </td> 
      <td> <p>Debe utilizar esta línea además de la <code>width=</code> línea al personalizar el ancho de una columna. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>makeFieldEditable=</strong> </td> 
      <td> <p>Esta línea define si el valor mostrado en una columna se puede editar en línea o no. Si esta línea es igual a <strong>true</strong>, el valor de la columna se puede editar en línea. Si esta línea es igual a <code>false</code>, el valor de la columna no se puede editar en línea.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valuefield=</strong> </td> 
      <td> <p>Inserte esta línea únicamente cuando desee que el valor mostrado en una columna se vincule al objeto asociado a ella. El vínculo abre la página de detalles del objeto. Este valor debe coincidir con el de <code>valuefield=</code> línea. Al insertar esto, también debe agregar el <code>link.valueformat=</code> línea. </p> <p> Por ejemplo, puede insertar <code>link.valuefield=priority</code> en una vista de problema, y la Prioridad del problema se muestra como un vínculo. Al hacer clic en este vínculo, se abre la página Problema.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueformat=</strong> </td> 
      <td> <p>Inserte esta línea solo cuando haya insertado el <code>link.valuefield</code> para añadir un vínculo al valor de una columna. El vínculo abre la página de detalles del objeto. Este valor debe coincidir con el de <code>valueformat=</code> línea e indica el formato utilizado para mostrar el <code>valuefield</code>. </p> <p>Importante: Cuando vea el modo de texto en una columna integrada que también incluye un vínculo, verá varias líneas que hacen referencia al vínculo. Es posible que algunas de esas líneas ya no sean compatibles o que sean innecesarias cuando crea su propia columna personalizada en modo de texto y le agrega las instrucciones de vínculo. Las líneas obligatorias al agregar un valor vinculado son las siguientes<code> link.valuefield</code> y <code>link.valueformat</code>. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>aggregator.function=</strong> </td> 
      <td> <p>Hace referencia a cómo se resumen los valores de cada columna. Hay varias líneas que comienzan con <code>aggregator.</code> y todas hacen referencia al agregador que resume los resultados de la columna. </p> <p>Como regla general, la variable <code>aggregator.</code> las líneas coinciden con las del objeto column. </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>">
        <span class="autonumber"><span><b>Ejemplo: </b></span></span> 
        <p>La columna Horas planificadas de un informe de tareas resumido por Suma puede tener el siguiente aspecto: </p> 
        <div>
         <pre>textmode=true</pre>
         <pre>valuefield=workRequired</pre>
         <pre>valueformat=compound</pre>
         <pre>aggregator.function=SUM</pre>
         <pre>aggregator.valuefield=workRequired</pre>
         <pre>aggregator.displayformat=minutesAsHoursString</pre>
         <pre>aggregator.valueformat=compound</pre>
         <pre>namekey=workRequired</pre>
         <pre>shortview=false</pre> 
        </div> 
       </div> 
       <div>
        El <code>aggregator. </code>las líneas pueden contener un <code>valuefield </code>o una <code>valueexpression</code>
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Aplicar** si desea guardar los cambios y continuar editando la vista.
1. Clic **Guardar + Cerrar** para guardar el informe.

   O

   Clic **Guardar vista** para guardar la vista en una lista.
