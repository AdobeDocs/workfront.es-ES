---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: Crear y editar reglas empresariales
description: Puede seleccionar si desea recibir las nuevas funciones de Workfront con periodicidad mensual o trimestral.
author: Lisa
feature: System Setup and Administration
role: Admin
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d96ddcc2f514d9f79e94a3437a3b66e07a270abc
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# Crear y editar reglas empresariales

Una regla de negocio permite aplicar la validación a objetos de Workfront e impedir que los usuarios creen, editen o eliminen un objeto cuando se cumplen determinadas condiciones. Las reglas empresariales ayudan a mejorar la calidad de los datos y la eficacia operativa mediante la prevención de acciones que podrían poner en peligro la integridad de los datos.

Una sola regla de negocio sólo se puede asignar a un objeto. Por ejemplo, si crea una regla de negocio para no editar proyectos en determinadas condiciones, no puede aplicar la misma regla a las tareas. Tendría que crear una regla de negocio independiente con las mismas condiciones para las tareas.

Los niveles de acceso y el uso compartido de objetos tienen una prioridad mayor que las reglas empresariales cuando un usuario interactúa con un objeto. Por ejemplo, si un usuario tiene un nivel de acceso o un permiso que no permite editar un proyecto, entonces esos permisos tendrían prioridad sobre una regla de negocio que permite editar un proyecto en ciertas condiciones.

También existe una jerarquía cuando se aplica más de una regla de negocio a un objeto. Por ejemplo, tiene dos reglas de negocio. Uno restringe la creación de gastos en el mes de febrero. La segunda impide editar un proyecto cuando el estado del proyecto es Completo. Si un usuario intenta agregar un gasto a un proyecto completado en junio, el gasto no se puede agregar porque ha activado la segunda regla.

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

Algunos escenarios de reglas de negocio simples son:

* Los usuarios no pueden agregar nuevos gastos durante la última semana de febrero. Esta fórmula puede expresarse de la siguiente manera: `IF(AND(MONTH($$TODAY) = 2, DAYOFMONTH($$TODAY) >= 22), "You cannot add new expenses during the last week of February.")`
* Los usuarios no pueden editar un proyecto que esté en estado completo. Esta fórmula puede expresarse de la siguiente manera: `IF({status} = "CPL", "You cannot edit this project because it is in Complete status.")`

La sintaxis para crear una regla de negocio es la misma que crear un campo calculado en un formulario personalizado. Para obtener más información sobre la sintaxis, consulte [Agregar campos calculados con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Para obtener información sobre las instrucciones IF, consulte [Información general sobre las instrucciones &quot;IF&quot;](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) y [Operadores de condición en campos personalizados calculados](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

Para obtener información sobre los comodines basados en usuarios, consulte [Utilice comodines basados en usuarios para generalizar informes](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Para obtener información sobre los comodines basados en fecha, consulte [Utilice comodines basados en fecha para generalizar informes](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

## Agregar nueva regla de negocio

{{step-1-to-setup}}

1. Clic **Reglas comerciales** en el panel izquierdo.
1. Clic **Nueva regla empresarial**.
1. Seleccione el tipo de objeto al que asignar la regla de negocio y haga clic en **Continuar**.

   ![Seleccionar un objeto](assets/object-for-business-rule2.png)

1. Escriba el **Nombre** para la regla de negocio.
1. En el **Está activo** , seleccione si la regla debe estar activa al guardarla.

   Si selecciona **No** Sin embargo, la regla se guarda como inactiva y puede activarla más adelante.

1. Seleccione una **Déclencheur** para la regla de negocio. Las opciones son:

   * **Al crear el objeto:** La regla se aplica cuando un usuario intenta crear un objeto.
   * **Al editar el objeto:** La regla se aplica cuando un usuario intenta editar un objeto.
   * **Al eliminar el objeto:** La regla se aplica cuando un usuario intenta eliminar un objeto.

1. (Opcional) Introduzca una **Descripción** de la regla de negocio y qué sucede cuando se aplica.
1. Cree la fórmula en el editor de fórmulas, en el centro del cuadro de diálogo de la regla de negocio.

   El formato de una regla de negocio es &quot;SI se cumple la condición definida, se impide al usuario realizar la acción en el objeto y se muestra el mensaje&quot;.

   En el área de fórmula, las partes de la regla de negocio que genere serán la condición y el mensaje que se mostrará en Workfront cuando se cumpla la condición.

   * El &quot;objeto&quot; es el tipo de objeto seleccionado al crear la regla de negocio. Se muestra en el encabezado del cuadro de diálogo.
   * La &quot;acción&quot; es el déclencheur seleccionado para la regla: crear, editar o borrar el objeto.
   * Como el objeto y la acción ya están definidos, no los incluye en la fórmula.
   * El mensaje de error personalizado se muestra al usuario cuando almacena en déclencheur la regla de negocio. Debe proporcionar instrucciones claras sobre qué ha fallado y cómo corregir el problema.

   ![Cuadro de diálogo Agregar regla de negocio](assets/add-business-rule-dialog-no-ai-button.png)

   Este ejemplo es una regla de negocio para gastos. Si el mes actual es junio, no se permite a los usuarios crear nuevos gastos y en el mensaje se explica esto.

   Para ver más ejemplos de reglas de negocio, consulte [Escenarios para reglas de negocio](#scenarios-for-business-rules) en este artículo.

1. (Opcional) Utilice la fórmula **Expresiones** y **Campos** en el panel derecho para ayudar a crear la regla.

   Busque una expresión o un campo para reducir la lista de elementos disponibles.

   La lista de campos disponibles se limita a los campos relacionados con el tipo de objeto de la regla de negocio.

1. Clic **Guardar** cuando haya terminado de crear la regla de negocio.

>[!NOTE]
>
>Después de agregar una regla de negocio, debe probarla agregando, editando o eliminando el objeto asociado para asegurarse de que la regla se aplica correctamente.

## Activar una regla de negocio

Cuando una regla de negocio está inactiva, el campo Está activo en la lista de reglas de negocio muestra Falso. No se puede actualizar el estado de la regla en la vista de lista.

Para activar una regla de negocio:

1. Seleccione la regla de negocio en la lista de reglas y haga clic en el icono Editar.
1. Seleccionar **Sí** para **Está activo** en el cuadro de diálogo regla de negocio.
1. Haga clic en **Guardar**.
