---
title: Mejoras de formularios personalizados
description: A continuación, se llevan a cabo mejoras significativas para administrar formularios personalizados en la versión 22.2.
author: Luke
feature: Product Announcements, Custom Forms
exl-id: 81568eab-8a65-4767-b8ab-fb9353a90bb6
source-git-commit: 8dac7959919014d7bfbbbd39d193d026ca31c4b2
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---

# Mejoras de formularios personalizados

A continuación, se llevan a cabo mejoras significativas para administrar formularios personalizados en la versión 22.2.

## Añadir widgets de recursos

Puede incrustar imágenes en los formularios personalizados. Esto le permite comunicarse con los usuarios de formularios personalizados de una manera más interactiva y visual. Próximamente habrá más tipos de widgets.

![](assets/image-in-custom-form.png)

Cuando se adjunta un formulario personalizado que contiene un widget a un objeto, los usuarios que trabajen con él podrán verlo en las siguientes áreas:

* El área Detalles del objeto (por ejemplo, para un proyecto, el área Detalles del proyecto)&#x200B;

  ![](assets/see-image-details-page.png)

* El cuadro Editar del objeto, si tiene el nuevo aspecto y funcionamiento de la experiencia Adobe Workfront (por ejemplo, los cuadros Editar proyecto y Editar tarea)&#x200B;

  ![](assets/image-see-in-edit.png)

Actualmente, los usuarios no pueden ver el widget en las siguientes áreas:&#x200B;

* Listas e informes
* Inicio y resumen
* El cuadro de edición del objeto, si no tiene el nuevo aspecto y funcionamiento de la experiencia de Adobe Workfront (por ejemplo, el cuadro de edición de gastos )
* &#x200B;La aplicación móvil de Workfront

## Asociar un formulario personalizado con varios tipos de objetos

Puede asociar varios tipos de objetos con cualquier formulario personalizado nuevo:

![](assets/new-custom-form-object-types.png)

O cualquier formulario personalizado existente:

![](assets/add-object-type-existing-form.png)

Esto le permite crear un único formulario personalizado para utilizarlo en proyectos, tareas, problemas y cualquier otro tipo de objetos compatibles con los formularios personalizados.

Esto resulta especialmente útil cuando se convierte un problema o una tarea, ya que puede transferir un formulario personalizado y sus datos al objeto convertido. Ya no es necesario crear y mantener copias exactas del mismo formulario personalizado para varios tipos de objetos; agregue el formulario personalizado al proyecto manualmente.

>[!INFO]
>
>**Ejemplo:**
>
>Alguien envía una solicitud de TI interna (problema) y proporciona detalles sobre lo que se necesita en un formulario personalizado adjunto.
>
>Convierte el problema en un proyecto para los usuarios que trabajarán en él.
>
>Dado que el formulario personalizado que contiene los detalles del remitente está asociado a los tipos de objeto Problema y Proyecto, el formulario personalizado y todos esos detalles se transfieren al proyecto durante la conversión.

>[!NOTE]
>
>Cuando se realice la conversión, el formulario personalizado ya debe estar asociado al tipo de objeto al que está convirtiendo.

Tenga en cuenta lo siguiente al crear o editar un formulario personalizado de varios objetos:

* [Opciones de permiso para saltos de sección](#permission-options-for-section-breaks)
* [Compatibilidad calculada con campos personalizados](#calculated-custom-field-compatibility)
* [Precaución al eliminar un tipo de objeto de un formulario personalizado](#caution-about-deleting-an-object-type-from-a-custom-form)

### Opciones de permiso para saltos de sección

El conjunto de opciones de permiso de salto de sección disponibles para los tipos de objeto Problema, Tarea, Proyecto y Usuario tiene una opción de permiso más que el conjunto de opciones de permiso para todos los demás tipos de objeto: Edición limitada.

![](assets/section-break-permissions-limited-edit.png)

El conjunto de permisos de salto de sección disponible para todos los demás tipos de objetos (Portfolio, documento, programa, gasto, compañía, iteración, registro de facturación y grupo) no incluye Edición limitada:

![](assets/section-break-permissions-no-limited-edit.png)

En un formulario personalizado asociado a tipos de objeto de ambos grupos, el sistema utiliza un conjunto común de permisos de salto de sección que funcionan para todos los tipos de objeto. En particular, en lugar de utilizar la opción de permiso Editar de forma limitada, este conjunto común sustituye la opción de permiso Editar por la opción de permiso Editar de forma limitada. La opción Editar es compatible con todos los tipos de objetos.

Cuando se asocia un tipo de objeto que utiliza opciones de permiso distintas de las de otros tipos de objeto que ya se encuentran en un formulario personalizado, aparece un mensaje que le permite cambiar al conjunto común de opciones de permiso que se utilizarán para el formulario. Este cambio se aplicará a todos los campos, incluso si no están en un salto de sección.

### Compatibilidad calculada con campos personalizados

En un formulario personalizado de varios objetos, si un campo calculado hace referencia a campos que están disponibles para su uso con todos los tipos de objetos asociados al formulario (como {name}, {description} y {entryDate}, que están disponibles para varios tipos de objetos), los datos se calculan correctamente, independientemente del objeto al que se adjunten.

Por ejemplo, si tiene un formulario de varios objetos para proyectos y problemas y agrega un campo calculado que contiene la expresión {name}, el campo mostrará el nombre del proyecto cuando agregue el formulario a un proyecto y el nombre de la tarea cuando agregue el formulario a una tarea.

Los campos no compatibles con el objeto mostrarán N/D en el formulario.

>[!INFO]
>
>**Ejemplo:** En un formulario personalizado asociado al tipo de objeto Task, crea un campo personalizado calculado que hace referencia al campo integrado Asignado a: Name para que pueda mostrar el nombre del usuario asignado principal a cargo siempre que el formulario esté adjunto a una tarea:
>
>```
>Assigned To: Name{assignedTo}.{name}
>```
>
>Posteriormente, se agrega el tipo de objeto Project al formulario personalizado. Un mensaje de advertencia le indica que el tipo de objeto Project no es compatible con el campo personalizado calculado. Esto se debe a que el campo Asignado a no está disponible para proyectos.

Cuando esto sucede, puede realizar una de las siguientes acciones:

* Quite uno de los dos elementos incompatibles del formulario personalizado: el tipo de objeto o el campo al que se hace referencia.
* Mantenga ambos elementos y utilice la variable de filtro comodín `$$OBJCODE` como condición en una expresión IF para crear dos versiones diferentes del campo In Charge. Esto permite que el campo funcione correctamente, independientemente del tipo de objeto al que esté adjunto el formulario.

  En el ejemplo anterior, aunque no hay un campo integrado Asignado a: Nombre para los proyectos, hay un campo Propietario integrado (que se rellena automáticamente con el nombre de la persona que creó el proyecto, a menos que alguien cambie esto manualmente). Por lo tanto, en su campo personalizado A cargo, puede utilizar `$$OBJCODE` como se muestra a continuación para hacer referencia al campo Propietario cuando el formulario personalizado se adjunta a un proyecto y al campo Asignado a: Nombre cuando el formulario se adjunta a una tarea:

  ```
  IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})
  ```

>[!NOTE]
>
>  Si agrega un tipo de objeto delante del nombre de campo, hace referencia al objeto principal del objeto, por lo que no puede utilizar `{project}.{name}` con un proyecto, pero puede utilizarlo con una tarea.


Para obtener más información acerca de variables como `$$OBJCODE`, vea [Resumen de las variables de filtro comodín](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

### Precaución al eliminar un tipo de objeto de un formulario personalizado

Puede eliminar un tipo de objeto en un formulario personalizado en cualquier momento, pero esto debe hacerse con precaución. Si los usuarios ya han adjuntado el formulario personalizado a objetos del tipo que desea eliminar y le han agregado datos, esos datos se eliminan de forma permanente al eliminar ese tipo de objeto en el formulario.

Además, no hay ningún sistema de notificación que avise a las personas que utilizan el formulario personalizado de que se ha eliminado.

Para obtener más información, consulte [Eliminar un campo o widget personalizado del sistema](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
