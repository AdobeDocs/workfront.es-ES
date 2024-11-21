---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: Crear y editar reglas de negocio
description: Una regla de negocio permite aplicar la validación a objetos de Workfront e impedir que los usuarios creen, editen o eliminen un objeto cuando se cumplen determinadas condiciones. Las reglas empresariales ayudan a mejorar la calidad de los datos y la eficacia operativa mediante la prevención de acciones que podrían poner en peligro la integridad de los datos.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 780c996c-5cf1-42fe-898d-2cc208bbae7b
source-git-commit: 5ebb756ba2f054c37d486d7f54a9f86cf8513328
workflow-type: tm+mt
source-wordcount: '1223'
ht-degree: 0%

---

# Crear y editar reglas empresariales

{{preview-fast-release-general}}

Una regla de negocio permite aplicar la validación a objetos de Workfront e impedir que los usuarios creen, editen o eliminen un objeto cuando se cumplen determinadas condiciones. Las reglas empresariales ayudan a mejorar la calidad de los datos y la eficacia operativa mediante la prevención de acciones que podrían poner en peligro la integridad de los datos.

Una sola regla de negocio sólo se puede asignar a un objeto. Por ejemplo, si crea una regla de negocio para no editar proyectos en determinadas condiciones, no puede aplicar la misma regla a las tareas. Tendría que crear una regla de negocio independiente con las mismas condiciones para las tareas.

Los niveles de acceso y el uso compartido de objetos tienen una prioridad mayor que las reglas empresariales cuando un usuario interactúa con un objeto. Por ejemplo, si un usuario tiene un nivel de acceso o un permiso que no permite editar un proyecto, entonces esos permisos tendrían prioridad sobre una regla de negocio que permite editar un proyecto en ciertas condiciones.

Cuando se aplica más de una regla de negocio a un objeto, las reglas se siguen todas, pero no se aplican en un orden determinado. Por ejemplo, tiene dos reglas de negocio. Uno restringe la creación de gastos en el mes de febrero. La segunda impide editar un proyecto cuando el estado del proyecto es Completo. Si un usuario intenta agregar un gasto a un proyecto completado en junio, el gasto no se puede agregar porque ha activado la segunda regla.

Las reglas empresariales se aplican a la creación, edición y eliminación de objetos a través de la API y en la interfaz de Workfront.

>[!NOTE]
>
>Como las reglas de negocio bloquean determinadas acciones, siempre debe configurar primero las reglas de negocio en un entorno de zona protegida o de vista previa y probarlas a fondo antes de habilitarlas en producción.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>plan de Adobe Workfront</td> 
   <td>Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>Estándar</td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Administrador del sistema</td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Escenarios para reglas de negocio

El formato de una regla de negocio es &quot;SI se cumple la condición definida, se impide al usuario realizar la acción en el objeto y se muestra el mensaje&quot;.

La sintaxis de las propiedades y otras funciones de una regla de negocio es la misma que la sintaxis de un campo calculado en un formulario personalizado. Para obtener más información sobre la sintaxis, vea [Agregar campos calculados con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Para obtener información acerca de las instrucciones IF, vea [&quot;IF&quot; instrucciones overview](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) y [Operadores de condición en los campos personalizados calculados](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

Para obtener información acerca de los comodines basados en usuarios, vea [Usar comodines basados en usuarios para generalizar informes](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Para obtener información acerca de los comodines basados en fecha, vea [Usar comodines basados en fecha para generalizar informes](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

También hay un comodín de API disponible en las reglas empresariales. Puede usar `$$ISAPI` para almacenar la regla en déclencheur solamente en la interfaz de usuario o solamente en la API.

Los caracteres comodín `$$BEFORE_STATE` y `$$AFTER_STATE` se utilizan en expresiones para acceder a los valores de campo del objeto antes y después de cualquier edición.

* Estos caracteres comodín están disponibles para el déclencheur de edición. El estado predeterminado para el déclencheur de edición (si no hay ningún estado incluido en la expresión) es `$$AFTER_STATE`.
* El déclencheur de creación de objetos solo permite `$$AFTER_STATE`, ya que el estado antes no existe.
* El déclencheur de eliminación de objetos solo permite `$$BEFORE_STATE`, ya que el estado después no existe.

Algunos escenarios de reglas de negocio simples son:

* Los usuarios no pueden agregar nuevos gastos durante la última semana de febrero. Esta fórmula se puede establecer como: `IF(MONTH($$TODAY) = 2 && DAYOFMONTH($$TODAY) >= 22, "You cannot add new expenses during the last week of February.")`
* Los usuarios no pueden editar el nombre de proyecto de un proyecto en estado completo. Esta fórmula se puede establecer como: `IF({status} = "CPL" && {name} != $$BEFORE_STATE.{name}, "You cannot edit the project name.")`

Un escenario con instrucciones IF anidadas es:

Los usuarios no pueden editar los proyectos completados y no pueden editar los proyectos con una fecha planificada de finalización en marzo. Esta fórmula puede expresarse de la siguiente manera:

```
IF(
    $$AFTER_STATE.{status}="CPL",
    "You cannot edit a completed project",
    IF(
        MONTH({plannedCompletionDate})=3,
        "You cannot edit a project with a planned completion date in March")
)
```

## Agregar nueva regla de negocio

{{step-1-to-setup}}

1. Haga clic en **Reglas de negocio** en el panel izquierdo.
1. Haga clic en **Nueva regla de negocio**.
1. Seleccione el tipo de objeto al que asignar la regla de negocio y haga clic en **Continuar**.

   ![Seleccionar un objeto](assets/object-for-business-rule2.png)

1. Escriba **Name** para la regla de negocio.
1. En el campo **Está activo**, seleccione si la regla debe estar activa al guardarla.

   Si selecciona **No**, la regla se guardará como inactiva y podrá activarla más tarde.

1. Seleccione un **Déclencheur** para la regla de negocio. Las opciones son:

   * **Al crear un objeto:** La regla se aplica cuando un usuario intenta crear un objeto.
   * **Al editar un objeto:** La regla se aplica cuando un usuario intenta editar un objeto.
   * **Al eliminar un objeto:** La regla se aplica cuando un usuario intenta eliminar un objeto.

1. (Opcional) Escriba una **Descripción** de la regla de negocio y qué sucede cuando se aplica.
1. Cree la fórmula en el editor de fórmulas, en el centro del cuadro de diálogo de la regla de negocio.

   El formato de una regla de negocio es &quot;SI se cumple la condición definida, se impide al usuario realizar la acción en el objeto y se muestra el mensaje&quot;.

   En el área de fórmula, las partes de la regla de negocio que genere serán la condición y el mensaje que se mostrará en Workfront cuando se cumpla la condición.

   * El &quot;objeto&quot; es el tipo de objeto seleccionado al crear la regla de negocio. Se muestra en el encabezado del cuadro de diálogo.
   * La &quot;acción&quot; es el déclencheur seleccionado para la regla: crear, editar o borrar el objeto.
   * Como el objeto y la acción ya están definidos, no los incluye en la fórmula.
   * El mensaje de error personalizado se muestra al usuario cuando almacena en déclencheur la regla de negocio. Debe proporcionar instrucciones claras sobre qué ha fallado y cómo corregir el problema.

     <span class="preview">Puede incluir una dirección URL estática en el mensaje de error para vincular a la documentación u otras páginas útiles y guiar al usuario sobre cómo modificar su acción dentro de la restricción de la regla.</span>

     <span class="preview">En este ejemplo, &quot;Más información&quot; se vinculará a la dirección URL. `"You are not allowed to add a new project in November.[Learn more](http://url)"`: la dirección URL debe estar entre paréntesis, pero no se requiere el texto entre corchetes para los vínculos. Puede mostrar la dirección URL completa, que será un vínculo en el que se podrá hacer clic.</span>

   ![Agregar cuadro de diálogo de regla de negocio](assets/add-business-rule-dialog-no-ai-button.png)

   Este ejemplo es una regla de negocio para proyectos. Si el mes actual es noviembre, no se permite a los usuarios crear nuevos proyectos y en el mensaje se explica esto.

   Para obtener más ejemplos de reglas de negocio, consulte [Escenarios para reglas de negocio](#scenarios-for-business-rules) en este artículo.

1. (Opcional) Use la fórmula **Expresiones** y **Campos** en el panel derecho para ayudar a crear la regla.

   Busque una expresión o un campo para reducir la lista de elementos disponibles.

   La lista de campos disponibles se limita a los campos relacionados con el tipo de objeto de la regla de negocio.

1. Haga clic en **Guardar** cuando termine de crear la regla de negocio.

>[!NOTE]
>
>Después de agregar una regla de negocio, debe probarla agregando, editando o eliminando el objeto asociado para asegurarse de que la regla se aplica correctamente.

## Activar una regla de negocio

Cuando una regla de negocio está inactiva, el campo Está activo en la lista de reglas de negocio muestra Falso. No se puede actualizar el estado de la regla en la vista de lista.

Para activar una regla de negocio:

1. Seleccione la regla de negocio en la lista de reglas y haga clic en el icono Editar.
1. Seleccione **Yes** para **Is Active** en el cuadro de diálogo de regla de negocio.
1. Haga clic en **Guardar**.
