---
product-area: reporting
navigation-topic: text-mode-reporting
title: Editar modo de texto en una agrupación
description: "NOTA: haga que todos los artículos de FVG sean iguales para su edición en modo de texto)"
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Editar modo de texto en una agrupación

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

Puede editar una agrupación en una lista o informe utilizando el modo de texto para acceder a campos que no están disponibles en la interfaz estándar y crear agrupaciones más complejas.

>[!TIP]
>
>Le recomendamos que genere la mayor cantidad posible de la agrupación en el modo estándar y luego la convierta al modo de texto para editarla.

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
   <td> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Editar el acceso a Informes, Tableros y Calendarios para editar agrupaciones en un informe</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe para editar agrupaciones en un informe</p> <p>Administración de permisos en una agrupación para editarla</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de empezar a utilizar el modo de texto en un informe o una lista, asegúrese siempre de estar familiarizado con la sintaxis del modo de texto de Workfront.

Para obtener más información, consulte:

* [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Descripción general de la sintaxis del modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Ejemplos de vistas, filtros y agrupaciones personalizadas: índice de artículos](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Editar modo de texto en una agrupación

La edición de una agrupación mediante el modo de texto es idéntica para informes y listas. El acceso a la agrupación desde un informe o desde una lista es distinto.

>[!NOTE]
>
>Las agrupaciones son un elemento de sistema de informes obligatorio para crear gráficos en los informes. Los gráficos no admiten agrupaciones en modo de texto. Para obtener información sobre cómo agregar gráficos a los informes, vea [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

Para obtener más información sobre cómo crear agrupaciones, consulte [Crear agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Para obtener información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Realice una de las siguientes acciones:

   1. Para acceder a la agrupación desde un informe, ve al informe y haz clic en **Acciones de informe** > **Editar** > pestaña **Agrupaciones**.
   1. Para acceder a la agrupación desde una lista, ve a la lista y, en el menú desplegable **Agrupación**, pasa el ratón sobre la agrupación que deseas modificar y haz clic en el icono **Editar** ![](assets/edit-icon.png).

      Se abrirá el generador de agrupaciones.

1. Haga clic en **Agregar agrupación** para agregar las agrupaciones y, a continuación, haga clic en **Cambiar al modo de texto** en la esquina superior derecha del generador.

   >[!TIP]
   >
   >Se pueden agregar hasta 3 agrupaciones en la interfaz estándar. Puede agregar una cuarta agrupación solo con el modo de texto y no puede tener más de 4 niveles de agrupación en Workfront.

1. Empiece a escribir el nombre del campo por el que desea agrupar.

   Seleccione el nombre del campo cuando lo vea en la lista.

1. Haga clic en **Cambiar al modo de texto** en la esquina superior derecha del generador.

   La agrupación se muestra en modo de texto.

   Cuando edita una agrupación en modo de texto, Workfront agrega la variable

   ```
   textmode=true
   ```

   línea de código a la agrupación. Esto indica que la agrupación se modifica en modo de texto.

   **Ejemplo:** Para agrupar una lista de tareas por el nombre del proyecto y, a continuación, por el nombre de la persona asignada principal, la agrupación debería tener el aspecto siguiente, en modo de texto.

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   >Las líneas en negrita son obligatorias.

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

   En la tabla siguiente se describen las líneas clave de una agrupación en modo de texto.

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   >
   >Las líneas clave de una agrupación de modo de texto son similares a las líneas necesarias para generar vistas de modo de texto.

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
      <td><strong>grupo.&lt;número&gt;.</strong> </td> 
      <td> <p>Cada línea de código va precedida de este texto. Las líneas de código que hacen referencia al mismo campo seleccionado en la agrupación se numeran con el mismo número, de la siguiente manera:</p> 
       <ul> 
        <li>La primera agrupación del informe tiene un número de grupo de 0. Todas las líneas que hacen referencia a la primera agrupación comienzan con <code>group.0</code>.</li> 
        <li>La segunda agrupación del informe tiene el número de grupo 1. Todas las líneas que hacen referencia a la segunda agrupación comienzan con <em><code>group.1</code></em>.</li> 
        <li>La tercera agrupación del informe tiene un número de grupo de 2. Todas las líneas que hacen referencia a la tercera agrupación comienzan con <em><code>group.2</code></em>.</li> 
        <li>Solo en el modo de texto puede agregar un número de grupo de 3, para una cuarta agrupación. Todas las líneas que hacen referencia a la cuarta agrupación comienzan con <em><code>group.3</code></em>.</li> 
       </ul> <p>Nota: No se admiten 4 agrupaciones en el generador. Solo se admiten cuando se utiliza el modo de texto. Workfront no admite más de 4 niveles de agrupaciones.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>Es el nombre del objeto o del campo tal como aparece en la base de datos. Para obtener más información sobre cómo aparecen los objetos y campos en la base de datos, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>.</p> <p>Existen los siguientes escenarios:</p> 
       <ol> 
        <li value="1"> <p> Si el nombre del campo que muestra es una frase en lugar de un nombre único, debe utilizar la sintaxis en minúscula para <code>valuefield</code>. Por ejemplo, para la fecha planificada de inicio de una tarea, el código es:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Si desea mostrar un campo personalizado, el valor <code>valuefield</code> es el nombre real del campo, tal como lo ve en la interfaz. Por ejemplo, para un campo personalizado llamado "Más información", el código es:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Si desea agrupar por objetos relacionados con otros objetos mediante la línea de código <code>valuefield</code>, los nombres y atributos de los objetos se separarán con dos puntos.</p> <p>Por ejemplo, una agrupación por nombre de Portfolio para una lista de tareas tiene el siguiente valor para la línea de campo de valor:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>Esto indica que desde el objeto del informe (tarea) puede acceder al siguiente objeto relacionado (proyecto); desde allí, puede acceder al siguiente objeto relacionado desde proyecto (portafolio); y después al nombre del portafolio (nombre).</p> </li> 
       </ol> <p>Para obtener información acerca de cómo se conectan los objetos entre sí, vea la sección <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependencia y jerarquía de objetos</a> en <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprender los objetos en Adobe Workfront</a>.</p> <p>Nota: Si elige un campo en modo de texto que no es válido en la interfaz estándar y cambia a la interfaz estándar, la agrupación se elimina.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>Esta línea representa el formato utilizado para mostrar <code>valuefield</code>. <code>valueformat</code> identifica si un objeto o campo se muestra como texto, número, porcentaje o fecha.</p> <p>Se recomienda usar <code>HTML</code> para su <code>valueformat</code>, especialmente cuando se usa <code>valueexpression</code>, a fin de garantizar la visualización más precisa de su información.</p> <p>Para obtener información acerca de los valores adicionales de esta línea, vea <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Usar formato condicional en el modo de texto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>Puede agregar esta línea para reemplazar <code>valuefield</code>, si desea agrupar la lista mediante un cálculo entre varios campos.</p> <p>Debe incluir el <code>valuefield</code> de los objetos entre llaves cada vez que lo utilice en un <code>valueexpression</code>.</p> <p>Existen los siguientes escenarios:</p> 
       <ol> 
        <li value="1"> <p>Si desea mostrar el nombre de una agrupación en mayúsculas, debe utilizar:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>El <code>valuefield</code> del objeto está escrito tal como aparece en el Explorador de API.</p> </li> 
        <li value="2">Si desea agregar varios(as) <code>valuefields</code> uniéndolos(as) en una línea de <code>valueexpression </code>, debe separarlos por un punto.<p>Por ejemplo, si desea mostrar el nombre del portafolio en mayúsculas en una lista de tareas, debe utilizar el siguiente código en la línea <code>valueexpression</code>:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>Si desea utilizar un campo personalizado en una línea de <code>valueexpression</code>, debe preceder el nombre del campo por <code>DE:</code> para indicar que se trata de un campo personalizado. El nombre del campo se escribe tal y como aparece en la interfaz.</p><p>Importante: <span>Cuando se usa un campo personalizado ubicado en una sección de formulario personalizado que tiene permisos restringidos para algunos usuarios, el cálculo de <code>valueexpression </code>está en blanco cuando dichos usuarios ven este cálculo en un informe. Para obtener información acerca de cómo ajustar permisos en secciones de formularios personalizados, vea </span> <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a></span>.</p><p>Por ejemplo, si tiene un campo personalizado etiquetado como "Nombre del desarrollador" y desea agrupar por este campo y mostrarlo en mayúsculas, puede utilizar el siguiente <code>valueexpression</code> para indicar esto:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>Al hacer referencia a un campo personalizado de tipo Escritura anticipada, utilice la siguiente expresión para hacer referencia al nombre del objeto seleccionado en un campo denominado "Nombre del desarrollador":</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Esta línea define la etiqueta de agrupación. En este caso, se utiliza el valor abreviado basado en la clave.</p> <p>Si desea modificar el nombre de la agrupación, puede cambiar este valor al siguiente:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> permite escribir cualquier texto para el nombre de agrupación, mientras que <code>namekey</code> requiere que escriba una clave que se utilice para traducir el nombre de una agrupación.</p> <p>Para cambiar el nombre de la agrupación, también puede agregar la línea <code>displayname </code>, si no hay ninguna.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>Puede agregar la línea siguiente para cambiar el nombre de una columna, que sobrescribe el valor <code>namekey/name</code>:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>Se recomienda quitar todas las líneas que contienen <code>name </code> al cambiar el nombre de una agrupación.</p> </td> 
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
   >   
   >* Cuando ajusta manualmente las agrupaciones al ver una lista, Workfront recuerda su preferencia manual hasta que cierre la sesión. Cuando vuelva a iniciar sesión, la lista se mostrará según esta configuración.
   >* Los resultados de una agrupación siempre se muestran expandidos después de acceder a ellos desde un elemento de gráfico.

1. Haga clic en **Listo** si desea guardar los cambios y seguir editando la agrupación o el informe.
1. Haga clic en **Guardar agrupación** en una lista o en **Guardar y cerrar** para guardar el informe.
