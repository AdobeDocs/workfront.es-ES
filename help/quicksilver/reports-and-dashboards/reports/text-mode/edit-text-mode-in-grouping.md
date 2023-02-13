---
product-area: reporting
navigation-topic: text-mode-reporting
title: Editar el modo de texto en una agrupación
description: '''NOTA: hacer que todos los artículos FVG sean iguales para editarlos en modo de texto)"'
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1559'
ht-degree: 1%

---

# Editar el modo de texto en una agrupación

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

Puede editar una agrupación en una lista o informe mediante el modo de texto para acceder a los campos que no están disponibles en la interfaz estándar y crear agrupaciones más complejas.

>[!TIP]
>
>Se recomienda crear la mayor cantidad posible de la agrupación en modo estándar y luego convertirla al modo de texto para editarla.

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
   <td> <p>Editar acceso a filtros, vistas y grupos</p> <p>Editar acceso a informes, tableros y calendarios para editar agrupaciones en un informe</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe para editar agrupaciones en un informe</p> <p>Administrar permisos en una agrupación para editarla</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
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

## Editar el modo de texto en una agrupación

La edición de una agrupación mediante el modo de texto es idéntica para los informes y las listas. El acceso a la agrupación desde un informe o desde una lista es distinto.

>[!NOTE]
>
>Los grupos son un elemento de informes obligatorio para la creación de gráficos en los informes. Las agrupaciones en modo texto no son compatibles con los gráficos. Para obtener información sobre cómo agregar gráficos a informes, consulte [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

Para obtener más información sobre la creación de agrupaciones, consulte [Crear agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Para obtener información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Realice una de las siguientes acciones:

   1. Para acceder a la agrupación desde un informe, vaya al informe y haga clic en **Acciones de informe** > **Editar** > **Agrupaciones** pestaña .
   1. Para acceder a la agrupación desde una lista, vaya a la lista y desde la **Agrupación** menú desplegable, pase el ratón sobre la agrupación que desea modificar y haga clic en la **Editar** icono ![](assets/edit-icon.png).

      Se abre el generador de agrupación.

1. Haga clic en **Agregar agrupación** para añadir las agrupaciones, haga clic en **Cambiar al modo de texto** en la esquina superior derecha del generador.

   >[!TIP]
   Puede añadir hasta 3 agrupaciones en la interfaz estándar. Puede agregar una cuarta agrupación solo mediante el modo de texto y no puede tener más de 4 niveles de agrupación en Workfront.

1. Empiece a escribir el nombre de un campo por el que desee agrupar.

   Seleccione el nombre del campo cuando lo vea en la lista.

1. Haga clic en **Cambiar al modo de texto** en la esquina superior derecha del generador.

   A continuación, la agrupación se muestra en modo de texto.

   Cuando edita una agrupación en modo de texto, Workfront agrega la variable

   ```
   textmode=true
   ```

   línea de código a la agrupación. Esto indica que la agrupación se modifica en modo de texto.

   **Ejemplo:** Para agrupar una lista de tareas por el Nombre del proyecto y, a continuación, por el nombre del Destinatario principal, la agrupación debe tener el aspecto siguiente, en modo de texto.

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   Las líneas en negrita son obligatorias.

   <!--
   <div class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <span class="autonumber"><span><b>Example: </b></span></span>
   <p>To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:</p>
   <p><code>textmode=true</code> </p>
   <p><code>group.0.linkedname=project</code> </p>
   <p><code>group.0.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.0.valuefield=project:name</code> </p>
   <p><code>group.0.namekeyargkey.0=project</code> </p>
   <p><code>group.0.namekeyargkey.1=name</code> </p>
   <p><code style="font-weight: bold;">group.0.valueformat=string</code> </p>
   <p><code>group.1.linkedname=assignedTo</code> </p>
   <p><code>group.1.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.1.valuefield=assignedTo:name</code> </p>
   <p><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   <p><code>group.1.namekeyargkey.1=nam</code>e</p>
   <p><code style="font-weight: bold;">group.1.valueformat=string</code> </p> <note type="important">
   The lines in bold are mandatory.
   </note>
   </div>
   -->

   Cada campo de la agrupación tiene varias líneas de código que hacen referencia a ese campo.

   La siguiente tabla describe las líneas clave de una agrupación en modo de texto.

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   Las líneas clave de una agrupación en modo de texto son similares a las líneas necesarias para generar vistas en modo de texto.

   <!--
   <note type="tip">  
   <p>The key lines in a text mode grouping are similar to the lines required to build text-mode views.</p>
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th><strong>Línea de muestra</strong> </th> 
      <th><strong>Descripción</strong> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><strong>grupo.&lt;number&gt;.</strong> </td> 
      <td> <p>Cada línea de código va precedida por este texto. Las líneas de código que hacen referencia al mismo campo seleccionado en la agrupación se numeran con el mismo número, de la siguiente manera:</p> 
       <ul> 
        <li>La primera agrupación del informe tiene un número de grupo de 0. Todas las líneas que hacen referencia a la primera agrupación comienzan por <code>group.0</code>.</li> 
        <li>La segunda agrupación del informe tiene un número de grupo de 1. Todas las líneas que hacen referencia a la segunda agrupación comienzan por <em><code>group.1</code></em>.</li> 
        <li>La tercera agrupación del informe tiene un número de grupo de 2. Todas las líneas que hacen referencia a la tercera agrupación comienzan por <em><code>group.2</code></em>.</li> 
        <li>Solo en el modo de texto, puede añadir un número de grupo de 3 para una cuarta agrupación. Todas las líneas que hacen referencia a la cuarta agrupación comienzan por <em><code>group.3</code></em>.</li> 
       </ul> <p>Nota: El generador no admite 4 agrupaciones. Solo son compatibles con el modo de texto. Workfront no admite más de 4 niveles de agrupaciones.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>campo de valor</strong>=</p> </td> 
      <td> <p>Es el nombre del objeto o del campo tal como aparece en la base de datos. Para obtener más información sobre cómo aparecen los objetos y los campos en la base de datos, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>.</p> <p>Existen los siguientes escenarios:</p> 
       <ol> 
        <li value="1"> <p> Si el nombre del campo que muestra es una frase en lugar de un solo nombre, debe utilizar la sintaxis de mayúsculas y minúsculas para la variable <code>valuefield</code>. Por ejemplo, para la Fecha de inicio planeada de una tarea, el código es:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Si desea mostrar un campo personalizado, la variable <code>valuefield</code> es el nombre real del campo, tal como se ve en la interfaz. Por ejemplo, para un campo personalizado llamado "Más información", el código es:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Si desea agrupar por objetos relacionados con otros objetos mediante la variable <code>valuefield</code> línea de código en la que los nombres y atributos de los objetos se separan con dos puntos.</p> <p>Por ejemplo, una agrupación por nombre de Portfolio para una lista de tareas tiene el siguiente valor para la línea de campo de valor:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>Esto indica que desde el objeto del informe (tarea), puede acceder al siguiente objeto relacionado (proyecto); desde allí, puede acceder al siguiente objeto relacionado desde proyecto (portafolio); a continuación, el nombre del portafolio (nombre).</p> </li> 
       </ol> <p>Para obtener información sobre cómo se conectan los objetos entre sí, consulte la sección <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependencia y jerarquía de objetos</a> en <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Explicación de los objetos en Adobe Workfront</a>.</p> <p>Nota: Si elige un campo en modo de texto que no es válido en la interfaz estándar y cambia a la interfaz estándar, se elimina la agrupación.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>Esta línea representa el formato utilizado para mostrar la variable <code>valuefield</code>. La variable <code>valueformat</code> identifica si un objeto o campo se muestra como texto, número, porcentaje o fecha.</p> <p>Se recomienda usar <code>HTML</code> para su <code>valueformat</code>, especialmente cuando se usa <code>valueexpression</code>, para garantizar la visualización más precisa de la información.</p> <p>Para obtener información sobre valores adicionales para esta línea, consulte <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Utilizar el formato condicional en modo de texto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>Puede añadir esta línea para reemplazar <code>valuefield</code>, si desea agrupar la lista por un cálculo entre varios campos.</p> <p>Debe incluir el <code>valuefield</code> de los objetos entre llaves cada vez que los utilice en un <code>valueexpression</code>.</p> <p>Existen los siguientes escenarios:</p> 
       <ol> 
        <li value="1"> <p>Si desea mostrar el nombre de una agrupación en mayúsculas, debe utilizar:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>La variable <code>valuefield</code> del objeto se escribe tal como aparece en el Explorador de API.</p> </li> 
        <li value="2">Si desea agregar varias <code>valuefields</code> uniéndolos en una <code>valueexpression </code>línea, debe separarlos por un punto.<p>Por ejemplo, si desea mostrar el nombre del portafolio en mayúsculas en una lista de tareas, debe utilizar el siguiente código en la <code>valueexpression</code> línea:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>Si desea utilizar un campo personalizado en un <code>valueexpression</code> línea debe preceder al nombre del campo por <code>DE:</code> para indicar que es un campo personalizado. El nombre del campo se escribe tal como aparece en la interfaz.</p><p>Importante: <span>Cuando se utiliza un campo personalizado que se coloca en una sección de formulario personalizado que tiene permisos restringidos para algunos usuarios, el cálculo de la variable <code>valueexpression </code>está en blanco cuando esos usuarios ven este cálculo en un informe. Para obtener información sobre el ajuste de permisos en secciones de formularios personalizados, consulte</span> <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a></span>.</p><p>Por ejemplo, si tiene un campo personalizado etiquetado como "Nombre del desarrollador" y desea agrupar por este campo y mostrarlo en mayúsculas, puede utilizar lo siguiente <code>valueexpression</code> para indicar esto:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>Al hacer referencia a un campo personalizado de tipo Typeforward , utilice la siguiente expresión para hacer referencia al nombre del objeto seleccionado en un campo denominado "Nombre del desarrollador":</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Esta línea define la etiqueta de agrupación. En este caso, utiliza el valor abreviado basado en la clave.</p> <p>Si desea modificar el nombre de la agrupación, puede cambiar este valor a lo siguiente:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> permite introducir cualquier texto para el nombre de la agrupación, mientras que <code>namekey</code> requiere que introduzca una clave que se utilice para traducir el nombre de una agrupación.</p> <p>Para cambiar el nombre de la agrupación, también puede agregar la variable <code>displayname </code>línea, si una no está presente.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>Puede añadir la siguiente línea para cambiar el nombre de una columna, que sobrescribe la columna <code>namekey/name</code> valor:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>Se recomienda quitar todas las líneas que contengan <code>name </code>al cambiar el nombre de una agrupación.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Agregue una de las siguientes líneas de código a cualquier agrupación para indicar si los resultados de la agrupación deben mostrarse en una lista expandida o contraída. De forma predeterminada, las agrupaciones se muestran expandidas:


   ```
   group.0.iscollapsed=true
   ```

   si desea que la agrupación se muestre con los resultados contraídos

   ```
   group.0.iscollapsed=false
   ```

   si desea que la agrupación se muestre con los resultados expandidos

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   * Cuando ajusta las agrupaciones manualmente al ver una lista, Workfront recuerda su preferencia manual hasta que cierre la sesión. Cuando vuelve a iniciar sesión, la lista se muestra según esta configuración.
   * Los resultados de una agrupación siempre se muestran expandidos después de acceder a ellos desde un elemento de gráfico.


1. Haga clic en **Listo** si desea guardar los cambios y seguir editando la agrupación o el informe.
1. Haga clic en **Guardar agrupación** en una lista o **Guardar + Cerrar** para guardar el informe.
