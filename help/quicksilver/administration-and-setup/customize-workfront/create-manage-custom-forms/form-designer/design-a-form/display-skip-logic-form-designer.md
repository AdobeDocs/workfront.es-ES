---
title: Agregar la lógica de visualización y la lógica de omisión a un formulario
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede decidir qué secciones de un formulario personalizado se deben mostrar u omitir en función de las opciones que realice un usuario al rellenarlo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5f5dbeb5-b974-489c-8f4d-ebaa00f5e5ba
source-git-commit: 75aaa531dba8037ed75c0d6baa6d7c69ec4cfefd
workflow-type: tm+mt
source-wordcount: '1317'
ht-degree: 93%

---

# Agregar lógica de visualización y saltar lógica a un formulario

Puede decidir qué secciones de un formulario personalizado se deben mostrar u omitir en función de las opciones que realice un usuario al rellenarlo.

>[!NOTE]
>
>La lógica solo se aplica dentro de un formulario y no se puede basar en selecciones de un formulario diferente.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Para realizar los pasos de este artículo, debe tener lo siguiente:

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

Los formularios personalizados muestran iconos para indicar qué lógica se aplica a determinados campos. Los iconos de un campo en el diseñador de formularios indican que se aplica lógica al campo.

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
Para obtener información sobre los campos y widgets personalizados en los formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
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

{{step-1-to-setup}}

1. Haga clic en **Formularios personalizados**.
1. Cree un nuevo formulario personalizado o abra uno existente. Consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) para obtener más información.
1. Agregue campos al formulario según sea necesario. Al menos un campo de opción múltiple (botón de radio, menú desplegable o casilla de verificación) debe estar posicionado antes del campo objetivo que se mostrará.
1. Seleccione el campo objetivo y haga clic en **Agregar lógica** en la parte inferior izquierda de la pantalla.
1. Seleccione la pestaña **Lógica de visualización**.
1. Haga clic en **Agregar regla de visualización** en el generador de lógica.

   ![Generador de lógica de visualización](assets/custom-form-logic-builder-display-blank.png)

1. Siga los pasos siguientes en el generador para crear la instrucción lógica.

   1. La primera opción es elegir el campo de definición. Este es el campo con el valor de selección que muestra el objetivo. Debe ser un campo de opción múltiple.
   1. La segunda opción es elegir el valor de selección. Solo están disponibles los valores ya definidos para ese campo.
   1. La tercera opción es **Seleccionado** o **No seleccionado**. Elegir **Seleccionado** significa que cuando se selecciona el valor, se muestra el campo de destino. Elegir **No seleccionado** significa que cuando se selecciona cualquier otro valor en el campo definitorio, se muestra el campo objetivo.
   1. Para añadir una regla **Y** a la instrucción lógica, haga clic en **Agregar regla** directamente debajo de la regla que acabas de crear. Siga las mismas indicaciones para generar la regla. Todas las reglas Y deben cumplirse para que el campo objetivo se muestre.

      ![Mostrar generador de lógica](assets/custom-form-logic-builder-display1.png)

   1. Para añadir una regla **O** a la instrucción lógica, haz clic en **Agregar regla** cerca de la parte inferior del generador de lógica. Luego, haga clic en **Agregar regla** dentro del área O y siga las mismas indicaciones para generar la regla. Cuando se cumple una regla O, el campo objetivo se muestra.

1. Haga clic en **Guardar** cuando termine de construir la instrucción lógica.

   Los iconos de la lógica de visualización se añaden al campo objetivo y al campo definitorio en el diseñador de formularios.

## Agregar lógica de omisión a un formulario personalizado

La lógica de omisión define campos de formulario personalizados que se omiten cuando el usuario selecciona un valor específico en un campo de opción múltiple. Los campos omitidos están ocultos en el formulario. La lógica se aplica al campo de definición donde se realiza la selección, no a los campos que se omiten.

{{step-1-to-setup}}

1. Haga clic en **Formularios personalizados**.
1. Cree un nuevo formulario personalizado o abra uno existente. Consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) para obtener más información.
1. Agregue campos al formulario según sea necesario. El campo de definición para la lógica de omisión debe ser un campo de selección múltiple (botón de opción, lista desplegable o casilla de verificación).
1. Seleccione el campo de definición y haga clic en **Agregar lógica** en la parte inferior izquierda de la pantalla.
1. Seleccione la pestaña **Lógica de omisión**.
1. Haga clic en **Agregar regla de omisión** en el generador de lógica.

   ![Omitir generador de lógica](assets/custom-form-logic-builder-skip-blank.png)

1. Siga los pasos siguientes en el generador para crear la instrucción lógica.

   1. El campo de definición se muestra en el generador. Es el campo seleccionado al que se aplica la lógica de omisión.
   1. La primera opción es elegir el valor de selección. Solo están disponibles los valores ya definidos para el campo.
   1. La segunda opción es **Seleccionado** o **No seleccionado**. Elegir **Seleccionado** significa que cuando se selecciona el valor, el campo objetivo se muestra y los campos intermedios se omiten. Elegir **No seleccionado** significa que cuando se selecciona cualquier otro valor en el campo de definición, se muestra el campo de destino y se omiten los campos intermedios.
   1. La tercera opción es el campo de destino o el punto al que saltar. Seleccione un nombre de campo o de **Fin de formulario**. Es posible que tenga que hacer clic primero en la palabra “vacío” antes de seleccionar una opción.

      ![Omitir generador de lógica](assets/custom-form-logic-builder-skip1.png)

   1. Para añadir una regla **O** a la instrucción lógica, haga clic en **Agregar regla** cerca de la parte inferior del generador de lógica. A continuación, seleccione las opciones siguiendo las mismas indicaciones para generar la regla. Cuando se cumple una regla **O** se muestra el campo de destino.

1. Haga clic en **Guardar** cuando termine de crear la instrucción lógica.

   Los iconos de lógica de omisión se agregan al campo de destino y al campo de definición en el diseñador de formularios.


