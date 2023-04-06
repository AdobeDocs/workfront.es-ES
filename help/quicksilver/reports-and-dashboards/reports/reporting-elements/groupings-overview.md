---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Información general sobre las agrupaciones en Adobe Workfront
description: Puede agregar agrupaciones para administrar el diseño de la información en los informes y listas.
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Información general sobre las agrupaciones en Adobe Workfront

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.) </p>
-->

Puede agregar agrupaciones para administrar el diseño de la información en los informes y listas.

Puede agregar agrupaciones a informes de las siguientes maneras:

* Puede crear agrupaciones editando las agrupaciones existentes.

   Para obtener información sobre la personalización de un grupo existente, consulte [Editar agrupaciones existentes](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* Puede crear agrupaciones desde cero.

   Para obtener información sobre cómo crear una agrupación desde cero, consulte [Crear agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

De forma predeterminada, las agrupaciones se muestran en un resaltado gris o azul en el informe o la lista. Los resultados del informe o la lista se enumeran en su agrupación individual, sin ningún énfasis.

Se pueden agregar hasta tres agrupaciones a un informe. Puede organizar la información con hasta cuatro agrupaciones creando un informe de matriz. Para obtener más información sobre los informes de matriz, consulte [Crear un informe de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

En un informe de agrupación estándar, la primera agrupación es de color más oscuro, la segunda y la tercera agrupación son más claras. No se puede personalizar el color del resaltado para la agrupación ni la fuente del nombre de la agrupación. El número que aparece entre paréntesis después del nombre de la agrupación representa el número de resultados de dicha agrupación. Si el informe abarca varias páginas, asegúrese de que se muestra *Todo* los resultados del informe o la lista para obtener un recuento preciso de los resultados en cada agrupación.

![Agrupación de muestras](assets/grouping-example-blue.png)

Tenga en cuenta lo siguiente cuando trabaje con agrupaciones:

* Puede personalizar la información en agrupaciones existentes. Todos los usuarios que pueden ver las agrupaciones también pueden ver sus cambios.
* El administrador de Workfront debe permitirle acceder a Editar filtros, vistas y grupos para crear agrupaciones.

   Para obtener información sobre la concesión de acceso a filtros, vistas y grupos, consulte [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* El nivel de permisos de una agrupación dicta cómo se guarda dicha agrupación. Si creó la agrupación originalmente, puede guardar los cambios; de lo contrario, se le pedirá que guarde una versión de la agrupación. Si realiza cambios en una agrupación que ha compartido con otras personas, también los afectará.
* Puede personalizar una agrupación que se compartió con usted solo si el usuario que la compartió le concedió acceso de Administrar. Para obtener información sobre cómo compartir una agrupación, consulte [Compartir un filtro, una vista o una agrupación](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* No se puede editar una agrupación en línea.
* No se puede agrupar por campos personalizados de selección múltiple (por ejemplo, casillas de verificación) ni por campos que puedan tener varios valores (por ejemplo, el Administrador de recursos).

## Información adicional sobre agrupaciones

Puede administrar aún más la información del informe al utilizar Groupings añadiendo los valores de cada columna en la fila Grouping , así como ordenar la información por el campo de su Grouping. También puede quitar un grupo cuando ya no lo necesite.

* [Agregar valores en agrupaciones](#aggregate-values-in-groupings)
* [Ordenar por una agrupación](#sort-by-a-grouping)
* [Eliminación de una agrupación](#remove-a-grouping)

### Agregar valores en agrupaciones {#aggregate-values-in-groupings}

Puede acumular los datos mostrados en el informe en la línea de agrupación resumiendo los valores de cada columna del informe. Para obtener más información sobre cómo resumir los datos de columnas en una agrupación, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>Las siguientes excepciones se aplican a los objetos principales (por ejemplo, tareas principales) cuando se agregan valores para los siguientes campos en agrupaciones:
>
>* Todos los campos de número y moneda excepto Horario real (por ejemplo, Coste laboral planeado/real, Coste planeado/real, Coste planeado/real, Horario planificado) agregan solamente los valores para las tareas secundarias y las tareas independientes. No acumulan los valores para las tareas principales o los principales de los padres.
>* Las horas reales agregan los valores para las tareas principales y las tareas independientes; no agregan los números para los elementos principales de las tareas principales o las tareas secundarias.
>* Los campos de datos personalizados para valores numéricos y monetarios agregan todas las tareas: padres, hijos, padres de padres y tareas independientes.


### Ordenar por una agrupación {#sort-by-a-grouping}

Los agrupamientos no se pueden ordenar. Las vistas se pueden ordenar. Para ordenar una lista por el valor capturado en la agrupación, debe incluir ese mismo valor en una de las columnas de la vista y aplicar la ordenación en la vista. De este modo, la lista se ordena indirectamente por el valor de la agrupación (se ordena por el valor de la vista que también se captura en la agrupación). Para obtener más información sobre cómo crear vistas y ordenar por valores dentro de las vistas, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Eliminación de una agrupación {#remove-a-grouping}

La forma de eliminar una agrupación depende de si creó la agrupación inicialmente o si se compartió con usted. No se puede quitar una agrupación predeterminada.

* **Si ha creado la agrupación y la ha eliminado**, la agrupación se elimina del sistema de Workfront. La agrupación ya no está disponible para ningún usuario con el que la haya compartido anteriormente.
* **Si la agrupación se compartió con usted y la elimina**, la agrupación se elimina únicamente por usted. El usuario que lo creó originalmente y cualquier otro usuario con el que se haya compartido siguen teniendo acceso a la agrupación.

Para obtener información sobre cómo quitar una agrupación, consulte el artículo [Eliminación de filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
