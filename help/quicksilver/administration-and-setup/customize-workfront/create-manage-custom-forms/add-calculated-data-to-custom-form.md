---
title: Agregar datos calculados a un formulario personalizado con el generador de formularios heredado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: En un formulario personalizado, puede crear un campo personalizado calculado que genere cálculos. Para ello, cree una instrucción que utilice expresiones de datos y los nombres de campos existentes, que pueden ser campos personalizados, campos de datos personalizados calculados y campos Workfront integrados. Esta instrucción calcula los datos especificados y muestra el resultado en el nuevo campo personalizado calculado.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 9174c4ef-3beb-4d47-9c5c-363f52105a2c
source-git-commit: 02b025f228b6e2abc58dbc30f88c055c7850b803
workflow-type: tm+mt
source-wordcount: '2895'
ht-degree: 0%

---

# Agregar datos calculados a un formulario personalizado con el generador de formularios heredado

<!--Audited: 01/2024-->

{{form-designer-default}}

En un formulario personalizado, puede agregar un campo personalizado calculado que utilice datos existentes para generar datos nuevos cuando el formulario personalizado se adjunta a un objeto.

Para ello, cree una instrucción que utilice expresiones de datos y los nombres de campos existentes, que pueden ser campos personalizados, campos de datos personalizados calculados y campos Adobe Workfront integrados.

Esta instrucción calcula los datos especificados y muestra el resultado en el nuevo campo personalizado calculado.

Un campo personalizado calculado puede contener:

* Una sencilla referencia a un único campo integrado.

  >[!INFO]
  >
  > **Ejemplo:** Para calcular los ingresos generados por proyectos y tareas, puede crear un campo personalizado calculado que contenga el campo integrado Ingresos reales. Cuando alguien adjunta el formulario personalizado a un proyecto o tarea, los ingresos del proyecto o tarea se muestran en el campo.

* Expresión que hace referencia a uno o varios campos. Pueden ser campos personalizados, otros campos personalizados calculados y campos integrados.

  >[!INFO]
  >
  >**Ejemplo:** Para calcular el beneficio generado por proyectos y tareas, puede crear un campo personalizado calculado denominado Beneficio que contenga una expresión matemática que reste costos de los ingresos.
  >
  >Para ello, se puede utilizar la expresión matemática SUB (subtract) con los campos integrados de Workfront Coste real e Ingresos reales.
  >
  >En los pasos siguientes, puede ver cómo se puede llevar a cabo este ejemplo.

Para obtener información sobre la creación de formularios personalizados para su organización y el tipo de campos que puede asociar a ellos, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td><p>Actual: plan</p>
   O
   <p>Nuevo: estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> </p> </td> 
  </tr>  
 </tbody> 
</table>

*Para saber qué configuraciones de plan, tipo de licencia o nivel de acceso tiene, póngase en contacto con su administrador de Workfront. Para obtener más información sobre los requisitos de acceso, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Agregar un campo calculado a un formulario personalizado {#add-a-calculated-field-to-a-custom-form}

Puede utilizar tanto los campos integrados de Workfront como los campos personalizados que ya ha creado en la expresión de un campo personalizado calculado.

>[!IMPORTANT]
>
>Antes de crear un campo personalizado calculado, identifique los campos existentes que desee incluir para estar seguro de que los datos necesarios para el cálculo están presentes en Workfront.

1. Comience a crear o editar un formulario personalizado, tal como se describe en [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. En el **Añadir un campo** pestaña, haga clic en **Calculado**.

   En el área de visualización de la derecha, el campo muestra un valor de relleno de 12345. Este indicador le recuerda que el campo es un campo personalizado calculado mientras crea o edita el formulario personalizado. Cuando el formulario se adjunta a un objeto y los usuarios lo rellenan, ven el resultado del cálculo en el campo y no el valor 12345.

1. Especifique la siguiente información para el campo calculado:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td>Escriba una etiqueta para el campo. Esto es lo que ven los usuarios cuando utilizan el formulario personalizado. El campo <b>Nombre</b>, que se rellena automáticamente y coincide con Label, Workfront hace referencia a él en los informes. Este campo es obligatorio.</td> 
     </tr>

   <tr> 
   <td role="rowheader">Nombre</td> 
   <td>De forma predeterminada, el Nombre de un campo es el mismo que la Etiqueta. Sin embargo, puede modificar el Nombre de un campo para que sea diferente a la Etiqueta de un campo. El campo <b>Nombre</b> Workfront hace referencia a en los informes. Este campo es obligatorio.</td> 
   </tr>

   <tr> 
     <td role="rowheader" id="instructions">Instrucciones</td> 
      <td> <p>Agregue texto para proporcionar información adicional sobre el campo y la fórmula que contiene.</p>
      <p>También puede pegar aquí la fórmula utilizada en el cálculo del campo personalizado. En este caso, le recomendamos que actualice primero el Calculation del campo personalizado y, a continuación, copie la expresión final del campo Calculation y péguela en el campo Instructions. </p>


   Esto puede resultar útil de las siguientes maneras:
   <ul> 
      <li> <p>Como recordatorio de qué es la fórmula y cómo funciona. Esto resulta especialmente útil si planea utilizar este campo personalizado calculado en varios formularios.</p> </li> 
       <li> <p>Como información de objeto, los usuarios pueden ver cuando pasan el ratón por encima del campo. Aquí puede agregar el texto que desee que vea en la información del objeto.</p> </li> 
       </ul>
       <p>Si no desea que los usuarios vean la fórmula en la información del objeto, lo que podría resultar confuso para ellos, no la agregue al campo Instrucciones. En su lugar, utilice la configuración "Mostrar fórmula en instrucciones" para mostrar u ocultar la fórmula, tal como se describe más adelante en este artículo <a href="#build-the-calculation-for-your-calculated-custom-field">Cree el cálculo para el campo personalizado calculado</a> en este artículo.</p>

   <p>Para obtener información sobre el uso del mismo campo personalizado calculado en un formulario nuevo, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md#using-an-existing-calculated-custom-field-on-a-new-form" class="MCXref xref">Reutilizar un campo personalizado calculado existente en un formulario personalizado</a>.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td> 
      <td> <p>El formato en el que desea que se almacenen y muestren los resultados del campo.</p> <p>Si planea utilizar el campo en cálculos matemáticos, utilice siempre un <strong>Número</strong> o una <strong>Moneda</strong> formato. Al seleccionar Número o Moneda, el sistema trunca automáticamente los números que comienzan por 0.</p> 
      <p><b>IMPORTANTE</b>: <p>Antes de elegir un formato, tenga en cuenta el formato correcto para el nuevo campo. El campo de formato no se puede editar después de guardar el formulario personalizado. Y seleccionar el formato incorrecto podría afectar a futuros cálculos y valores acumulados en las agrupaciones de informes y listas.</p>
      <p><strong>NOTA:</strong> Los campos calculados con un formato de moneda no deben incluir comillas. (Por ejemplo, use 800,00 y no "800,00"). El uso de comillas puede tener consecuencias inesperadas debido a los matices del formato de idioma para los tipos de moneda.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continúe actualizando la información del campo personalizado como se describe en la sección [Cree el cálculo para el campo personalizado calculado](#build-the-calculation-for-your-calculated-custom-field) en este artículo.

## Cree el cálculo para el campo personalizado calculado {#build-the-calculation-for-your-calculated-custom-field}

1. Comience a crear el campo personalizado calculado, tal como se describe en la sección [Agregar un campo calculado a un formulario personalizado](#add-a-calculated-field-to-a-custom-form) en este artículo.

1. Clic **Maximizar** para abrir **Editor de cálculo** y genere su cálculo.

   >[!INFO]
   >
   >**Ejemplo:** Con el ejemplo de la introducción a este artículo, puede crear un campo personalizado calculado llamado Beneficio en un formulario personalizado para proyectos y tareas. Este campo puede contener un cálculo que muestre la diferencia entre los ingresos reales y el costo real:
   >
   >`SUB({actualRevenue},{actualCost})`
   >
   >En este ejemplo, `SUB` es la expresión y los campos a los que se hace referencia son `actualRevenue` y `actualCost`.

   Un cálculo suele comenzar con una expresión, seguida de paréntesis que contienen los campos a los que se desea hacer referencia cuando se adjunta el formulario personalizado a un objeto. Para obtener información sobre las expresiones disponibles, consulte [Resumen de las expresiones de datos calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Cada campo debe estar comprendido entre llaves, tal como se explica en la sección [Sintaxis requerida en los campos personalizados calculados](#syntax-required-in-calculated-custom-fields) en este artículo. Cuando empiece a escribir el nombre de un campo, el sistema realiza sugerencias y puede seleccionar una para insertarla en el cálculo.

   >[!NOTE]
   >
   >   No se puede hacer referencia a campos de los siguientes tipos en un cálculo: 
   >   
   >   * Campo de texto con formato
   >   * Texto descriptivo.
   >   
   >   Para obtener información sobre los tipos de campos personalizados, consulte [Agregar un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).

1. Haga clic en el cuadro de texto grande del cuadro Editor de cálculos y, a continuación, haga clic en buscar o expandir y haga clic en una opción del **Expresiones** y **Campos** secciones a la derecha del cuadro de texto. Esto los añade al cálculo.

   También puede empezar a escribir una expresión o campo en el cuadro de texto grande y, a continuación, seleccionarlo cuando se muestre. Cada elemento se muestra con una &quot;F&quot; para el campo o una &quot;E&quot; para la expresión.

   Si escribe un paréntesis de apertura, el paréntesis de cierre se agrega automáticamente.

   >[!TIP]
   >
   >Puede realizar cualquiera de las siguientes acciones para obtener ayuda con el cálculo:
   > 
   >* Pase el ratón sobre una expresión del cálculo para ver una descripción, un ejemplo que muestre cómo se puede utilizar y un vínculo &quot;Más información&quot; para obtener más información en el artículo [Resumen de las expresiones de datos calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
   >  ![](assets/hover-expression-help-text.jpg)
   >* Utilice la codificación de color para identificar los componentes que ha añadido. Las expresiones se muestran en azul y los campos en verde.
   >  ![](assets/colors-fields-expressions.jpg)
   >* Busque errores de cálculo resaltados en rosa a medida que avanza. Puede situarse sobre un error resaltado para mostrar una breve descripción de su causa.
   >  ![](assets/error-help.png)
   >* En el **Vista previa de un objeto existente** debajo del cálculo, empiece a escribir el nombre de un objeto Workfront, selecciónelo cuando se muestre en la lista. Esto le proporciona una vista previa del aspecto que tendrá el campo cuando se adjunte el formulario al objeto.
   ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
   >  ![](assets/preview-calc.jpg)
   >* Expresiones de referencia en un cálculo largo utilizando los números de línea que se muestran a la izquierda.

1. Clic **Minimizar** cuando haya terminado de crear el cálculo para el campo personalizado calculado.

   >[!NOTE]
   >
   >En el área de visualización de la derecha, el campo muestra un valor de relleno de 12345. Este indicador le recuerda que el campo es un campo personalizado calculado mientras crea o edita el formulario personalizado. Cuando el formulario se adjunta a un objeto y los usuarios lo rellenan, ven el resultado del cálculo en el campo y no el valor 12345.

1. (Opcional) Utilice cualquiera de las siguientes opciones para configurar aún más el campo personalizado calculado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Agregar lógica</td> 
      <td>Puede agregar Lógica de visualización para determinar si el campo calculado se muestra, en función de al menos una opción que realice un usuario en un campo de opción múltiple anterior (Lista desplegable, Casillas de verificación o Botones de opción) al rellenar el formulario. Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Agregar lógica de visualización y saltar lógica a un formulario personalizado</a>. <p>Esto solo está disponible cuando al menos una casilla de verificación, un botón de opción o un campo desplegable precede al campo personalizado calculado en el formulario. </p> <p>La lógica de omisión no está disponible para los campos personalizados calculados.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actualizar cálculos anteriores</td> 
      <td>Cuando esté editando un campo personalizado calculado existente, puede seleccionar esta opción para almacenar en déclencheur una actualización en el cálculo al guardar el formulario personalizado. Esto solo ocurre una vez al guardar el formulario personalizado. La opción vuelve a su estado deshabilitado después de hacerlo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar fórmula en las instrucciones</td> 
      <td>Deje esta opción habilitada si desea que los usuarios que rellenan el formulario personalizado vean la fórmula del campo cuando pasan el ratón por encima del campo. Para obtener más información, consulte la información sobre <a href="#instructions" class="MCXref xref">Instrucciones</a> anteriormente en esta tabla.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Listo** cuando se completen todos los cambios en el campo personalizado calculado.

   O haga clic en **Aplicar** para aplicar los cambios al formulario hasta el momento si desea seguir agregando campos personalizados al formulario.

   O haga clic en **Guardar + Cerrar** cuando se completen todos los cambios en el formulario personalizado.
1. Para comprobar que el campo personalizado calculado funciona correctamente, adjunte el formulario personalizado a un objeto y, a continuación, revise el resultado en el campo personalizado calculado.

   Para obtener instrucciones sobre cómo adjuntar un formulario personalizado, consulte [Agregar un formulario personalizado a un objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Si desea seguir creando el formulario personalizado de otras formas, puede continuar con uno de los siguientes artículos:

   * [Agregar un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Colocar campos y widgets personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Reutilizar un campo personalizado calculado existente en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Agregar lógica de visualización y saltar lógica a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Previsualización y cumplimentación de un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Sintaxis requerida en los campos personalizados calculados

Cada campo utilizado en un campo calculado personalizado debe utilizar la sintaxis explicada a continuación, con llaves alrededor de cada nombre de campo. Cuando empiece a escribir el nombre de un campo, el sistema realiza sugerencias y puede seleccionar una para insertarla en el cálculo. Si introduce datos incorrectamente en un cálculo, un mensaje de advertencia le avisará. No puede guardar el formulario a menos que edite el cálculo para que contenga campos válidos y una expresión calculada válida.

>[!NOTE]
>
>Actualmente, el sistema solo realiza sugerencias cuando empieza a escribir el nombre de un campo al que desea hacer referencia en un objeto al que se adjuntará el formulario personalizado, no en el objeto principal.

### Envolver nombres de campo con llaves

* Si desea que el cálculo haga referencia a un campo integrado, el nombre del campo debe estar entre llaves y debe tener el formato que aparece en la base de datos de Workfront. No puede utilizar el nombre de los campos tal como se muestran en la interfaz de Workfront.

Por ejemplo: `{actualRevenue}`

Los nombres de los campos distinguen entre mayúsculas y minúsculas y deben aparecer en mayúsculas o minúsculas, tal y como aparecen en el sistema de Workfront.

* Si desea que el cálculo haga referencia a un campo personalizado, el nombre del campo debe estar entre llaves y precedido por `DE:` entre corchetes. Los campos personalizados distinguen entre mayúsculas y minúsculas y deben recibir el formato que muestran en la interfaz de Workfront.

Por ejemplo: `{DE:Profit}`

El sistema enumera todos los campos personalizados entre los que puede elegir al escribir `DE:`.

* Si desea que el cálculo haga referencia a un campo que extraerá datos del objeto principal cuando el formulario personalizado esté adjunto a un objeto, debe anteponer el nombre del campo al tipo de objeto del objeto principal, también entre llaves.

  Por ejemplo, si el formulario personalizado está configurado para trabajar con tareas y desea que el campo calcule los ingresos reales del objeto principal cuando el formulario se adjunta a una tarea, debe indicar `project` como tipo de objeto del campo:

  `{project}.{actualRevenue}`

  O bien, si es un campo personalizado:

  `{project}.{DE:profit}`

  Si no está seguro de cuál será el tipo de objeto del objeto principal porque el formulario personalizado está configurado para varios tipos de objetos, puede utilizar la variable de filtro comodín `$$OBJCODE` para permitir que el cálculo funcione para cada uno de los tipos posibles. Para obtener más información, consulte [Campos personalizados calculados en formularios personalizados de varios objetos](#calculated-custom-fields-in-multi-object-custom-forms) en este artículo.

### Separar elementos con puntos

Cuando haga referencia a un objeto relacionado en un campo personalizado calculado, debe separar los nombres y atributos de los objetos con puntos.

Por ejemplo, en un formulario personalizado de tipo de tarea, para mostrar el nombre del Propietario del Portfolio en un campo personalizado calculado, debe escribir lo siguiente:

`{project}.{porfolio}.{owner}`

Este sistema recupera la información en los siguientes pasos (en este orden):

1. Desde el objeto del formulario personalizado (una tarea),
1. Acceda al objeto principal de la tarea u otro objeto relacionado (proyecto) y, a continuación,
1. Acceda al objeto principal o a otro objeto relacionado del proyecto (un portafolio) y, a continuación,
1. Acceda al siguiente objeto relacionado con el portafolio (el propietario del portafolio).

### Sintaxis de nombre para hacer referencia a un campo personalizado

Cuando se hace referencia a otro campo personalizado en un campo personalizado calculado, es necesario introducir el nombre del campo tal y como se muestra en la interfaz de Workfront.

Por ejemplo, para hacer referencia a la opción seleccionada en un campo personalizado denominado Patrocinador ejecutivo, debe escribir lo siguiente:

`{DE:Executive sponsor}`

>[!NOTE]
>
>La sintaxis de un campo de escritura anticipada es diferente a la de otros tipos de campos porque es necesario agregar `:name` al final.
>
>Por ejemplo, para hacer referencia a la opción seleccionada en un campo de escritura anticipada personalizado denominado &quot;Patrocinador ejecutivo&quot;, escribiría:
>
>`{DE:Executive sponsor:name}`

## Campos personalizados calculados en formularios personalizados de varios objetos {#calculated-custom-fields-in-multi-object-custom-forms}

En un formulario personalizado de varios objetos, los tipos de objeto seleccionados deben ser compatibles con todos los campos a los que se hace referencia en los campos personalizados calculados del formulario.

>[!INFO]
>
>**Ejemplo:**
>
>En un formulario personalizado configurado para trabajar con el tipo de objeto Task, se crea un campo personalizado calculado denominado In Charge. Puede configurarlo para que haga referencia al campo integrado y pueda mostrar el nombre del usuario principal asignado cada vez que el formulario se adjunte a una tarea:
>
>`{assignedTo}.{name}`
>
>Posteriormente, se agrega el tipo de objeto Project al formulario personalizado, pero el tipo de objeto Project no es compatible con el campo personalizado calculado.

Cuando esto sucede, puede realizar una de las siguientes acciones:

* Quite uno de los dos elementos incompatibles del formulario personalizado: el tipo de objeto o el campo personalizado calculado al que se hace referencia.
* Mantener ambos elementos y utilizar la variable de filtro comodín `$$OBJCODE` como condición en una expresión IF para crear dos versiones diferentes del campo In Charge. Esto permite que el campo funcione correctamente, independientemente del tipo de objeto al que esté adjunto el formulario.

>[!INFO]
>
>**Ejemplo:** Aunque no hay ningún campo Asignado a: Nombre en los proyectos, hay un campo Propietario integrado (que se rellena automáticamente con el nombre de la persona que creó el proyecto, a menos que alguien cambie esto manualmente).
>
>Por lo tanto, en el campo a cargo personalizado, puede utilizar `$$OBJCODE` como se muestra a continuación, para hacer referencia al campo Propietario cuando el formulario personalizado se adjunta a un proyecto y al campo Asignado a: Nombre cuando el formulario se adjunta a una tarea:
>
>`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

Para obtener más información sobre variables como `$$OBJCODE,` consulte [Resumen de variables de filtro comodín](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Actualizaciones automáticas de campos personalizados calculados

Los campos personalizados calculados en un objeto se vuelven a calcular automáticamente cuando ocurren las siguientes cosas:

* Algo en el objeto cambia, como un cálculo diario de la escala de tiempo.
* Alguien edita otro campo al que se hace referencia mediante un campo personalizado calculado en el objeto.
* La expresión calculada está vacía y el campo contiene un valor; esto establece el valor en nulo.

  >[!NOTE]
  >
  >En un formulario personalizado adjunto a un objeto, las instrucciones de fecha y hora de los campos personalizados calculados se calculan y guardan según la hora universal coordinada (UTC), no según las configuraciones de zona horaria establecidas para la instancia de su organización y el perfil de usuario. Sin embargo, los cálculos de un formulario personalizado se muestran en función de la zona horaria individual de cada usuario.
