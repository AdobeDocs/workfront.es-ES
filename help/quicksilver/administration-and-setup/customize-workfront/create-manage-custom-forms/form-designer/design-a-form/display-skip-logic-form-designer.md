---
title: Agregar lógica de visualización y lógica de omisión con el diseñador de formularios
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede decidir qué secciones de un formulario personalizado se deben mostrar o omitir en función de las opciones que realice un usuario al rellenarlo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: 930a04e02d73b75a6dac957e4dfbc76a5f73246f
workflow-type: tm+mt
source-wordcount: '1358'
ht-degree: 0%

---

# Agregar lógica de visualización y lógica de omisión con el diseñador de formularios

<span class="preview">La información de esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes de o en el entorno de producción para los clientes que habilitaron versiones rápidas de.</span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Activar o desactivar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Para obtener más información sobre la versión actual, consulte [Información general sobre la versión del segundo trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Puede decidir qué secciones de un formulario personalizado se deben mostrar o omitir en función de las opciones que realice un usuario al rellenarlo.

>[!NOTE]
>
>La lógica solo se aplica dentro de un formulario y no se puede basar en selecciones de un formulario diferente.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">plan de Adobe Workfront </td> 
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

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Mostrar y omitir iconos lógicos

Los formularios personalizados muestran iconos para indicar qué lógica se aplica a determinados campos. Los iconos de un campo en el diseñador de formularios indican que se aplica lógica al campo.

| Icono | Ubicación en el campo en el diseñador de formularios | Definición |
|--- |--- |--- |
| ![Mostrar lógica para el campo de destino](assets/display-logic-bottom-left.png) | Inferior izquierda | El campo es el campo de destino para la lógica de visualización. Si se realiza una selección específica en el formulario, se muestra este campo. |
| ![Definir icono de lógica de visualización](assets/display-logic-bottom-right.png) | Inferior derecha | El campo define la lógica de visualización. Una selección o un valor específico de este campo muestra el campo de destino. |
| ![Omitir lógica para campo de destino](assets/skip-logic-bottom-left.png) | Inferior izquierda | El campo es el campo de destino para la lógica de omisión. Si se realiza una selección específica en el formulario, este se salta este campo y los campos intermedios están ocultos. |
| ![Definir icono de lógica de omisión](assets/skip-logic-bottom-right.png) | Inferior derecha | El campo define la lógica de omisión. Una selección o valor específico de este campo omite otros campos y va directamente al campo de destino. |

![Iconos lógicos](assets/logic-icons-3.png)

Seleccione un campo con lógica aplicada para mostrar las reglas lógicas existentes en la configuración del campo.

![Reglas lógicas](assets/form-designer-view-only-logic.png)

## Consideraciones para utilizar la lógica de visualización y la lógica de omisión

* Para agregar lógica de visualización en un campo personalizado, widget o salto de sección, debe colocarse al menos un campo de opción múltiple (botones de opción, listas desplegables o casillas de verificación) antes de él en el formulario.
Para obtener información sobre los campos y widgets personalizados en los formularios personalizados, consulte [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* No se puede agregar lógica de omisión a un widget o salto de sección. Solo puede agregarlo a un campo de opción múltiple (botones de opción, listas desplegables o casillas de verificación).
* Puede agregar lógica de visualización y lógica de omisión a un campo personalizado si se cumplen todas las condiciones siguientes en relación con el campo personalizado:

   * Es un campo de opción múltiple (botones de opción, listas desplegables o casillas de verificación)
   * Va precedido de un campo de opción múltiple
   * Va seguido de otro campo personalizado

* Al copiar formularios con lógica de visualización u lógica de omisión, la lógica se copia en el nuevo formulario personalizado.
* Al editar objetos de forma masiva, todos los campos personalizados se muestran en el cuadro Editar objetos, incluidos los campos omitidos u ocultos.
* Tenga en cuenta lo siguiente al crear una regla de lógica de visualización para un formulario personalizado:

   * De forma predeterminada, los campos personalizados no incluidos en una instrucción de lógica de visualización se muestran en un formulario personalizado.
   * Puede crear instrucciones de lógica de visualización de varios campos.
   * Si se les ha aplicado lógica de visualización a todos los campos debajo de un salto de sección y, como resultado de la lógica, todos ellos están ocultos, toda la sección estará oculta en el formulario personalizado.

## Agregar lógica de visualización a un formulario personalizado

La lógica de visualización define qué campos personalizados aparecen en el formulario cuando el usuario selecciona un valor específico en un campo de opción múltiple. La lógica se añade al campo de destino, que solo se muestra cuando se selecciona el valor.

{{step-1-to-setup}}

1. Clic **Forms personalizado**.
1. Cree un nuevo formulario personalizado o abra uno existente. Consulte [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) para obtener más información.
1. Agregue campos al formulario según sea necesario. Al menos un campo de opción múltiple (botón de opción, lista desplegable o casilla de verificación) debe colocarse antes del campo de destino que se va a mostrar.
1. Seleccione el campo de destino y haga clic en **Agregar lógica** en la parte inferior izquierda de la pantalla.
1. Seleccione el **Lógica de visualización** pestaña.
1. Clic **Agregar regla de visualización** en el generador de lógica.

   ![Mostrar generador de lógica](assets/custom-form-logic-builder-display-blank.png)

1. Siga los pasos siguientes en el generador para crear la instrucción lógica.

   1. La primera opción es elegir el campo de definición. Este es el campo con el valor de selección que muestra el objetivo. Debe ser un campo de opción múltiple.
   1. La segunda opción es elegir el valor de selección. Solo están disponibles los valores ya definidos para ese campo.
   1. La tercera opción es **Seleccionado** o **No seleccionado**. Elección **Seleccionado** significa que, cuando se selecciona el valor, se muestra el campo de destino. Elección **No seleccionado** significa que cuando se selecciona cualquier otro valor en el campo de definición, se muestra el campo de destino.
   1. Para agregar un **Y** a la sentencia lógica, haga clic en **Agregar regla** directamente debajo de la regla que acaba de crear. Siga las mismas indicaciones para crear la regla. Todas las reglas Y deben cumplirse para que se muestre el campo de destino.

      ![Mostrar generador de lógica](assets/custom-form-logic-builder-display1.png)

   1. Para agregar un **O** a la sentencia lógica, haga clic en **Agregar regla** cerca de la parte inferior del generador de lógica. A continuación, haga clic en **Agregar regla** dentro del área O y siga las mismas indicaciones para crear la regla. Cuando se cumple una regla O, se muestra el campo de destino.

1. Clic **Guardar** cuando haya terminado de crear la instrucción lógica.

   Los iconos de lógica de visualización se agregan al campo de destino y al campo de definición en el diseñador de formularios.

>[!NOTE]
>
>La lógica de visualización no está disponible temporalmente al obtener una vista previa del formulario en el diseñador de formularios.

## Agregar lógica de omisión a un formulario personalizado

La lógica de omisión define campos de formulario personalizados que se omiten cuando el usuario selecciona un valor específico en un campo de opción múltiple. Los campos omitidos están ocultos en el formulario. La lógica se aplica al campo de definición donde se realiza la selección, no a los campos que se omiten.

{{step-1-to-setup}}

1. Clic **Forms personalizado**.
1. Cree un nuevo formulario personalizado o abra uno existente. Consulte [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) para obtener más información.
1. Agregue campos al formulario según sea necesario. El campo de definición para la lógica de omisión debe ser un campo de selección múltiple (botón de opción, lista desplegable o casilla de verificación).
1. Seleccione el campo de definición y haga clic en **Agregar lógica** en la parte inferior izquierda de la pantalla.
1. Seleccione el **Omitir lógica** pestaña.
1. Clic **Agregar regla de omisión** en el generador de lógica.

   ![Omitir generador de lógica](assets/custom-form-logic-builder-skip-blank.png)

1. Siga los pasos siguientes en el generador para crear la instrucción lógica.

   1. El campo de definición se muestra en el generador. Es el campo seleccionado al que se aplica la lógica de omisión.
   1. La primera opción es elegir el valor de selección. Solo están disponibles los valores ya definidos para el campo.
   1. La segunda opción es **Seleccionado** o **No seleccionado**. Elección **Seleccionado** significa que, cuando se selecciona el valor, se muestra el campo de destino y se omiten los campos intermedios. Elección **No seleccionado** significa que cuando se selecciona cualquier otro valor en el campo de definición, se muestra el campo de destino y se omiten los campos intermedios.
   1. La tercera opción es el campo de destino o dónde ir. Seleccione un nombre de campo o **Fin de formulario**. Es posible que tenga que hacer clic primero en la palabra &quot;vacío&quot; antes de seleccionar una opción.

      ![Omitir generador de lógica](assets/custom-form-logic-builder-skip1.png)

   1. Para agregar un **O** a la sentencia lógica, haga clic en **Agregar regla** cerca de la parte inferior del generador de lógica. A continuación, seleccione las opciones siguiendo las mismas indicaciones para generar la regla. Cuando uno **O** Cuando se cumple la regla, se muestra el campo de destino.

1. Clic **Guardar** cuando haya terminado de crear la instrucción lógica.

   Los iconos de lógica de omisión se agregan al campo de destino y al campo de definición en el diseñador de formularios.

>[!NOTE]
>
>La lógica de omisión no está disponible temporalmente al obtener una vista previa del formulario en el diseñador de formularios.
