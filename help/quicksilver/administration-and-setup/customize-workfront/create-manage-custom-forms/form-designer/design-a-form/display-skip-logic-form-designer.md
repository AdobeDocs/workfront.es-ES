---
title: añadir reglas lógicas a Forms y campos personalizados
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede decidir qué secciones de un formulario personalizado se deben mostrar u omitir en función de las opciones que realice un usuario al rellenarlo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5f5dbeb5-b974-489c-8f4d-ebaa00f5e5ba
source-git-commit: 428e6a9365c793ce5944941ec5368a674c208c78
workflow-type: tm+mt
source-wordcount: '1680'
ht-degree: 66%

---

# Agregar reglas lógicas a formularios y campos personalizados

Las reglas lógicas permiten personalizar aún más los campos del formulario.

Por ejemplo, puede mostrar u omitir campos o secciones en un formulario personalizado en función de las opciones que realice un usuario al rellenarlo.

>[!NOTE]
>
>La lógica solo se aplica dentro de un formulario y no se puede basar en selecciones de un formulario diferente.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Plan de Adobe Workfront </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Acceso administrativo a formularios personalizados </td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mostrar y omitir iconos lógicos

Los formularios personalizados muestran iconos para indicar cuándo se aplica la lógica de visualización u omisión a determinados campos. Los iconos de un campo en el diseñador de formularios indican que se aplica lógica al campo.

| Icono | Ubicación en el campo en el diseñador de formularios | Definición |
|--- |--- |--- |
| ![Lógica de visualización para el campo de destino](assets/display-logic-bottom-left.png) | Inferior izquierda | El campo es el campo de destino para la lógica de visualización. Si se realiza una selección específica en el formulario, se muestra este campo. |
| ![Definir icono de lógica de visualización](assets/display-logic-bottom-right.png) | Inferior derecha | El campo define la lógica de visualización. Una selección o un valor específico de este campo muestra el campo de destino. |
| ![Omitir lógica para campo de destino](assets/skip-logic-bottom-left.png) | Inferior izquierda | El campo es el campo de destino para la lógica de omisión. Si se realiza una selección específica en el formulario, este se salta este campo y los campos intermedios están ocultos. |
| ![Definir icono de omisión de lógica](assets/skip-logic-bottom-right.png) | Inferior derecha | El campo define la lógica de omisión. Una selección o valor específico de este campo omite otros campos y va directamente al campo de destino. |

![Iconos lógicos](assets/logic-icons-3.png)

Seleccione un campo con lógica aplicada para mostrar las reglas lógicas existentes en la configuración del campo.

![Reglas lógicas](assets/form-designer-view-only-logic.png)

## Consideraciones para utilizar la lógica de visualización y la lógica de omisión

* Para agregar lógica de visualización en un campo personalizado, widget o salto de sección, debe colocarse al menos un campo de opción múltiple (botones de opción, listas desplegables o casillas de verificación) antes de él en el formulario.
Para obtener información sobre los campos personalizados y las utilidades de los formularios personalizados, consulte [Crear formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* No se puede añadir lógica de omisión a un widget o salto de sección. Solo puede añadirlo a un campo de opción múltiple (botones de opción, listas desplegables o casillas de verificación).
* No se puede aplicar la lógica de visualización u omisión para mostrar u ocultar las opciones de un campo de varias opciones. Por ejemplo, no puede restringir las opciones que se muestran para un campo Desplegable, un grupo de casillas de verificación o un campo de botón de opción en función de la lógica de visualización u omisión de otro campo.
* Puede añadir lógica de visualización y lógica de omisión a un campo personalizado si se cumplen todas las condiciones siguientes en relación con el campo personalizado:

   * Es un campo de opción múltiple (botones de opción, listas desplegables o casillas de verificación)
   * Va precedido de un campo de opción múltiple
   * Va seguido de otro campo personalizado

* Al copiar formularios con lógica de visualización o lógica de omisión, la lógica se copia al nuevo formulario personalizado.
* Al editar objetos de forma masiva, todos los campos personalizados se muestran en el cuadro Editar objetos, incluidos los campos omitidos u ocultos.
* Tenga en cuenta lo siguiente al crear una regla de lógica de visualización para un formulario personalizado:

   * De forma predeterminada, los campos personalizados no incluidos en una instrucción lógica de visualización se muestran en un formulario personalizado.
   * Puede crear instrucciones lógicas de visualización de varios campos.
   * Si todos los campos bajo una división de sección tienen lógica de visualización aplicada y todos están ocultos como resultado de la lógica, toda la sección se ocultará en el formulario personalizado.

## Agregar lógica de visualización a un formulario personalizado

La lógica de visualización define qué campos personalizados aparecen en el formulario cuando el usuario selecciona un valor específico en un campo de opción múltiple. La lógica se añade al campo de destino, que solo se muestra cuando se selecciona el valor.

<!--
>[!NOTE]
>
><span class="preview">This procedure describes the basic mode for display logic. Advanced display logic is also available. For more information, see [Add advanced display logic to a custom form](#add-advanced-display-logic-to-a-custom-form), in this article.</span>
-->

{{step-1-to-setup}}

1. Haga clic en **Formularios personalizados**.
1. Cree un nuevo formulario personalizado o abra uno existente. Consulte [Crear un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) personalizado para obtener más detalles.
1. Agregue campos al formulario según sea necesario. Al menos un campo de opción múltiple (botón de radio, menú desplegable o casilla de verificación) debe estar posicionado antes del campo objetivo que se mostrará.
1. Seleccione el campo de destino y haga clic en **Agregar lógica**.
1. Seleccione la ficha **Mostrar** en el generador de lógica.
1. Haga clic en **Agregar regla para mostrar**.

   ![Generador de lógica de visualización](assets/simple-display-logic1-val-only-in-menu.png)

1. Siga los pasos a continuación para crear la instrucción lógica en el generador.

   1. La primera opción es elegir el campo de definición. Este es el campo con el valor de selección que muestra el objetivo. Debe ser un campo de opción múltiple.
   1. La segunda opción es elegir el valor de selección. Solo están disponibles los valores ya definidos para ese campo.
   1. La tercera opción es **Seleccionado** o **No seleccionado**. Elegir **Seleccionado** significa que cuando se selecciona el valor, se muestra el campo de destino. Elegir **No seleccionado** significa que cuando se selecciona cualquier otro valor en el campo definitorio, se muestra el campo objetivo.
   1. Para añadir una regla **Y** a la instrucción lógica, haga clic en **Agregar regla** directamente debajo de la regla que acabas de crear. Siga las mismas indicaciones para generar la regla. Todas las reglas Y deben cumplirse para que el campo objetivo se muestre.

      ![Mostrar generador de lógica](assets/simple-display-logic2.png)

   1. Para añadir una regla **O** a la instrucción lógica, haz clic en **Agregar regla** cerca de la parte inferior del generador de lógica. Luego, haga clic en **Agregar regla** dentro del área O y siga las mismas indicaciones para generar la regla. Cuando se cumple una regla O, el campo objetivo se muestra.

1. Haga clic en **Aplicar** cuando haya terminado de generar la instrucción lógica.

   Los iconos de la lógica de visualización se añaden al campo objetivo y al campo definitorio en el diseñador de formularios.

<!--
<div class="preview">

## Add advanced display logic to a custom form

The advanced display logic for custom form fields allows you to build complex logic using formulas. You can apply this logic to the following field types: drop-down, radio button, checkbox, typeahead, single line text, paragraph text, date field, text with formatting, and calculated fields.

### Examples

You can use advanced display logic to control the visibility of custom form sections based on user roles and the visibility of a field based on another field's status.

No logic is applied to the default section on the form, so it is always visible to all users.

Using the following condition, the Resources Required section is only displayed when a user with the job role of Resource Manager views the form.

```IF($$USER.{roleID}="123abc", true)```

Note that ```123abc``` represents the role ID of the Resource Manager.

![Form section displayed for role](assets/advanced-display-on-form1.png)

The same condition with a different role ID is applied to the Project Financial KPIs section to define that  only the Financial Advisor role can view the section.

Using the following condition, the Sold KPI field only becomes visible when the project is complete. This logic is applied directly to the field instead of to a form section. There is no need to specify which role can view the field, because that is already defined in the section that the field is in.

```IF({status}="CPL", true)```

![Field is visible on complete project](assets/advanced-display-on-form2.png)

### Define advanced display logic

{{step-1-to-setup}}

1. Click **Custom Forms**.
1. Create a new custom form or open an existing form. See [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) for details.
1. Add fields to the form as needed.
1. Select the field to apply logic to, and click **Add Logic**.
1. Select the **Display** tab on the logic builder.
1. Turn on **Advanced mode**.
   
   This option might be turned on automatically, for fields that do not support the simple mode of display logic.

   ![Advanced mode for display logic](assets/advanced-display-logic-blank-editor.png)

1. Build the display condition in the editor.

   For more information about calculations and expressions, see [Add calculated fields to a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) and [Overview of calculated data expressions](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. Click **Apply**.
   
   The logic is applied to the field and the display logic icon is added in the form designer.

</div>
-->

## Agregar lógica de omisión a un formulario personalizado

La lógica de omisión define campos de formulario personalizados que se omiten cuando el usuario selecciona un valor específico en un campo de opción múltiple. Los campos omitidos están ocultos en el formulario. La lógica se aplica al campo de definición donde se realiza la selección, no a los campos que se omiten.

{{step-1-to-setup}}

1. Haga clic en **Formularios personalizados**.
1. Cree un nuevo formulario personalizado o abra uno existente. Consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) para obtener más información.
1. Agregue campos al formulario según sea necesario. El campo de definición para la lógica de omisión debe ser un campo de selección múltiple (botón de opción, lista desplegable o casilla de verificación).
1. Seleccione el campo de definición y haga clic en **Agregar lógica** en la parte inferior izquierda de la pantalla.
1. Seleccione el **pestaña Omitir** en el generador lógico.
1. Haga clic en **añadir regla** de omisión.

   ![Omitir generador de lógica](assets/skip-logic1-val-only-in-menu.png)

1. Siga los pasos a continuación para crear la instrucción lógica en el generador.

   1. El campo de definición se muestra en el generador. Es el campo seleccionado al que se aplica la lógica de omisión.
   1. La primera opción es elegir el valor de selección. Solo están disponibles los valores ya definidos para el campo.
   1. La segunda opción es **Seleccionado** o **No seleccionado**. Elegir **Seleccionado** significa que cuando se selecciona el valor, el campo objetivo se muestra y los campos intermedios se omiten. Elegir **No seleccionado** significa que cuando se selecciona cualquier otro valor en el campo de definición, se muestra el campo de destino y se omiten los campos intermedios.
   1. La tercera opción es el campo de destino o el punto al que saltar. Seleccione un nombre de campo o de **Fin de formulario**. Es posible que tenga que hacer clic primero en la palabra “vacío” antes de seleccionar una opción.

      ![Omitir generador de lógica](assets/skip-logic2.png)

   1. Para añadir una regla **O** a la instrucción lógica, haga clic en **Agregar regla** cerca de la parte inferior del generador de lógica. A continuación, seleccione las opciones siguiendo las mismas indicaciones para generar la regla. Cuando se cumple una regla **O** se muestra el campo de destino.

1. Haga clic en **Aplicar** cuando termine de crear la instrucción lógica.

   Los iconos de lógica de omisión se agregan al campo de destino y al campo de definición en el diseñador de formularios.

## añadir lógica validación a un formulario personalizado

La lógica de validación se construye mediante fórmulas y puede hacer que la lógica sea tan simple o tan compleja como sea necesario. La validación puede basarse en los valores de otros campos o en el estado de los objetos, y se puede proporcionar un mensaje de error para cuando se produzca un error en el validación.

Si el campo con la lógica aplicada cumple las condiciones de validación definidas cuando un usuario rellena el formulario personalizado, el campo se resalta y aparece el mensaje de error.

Puede aplicar validación lógica a los siguientes tipos de campo: texto de una sola línea, párrafo, menú desplegable de selección única, menú desplegable de selección múltiple, búsqueda externa, botones de opción, grupo casilla de verificación y escritura anticipada.

### Ejemplos

Con la siguiente condición, el campo Presupuesto muestra un mensaje debajo del campo cuando el usuario introduce un valor que activa el mensaje. Por ejemplo, si el valor introducido es negativo, se muestra el primer mensaje. Si el usuario intenta cambiar el estado del proyecto a Actual antes de introducir un valor de presupuesto, se muestra el segundo mensaje.

```
IF({DE:Budget Field} < 0,
     "Budget cannot be negative",
     IF({DE:Budget Field} == 0 && {status} == "CUR", "Budget must be specified before moving to Current status")
)
```

Otro ejemplo sencillo es que un campo de número de teléfono debe contener un determinado número de dígitos para que sea válido.

Un ejemplo adicional de validación basado en otros campos es un campo para el tamaño de la sala de reuniones (pequeña, mediana o grande) y un campo independiente para el número de asistentes a la reunión. El número de personas para cada tamaño de habitación se escribe en la fórmula de validación. Si el número de asistentes que el usuario introduce es demasiado para la sala de reuniones elegida, se muestra el mensaje de error.

### Definir validación lógica

{{step-1-to-setup}}

1. Haga clic en **Formularios personalizados**.
1. Cree un nuevo formulario personalizado o abra uno existente. Consulte [Crear un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) personalizado para obtener más detalles.
1. añadir campos al formulario según sea necesario.
1. Seleccione el campo al que desea aplicar lógica y haga clic en **añadir lógica**.
1. Seleccione el pestaña validación **** en el generador lógico.

   ![Generador lógico de validación](assets/validation-logic-blank-editor-val-only-in-menu.png)

1. Genere la condición validación en el editor, incluido el mensaje de error que se muestra cuando no se cumple el validación.

   Para obtener más información sobre cálculos y expresiones, vea [Agregar campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) y [Información general sobre expresiones de datos calculados](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. Haga clic en **Aplicar**.

   La lógica se aplica al campo en el diseñador de formularios.

<!--
<div class="preview">

## Add formatting logic to a custom form

Formatting logic highlights a field value when it meets the defined conditions. You can apply formatting logic to all field types, and it will work on multiple fields at once.

Formatting applied to custom forms is separate from formatting applied to lists and reports. For information on report formatting, see [Use conditional formatting in views](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Example

Using the following condition, the Budget field appears red when the user enters a value of 1000 or more. The field appears yellow when the user enters a value of 500 or more.

To add a hover-over definition of the formatting, use the Instructions field in the custom form. For example, a message on the Budget field could say "Please enter a budget within a reasonable range. Values over 500 are a warning notice, and above 1000 is considered too high."

```
IF(
     {DE:Budget Field} >=1000,
     FORMAT($$NEGATIVE),
     IF({DE:Budget Field} >= 500, FORMAT($$NOTICE))
)
```

### Define formatting logic

{{step-1-to-setup}}

1. Click **Custom Forms**.
1. Create a new custom form or open an existing form. See [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) for details.
1. Add fields to the form as needed.
1. Select the field to apply logic to, and click **Add Logic**.
1. Select the **Formatting** tab on the logic builder.

   ![Formatting logic builder](assets/formatting-logic-blank-editor.png)

1. Build the formatting condition in the editor.

   You can add up to five formatting rules per field.

   The field highlighting color options are:

   * `$$POSITIVE (green)`
   * `$$INFORMATIVE (blue)`
   * `$$NEGATIVE (red)`
   * `$$NOTICE (orange)`
   
   The text formatting options are:
   
   * `$$BOLD`
   * `$$ITALIC`
   * `$$UNDERLINE`

   Only one color option may be used per function, along with up to three additional text formatting options. If no color option is specified, the system's default color is applied.

   For more information about calculations and expressions, see [Add calculated fields to a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) and [Overview of calculated data expressions](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. Click **Apply**.
   
   The logic is applied to the field in the form designer.

</div>
-->
