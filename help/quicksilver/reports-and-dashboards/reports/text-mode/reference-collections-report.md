---
product-area: reporting
navigation-topic: text-mode-reporting
title: Colecciones de referencia en un informe
description: Colecciones de referencia en un informe
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: 8b6324302a70319f387d1e09d1eb92fbdabf7e32
workflow-type: tm+mt
source-wordcount: '2609'
ht-degree: 0%

---

# Colecciones de referencia en un informe

La creación de un informe en Adobe Workfront permite mostrar un conjunto de objetos, sus respectivos campos u objetos vinculados en una lista, una cuadrícula o un formato de gráfico.

Para obtener más información sobre cómo crear un informe en Workfront, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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
   <td> <p>Editar acceso a filtros, vistas y grupos</p> <p>Editar acceso a informes, tableros y calendarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Administrar permisos para una vista, filtro o agrupación </p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Explicación de las colecciones

Una colección es una lista de objetos vinculados a otro objeto.

Tiene las dos relaciones siguientes entre objetos en Workfront:

* **Una relación uno a uno**: Un objeto solo se puede vincular a otro objeto a la vez.\
   Por ejemplo, un proyecto solo se puede vincular a un portafolio a la vez.

* **Una relación &quot;uno a varios&quot;**: Un objeto se puede vincular a otros objetos a la vez.\
   Por ejemplo, un proyecto puede tener varias tareas. En este caso, la lista de tareas forma una colección para el proyecto.

>[!IMPORTANT]
>
>Puede crear un informe que muestre la relación uno a uno entre los objetos mediante el Creador de informes estándar. Sin embargo, solo puede crear un informe que muestre la relación uno a varios entre objetos mediante la interfaz de modo de texto del creador de informes.

Para obtener más información sobre la creación de informes en el creador de informes estándar, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obtener más información sobre la creación de un informe mediante la interfaz de modo de texto, consulte:

* [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Descripción general de los usos comunes del modo Texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [Información general sobre la sintaxis del modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## Busque objetos de colección y sus campos en el Explorador de API {#find-collection-objects-and-their-fields-in-the-api-explorer}

No se puede informar de todas las colecciones.

Para comprender qué objetos se pueden asociar a una colección de otros, debe utilizar el Explorador de API.\
Para obtener más información sobre la tabla API Explorer, consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).

Para saber sobre qué colecciones se pueden crear informes:

1. Vaya a la [Explorador de API](../../../wf-api/general/api-explorer.md).
1. Busque el objeto del informe.
1. Seleccione el **colecciones** pestaña .

   >[!NOTE]
   >
   >Solo los objetos enumerados en esta ficha pueden representarse como una colección en un informe para el objeto seleccionado.

1. Expanda el objeto de la colección haciendo clic en él.
1. Haga clic en el vínculo mostrado para ir al objeto de la colección.\
   Esto abre el **campos** para el objeto de la colección.

   >[!NOTE]
   >
   >Solo se puede hacer referencia a los campos enumerados en esta ficha en el informe de recopilación o a los campos asociados con los objetos enumerados en esta ficha.

## Colecciones de referencia en informes

Puede hacer referencia a objetos de una colección en los siguientes elementos de informes:

* Vistas
* Filtros
* Indicadores

No se puede hacer referencia a objetos de una colección en los siguientes elementos de informes:

* Agrupaciones
* Gráfico

Por ejemplo, puede hacer referencia a las colecciones de tareas o problemas de un informe de proyecto para mostrar información de tareas o problemas a nivel de proyecto.

* [Hacer referencia a una colección en la Vista de un informe](#reference-a-collection-in-the-view-of-a-report)
* [Hacer referencia a una colección en el Filtro de un informe](#reference-a-collection-in-the-filter-of-a-report)
* [Hacer referencia a una colección en la solicitud personalizada de un informe](#reference-a-collection-in-the-custom-prompt-of-a-report)

### Hacer referencia a una colección en la Vista de un informe {#reference-a-collection-in-the-view-of-a-report}

Puede hacer referencia a una colección de objetos en la vista de un informe, para mostrar atributos de objetos asociados al objeto del informe.

Por ejemplo, puede mostrar información de tareas o problemas en un informe de proyecto creando una columna de recopilación para tareas o problemas en la vista del informe.

Puede mostrar información sobre las tareas o los problemas, como nombres, fechas, asignadores primarios, porcentaje completado, etc. en la vista de colección.

La vista muestra información de tareas o problemas en formato de lista, y cada línea de la lista representa información sobre una tarea o un problema. La lista de tareas o problemas y sus campos aparecen en la misma línea que el proyecto al que pertenecen las tareas o los problemas.\
![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png)

* [Agregar una columna de colección en una vista de informe](#add-a-collection-column-in-a-report-view)
* [Explicación de las líneas de una vista de colección en el modo de texto](#understand-the-lines-of-a-collection-view-in-text-mode)
* [Limitaciones de una vista de colección](#limitations-of-a-collection-view)

### Agregar una columna de colección en una vista de informe {#add-a-collection-column-in-a-report-view}

Para agregar una columna de colección en una vista de informe:

1. Haga clic en el **Principal** menú ![](assets/main-menu-icon.png)y haga clic en **Informes**.
1. Haga clic en **Nuevo informe**.
1. Seleccione el objeto del informe.
1. Alejarse del informe y usar la variable [Explorador de API](../../../wf-api/general/api-explorer.md), determine qué colecciones están disponibles para el objeto seleccionado para el informe.

   Para obtener más información sobre la selección del objeto de la colección, consulte la sección [Busque objetos de colección y sus campos en el Explorador de API](#find-collection-objects-and-their-fields-in-the-api-explorer) en este artículo.\
   Anote cuál es el nombre del objeto para la colección.

1. Al usar la variable [Explorador de API](../../../wf-api/general/api-explorer.md), vaya a la lista de campos del objeto que desea mostrar en la colección.

   Para obtener más información sobre cómo encontrar los campos del objeto de la colección, consulte la sección [Busque objetos de colección y sus campos en el Explorador de API](#find-collection-objects-and-their-fields-in-the-api-explorer) en este artículo.

   Anote cuál es el nombre del campo que desea mostrar en la colección.

1. Vuelva al informe y, en la sección **Columnas (Vista)** , haga clic en **Agregar columna**.
1. Haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el cuadro de diálogo y haga clic en **Haga clic para editar texto**.
1. Seleccione todo el texto de la **Modo de texto** y elimínelo y pegue el siguiente código si hace referencia a un campo del objeto de colección:

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. Reemplazar **Nombre de columna** con el nombre de su columna en la `displayname` línea.
1. Reemplazar **nombre del objeto de colección** con el nombre del objeto de colección en la `listmethod` como aparece en la [Explorador de API](../../../wf-api/general/api-explorer.md).

1. Reemplazar **campo de objeto de colección** con el nombre del campo del objeto de colección en la `valuefield` como aparece en la [Explorador de API](../../../wf-api/general/api-explorer.md).

   Puede reemplazar **campo de valor** con **valueexpression**, si desea crear una expresión personalizada en la vista.

   Para obtener más información sobre las expresiones personalizadas calculadas, consulte [Expresiones de datos calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Por ejemplo, si desea mostrar una lista de las tareas en un informe de proyecto. Esta colección utiliza un `valuefield` para hacer referencia a los nombres de las tareas.

   Realice una de las siguientes acciones:

   * Utilice el siguiente código para crear la columna:

      ```
      valueformat=HTML
      textmode=true
      type=iterate
      listdelimiter=<p>
      displayname=Project Tasks Names
      listmethod=nested(tasks).lists
      valuefield=name
      ```

   * Utilice el siguiente código para mostrar una lista de problemas en el informe:

      ```
      displayname=Project Issues Names
      listdelimiter=<p>
      listmethod=nested(issues).lists
      textmode=true
      type=iterate
      valuefield=name
      valueformat=HTML
      ```

      Tenga en cuenta que en una colección debe usar **problemas** para el **listmethod** línea, en lugar de **opTasks** que es el nombre de la base de datos para Problemas. Para obtener información sobre cuándo usar **problema** y cuándo usar **opTask** al hacer referencia a problemas, consulte [Utilice &quot;opTask&quot; y &quot;issue&quot; al hacer referencia a problemas](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * Si desea mostrar una lista de las tareas en un informe de proyecto junto con su usuario asignado principal, utilizaría un **valueexpression** línea para hacer referencia a los nombres de las tareas adyacentes a los nombres de sus principales asignadores en lugar de **campo de valor**.

      Utilice el siguiente código para crear la columna:

      ```
      valueformat=HTML
      textmode=true
      type=iterate
      listdelimiter=<p>
      displayname=Tasks Names - Primary Assignee
      listmethod=nested(tasks).lists
      valueexpression=CONCAT({name},' - ',{assignedTo}.{name})
      ```

1. La siguiente columna se muestra en el informe de proyecto, donde se enumeran todas las tareas de cada proyecto junto con sus principales destinatarios asignados:

   ![](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png)

1. Haga clic en **Guardar**.
1. (Opcional) Continúe editando el informe.

   O

   Haga clic en **Guardar + Cerrar** para guardar el informe.

#### Explicación de las líneas de una vista de colección en el modo de texto

Las líneas de una vista en modo de texto para una colección se describen en la siguiente tabla:

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
   <td><code>valueformat=HTML</code> </td> 
   <td> <p>Puede utilizar varios valores para esta línea, pero le recomendamos que <code style="font-weight: normal;">valueformat</code> para una lista de colección debe <strong>HTML.</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>Esta línea indica que la columna se ha configurado con el modo de texto. Si quita esta línea, Workfront la agrega de nuevo de forma predeterminada.</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>La variable <code>type</code> de una lista siempre <code>iterate</code>, al crear una vista.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>Este es el delimitador que se utiliza para separar los valores de la lista.<br>Se recomienda usar <code>&lt;p&gt;</code> que añade un salto de línea entre los valores.</p> <p>También puede utilizar lo siguiente:</p> <p><code>&amp;zwj;</code> (unión de ancho cero). Los valores de la colección no tienen separación entre ellos.<br><strong>,</strong> =separador de coma. Los valores de la colección se separan con una coma y no hay espacio.<br><strong>/</strong> = separador de barras. Los valores de la colección se separan con una barra diagonal.<br><strong>-</strong> = separador de guión. Los valores de la colección se separan con una raya.<br>Si deja esta línea vacía, se añade una coma seguida de un espacio entre los valores de la colección de forma predeterminada.</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>Nombre de columna</em> </td> 
   <td> <p>Reemplazar <strong>Nombre de columna</strong> con el nombre real de la nueva columna.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> Esta línea define la colección a la que hace referencia.</p> <p>Reemplazar <strong>nombre del objeto de colección</strong> con el nombre del objeto al que se hace referencia en la colección, tal como aparece en la <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>. Este valor suele ser la forma plural del nombre del objeto de colección.</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>Esta línea define a qué campo hace referencia desde el objeto de colección.</p> <p>Reemplazar <strong>campo de objeto de colección</strong> con el nombre del campo del objeto al que se hace referencia en la colección, tal como aparece en la <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>.</p> <p>Puede reemplazar esta línea por:</p> <p><strong>valueexpression</strong>=campo/campos del objeto de colección calculada</p> <p>Uso <strong>valueexpression</strong>, puede mostrar una expresión personalizada calculada en la columna .</p> <p>Para obtener más información sobre cómo dar formato <strong>valueexpression</strong> líneas, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Información general sobre la sintaxis del modo de texto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Limitaciones de una vista de colección {#limitations-of-a-collection-view}

Tenga en cuenta las siguientes limitaciones al crear una vista de colección:

* No se puede controlar el orden en que se muestran los datos de recopilación.
* No se puede aplicar formato condicional a una vista de colección.
* No se puede hacer que un objeto de una colección sea un vínculo en el que se puede hacer clic.
* No se puede crear una vista de colección de otra colección.\
   Por ejemplo, no se pueden mostrar todos los asignadores en cada tarea en un informe de proyecto. Solo puede mostrar el usuario asignado principal en cada tarea en una vista de proyecto.

### Hacer referencia a una colección en el Filtro de un informe {#reference-a-collection-in-the-filter-of-a-report}

Puede hacer referencia a una colección de objetos en el filtro de un informe, para filtrar por los atributos de los objetos asociados con el objeto del informe.

Por ejemplo, puede filtrar por información de tareas o problemas en un informe de proyecto mediante una referencia a los atributos de tareas o problemas del proyecto en la instrucción filter.

Para agregar una referencia a una colección en un filtro de informe:

1. Haga clic en el **Principal** menú ![](assets/main-menu-icon.png)y haga clic en **Informes**.
1. Haga clic en **Nuevo informe**.
1. Seleccione el objeto del informe.
1. Alejarse del informe y usar la variable [Explorador de API](../../../wf-api/general/api-explorer.md), determine qué colecciones están disponibles para el objeto seleccionado para el informe.

   Para obtener más información sobre la selección del objeto de la colección, consulte la sección [Busque objetos de colección y sus campos en el Explorador de API](#find-collection-objects-and-their-fields-in-the-api-explorer) en este artículo.

   Anote cuál es el nombre del objeto para la colección.

1. Al usar la variable [Explorador de API](../../../wf-api/general/api-explorer.md), vaya a la lista de campos del objeto que desea mostrar en la colección.

   Para obtener más información sobre cómo encontrar los campos del objeto de la colección, consulte la sección [Busque objetos de colección y sus campos en el Explorador de API](#find-collection-objects-and-their-fields-in-the-api-explorer) en este artículo.

   Anote el campo que desea mostrar en la colección.

1. Vuelva al informe y, en la sección **Filtros** , haga clic en **Cambiar al modo de texto**.

1. En el **Definir reglas de filtro para el informe** pegue el siguiente código:

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. Reemplazar **nombre del objeto de colección** con el nombre del objeto de colección tal como aparece en la [Explorador de API](../../../wf-api/general/api-explorer.md). Este valor suele ser la forma plural del nombre del objeto de colección.

1. Reemplazar **campo de objeto de colección** con el nombre del campo del objeto de colección en, como aparece en la [Explorador de API](../../../wf-api/general/api-explorer.md).

1. Reemplazar **valor del objeto de colección** con el valor del objeto de colección tal como aparece en Workfront.
1. Reemplazar **valor del modificador** con un modificador válido.

   Para obtener una lista de modificadores, consulte [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
   Por ejemplo, para crear un informe de proyecto que muestre solamente proyectos con tareas que tengan &quot;Marketing&quot; en su nombre, use el siguiente código:

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   Este informe solo muestra proyectos que tienen al menos una tarea con la palabra &quot;marketing&quot; en su nombre.

   ![](assets/marketing-only-tasks-in-project-report-nwe-350x309.png)

1. Para filtrar por el nombre de un problema, utilice el siguiente código:

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >Tenga en cuenta que debe usar `issues` para el nombre del objeto de colección, en lugar de `optask` así es como aparecen los problemas en el Explorador de API.

1. Haga clic en **Listo**.
1. (Opcional) Continúe editando el informe.

   O

   Haga clic en **Guardar + Cerrar** para guardar el informe.

### Hacer referencia a una colección en la solicitud personalizada de un informe {#reference-a-collection-in-the-custom-prompt-of-a-report}

Puede hacer referencia a una colección de objetos en la solicitud personalizada de un informe, para filtrar los resultados del informe por los atributos de los objetos asociados al objeto del informe.

Por ejemplo, puede solicitar información de tareas en un informe de proyecto utilizando una referencia a los atributos de tareas del proyecto en la solicitud personalizada del informe.

>[!NOTE]
>
>No se puede hacer referencia a las colecciones en una solicitud estándar.

Un mensaje personalizado es un filtro personalizado en el que las instrucciones se unen mediante símbolos ampersand. Se recomienda crear la instrucción en un filtro, primero, y después unir las líneas de las instrucciones con ampersands.

Para obtener más información sobre la creación de una instrucción de filtro con una referencia de colección, consulte la sección [Hacer referencia a una colección en el Filtro de un informe](#reference-a-collection-in-the-filter-of-a-report) en este artículo.

Para añadir una referencia a una colección en el mensaje personalizado de un informe:

1. Haga clic en el **Principal** menú ![](assets/main-menu-icon.png)y haga clic en **Informes**.
1. Haga clic en **Nuevo informe**.
1. Seleccione el objeto del informe.
1. Genere un filtro con una referencia de colección como se describe en la sección [Hacer referencia a una colección en el Filtro de un informe](#reference-a-collection-in-the-filter-of-a-report) en este artículo.
1. Haga clic en **Configuración de informes**.
1. Haga clic en **Mensajes del informe**.
1. Haga clic en **Agregar mensaje**.
1. Haga clic en **Mensaje personalizado**.
1. Especifique el nombre del mensaje en la variable **Field****name** campo .

1. Especifique un **Etiqueta de elemento desplegable**.
1. Especifique lo siguiente en la **Condición** campo:

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. (Opcional) Especifique si esta opción se muestra de forma predeterminada en el mensaje.
1. Reemplazar **nombre del objeto de colección** con el nombre del objeto de colección tal como aparece en la [Explorador de API](../../../wf-api/general/api-explorer.md). Este valor suele ser la forma plural del nombre del objeto de colección.
1. Reemplazar **campo de objeto de colección** con el nombre del campo del objeto de colección, tal como aparece en el [Explorador de API](../../../wf-api/general/api-explorer.md).
1. Reemplazar **valor del objeto de colección** con el valor del objeto de colección tal como aparece en Workfront.

   Por ejemplo, si está filtrando proyectos en los que el nombre de la tarea contenga &quot;Marketing&quot;, reemplace **valor del objeto de colección** con **marketing**.

1. Reemplazar **valor del modificador** con un modificador válido.

   Para obtener una lista de modificadores, consulte  [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **Ejemplo:** Por ejemplo, para crear un informe de proyecto con una solicitud personalizada en la que quiera mostrar solo los proyectos que tengan al menos una tarea asignada a un usuario específico, utilice el siguiente código:

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   Esto genera un informe donde todos los proyectos listados tienen al menos una tarea asignada al usuario cuyo GUID es 57cf1b7a000077c9f02f66cb09c8f86c.

   >[!NOTE]
   >
   >No se puede hacer referencia al nombre del usuario asignado principal (campo &quot;Asignado a&quot;) de una tarea, según el [Explorador de API](../../../wf-api/general/api-explorer.md). Solo puede hacer referencia al ID del usuario asignado principal.

   Por ejemplo, para filtrar para cualquier proyecto en el que se hayan asignado problemas de proyecto a un usuario específico, utilice el siguiente código para el mensaje personalizado:

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   Esto genera un informe donde todos los proyectos listados tienen al menos un problema asignado al usuario cuyo GUID es 57cf1b7a000077c9f02f66cb09c8f86c.

   >[!NOTE]
   Tenga en cuenta que debe usar **problemas** para el nombre del objeto de colección. El Explorador de API no ofrece un nombre de objeto de colección para problemas en este momento.

1. Haga clic en **Listo**.
1. (Opcional) Continúe editando el informe.

   O

   Haga clic en **Guardar + Cerrar** para guardar el informe.
