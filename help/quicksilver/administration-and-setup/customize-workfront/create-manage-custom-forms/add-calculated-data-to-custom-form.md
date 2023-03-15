---
title: Agregar datos calculados a un formulario personalizado con el generador de formularios heredado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: En un formulario personalizado, puede crear un campo personalizado calculado que genere cálculos. Para ello, se crea una instrucción que utiliza expresiones de datos y los nombres de campos existentes, que pueden ser campos personalizados, campos de datos personalizados calculados y campos integrados de Workfront. Esta instrucción calcula los datos introducidos y muestra el resultado en el nuevo campo personalizado calculado.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9174c4ef-3beb-4d47-9c5c-363f52105a2c
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '2573'
ht-degree: 0%

---

# Agregar datos calculados a un formulario personalizado con el generador de formularios heredado

En un formulario personalizado, puede agregar un campo personalizado calculado que utilice datos existentes para generar nuevos datos cuando el formulario personalizado esté adjunto a un objeto.

Un campo personalizado calculado puede contener:

* Referencia sencilla a un único campo integrado.

   >[!INFO]
   >
   > **Ejemplo:** Para calcular los ingresos generados por los proyectos y las tareas, puede crear un campo personalizado calculado que contenga el campo integrado Ingresos reales. Cuando alguien adjunta el formulario personalizado a un proyecto o tarea, los ingresos del proyecto o la tarea se muestran en el campo .

* Expresión que hace referencia a uno o varios campos. Pueden ser campos personalizados, otros campos personalizados calculados y campos integrados.

   >[!INFO]
   >
   >**Ejemplo:** Para calcular el beneficio generado por proyectos y tareas, puede crear un campo personalizado calculado llamado Beneficio que contenga una expresión matemática que reste el coste de los ingresos.
   >
   >Para ello, puede utilizar la expresión matemática SUB (restar) con los campos integrados de Workfront Coste real e Ingresos reales.
   >
   >En los pasos siguientes, puede ver cómo se puede llevar a cabo este ejemplo.

Para obtener información sobre la creación de formularios personalizados para su organización y comprender el tipo de campos que puede asociar con ellos, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo los administradores de Workfront conceden este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o configuraciones de nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

## Agregar un campo calculado a un formulario personalizado {#add-a-calculated-field-to-a-custom-form}

Puede utilizar los campos integrados de Workfront y los campos personalizados que ya ha creado.

>[!IMPORTANT]
>
>Antes de crear un nuevo campo personalizado calculado, identifique los campos existentes que desee incluir para asegurarse de que los datos necesarios para el cálculo están presentes en Workfront.

1. Comience a crear o editar un formulario personalizado, tal como se describe en [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. En el **Agregar un campo** , haga clic en **Calculado**.

   En el área de visualización de la derecha, se muestra el campo *12345*. Se trata simplemente de un indicador para recordarle que el campo es un campo personalizado calculado mientras crea o edita el formulario personalizado. Cuando el formulario está adjunto a un objeto y los usuarios lo rellenan, ven el resultado del cálculo en el campo , nunca el *12345* indicador.

1. Especifique la siguiente información para el campo calculado:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td>Escriba una etiqueta para el campo. Esto es lo que verán los usuarios cuando utilicen el formulario personalizado. El campo <b>Nombre</b>, que se rellena automáticamente, Workfront hace referencia a ella en los informes.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">Instrucciones</td> 
      <td> De forma predeterminada, la fórmula que cree para el campo se almacena aquí. Puede añadir texto para proporcionar información adicional sobre el campo y la fórmula que contiene. Esto puede resultar útil de dos maneras: 
       <ul> 
        <li> <p>Como recordatorio de qué es la fórmula y cómo funciona. Esto resulta especialmente útil si planea utilizar este campo personalizado calculado en varios formularios.</p> </li> 
        <li> <p>Como información sobre herramientas, los usuarios pueden ver cuando pasan el ratón por encima del campo. Agregue aquí cualquier texto que desee que vean en la información del objeto.</p> <p>Si no desea que vean la fórmula en la información del objeto, lo que puede ser confuso para ellos, puede ocultarla. Para obtener instrucciones, consulte la fila de la tabla "Mostrar fórmula en instrucciones" en la sección <a href="#build-the-calculation-for-your-calculated-custom-field" class="MCXref xref">Generar el cálculo del campo personalizado calculado</a> en este artículo.</p> </li> 
       </ul> <p>Para obtener información sobre el uso del mismo campo personalizado calculado en un formulario nuevo, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md#using-an-existing-calculated-custom-field-on-a-new-form" class="MCXref xref">Reutilizar un campo personalizado calculado existente en un formulario personalizado</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td> 
      <td> <p>El formato en el que desea que se almacenen y muestren los resultados del campo.</p> <p>Si el campo se va a utilizar en cálculos matemáticos, utilice siempre un <strong>Número</strong> o <strong>Moneda</strong> formato. Cuando selecciona Número o Moneda, el sistema trunca automáticamente los números que comienzan por 0.</p> 
      <p><b>IMPORTANTE</b>: Antes de elegir un formato, considere el formato correcto para el nuevo campo. El campo de formato no se puede editar una vez guardado el formulario personalizado. Y seleccionar el formato incorrecto podría afectar a los cálculos futuros y a los valores acumulados en las agrupaciones de informes y listas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Continúe con [Generar el cálculo del campo personalizado calculado](#build-the-calculation-for-your-calculated-custom-field) en este artículo.

## Generar el cálculo del campo personalizado calculado {#build-the-calculation-for-your-calculated-custom-field}

1. Comience a crear el campo personalizado calculado, tal como se explica en la sección [Agregar un campo calculado a un formulario personalizado](#add-a-calculated-field-to-a-custom-form) en este artículo.

1. Haga clic en **Maximizar** para abrir el **Editor de cálculo** y cree su cálculo.

   >[!INFO]
   >
   >**Ejemplo:** Con el ejemplo de la introducción a este artículo, puede crear un campo personalizado calculado denominado Beneficio en un formulario personalizado para proyectos y tareas. Este campo puede contener un cálculo que muestre la diferencia entre los ingresos reales y el costo real:
   >
   >`SUB({actualRevenue},{actualCost})`
   >
   >En este ejemplo, `SUB` es la expresión y los campos a los que se hace referencia son `actualRevenue` y `actualCost`.

   Un cálculo suele comenzar con una expresión, seguida de paréntesis que contienen los campos a los que desea hacer referencia cuando el formulario personalizado está adjunto a un objeto. Para obtener información sobre las expresiones disponibles, consulte [Expresiones de datos calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Cada campo debe estar rodeado de llaves, como se explica en la sección [Sintaxis requerida en los campos personalizados calculados](#syntax-required-in-calculated-custom-fields) en este artículo. Al empezar a escribir el nombre de un campo, el sistema realiza sugerencias y puede seleccionar una para insertarla en el cálculo.

   Puede hacer referencia a cualquier tipo de campo personalizado en un cálculo, excepto a dos: Campo de texto con tipo Formato y Texto descriptivo. Para obtener información sobre los tipos de campo personalizados, consulte [Añadir un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)

1. Haga clic en el cuadro de texto grande y, a continuación, haga clic en **Expresiones** y **Campos** que están disponibles para agregarlas al cálculo.

   También puede empezar a escribir una expresión o campo en el cuadro de texto grande y, a continuación, seleccionarlo cuando se muestre. Cada elemento aparece con una &quot;F&quot; para el campo o una &quot;E&quot; para la expresión.

   Si escribe un paréntesis de apertura, el paréntesis de cierre se agrega automáticamente.

   >[!TIP]
   >
   >Puede realizar cualquiera de las siguientes acciones para obtener ayuda con su cálculo:
   > 
   >* Pase el ratón sobre una expresión en el cálculo para ver una descripción, un ejemplo que muestre cómo se puede utilizar y un vínculo &quot;Más información&quot; para obtener más información en el artículo [Expresiones de datos calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
      >  ![](assets/hover-expression-help-text.jpg)
   >* Utilice la codificación de color para identificar los componentes que ha añadido. Las expresiones se muestran en azul y los campos en verde.
      >  ![](assets/colors-fields-expressions.jpg)
   >* Busque errores de cálculo, resaltados en rosa, a medida que avanza. Puede situarse sobre un error resaltado para mostrar una breve descripción de su causa.
      >  ![](assets/error-help.png)
   >* En el área inferior al cálculo, previsualice los resultados en un objeto de Workfront existente.
      ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->

      >  ![](assets/preview-calc.jpg)
   >* Haga referencia a las expresiones en un cálculo largo utilizando los números de línea que aparecen a la izquierda.


1. Haga clic en **Minimizar** cuando haya terminado de crear el cálculo para el campo personalizado calculado.

   >[!NOTE]
   >
   >En el área de visualización de la derecha, se muestra el campo *12345.* Se trata simplemente de un indicador para recordarle que el campo es un campo personalizado calculado mientras crea o edita el formulario personalizado. Cuando el formulario está adjunto a un objeto y los usuarios lo rellenan, ven el resultado del cálculo en el campo , nunca el *12345* indicador.

1. (Opcional) Utilice cualquiera de las siguientes opciones para seguir configurando el campo personalizado calculado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Agregar lógica</td> 
      <td>Puede agregar Lógica de visualización para determinar si se muestra el campo calculado, en función de al menos una opción que realice un usuario en un campo de opción múltiple anterior (menú desplegable, casillas de verificación o botones de opción) al rellenar el formulario. Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Agregar lógica de visualización y de omisión de lógica a un formulario personalizado</a>. <p>Solo está disponible cuando al menos una casilla de verificación, un botón de opción o un campo desplegable precede al campo personalizado calculado del formulario. </p> <p>La lógica de omisión no está disponible para los campos personalizados calculados.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actualizar cálculos anteriores</td> 
      <td>Cuando edita un campo personalizado calculado existente, puede seleccionar esta opción para almacenar en déclencheur una actualización en el cálculo al guardar el formulario personalizado. Esto sucede solo una vez cuando se guarda el formulario personalizado. Después de hacerlo, la opción vuelve a su estado desactivado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar fórmula en las instrucciones</td> 
      <td>Deje esta opción activada si desea que los usuarios que rellenen el formulario personalizado vean la fórmula del campo cuando pasen el ratón por encima del campo. Para obtener más información, consulte la información sobre <a href="#instructions" class="MCXref xref">Instrucciones</a> más temprano en esta tabla.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Listo** cuando se hayan completado todos los cambios en el campo personalizado calculado.

   O bien, haga clic en **Aplicar** para aplicar los cambios al formulario hasta ahora si desea seguir agregando campos personalizados al formulario.

   O bien, haga clic en **Guardar + Cerrar** cuando se hayan completado todos los cambios en el formulario personalizado.
1. Para comprobar que el campo personalizado calculado funciona correctamente, adjunte el formulario personalizado a un objeto y, a continuación, revise el resultado en el campo personalizado calculado.

   Para obtener instrucciones sobre cómo adjuntar un formulario personalizado, consulte [Adición de un formulario personalizado a un objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Si desea seguir creando el formulario personalizado de otras formas, puede continuar con uno de los siguientes artículos:

   * [Añadir un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Colocación de campos y widgets personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Reutilizar un campo personalizado calculado existente en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Agregar lógica de visualización y de omisión de lógica a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Obtener una vista previa y completar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Sintaxis requerida en los campos personalizados calculados

Cada campo debe utilizar la sintaxis que se explica a continuación, con llaves alrededor de cada nombre de campo. Al empezar a escribir el nombre de un campo, el sistema realiza sugerencias y puede seleccionar una para insertarla en el cálculo. Si introduce datos incorrectamente en un cálculo, un mensaje de advertencia le avisará. No se puede guardar el formulario a menos que edite el cálculo para que contenga campos válidos y una expresión calculada válida.

>[!NOTE]
>
>Actualmente, el sistema solo realiza sugerencias cuando comienza a escribir el nombre de un campo al que desea hacer referencia en un objeto al que se adjuntará el formulario personalizado, no en el objeto principal.

### Rodee los nombres de los campos con llaves

* Si desea que el cálculo haga referencia a un campo integrado, el nombre del campo debe estar entre llaves.

Por ejemplo: `{actualRevenue}`

Los nombres de campo distinguen entre mayúsculas y minúsculas y deben aparecer en el cálculo exactamente como aparecen en el sistema Workfront.

* Si desea que el cálculo haga referencia a un campo personalizado, el nombre del campo debe estar entre llaves y precedido por `DE:` entre corchetes.

Por ejemplo: `{DE:Profit}`

El sistema enumera todos los campos personalizados que puede elegir al escribir `DE:`.

* Si desea que el cálculo haga referencia a un campo que extraerá datos del *parent* cuando el formulario personalizado está adjunto a un objeto, debe preceder al nombre del campo con el tipo de objeto del objeto principal, también entre llaves.

   Por ejemplo, si el formulario personalizado está configurado para funcionar con tareas y desea que el campo calcule los ingresos reales del objeto principal cuando el formulario está adjunto a una tarea, debe indicar `Project` como tipo de objeto del campo:

   `{project}.{actualRevenue}`

   O, si es un campo personalizado:

   `{project}.{DE:profit}`

   Si no está seguro de cuál será el tipo de objeto del objeto principal porque el valor personalizado de está configurado para varios tipos de objeto, puede utilizar la variable de filtro comodín `$$OBJCODE` para permitir que el cálculo funcione para cada uno de los tipos posibles. Para obtener más información, consulte [Campos personalizados calculados en formularios personalizados con varios objetos](#calculated-custom-fields-in-multi-object-custom-forms) en este artículo.

### Separar elementos con períodos

Cuando se hace referencia a un objeto relacionado en un campo personalizado calculado, se deben separar los nombres y atributos de los objetos con puntos.

Por ejemplo, en un formulario personalizado de tipo tarea, para mostrar el nombre del propietario del Portfolio en un campo personalizado calculado, debe escribir lo siguiente:

`{project}.{porfolio}.{owner}`

Esto determinaría lo siguiente: Desde el objeto del formulario personalizado (una tarea), puede acceder al siguiente objeto relacionado con la tarea (un proyecto). Desde allí, puede acceder al siguiente objeto relacionado del proyecto (un portafolio) y, a continuación, al siguiente objeto relacionado del portafolio (el propietario).

### Sintaxis del nombre para hacer referencia a un campo personalizado

Al hacer referencia a otro campo personalizado en un campo personalizado calculado, debe introducir el nombre del campo que aparece tal como aparece en la interfaz de usuario de Workfront.

Por ejemplo, para hacer referencia a la opción seleccionada en un campo personalizado etiquetado como patrocinador ejecutivo, debe escribir lo siguiente:

`{DE:Executive sponsor}`

>[!NOTE]
>
>La sintaxis de un campo typeforward es un poco diferente a la de otros tipos de campos, ya que es necesario agregar `:name` al final.
>
>Por ejemplo, para hacer referencia a la opción seleccionada en un campo personalizado de tipo &quot;Analizador ejecutivo&quot;, debe escribir:
>
>`{DE:Executive sponsor:name}`


## Campos personalizados calculados en formularios personalizados con varios objetos {#calculated-custom-fields-in-multi-object-custom-forms}

En un formulario personalizado de varios objetos, los tipos de objeto seleccionados deben ser compatibles con todos los campos a los que se hace referencia en los campos personalizados calculados del formulario. Si hay una incompatibilidad, un mensaje le alerta para que realice ajustes.

>[!INFO]
>
>**Ejemplo:**
>
>En un formulario personalizado configurado para trabajar con el tipo de objeto Task , se crea un campo personalizado calculado llamado In Charge. Se configura para que haga referencia al campo integrado de modo que pueda mostrar el nombre del usuario asignado principal a cargo cada vez que el formulario esté adjunto a una tarea:
>
>`{assignedTo}.{name}`
>
>Posteriormente, se agrega el tipo de objeto Project al formulario personalizado. Un mensaje de advertencia indica que el tipo de objeto Project es incompatible con el campo personalizado calculado.

Cuando esto sucede, puede realizar una de las siguientes acciones:

* Elimine uno de los dos elementos incompatibles del formulario personalizado: el tipo de objeto o el campo personalizado calculado al que se hace referencia.
* Mantener ambos elementos y utilizar la variable de filtro comodín `$$OBJCODE` como condición en una expresión IF para crear dos versiones diferentes del campo In Charge . Esto permite que el campo funcione correctamente, independientemente del tipo de objeto al que esté adjunto el formulario.

>[!INFO]
>
>**Ejemplo:** Aunque no hay asignado a: Campo Nombre de los proyectos, hay un campo Propietario integrado (que se rellena automáticamente con el nombre de la persona que creó el proyecto, a menos que alguien lo cambie manualmente).
>
>Por lo tanto, en el campo personalizado A cargo, puede usar `$$OBJCODE` como se muestra a continuación para hacer referencia al campo Propietario cuando el formulario personalizado está adjunto a un proyecto y Assigned To: Campo Nombre cuando el formulario está adjunto a una tarea:
>
>`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

Para obtener más información sobre variables como `$$OBJCODE,` see [Variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Actualizaciones automáticas de campos personalizados calculados

Los campos personalizados calculados en un objeto se vuelven a calcular automáticamente cuando suceden los siguientes hechos:

* Algo en el objeto cambia, como el cálculo diario de la cronología.
* Alguien edita otro campo al que se hace referencia en un campo personalizado calculado del objeto.
* La expresión calculada está vacía y el campo contiene un valor; esto establece el valor en null.

   >[!NOTE]
   >
   ><div>En un formulario personalizado adjunto a un objeto, las instrucciones de fecha y hora de los campos personalizados calculados se calculan y se guardan en la Hora universal coordinada (UTC), no en las configuraciones de zona horaria establecidas para la instancia de su organización y su perfil de usuario. Los cálculos en un formulario personalizado se generan en función de los husos horarios individuales de cada usuario.</div>

