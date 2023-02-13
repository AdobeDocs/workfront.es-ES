---
title: Mejoras en los formularios personalizados
description: En la versión 2.2 se realizaron las siguientes mejoras significativas para administrar formularios personalizados.
author: Luke
exl-id: 81568eab-8a65-4767-b8ab-fb9353a90bb6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Mejoras en los formularios personalizados

En la versión 2.2 se realizaron las siguientes mejoras significativas para administrar formularios personalizados.

## Agregar widgets de recursos

Puede incrustar una imagen en los formularios personalizados. Esto le permite comunicarse con los usuarios de formularios personalizados de forma más interactiva y visual. Próximamente habrá más tipos de utilidades.

![](assets/image-in-custom-form.png)

Cuando un formulario personalizado que contiene un widget está adjunto a un objeto, los usuarios que trabajan con él pueden verlo en las siguientes áreas:

* El área Detalles del objeto (por ejemplo, para un proyecto, el área Detalles del proyecto) &#x200B;

   ![](assets/see-image-details-page.png)

* El cuadro Editar del objeto, si tiene el nuevo aspecto y presentación de la experiencia de Adobe Workfront (por ejemplo, los cuadros Editar proyecto y Editar tarea) &#x200B;

   ![](assets/image-see-in-edit.png)

Actualmente, los usuarios no pueden ver el widget en las siguientes áreas: &#x200B;

* Listas e informes
* Inicio y resumen
* El cuadro Editar del objeto, si no tiene el aspecto y la presentación de la nueva experiencia de Adobe Workfront (por ejemplo, el cuadro Editar gasto)
* &#x200B; de la aplicación móvil de Workfront

Para obtener más información sobre cómo agregar widgets a formularios personalizados, consulte [Agregar o editar una imagen u otro widget de recursos en un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Asociación de un formulario personalizado a varios tipos de objetos

Puede asociar varios tipos de objetos con cualquier nuevo formulario personalizado:

![](assets/new-custom-form-object-types.png)

O cualquier formulario personalizado existente:

![](assets/add-object-type-existing-form.png)

Esto le permite crear un único formulario personalizado para utilizarlo en proyectos, tareas, problemas y cualquier otro tipo de objetos compatibles con los formularios personalizados.

Esto resulta especialmente útil cuando se convierte un problema o una tarea, ya que se puede transferir un formulario personalizado y sus datos al objeto convertido. Ya no es necesario crear y mantener copias exactas del mismo formulario personalizado para varios tipos de objetos, agregue el formulario personalizado al proyecto manualmente.

>[!INFO]
>
>**Ejemplo:**
>
>Alguien envía una solicitud de TI interna (problema) y proporciona detalles sobre lo que se necesita en un formulario personalizado adjunto.
>
>El problema se convierte en un proyecto para los usuarios que trabajan en él.
>
>Dado que el formulario personalizado que contiene los detalles del remitente está asociado con los tipos de objeto Problema y Proyecto , el formulario personalizado y todos esos detalles se transfieren al proyecto durante la conversión.

>[!NOTE]
>
>Cuando se produce la conversión, el formulario personalizado ya debe estar asociado al tipo de objeto al que se está convirtiendo.

Para obtener instrucciones sobre cómo agregar un widget de recursos a un formulario personalizado, consulte [Agregar o editar una imagen u otro widget de recursos en un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

Tenga en cuenta lo siguiente cuando cree o edite un formulario personalizado con varios objetos:

* [Opciones de permiso para saltos de sección](#permission-options-for-section-breaks)
* [Compatibilidad calculada de campos personalizados](#calculated-custom-field-compatibility)
* [Precaución sobre la eliminación de un tipo de objeto de un formulario personalizado](#caution-about-deleting-an-object-type-from-a-custom-form)

### Opciones de permiso para saltos de sección

El conjunto de opciones de permiso de salto de sección disponibles para los tipos de objeto Problema, Tarea, Proyecto y Usuario tiene una opción de permiso más que el conjunto de opciones de permiso para todos los demás tipos de objeto: Edición limitada.

![](assets/section-break-permissions-limited-edit.png)

El conjunto de permisos de salto de sección disponibles para todos los demás tipos de objetos (Portfolio, documento, programa, gastos, empresa, iteración, registro de facturación y grupo) no incluye Edición limitada:

![](assets/section-break-permissions-no-limited-edit.png)

En un formulario personalizado asociado con tipos de objeto de ambos grupos, el sistema utiliza un conjunto común de permisos de salto de sección que funcionan para todos los tipos de objeto. En concreto, en lugar de utilizar la opción de permiso Editar limitada , este conjunto común sustituye la opción de permiso Editar limitada por la opción de permiso Editar limitada . La opción Editar es compatible con todos los tipos de objetos.

Cuando se asocia un tipo de objeto que utiliza diferentes opciones de permiso que los demás tipos de objeto que ya se encuentran en un formulario personalizado, se muestra un mensaje que le permite cambiar al conjunto común de opciones de permiso que se utilizará para el formulario. Este cambio se aplicará a todos los campos, incluso si no están en un salto de sección.

Para obtener más información, consulte [Agregar un salto de sección a un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).

### Compatibilidad calculada de campos personalizados

En un formulario personalizado de varios objetos, si un campo calculado hace referencia a campos que están disponibles para su uso con todos los tipos de objeto asociados al formulario (como {name}, {description} y {entryDate}, que están disponibles para varios tipos de objeto), los datos se calculan correctamente, independientemente del objeto al que se adjunte.

Por ejemplo, si tiene un formulario de varios objetos para proyectos y problemas y agrega un campo calculado que contiene la expresión {nombre}, el campo muestra el nombre del proyecto cuando agrega el formulario a un proyecto y el nombre de la tarea que agrega al formulario a una tarea.

Sin embargo, si un campo calculado del formulario hace referencia a un campo que no es compatible con todos los tipos de objeto del formulario, un mensaje le alerta para que realice ajustes.

>[!INFO]
>
>**Ejemplo:** En un formulario personalizado asociado al tipo de objeto Task , se crea un campo personalizado calculado que hace referencia al campo integrado Assigned To: Nombre para que pueda mostrar el nombre del usuario asignado principal a cargo cada vez que el formulario esté adjunto a una tarea:
>
>
```
>Assigned To: Name{assignedTo}.{name}
>```
>
>Posteriormente, se agrega el tipo de objeto Project al formulario personalizado. Un mensaje de advertencia indica que el tipo de objeto Project es incompatible con el campo personalizado calculado. Esto se debe a que el campo Asignado a no está disponible para proyectos.

Cuando esto sucede, puede realizar una de las siguientes acciones:

* Elimine uno de los dos elementos incompatibles del formulario personalizado: el tipo de objeto o el campo al que se hace referencia.
* Mantener ambos elementos y utilizar la variable de filtro comodín `$$OBJCODE` como condición en una expresión IF para crear dos versiones diferentes del campo In Charge . Esto permite que el campo funcione correctamente, independientemente del tipo de objeto al que esté adjunto el formulario.

   Con el ejemplo anterior, aunque no hay ningún elemento integrado asignado a: Campo Nombre para proyectos, hay un campo Propietario integrado (que se rellena automáticamente con el nombre de la persona que creó el proyecto, a menos que alguien lo cambie manualmente). Por lo tanto, en el campo personalizado A cargo, puede usar `$$OBJCODE` como se muestra a continuación para hacer referencia al campo Propietario cuando el formulario personalizado está adjunto a un proyecto y Assigned To: Campo Nombre cuando el formulario está adjunto a una tarea:

   ```
   IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})
   ```

>[!NOTE]
>
>  Si agrega un tipo de objeto delante de un nombre de campo, hace referencia al objeto principal del objeto, por lo que no puede utilizar `{project}.{name}` con un proyecto, pero puede utilizarlo con una tarea.

Para obtener instrucciones sobre cómo agregar un campo personalizado calculado a un formulario personalizado, consulte [Agregar datos calculados a un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Para obtener más información sobre variables como `$$OBJCODE`, consulte [Variables de filtro comodín](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

### Precaución sobre la eliminación de un tipo de objeto de un formulario personalizado

Puede eliminar un tipo de objeto en un formulario personalizado en cualquier momento, pero esto debe hacerse con precaución. Si los usuarios ya han adjuntado el formulario personalizado a objetos del tipo que desea eliminar y le han agregado datos, esos datos se eliminarán de forma permanente cuando elimine ese tipo de objeto en el formulario.

Además, no hay ningún sistema de notificación para avisar a las personas que usan el formulario personalizado de que se eliminó.

Para obtener más información, consulte [Eliminar un campo o widget personalizado del sistema](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
