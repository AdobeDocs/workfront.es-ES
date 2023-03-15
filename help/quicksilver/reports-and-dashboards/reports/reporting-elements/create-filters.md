---
product-area: reporting
navigation-topic: reporting-elements
title: Crear o editar filtros en Adobe Workfront
description: Puede limitar la cantidad de información que muestra en la pantalla en una lista de elementos con un filtro. Puede definir ciertos criterios basados en información concreta sobre un objeto y mostrar únicamente los objetos que cumplan esos criterios.
author: Lisa
feature: Reports and Dashboards
exl-id: 2e912e32-7924-418d-9d55-ce3c09f67d3e
source-git-commit: b56e6591c7da166bd1548420b562b838cc7fe0f2
workflow-type: tm+mt
source-wordcount: '2513'
ht-degree: 1%

---

# Crear o editar filtros en Adobe Workfront

<span class="preview">Tenga en cuenta que en el entorno de Vista previa, la experiencia de filtro mejorada (anteriormente denominada &quot;beta&quot;) es ahora la predeterminada. Estos filtros mejorados ahora son &quot;estándar&quot; y la experiencia de filtrado anterior es &quot;heredada&quot;.</span>

Puede limitar la cantidad de información que muestra en la pantalla en una lista de elementos con un filtro. Puede definir ciertos criterios basados en información concreta sobre un objeto y mostrar únicamente los objetos que cumplan esos criterios.

Puede aplicar los siguientes tipos de filtros en Adobe Workfront:

* Filtros rápidos en una lista de objetos para buscar un elemento mediante una palabra clave. Son filtros temporales que no se pueden guardar para uso futuro.

   Para obtener información sobre los filtros rápidos, consulte [Aplicar el filtro rápido a una lista](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

* Filtros permanentes que se pueden guardar y usar durante mucho tiempo en varias listas e informes. Este artículo describe cómo crear un filtro permanente o editar uno existente en una lista o informe.

* Filtros en otras áreas de Workfront, fuera de listas e informes.

   Para obtener una lista de todos los filtros de Workfront y las áreas en las que puede aplicarlos, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a filtros, vistas y agrupamientos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Administrar permisos en un filtro</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Tipos de interfaces de generación de filtros

Puede crear filtros utilizando los tipos de generadores de filtros que se describen en la tabla siguiente:

<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Tipo de generador</strong></td>
<td><strong>Objeto Filter</strong></td>
<td><strong>Donde esté disponible</strong></td>
</tr>
<tr>
<td>Generador estándar</td>
<td>Todos los objetos </td>
<td>Listas e informes</td>
</tr>
<tr>
<td>Creador beta</td>
<td>
<ul>
<li> <p>Proyectos</p> </li>
<li> <p>Tareas </p> </li>
<li> <p>Problemas</p> </li>
<li> <p>Portafolios</p> </li>
<li> <p>Programas</p> </li>
<li> <p>Usuarios</p> </li>
<li> <p>Plantillas</p> </li>
<li> <p>Grupos</p> </li>
</ul>
</td>
<td>
<ul>
<li> <p>Listas </p> </li>
</ul>
<ul>
<li> <p>La lista Proyectos del planificador de escenarios</p> <p>El planificador de escenarios requiere una licencia adicional. Para obtener información sobre el planificador de escenarios de Workfront, consulte <a href="../../../scenario-planner/scenario-planner-overview.md">Información general del planificador de escenarios</a>. </p> </li>
</ul>
<p>NOTA: Los creadores beta para filtros no están disponibles en los informes.
</td>
</tr>
</tbody>
</table>

Para obtener información sobre los objetos de Workfront, consulte [Explicación de los objetos en Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Crear o editar un filtro en el generador estándar {#create-filter-in-standard-builder}

Puede crear filtros en listas e informes de las siguientes maneras:

* Desde cero
* Editar un filtro existente y guardarlo como un filtro nuevo

Independientemente del método que utilice para crear filtros, la creación de un filtro desde cero o desde un filtro existente es similar.

1. Vaya a una lista o a un informe que contenga el filtro que desea personalizar.
1. Haga clic en el **Filtro** icono ![Icono de filtro](assets/filter-nwepng.png).

   >[!TIP]
   >
   >El creador del informe debe permitir que se editen los filtros para poder ver la lista desplegable Filtro en un informe. El filtro Predeterminado de informe se aplica a un informe de forma predeterminada. El filtro Predeterminado de informe solo se puede personalizar al editar el informe.

   ![Menú desplegable Filtro](assets/filter-drop-down-expanded-nwe.png)

1. Haga clic en **Nuevo filtro** en la parte superior de la lista de filtros

   O

   Pase el ratón sobre el filtro que desea modificar y haga clic en el botón **Editar** icono ![](assets/edit-icon.png).

   Se inicia el generador para personalizar el filtro.

1. Realice una de las siguientes acciones:

   * Modifique las reglas de filtro existentes haciendo clic en la regla existente y seleccionando una nueva opción.
   * Agregue una regla de filtro haciendo clic en **Añadir otra regla de filtro**, empiece a escribir el nombre de la opción para la que desea agregar una regla en la **Empezar a escribir el nombre del campo** y haga clic en él cuando aparezca en la lista desplegable.

      Los campos asociados al objeto del filtro se enumeran en la **Empezar a escribir el nombre del campo** en la ventana

   * Haga clic en **Y** o **O** al agregar una regla de filtro nueva.\
      Al agregar reglas de filtro, utilice los modificadores de filtro para establecer la condición del filtro. Para obtener más información sobre los modificadores de filtro, consulte [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

      >[!NOTE]
      >
      >Cuando conecte un grupo de instrucciones AND mediante varias instrucciones OR, debe repetir los campos que no están cambiando entre las instrucciones OR para cada grupo de instrucciones.
      >
      >![Instrucciones de filtro conectadas](assets/filters-and-statements-connected-by-or-statements-builder-ui-old-filters-2022.png)
      >
      >Cuando crea un filtro para tareas que contienen la palabra &quot;marketing&quot; y están en proyectos con un estado de Actual o Planning, debe tener las siguientes reglas de filtro:
      >
      >`Task: Name Contains Marketing`
      >`AND`
      >`Project: Status Equals Current`
      >`OR`
      >`Task: Name Contains Marketing`
      >`AND`
      >`Project: Status Equals Planning`
      >
      >Aunque tarea: Nombre Contiene &quot;marketing&quot; no cambia entre los dos grupos de filtros AND, debe repetirse en el segundo grupo.

   * Elimine una regla de filtro existente haciendo clic en el icono &quot;X&quot;.

1. (Opcional) Haga clic en **Cambiar al modo de texto** para añadir un filtro mediante la interfaz de modo de texto.

   Para obtener más información sobre la creación de un filtro mediante la interfaz de modo de texto, consulte [Edición de un filtro mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

1. Haga clic en **Guardar filtro** para crear un nuevo filtro o reemplazar el seleccionado por los cambios.

   O

   Haga clic en **Guardar como nuevo filtro** para crear un nuevo filtro a partir del seleccionado.

   El nuevo filtro se muestra en la lista de filtros y se aplica automáticamente a la lista o informe seleccionado.

1. (Opcional) Realice una de las siguientes acciones:

   * Comparta los filtros que cree con otros usuarios o haga que estén disponibles en todo el sistema. Para obtener más información, consulte [Compartir un filtro, una vista o una agrupación](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
   * Elimine los filtros que ya no desee mostrar en la lista. Para obtener más información, consulte [Eliminación de filtros, vistas y agrupaciones](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).

## Creación o edición de un filtro en el generador de beta

Tenga en cuenta lo siguiente al crear filtros con las diferentes interfaces:

* Puede encontrar el generador de beta en los mismos lugares donde se encuentra la interfaz de filtro estándar para las áreas enumeradas en la tabla anterior.
* Puede alternar entre el estándar y la interfaz del generador beta, donde está disponible la opción beta.
* Después de habilitar el generador de beta en un área, es la experiencia predeterminada para todas las áreas en las que está disponible. Por ejemplo, si activa el generador de beta en una lista de proyectos, también será la experiencia predeterminada para crear filtros de problemas y tareas en listas.
* Puede crear filtros mediante la interfaz del generador de beta de las siguientes maneras:

   * Desde cero
   * Editar un filtro existente
   * Duplicar un filtro existente
   * Duplicar un filtro existente, editarlo y guardarlo como un filtro nuevo

* Los filtros guardados están disponibles en ambos creadores, independientemente de la experiencia que se haya utilizado para crearlos originalmente. Por ejemplo, si ha creado un filtro utilizando el generador estándar, también puede encontrarlo y modificarlo en la interfaz del creador beta.

   >[!TIP]
   >
   >Un filtro &quot;Todos&quot; no se incluye con el creador beta porque todos los elementos de la lista se muestran cuando no se aplican filtros. Haga clic en **Borrar todo** en la parte superior derecha del generador para borrar los filtros activos y mostrar todos los elementos. If **Borrar todo** atenuado, no se aplica ningún filtro.

* Los generadores estándar y beta tienen una sintaxis ligeramente diferente al crear filtros de varias instrucciones que combinan los operadores Y y O. Como resultado, estos filtros pueden mostrarse de forma diferente al cambiar de un generador a otro.

   >[!INFO]
   >
   >El siguiente escenario existe:
   >
   >1. Utilice el generador beta para crear un filtro que tenga la siguiente sintaxis:
   >
   >   `(A OR B) AND C`
   >
   >1. Vuelva al generador estándar y edite el filtro utilizando la sintaxis del generador estándar como se describe en la sección [Crear o editar un filtro en el generador estándar](#create-filter-in-standard-builder) en este artículo. La sintaxis del generador estándar muestra las instrucciones de filtro de la siguiente manera:
   >
   >   `A AND C`
   >   `OR`
   >   `B AND C`
   >
   >1. Realice un cambio en el filtro en la interfaz estándar.
   >1. Vuelva al generador beta. La sentencia de filtro se muestra según la lógica admitida en el generador estándar, como se describió anteriormente.

   >
   >   El filtro se muestra en la interfaz del generador beta de la siguiente manera:
   >  
   >   `A AND C`
   >   `OR`
   >   `B AND C`
   > 
   >   Esto sucede porque el filtro se modificó en la interfaz estándar.

Cree un filtro mediante la interfaz del creador beta:

1. Vaya a una lista donde desee crear un filtro o que contenga el filtro que desea personalizar.
1. Haga clic en el **Filtro** icono ![Icono de filtro](assets/filter-nwepng.png)y, a continuación, active la variable **Configuración beta** ![Configuración beta](assets/beta-toggle-white-on-existing-filters.png) para acceder al generador beta. Está desactivado de forma predeterminada.

   A continuación, acepte el acuerdo beta si es necesario. Solo es necesario ponerse de acuerdo una vez, y el generador beta permanece habilitado.

   Se abrirá la interfaz del generador de filtros beta.

   >[!TIP]
   >
   >El encabezado de la interfaz del generador de filtros cambia a azul cuando se activa el generador beta. Una vez que habilite la interfaz del generador beta, Workfront la mantendrá habilitada para todas las áreas en las que esté disponible.

   ![Generador de filtros beta](assets/new-filters-all-filter-types.png)

1. Revise las siguientes listas de filtros:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Marcado como favorito</strong></td>
   <td>Filtros que ha marcado como favoritos. Cuando marque como favorito un filtro, su ubicación original se muestra debajo del nombre del filtro y se oculta en la lista original a menos que lo elimine como favorito.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Guardado</strong></td>
   <td>Filtros que ha creado y guardado usted mismo.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Valores predeterminados del sistema</strong></td>
   <td>Los filtros predeterminados del sistema de Workfront, así como los filtros que el administrador de Workfront agregó a su lista de filtros, ya sea en el nivel del sistema o en la plantilla de diseño.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Compartido conmigo</strong></td>
   <td>Filtros que otros usuarios crearon y compartieron con usted o que se comparten en todo el sistema.</td>
   </tr>
   </tbody>
   </table>

1. Realice una de las siguientes acciones:

   * Haga clic en **Nuevo filtro** para crear un filtro desde cero.
   * Pase el ratón sobre un filtro existente que tenga permisos para administrar y haga clic en el botón **Editar** icono ![Icono Editar](assets/edit-icon.png) para editarlo.

      O

      Pase el ratón sobre un filtro existente que tenga permisos para ver y haga clic en el botón **Más** menú ![Más menú](assets/more-icon-spectrum.png)y haga clic en **Duplicar** para copiar el filtro existente y editar una copia.
   ![Más opciones de menú](assets/new-filters-more-menu-options-with-delete.png)

1. (Condicional) Dependiendo de si desea buscar objetos que coincidan con todas o cualquiera de las instrucciones de un grupo de filtros, seleccione entre las siguientes opciones:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Incluir si todos son verdaderos</strong></td>
   <td>Los objetos que encuentra el filtro deben coincidir con todos los criterios de filtro de un grupo de filtros. En este caso, las instrucciones de filtro están conectadas por el operador AND. Esta es la selección predeterminada.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Incluir si alguno es verdadero</strong></td>
   <td>Los objetos que encuentra el filtro deben coincidir con cualquier criterio de filtro de un grupo de filtros. En este caso, las instrucciones de filtro están conectadas por el operador OR.</td>
   </tr>
   </tbody>
   </table>

   ![Incluir si es todo, cualquiera o verdadero menú desplegable](assets/new-filters-all-or-any-are-true-drop-down-menu-nwe.png)

   Para obtener más información sobre los operadores de filtro, consulte [Información general sobre filtros en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Haga clic en el menú desplegable de campos para ver una lista de los campos utilizados recientemente y los campos sugeridos para filtrar. Los campos sugeridos se muestran actualmente en la lista que está filtrando.

   También puede seleccionar **Campos de exploración** para ver una lista de todos los campos por los que puede filtrar. Los campos de la búsqueda avanzada se agrupan por categoría de objeto.

   ![Busque un campo para filtrar por](assets/new-filter-search-for-field.png)

1. Haga clic en el menú desplegable del modificador para seleccionar un modificador. El modificador predeterminado es &quot;Es igual que&quot;.

   Para obtener más información, consulte [Modificadores de filtro y condición](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!TIP]
   >
   >A medida que crea el filtro, los resultados aparecen inmediatamente en la lista. Si el panel de filtro cubre la lista, puede cerrarlo para ver la pantalla. La información introducida permanece en el generador beta cuando se vuelve a abrir el panel.

1. Empiece a escribir el valor de un campo por el que desee filtrar. Por ejemplo, empiece a escribir el nombre de un problema si desea filtrar por `Issue:Name`. Seleccione el valor cuando se muestre en la lista.

   >[!TIP]
   >
   >Según el modificador que haya seleccionado, puede seleccionar varios valores.

1. Haga clic en **Añadir filtro** para seleccionar otro campo y añadir un nuevo criterio de filtrado a la instrucción filter.
1. (Opcional) Haga clic en el **Eliminar** icono ![Icono Eliminar](assets/delete.png) para quitar instrucciones de filtro existentes.

   O

   Haga clic en **Borrar todo** para borrar todos los criterios de filtrado.

1. (Opcional) Haga clic en **Agregar grupo de filtros** para agregar otro conjunto de criterios de filtrado. El operador predeterminado entre los conjuntos es AND. Haga clic en el operador para cambiarlo a O.

   >[!TIP]
   >
   >Puede que desee utilizar otro grupo de filtros cuando desee que los grupos estén conectados por un operador distinto del operador en una instrucción de filtro.

   >[!INFO]
   >
   >Cuando filtra para un proyecto que contiene &quot;marketing&quot; en el nombre que no está completo y que no está en espera, puede utilizar los siguientes grupos de filtros múltiples:
   >`(Project: Name Contains Marketing AND Project: Percent Complete Does not equal 100)`
   >`OR`
   >`(Project: Name Contains Marketing AND Project: Status Does not equal On Hold)`
   >En este caso, cada instrucción de filtro está conectada mediante una condición AND y los grupos de filtros están conectados mediante una condición OR.

1. (Opcional) Haga clic en **Modo de texto** para seguir creando el filtro mediante el modo de texto.

   ![Seleccionar modo de texto](assets/new-filter-select-text-mode.png)

   Se abre la interfaz del modo de texto.

   ![Interfaz de modo de texto](assets/text-mode-interface-for-beta-filters-nwe.png)

   >[!TIP]
   >
   >Se recomienda crear la mayor cantidad posible del filtro mediante la interfaz del generador de beta y solo mediante el modo de texto cuando se deban realizar modificaciones en el filtro que solo se admitan en el modo de texto.

   Para obtener más información sobre la creación de un filtro mediante la interfaz de modo de texto, consulte [Edición de un filtro mediante el modo de texto](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

1. Haga clic en **Salir del modo de texto** para volver a la interfaz del generador beta.

   >[!WARNING]
   >
   >Algunas instrucciones de modo de texto no son compatibles con el generador beta o la interfaz estándar. Si sale del modo de texto cuando ha creado estos tipos de instrucciones, puede que se genere un mensaje de advertencia.

1. (Opcional) Haga clic en **Aplicar** para aplicar el filtro a la lista y ver los resultados.

   Si el filtro no produce ningún resultado, la lista estará vacía.

1. Haga clic en **Guardar como nuevo** para guardar el filtro para uso futuro.

   ![Asigne un nombre al filtro y guárdelo](assets/save-as-untitled-filter-ui-nwe.png)

1. Select **Filtro sin título** y escriba el nombre del nuevo filtro en su lugar.

   >[!TIP]
   >
   >Asegúrese de asignar un nombre al filtro para que pueda encontrarlo más adelante. Si no nombra el filtro, se llamará Filtro sin título en el sistema.

1. Seleccione un icono para el nuevo filtro en el **Icono** menú desplegable.

   ![Seleccionar un icono para el filtro](assets/new-filter-select-icon.png)

1. (Opcional) Añada una descripción para el filtro para indicar qué es lo único que tiene al respecto. La descripción se muestra bajo el nombre del filtro en la lista de filtros.

   >[!TIP]
   >
   >Hacer clic **Cancelar** en cualquier momento le lleva de nuevo al área de creación de filtros.

1. Haga clic en **Guardar**. El filtro se guarda en la lista Guardar y se aplica a la lista de elementos.
1. (Opcional) Para mover un filtro a la lista Favoritos, pase el ratón sobre cualquier filtro del cajón de filtros y haga clic en el icono Favorito . ![Icono de favorito](assets/favorites-icon-small.png).

   O

   Pase el ratón sobre cualquier filtro del cajón de filtros y haga clic en el menú Más ![Más menú](assets/more-icon-spectrum.png)y haga clic en **Favorito**.

1. (Opcional) Haga clic en el **Filtros de pila** para activar los filtros apilados. Esta opción le permite aplicar más de un filtro guardado. Las reglas de filtro se aplican en el orden en que se seleccionan.

   >[!TIP]
   >
   >No hay límite en el número de filtros que puede seleccionar.
   >
   >Al seleccionar varios filtros, todas sus condiciones deben cumplirse simultáneamente para mostrar los resultados coincidentes.

   ![Apilar filtros](assets/new-filter-stack-filters.png)

   El número de filtros que ha seleccionado aparece junto al icono de filtro en la parte superior de la lista de elementos.

   ![Número de filtros seleccionados](assets/number-of-filters-selected.png)

1. (Opcional) Realice una de las siguientes acciones:

   * Comparta el filtro con otros o haga que esté disponible en todo el sistema. Para obtener más información, consulte [Compartir un filtro, una vista o una agrupación](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

   * Elimine el filtro si ya no es válido o está duplicado. Solo puede eliminar los filtros que le pertenecen. Puede eliminar los filtros que se compartieron con usted. Para obtener más información, consulte [Eliminación de filtros, vistas y agrupaciones](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).

