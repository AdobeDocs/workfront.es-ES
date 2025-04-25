---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Información general sobre agrupaciones en Adobe Workfront
description: Puede agregar agrupaciones para administrar el diseño de la información en los informes y las listas.
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 4%

---

# Información general sobre agrupaciones en Adobe Workfront

<!-- Audited: 11/2024 -->

<!--(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.)-->

Puede agregar agrupaciones para administrar el diseño de la información en los informes y las listas.

Puede agregar agrupaciones a informes de las siguientes maneras:

* Puede crear agrupaciones si edita las agrupaciones existentes.

  Para obtener información acerca de cómo personalizar una agrupación existente, vea [Editar agrupaciones existentes](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* Puede crear agrupaciones desde cero.

  Para obtener información sobre cómo crear una agrupación desde cero, consulte [Crear agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

De forma predeterminada, las agrupaciones se muestran en un resaltado gris en el informe o la lista. Los resultados del informe o la lista se enumeran en su grupo individual, sin resaltado.

![Ejemplo de agrupación](assets/grouping-example-blue.png)

Se pueden agregar hasta tres agrupaciones a un informe. Puede organizar la información con hasta cuatro agrupaciones creando un informe de matriz. Para obtener más información sobre los informes de matriz, consulte [Creación de un informe de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

El número entre paréntesis después del nombre de la agrupación representa el número de resultados bajo esa agrupación. Si el informe abarca varias páginas, asegúrese de mostrar *Todos* los resultados en el informe o lista para obtener un recuento preciso de los resultados en cada agrupación.

Tenga en cuenta lo siguiente al trabajar con agrupaciones:

* Puede personalizar la información en las agrupaciones existentes. Todos los usuarios que puedan ver las agrupaciones también podrán ver los cambios.
* El administrador de Workfront debe otorgarle acceso a Editar filtros, vistas y agrupaciones para crear agrupaciones.

  Para obtener información sobre cómo conceder acceso a filtros, vistas y agrupaciones, vea [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* El nivel de permisos para una agrupación dicta cómo se guarda una agrupación. Si creó la agrupación originalmente, puede guardar los cambios; de lo contrario, se le pedirá que guarde una versión de la agrupación. Si realiza cambios en una agrupación que ha compartido con otros, también les afectará.
* Puede personalizar una agrupación que se haya compartido con usted solo si el usuario que la ha compartido le ha concedido el acceso de Administración. Para obtener información acerca de cómo compartir una agrupación, vea [Compartir un filtro, una vista o una agrupación](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* No se puede editar una agrupación en línea.
* No se puede agrupar por campos personalizados de selección múltiple (por ejemplo, casillas de verificación) ni por campos que puedan tener varios valores (por ejemplo, Administrador de recursos).

## Información adicional sobre agrupaciones

También puede administrar la información del informe al usar Agrupaciones agregando los valores de cada columna en la fila Agrupación, así como ordenar la información por el campo de la Agrupación. También puede quitar una agrupación cuando ya no la necesite.

* [Valores agregados en agrupaciones](#aggregate-values-in-groupings)
* [Ordenar por una agrupación](#sort-by-a-grouping)
* [Quitar una agrupación](#remove-a-grouping)

### Valores agregados en agrupaciones {#aggregate-values-in-groupings}

Puede acumular los datos mostrados en el informe en la línea de agrupación resumiendo los valores en cada columna del informe. Para obtener más información sobre cómo resumir los datos de columna en una agrupación, consulte [Información general de vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).


>[!NOTE]
>
>Las siguientes excepciones se aplican a los objetos principales (por ejemplo, las tareas principales) cuando se agregan valores para los siguientes campos en >agrupaciones:
>
>* Todos los campos de número, moneda y fecha, excepto Horas reales, agregan valores solo para tareas secundarias y tareas independientes. No acumulan valores para tareas principales o principales de elementos principales. Al agregar campos de número, moneda y fecha en una lista que incluya sólo tareas principales, no se mostrará un valor agregado en la barra de agrupación.
>
>* Las horas reales acumulan valores para las tareas principales e independientes; no acumulan los números de las tareas secundarias o principales de las tareas principales. <!--Examples of Actual hours include Planned/Actual Labor Cost, Planned/Actual Expense Cost, Planned/Actual Cost, and Planned Hours.-->
>
>* Los campos de datos personalizados para valores numéricos y de moneda agregan todas las tareas: principales, secundarias, principales de principales y tareas independientes.


### Ordenar por una agrupación {#sort-by-a-grouping}

No se pueden ordenar las agrupaciones. Las vistas se pueden ordenar. Para ordenar una lista por el valor capturado en la agrupación, debe incluir el mismo valor en una de las columnas de la vista y aplicar el orden en la vista. De este modo, la lista se ordena indirectamente por el valor de la agrupación (se ordena por el valor de la vista que también se captura en la agrupación). Para obtener más información acerca de cómo crear vistas y ordenar por valores dentro de las vistas, vea [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Quitar una agrupación {#remove-a-grouping}

La forma de quitar una agrupación depende de si la creó inicialmente o de si la agrupación se compartió con usted. No se puede quitar una agrupación predeterminada.

* **Si ha creado la agrupación y la elimina**, la agrupación se eliminará del sistema de Workfront. La agrupación ya no está disponible para los usuarios con los que la haya compartido anteriormente.
* **Si la agrupación se compartió con usted y la elimina**, la agrupación se eliminará únicamente por usted. El usuario que lo creó originalmente y cualquier otro usuario con el que se haya compartido siguen teniendo acceso a la agrupación.

Para obtener información acerca de cómo quitar una agrupación, vea el artículo [Quitar filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).


<!--Original note

The following exceptions apply for parent objects (for example, parent tasks) when you are aggregating values for the following fields in groupings:
All the number and currency fields except Actual Hours (for example, Planned/ Actual Labor Cost, Planned/ Actual Expense Cost, Planned/ Actual Cost, Planned Hours) aggregate only the values for the children tasks, and standalone tasks. They do not aggregate the values for the parent tasks or parents of parents.
Actual Hours aggregate the values for the main parent and the standalone tasks; they do not aggregate the numbers for the parents of parent tasks or the children tasks.
Custom data fields for number and currency values aggregate all tasks: parents, children, parents of parents, and standalone tasks.

-->
