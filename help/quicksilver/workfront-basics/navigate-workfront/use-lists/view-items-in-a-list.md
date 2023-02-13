---
navigation-topic: use-lists
title: Introducción a las listas en [!DNL Adobe Workfront]
description: Puede ver listas de objetos en [!DNL Adobe Workfront] para obtener información sobre ellos, como sus fechas de inicio y caducidad, los usuarios asignados a ellos y otros objetos asociados a ellos.
feature: Get Started with Workfront
author: Lisa
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '2370'
ht-degree: 0%

---

# Introducción a las listas en [!DNL Adobe Workfront]

<!--
{{highlighted-preview}}
-->

Puede ver listas de objetos en [!DNL Adobe Workfront] para obtener información sobre ellos, como sus fechas de inicio y caducidad, los usuarios asignados a ellos y otros objetos asociados a ellos.

Las siguientes son algunas características de las listas de [!DNL Workfront]:

* Las listas se actualizan automáticamente cada cinco minutos para actualizar la información que otros usuarios del sistema están actualizando en otras partes.
* Algunas áreas en [!DNL Workfront] están preconfigurados con listas predeterminadas de objetos.

   Puede personalizar la mayoría de estas listas preconfiguradas.

* A [!DNL Workfront] el administrador puede crear listas personalizadas para aplicarlas a varias áreas de [!DNL Workfront].

   Para obtener más información sobre la creación de listas de nivel de sistema, consulte el artículo [Crear, editar y compartir filtros, vistas y agrupaciones predeterminadas](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Request] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>[!UICONTROL View] o acceso superior a filtros, vistas, agrupaciones</p> <P>Para los elementos del área [!UICONTROL Setup], necesita acceso administrativo para el elemento o el nivel de acceso [!UICONTROL System Administrator].</P> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso.<br>Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Permisos de [!UICONTROL View] o superior con acceso para compartir</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td>
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Listas de objetos

A continuación se muestran algunos tipos de listas de objetos que puede encontrar en [!DNL Workfront] y algunas de las áreas en las que se muestran de forma predeterminada cuando tiene derechos para ver un objeto.

>[!NOTE]
>
>* Esta lista no es completa. Cada una de estas listas de objetos también puede aparecer en un informe o un tablero. Por ejemplo, un informe de proyecto o un tablero que contenga un informe de proyecto también muestran una lista de proyectos.
>* En esta lista, &quot;seleccionar&quot; significa que debe hacer clic en el nombre del elemento, no en la casilla de verificación a la izquierda del nombre.



<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] list</strong></th> 
   <th><strong>Ubicación de la lista de objetos</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Lista de portafolios</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolio]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de programas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolio] &gt;[!UICONTROL seleccionar un portafolio] &gt;[!UICONTROL Programas]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL Programs]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de proyectos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos]</p> </li> 
     <li> <p>[!UICONTROL Portfolio] &gt;[!UICONTROL seleccionar un portafolio] &gt;[!UICONTROL Proyectos]</p> </li> 
     <li> <p>[!UICONTROL Portfolio] &gt;[!UICONTROL seleccionar un portafolio] &gt;[!UICONTROL Programas] &gt;[!UICONTROL seleccionar un programa] &gt;[!UICONTROL Proyectos]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de tareas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleccionar un proyecto] &gt; [!UICONTROL Tasks]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL seleccionar una tarea] &gt;[!UICONTROL Subtasks]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL seleccionar una tarea] &gt; [!UICONTROL Predecesores*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de problemas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL seleccionar] un proyecto &gt;[!UICONTROL Issues]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL seleccionar una tarea] &gt; [!UICONTROL Issues]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL seleccionar una tarea] &gt;[!UICONTROL Subtasks] &gt;[!UICONTROL seleccionar una tarea] &gt; [!UICONTROL problemas]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de informes</td> 
   <td> 
    <ul> 
     <li> <p>  [!UICONTROL Reports]  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de tableros</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Tableros]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de iteraciones</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Teams] &gt; [!UICONTROL Iterations]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de usuarios</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Usuarios]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de documentos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Portfolio] &gt;[!UICONTROL seleccionar un portafolio] &gt; [!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Portfolio] &gt; [!UICONTROL seleccionar un portafolio] &gt;[!UICONTROL Programas] &gt;[!UICONTROL seleccionar un programa] &gt;[!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL seleccionar una tarea] &gt; [!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL seleccionar] un proyecto &gt; [!UICONTROL Issues] &gt;[!UICONTROL seleccionar un problema] &gt; [!UICONTROL Documents]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de partes de horas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Hoja de horas] s &gt; [!UICONTROL Todas las hojas de horas]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de tasas de facturación</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tasas de facturación*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de registros de facturación</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt; [!UICONTROL seleccionar un proyecto] &gt; [!UICONTROL Registros de facturación]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de riesgos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Riesgos]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de gastos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleccionar] un proyecto &gt;[!UICONTROL Expenses]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL seleccionar una tarea] &gt;[!UICONTROL Expenses]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de entradas de hora</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar] un proyecto</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL seleccionar una tarea] &gt;[!UICONTROL Hours]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleccionar] un proyecto &gt;[!UICONTROL Issues] &gt;[!UICONTROL select] un problema &gt;[!UICONTROL Hours]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td class="preview">Lista de formularios personalizados</td> 
   <td> 
    <ul> 
     <li class="preview"> <p>[!UICONTROL Configuración] &gt;[!UICONTROL Forms personalizado]</p>
     <!--Remove the following note box when this goes to Production. Or do this when the Preview highlighting becomes available.-->
     <p><b>NOTA</b>: Actualmente solo está disponible en el entorno de vista previa</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>Lista de grupos o subgrupos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups]</p> </li>
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups] &gt;[!UICONTROL seleccionar el grupo principal] &gt;[!UICONTROL Subgroups] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de equipos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Equipos]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de empresas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Companies]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de programas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Schedules]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de plantillas de diseño</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Layout Templates]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

No se puede personalizar la lista en el área especificada. A [!DNL Workfront] El administrador puede crear una lista personalizada a nivel del sistema o crear un informe para este objeto si el nivel de acceso le permite editar informes.

## Elementos de lista

Una lista contiene ciertos elementos que definen su formato y la información que se muestra. Puede encontrar varios elementos de la lista del sistema que están disponibles de forma predeterminada. También puede crear elementos personalizados para satisfacer sus necesidades.

>[!NOTE]
>
>Al seleccionar un filtro, una vista o una agrupación nuevos de una lista, esa selección se conserva aunque cierre la sesión [!DNL Workfront] o cierre el explorador.

Los siguientes son los elementos de una lista:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Elemento</strong></th> 
   <th><strong>Explicación</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Filtro]</strong></td> 
   <td> <p>Los filtros mantienen la información innecesaria fuera de una lista, según los criterios especificados. </p> <p>Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Información general sobre filtros en [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL View]</strong></td> 
   <td> <p>Las vistas definen qué campos (columnas) se muestran en la pantalla.</p> <p>Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Información general sobre vistas en [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Grouping]</strong></td> 
   <td> <p>Los grupos separan los objetos de la lista en áreas según los criterios especificados.</p> <p>Por ejemplo, los problemas de una lista pueden mostrarse en secciones por estado o prioridad.</p> <p>Puede tener hasta tres capas de agrupaciones en una agrupación estándar y puede agregar una cuarta capa si configura una agrupación en modo de texto.</p> <p>Para obtener más información sobre las agrupaciones, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Información general sobre las agrupaciones en [!DNL Adobe Workfront]</a>.</p> <p>Para obtener más información sobre el modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Información general sobre el modo de texto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Estos elementos se muestran en la parte superior de cada lista de forma predeterminada. Son duraderas y no se mueven a medida que se desplaza por la lista. Pase el ratón sobre el icono de cada elemento para identificarlos.

![](assets/nwe-list-elements.png)

Puede personalizar los elementos de la lista en las siguientes áreas y compartirlos con otros usuarios:

* Cualquier lista predeterminada del sistema que se encuentre en la sección [Introducción a las listas en [!DNL Adobe Workfront]](#default-workfront-lists) en este artículo
* Cualquier informe que se comparta con usted

Los elementos de creación de las listas son los mismos que los elementos de creación de los informes.

Para obtener más información sobre la creación y personalización de los elementos de creación de listas e informes, consulte [Elementos de informes: filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Enumerar acciones

Puede completar las siguientes acciones en una lista:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Acción</strong></th> 
   <th><strong>Información</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Edición en línea</strong> </td> 
   <td> <p>Edite los objetos y su información directamente en la lista.</p> <p>Para obtener más información, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">Editar elementos en línea en una lista de [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>Actualización con el [!UICONTROL Summary]</strong> </td> 
   <td> <p>Actualice tareas y problemas a nivel de proyecto mediante el panel [!UICONTROL Summary].</p> <p>Sugerencia: El Resumen no está disponible para todos los objetos y no está disponible en los informes Tarea o Problema.</p> <p>Para obtener más información, consulte <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Resumen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Personalización de la visualización de la lista</strong> </td> 
   <td> <p>Personalice el aspecto de una lista, la organización de columnas, el orden de los elementos o el número de elementos que se muestran.</p> <p>Nota: Los cambios que realice en el número de elementos que se mostrarán en una página se revertirán cuando cierre la sesión [!DNL Workfront] o cierre el explorador. Los cambios también se pueden revertir después de un período de 8 horas.</p> <p>Para obtener más información, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">Modificar el modo en que se muestra la lista</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Filtro rápido</strong> </td> 
   <td> <p>Aplique un filtro rápido para buscar solo elementos que sean importantes para usted, de modo que pueda revisarlos, actualizarlos o compartirlos rápidamente con otros.</p> <p>Importante: Puede encontrar elementos que contengan una palabra de búsqueda mediante el filtro rápido, tanto si el elemento está visible en la pantalla como si se mostrará después de desplazarse hasta la parte inferior de la página. Al utilizar las funciones de búsqueda del explorador, solo puede encontrar los elementos que ya están visibles en la pantalla. Si la lista tiene varias páginas, los filtros rápidos encontrarán solamente los elementos de la página actual.</p> <p>Para obtener más información, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Aplicar el filtro rápido a una lista</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Exportar</strong> </td> 
   <td> <p>Exportación de una lista de objetos desde [!DNL Workfront]. Cuando una lista contiene más de 2000 elementos, exportar la lista es la única manera de revisar todos los elementos de una página.</p> <p>Para obtener más información sobre cómo exportar una lista, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">Exportación de una lista</a>. Para obtener más información sobre los formatos y límites de exportación, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportar datos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Barra de herramientas de lista

En la tabla siguiente se enumeran muchos de los iconos disponibles en la barra de herramientas e indica lo que sucede al hacer clic en ellos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Icono</strong></td> 
   <td><strong>Descripción</strong></td> 
   <td><strong>Al hacer clic</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/add-icon-plus-in-circle.png"> </td> 
   <td>[!UICONTROL Agregar elemento o usuario]</td> 
   <td>Abra más opciones, incluida la adición de un nuevo elemento o usuario.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insertar tarea arriba]</td> 
   <td> <p>Inserte una tarea encima de la tarea seleccionada.</p> <p>Esto solo está disponible para tareas. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insertar tarea a continuación]</td> 
   <td> <p>Inserte una tarea debajo de la tarea seleccionada.</p> <p>Esto solo está disponible para tareas. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[!UICONTROL Editar]</td> 
   <td>Edite el elemento seleccionado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/copy-icon.png"> </td> 
   <td>[!UICONTROL Copy]</td> 
   <td>Copie el elemento seleccionado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/delete.png"> </td> 
   <td>[!UICONTROL Eliminar]</td> 
   <td>Eliminar el elemento seleccionado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-add-to-iteration-icon-in-new-toolbar-for-issues.png"> </td> 
   <td>[!UICONTROL Agregar a]</td> 
   <td> <p>Abra el cuadro de diálogo para agregar el problema seleccionado a una iteración.</p> <p>Esto solo está disponible para problemas.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/share-icon.png"> </td> 
   <td>[!UICONTROL Compartir]</td> 
   <td>Compartir el elemento seleccionado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-indent-outdent-tasks-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Tareas de sangría y sangría] </td> 
   <td> <p>Sangra o anula la sangría de la tarea seleccionada. </p> <p>Esto solo está disponible para tareas. </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[!UICONTROL Más]</td> 
   <td>Abra opciones adicionales para el elemento seleccionado.</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[!UICONTROL Filtro rápido] </p> </td> 
   <td> <p>Abra el cuadro de búsqueda filtro rápido para buscar elementos en la lista mostrada.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[!UICONTROL Export]</td> 
   <td>Exporte la lista a archivos de PDF, Excel o separados por tabuladores.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Vista Agile]</td> 
   <td>Muestre la lista en la vista Águila.<br>Esto solo está disponible para tareas.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Diagrama de Gantt]</td> 
   <td> <p>Muestre la lista en la vista [!UICONTROL Gantt Chart].</p> <p>Esto solo está disponible para proyectos y tareas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>Menú desplegable [!UICONTROL Filtro]</td> 
   <td> <p>Muestre una lista de filtros y opciones adicionales para administrar filtros, incluida la creación de uno. </p> <p>En una pantalla pequeña, el nombre de filtro se sustituye por el icono de filtro. Aparece un punto azul en el icono Filtro cuando se aplica cualquier filtro que no sea "[!UICONTROL Todo]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menú desplegable [!UICONTROL View]</td> 
   <td> <p>Muestre una lista de vistas y opciones adicionales para administrar vistas, incluida la creación de una. </p> <p>En una pantalla pequeña, el nombre de la vista se sustituye por el icono [!UICONTROL view]. Aparece un punto azul en el icono [!UICONTROL View] cuando se aplica cualquier vista que no sea "[!UICONTROL Standard]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menú desplegable [!UICONTROL Grouping]</td> 
   <td> <p>Muestre una lista de agrupaciones y opciones adicionales para administrar agrupaciones, incluida la creación de una. </p> <p>En una pantalla pequeña, el nombre de la agrupación se reemplaza por el icono [!UICONTROL grouping] . Aparece un punto azul en el icono [!UICONTROL Grouping] cuando se aplica cualquier agrupación que no sea "[!UICONTROL Nothing]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL modo Plan]</p> </td> 
   <td> <p>Elija si desea guardar los cambios realizados en una lista de tareas de forma automática o manual. </p> <p>Para obtener información sobre la edición de tareas en una lista, consulte <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Editar tareas en una lista</a>. </p> <p>Esto solo está disponible para tareas.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[!UICONTROL Resumen]</td> 
   <td> <p>Mostrar u ocultar el cuadro [!UICONTROL Summary] para el elemento seleccionado.</p> <p>Esto solo está disponible para tareas y problemas.</p> <p>Para obtener información sobre el panel [!UICONTROL Summary] en la nueva [!DNL Adobe Workfront] experiencia, consulte <a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Resumen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL Quitar]</td> 
   <td>Elimine algo de la lista. Por ejemplo, como administrador de grupo que administra las pertenencias a grupos o subgrupos, elimine un miembro de grupo como se explica en <a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">Ver y administrar las suscripciones de un grupo</a>.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[!UICONTROL Comment] /[!UICONTROL Update]</td> 
   <td> <p>Escriba un comentario o actualice.</p> </td> 
  </tr> 
 </tbody> 
</table>

## La diferencia entre listas e informes

Tanto las listas como los informes son cuadrículas que contienen información sobre un tipo de objeto.

La siguiente tabla describe las similitudes y diferencias entre listas e informes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Funcionalidad</strong> </th> 
   <th><strong>Lista</strong> </th> 
   <th><strong>Informe</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Cualquiera puede crearlos</p> </td> 
   <td><span>✓*</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Solo un [!DNL Workfront] el administrador y los usuarios con una licencia de [!UICONTROL Plan] pueden crearlos</p> </td> 
   <td> </td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td> <p>Hay un conjunto predeterminado disponible en [!DNL Workfront]</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Personalizable en modo estándar</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Personalizable en modo de texto</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puede compartirlas con otros usuarios</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puede compartirlas en todo el sistema</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Puede compartirlas fuera del sistema</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Puede exportar a .pdf, [!DNL Excel]y formatos delimitados por tabulaciones</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Puede programarlos para enviarlos por correo electrónico</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Puede agregar a una plantilla de diseño</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Puede agregarlas a secciones personalizadas </p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puede agregarlas a un tablero</p> </td> 
   <td> ✓*** </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puede utilizar las indicaciones para personalizar lo que muestran</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puede mostrarlos en un gráfico</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puede editar objetos en línea en ellos</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Debe tener acceso a filtros, vistas y agrupaciones para poder crearlos. Para obtener más información, consulte [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

Para poder crearlos, debe tener acceso a filtros, vistas y agrupaciones, así como a informes, tableros y calendarios. Para obtener más información, consulte [Conceder acceso a informes, tableros y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Puede personalizar las listas de los informes que se coloquen en un tablero solo si el creador del informe ha configurado los elementos de la lista para que sean visibles en el tablero.

>[!NOTE]
>
>No puede agregar una lista a un tablero sin crear un informe y agregarlo primero al tablero.

Para obtener más información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Para obtener información sobre la creación de secciones personalizadas, consulte [Crear fichas o secciones personalizadas](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## La diferencia entre las listas actualizadas y las listas heredadas

Existen dos tipos de listas en [!DNL Workfront]:

* Listas heredadas

   ![](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* Listas actualizadas

   ![](assets/updated-list-screen-shot-gray-groupings-350x71.png)

Ambos tipos de listas aparecen en la [!DNL Adobe Workfront].

Todas las listas e informes de [!DNL Adobe Workfront] son listas actualizadas, excepto por lo siguiente:

* Las listas de [!UICONTROL Configuración] area
* Las listas de [!UICONTROL Informes] area

La siguiente tabla muestra algunas de las diferencias entre las listas heredadas y actualizadas de [!DNL Workfront]:

<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> [Legacy does not equal Classic. Legacy lists appear in NWE and Classic. Updated lists appear in NWE and Classic.]</span>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Listas heredadas</b></td> 
   <td><b>Listas actualizadas</b></td> 
  </tr> 
  <tr> 
   <td> <p>Fuentes heredadas, encabezados de columna, combinación de colores azul</p> </td> 
   <td> <p>Fuentes actualizadas, encabezados de columna, esquema de colores de agrupación gris</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Edición en línea más lenta</p> </td> 
   <td> <p>Edición en línea más rápida</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Mostrar <strong>100</strong> items de forma predeterminada</p> </td> 
   <td> <p>Mostrar <strong>Todo</strong> o hasta <strong>2000</strong> items de forma predeterminada</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilice CTRL+F para buscar elementos en una lista</p> </td> 
   <td> <p>Utilice filtros rápidos para encontrar rápidamente información en una lista grande</p> <p>Para obtener información sobre el uso de filtros rápidos en listas, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Aplicar el filtro rápido a una lista</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>No se pueden editar en línea campos personalizados con formato de texto enriquecido.</td> 
   <td> <p>El texto de los campos personalizados con formato se puede configurar para permitir negrita, cursiva, subrayado, viñetas, numeración, hipervínculos y comillas de bloque.</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>El formato condicional puede cambiar el color del texto de los vínculos de una lista</td> 
   <td>No se pueden aplicar cambios de color de texto a los vínculos de una lista</td> 
  </tr> 
 </tbody> 
</table>
