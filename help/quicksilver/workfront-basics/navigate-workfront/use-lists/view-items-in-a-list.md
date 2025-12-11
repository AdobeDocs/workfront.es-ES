---
navigation-topic: use-lists
title: Introducción a las listas en  [!DNL Adobe Workfront]
description: Puede ver listas de objetos en  [!DNL Adobe Workfront]  para obtener información sobre ellos, como sus fechas de inicio y vencimiento, los usuarios asignados a ellos y otros objetos asociados con ellos.
feature: Get Started with Workfront
author: Nolan
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 0c0ffbeefb0eed8d1ca2a6e68ed19b40080726df
workflow-type: tm+mt
source-wordcount: '2301'
ht-degree: 72%

---

# Introducción a las listas en [!DNL Adobe Workfront]

<!--Audited: 12/2025-->

Puede ver listas de objetos en [!DNL Adobe Workfront] para obtener información sobre ellos, como sus fechas de inicio y vencimiento, los usuarios asignados a ellos y otros objetos asociados con ellos.

Las siguientes son algunas características de las listas en [!DNL Workfront]:

* Las listas se actualizan automáticamente cada cinco minutos para actualizar la información que otros usuarios del sistema están actualizando en otra parte.
* Algunas áreas en [!DNL Workfront] están preconfiguradas con listas predeterminadas de objetos.

  Puede personalizar la mayoría de estas listas preconfiguradas.

* Un administrador de [!DNL Workfront] puede crear listas personalizadas para aplicarlas a varias áreas de [!DNL Workfront].

  Para obtener más información acerca de cómo crear listas de nivel de sistema, consulte el artículo [Crear, editar y compartir filtros, vistas y agrupaciones predeterminados](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

* A continuación se indican los tipos de listas de Workfront:

   * Listas estándar
   * Listas mejoradas

  Para obtener más información, vea la sección [Diferencia entre las listas estándar y las mejoradas](#the-difference-between-the-standard-and-the-enhanced-lists) en este artículo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior</p>
   <p>Solicitud o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a filtros, vistas y agrupaciones </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores de un filtro, vista o agrupación con acceso para compartir </p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old access: 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Request] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>[!UICONTROL View] or higher access to filters, views, groupings</p> <P>For items in the [!UICONTROL Setup] area, you need administrative access for the item or the [!UICONTROL System Administrator] access level.</P> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level.<br>For information on how a [!DNL Workfront] administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>[!UICONTROL View] or higher permissions with access to share</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.
-->

## Listas de objetos

A continuación se muestran algunos tipos de listas de objetos que se pueden encontrar en [!DNL Workfront] y algunas de las áreas en las que se muestran de forma predeterminada cuando tiene derechos para ver un objeto.

>[!NOTE]
>
>Esta lista no es completa. Cada una de estas listas de objetos también puede aparecer en un informe o en un panel de control. Por ejemplo, un informe de proyecto o un panel de control que contenga un informe de proyecto también mostrará una lista de proyectos.



<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] lista</strong></th> 
   <th><strong>Ubicación de la lista de objetos</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Lista de portafolios</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolios]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de programas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portafolios] &gt;[!UICONTROL haga clic en un portafolio] &gt;[!UICONTROL Programas]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL Programs]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de proyectos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects]</p> </li> 
     <li> <p>[!UICONTROL Portafolios] &gt;[!UICONTROL haga clic en un portafolio] &gt;[!UICONTROL Proyectos]</p> </li> 
     <li> <p>[!UICONTROL Portafolios] &gt;[!UICONTROL haga clic en un portafolio] &gt;[!UICONTROL Programas] &gt;[!UICONTROL haga clic en un programa] &gt;[!UICONTROL Proyectos]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de tareas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL haga clic en un proyecto] &gt; [!UICONTROL Tareas]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL haga clic en un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL haga clic en una tarea] &gt;[!UICONTROL Subtareas]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL haga clic en un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL haga clic en una tarea] &gt; [!UICONTROL Predecesores*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de problemas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt; [!UICONTROL haga clic] en un proyecto &gt;[!UICONTROL Problemas]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL haga clic en un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL haga clic en una tarea] &gt; [!UICONTROL Problemas]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL haga clic en un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL haga clic en una tarea] &gt;[!UICONTROL Subtareas] &gt;[!UICONTROL haga clic en una tarea] &gt; [!UICONTROL Problemas]</p> </li> 
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
   <td>Lista de paneles de control</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Dashboards]</p> </li> 
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
     <li> <p>[!UICONTROL Users]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de documentos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Portafolios] &gt;[!UICONTROL haga clic en un portafolio] &gt; [!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Portafolios] &gt; [!UICONTROL haga clic en un portafolio] &gt;[!UICONTROL Programas] &gt;[!UICONTROL haga clic en un programa] &gt;[!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL haga clic en un proyecto] &gt;[!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL hacer clic en un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL hacer clic en una tarea] &gt; [!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt; [!UICONTROL hacer clic] en un proyecto &gt; [!UICONTROL Problemas] &gt;[!UICONTROL hacer clic en un problema] &gt; [!UICONTROL Documentos]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de plantillas de horas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Plantillas de horas] &gt; [!UICONTROL Todas las plantillas de horas]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de tarifas de facturación</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL haga clic en un proyecto] &gt;[!UICONTROL Tarifas de facturación*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de registros de facturación</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt; [!UICONTROL haga clic en un proyecto] &gt; [!UICONTROL Registros de facturación]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de riesgos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL haga clic en un proyecto] &gt;[!UICONTROL Riesgos]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de gastos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL haga clic] en un proyecto &gt;[!UICONTROL Gastos]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt; [!UICONTROL haga clic en un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL haga clic en una tarea] &gt;[!UICONTROL Gastos]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de entradas de horas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL haga clic] en un proyecto</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL haga clic en un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL haga clic en una tarea] &gt;[!UICONTROL Horas]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL clic] un proyecto &gt;[!UICONTROL Problemas] &gt;[!UICONTROL clic] un problema &gt;[!UICONTROL Horas]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de formularios personalizados</td> 
   <td> 
    <ul> 
     <li>[!UICONTROL Setup] &gt;[!UICONTROL Custom Forms] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>Lista de grupos o subgrupos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups]</p> </li>
     <li> <p>[!UICONTROL Configuración] &gt;[!UICONTROL Grupos] &gt;[!UICONTROL Haga clic en el grupo principal] &gt;[!UICONTROL Subgrupos] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de equipos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Teams]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de compañías</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Companies]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de horarios</td> 
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

* No se puede personalizar la lista en el área especificada. Un administrador de [!DNL Workfront] puede generar una lista personalizada a nivel de sistema, o el usuario puede generar un informe para este objeto si su nivel de acceso le permite tener acceso a la edición de informes.

## Lista de elementos

Una lista contiene ciertos elementos que definen su formato y la información que se muestra. Puede encontrar varios elementos de lista del sistema disponibles de forma predeterminada. También puede crear elementos personalizados para satisfacer sus necesidades.

>[!NOTE]
>
>Al seleccionar un nuevo filtro, vista o agrupación de una lista, esa selección se conserva aunque cierre la sesión de [!DNL Workfront] o el explorador.

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
   <td><strong>[!UICONTROL Filter]</strong></td> 
   <td> <p>Los filtros mantienen la información innecesaria fuera de una lista, según los criterios especificados. </p> <p>Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Información general sobre los filtros</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL View]</strong></td> 
   <td> <p>Las vistas definen qué campos (columnas) se muestran en la pantalla.</p> <p>Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Información general sobre las vistas en [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Grouping]</strong></td> 
   <td> <p>Las agrupaciones separan los objetos de la lista en áreas basadas en los criterios especificados.</p> <p>Por ejemplo, los problemas de una lista pueden mostrarse en secciones por estado o prioridad.</p> <p>Puede tener hasta tres capas de agrupaciones en una agrupación estándar y puede añadir una cuarta capa si configura una agrupación en modo de texto.</p> <p>Para obtener más información acerca de las agrupaciones, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Información general sobre agrupaciones en [!DNL Adobe Workfront]</a>.</p> <p>Para obtener más información acerca del modo de texto, consulte <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Información general sobre el modo de texto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Estos elementos se muestran en la parte superior de cada lista de forma predeterminada. Son fijas y no se mueven a medida que se desplaza por la lista. Pase el ratón sobre el icono de cada elemento para identificarlo.

![Elementos de lista](assets/nwe-list-elements.png)

Puede personalizar los elementos de la lista en las siguientes áreas y compartirlos con otros usuarios:

* Se encontró cualquier lista predeterminada del sistema en la sección [Introducción a las listas en [!DNL Adobe Workfront]](#default-workfront-lists) en este artículo
* Cualquier informe que se comparta con usted

Los elementos de creación para las listas son los mismos que para los informes.

Para obtener más información acerca de cómo crear y personalizar los elementos de creación de listas e informes, consulte [Elementos para la creación de informes: filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

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
   <td> <p>Editar objetos y su información directamente en la lista.</p> <p>Para obtener más información, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">Editar elementos en línea en una lista de [!DNL Adobe Workfront]</a>.</p> 
   <p><b>NOTA:</b></p>
   <p>La edición en línea no es posible en una agrupación.</p>

</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>Actualización con el [!UICONTROL Summary]</strong> </td> 
   <td> <p>Actualice tareas y problemas en el nivel de proyecto mediante el panel [!UICONTROL Summary].</p> <p><b>SUGERENCIA:</b></p> <p>El resumen no está disponible para todos los objetos y no está disponible en los informes de Tareas o Problemas.</p> <p>Para obtener más información, consulte <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Información general sobre el resumen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Personalizar visualización de lista</strong> </td> 
   <td> <p>Personalice el aspecto de una lista, la disposición de columnas, el orden de clasificación de los elementos o el número de elementos que se muestran.</p> <p><b>NOTA:</b></p> <p>Los cambios que realice en el número de elementos que se mostrarán en una página se revertirán cuando cierre la sesión de [!DNL Workfront] o el explorador. Los cambios también se pueden revertir después de un periodo de 8 horas.</p> <p>Para obtener más información, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">Modificación del modo en que se muestra una lista</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Filtro rápido</strong> </td> 
   <td> <p>Aplique un filtro rápido para encontrar solo los elementos que son importantes para usted, de modo que pueda revisarlos, actualizarlos o compartirlos rápidamente con otras personas.</p> <p><b>IMPORTANTE:</b></p> <p> Puede buscar elementos que contengan una palabra de búsqueda mediante el filtro rápido, independientemente de si ese elemento está visible en la pantalla o se mostrará después de desplazarse hasta la parte inferior de la página. Cuando se utilizan las funciones de búsqueda del explorador, solo se pueden encontrar elementos que ya están visibles en la pantalla. Si la lista tiene varias páginas, los filtros rápidos solo encontrarán los elementos de la página actual.</p> <p>Para obtener más información, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Aplicar el filtro rápido a una lista</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Exportar</strong> </td> 
   <td> <p>Exportar una lista de objetos desde [!DNL Workfront]. Cuando una lista contiene más de 2000 elementos, exportar la lista es la única manera de revisar todos los elementos de una página.</p> <p>Para obtener más información acerca de cómo exportar una lista, consulte <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">Exportar una lista</a>. Para obtener más información sobre los formatos y límites de exportación, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportar datos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Barra de herramientas de lista

En la tabla siguiente se enumeran muchos de los iconos disponibles en la barra de herramientas y se indica lo que sucede cuando se hace clic en ellos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Icono</strong></td> 
   <td><strong>Descripción</strong></td> 
   <td><strong>Al hacer clic, se puede</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/add-icon-plus-in-circle.png"> </td> 
   <td>[!UICONTROL Add item or user]</td> 
   <td>Abrir más opciones, incluida la de añadir un nuevo elemento o usuario.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insert task above]</td> 
   <td> <p>Insertar una tarea encima de la tarea seleccionada.</p> <p>Esta opción solo está disponible para tareas. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insert task below]</td> 
   <td> <p>Insertar una tarea debajo de la tarea seleccionada.</p> <p>Esta opción solo está disponible para tareas. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[!UICONTROL Edit]</td> 
   <td>Editar el elemento seleccionado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/copy-icon.png"> </td> 
   <td>[!UICONTROL Copy]</td> 
   <td>Copiar el elemento seleccionado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/delete.png"> </td> 
   <td>[!UICONTROL Delete]</td> 
   <td>Eliminar el elemento seleccionado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-add-to-iteration-icon-in-new-toolbar-for-issues.png"> </td> 
   <td>[!UICONTROL Add to]</td> 
   <td> <p>Abrir el cuadro de diálogo para añadir el problema seleccionado a una iteración.</p> <p>Esto solo está disponible para problemas.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/share-icon.png"> </td> 
   <td>[!UICONTROL Share]</td> 
   <td>Compartir el elemento seleccionado.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-indent-outdent-tasks-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Indent and outdent tasks] </td> 
   <td> <p>Aplicar sangría o anular sangría a la tarea seleccionada. </p> <p>Esta opción solo está disponible para tareas. </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[!UICONTROL More]</td> 
   <td>Abrir opciones adicionales para el elemento seleccionado.</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[!UICONTROL Quick filter] </p> </td> 
   <td> <p>Abrir el cuadro de búsqueda de filtros rápidos para buscar elementos en la lista mostrada.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[!UICONTROL Export]</td> 
   <td>Exportar la lista a archivos de PDF, Excel o delimitados por tabuladores.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Agile View]</td> 
   <td>Mostrar la lista en la vista de Agile.<br>Esto solo está disponible para tareas.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Gantt Chart]</td> 
   <td> <p>Mostrar la lista en la vista [!UICONTROL Gantt Chart].</p> <p>Esto solo está disponible para proyectos y tareas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>Menú desplegable [!UICONTROL Filter]</td> 
   <td> <p>Mostrar una lista de filtros y opciones adicionales para administrar filtros, incluido el proceso de crear uno. </p> <p>En una pantalla pequeña, el nombre del filtro se reemplaza por el icono de filtro. Se muestra un punto azul en el icono Filtro cuando se aplica cualquier filtro que no sea “[!UICONTROL All]”.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menú desplegable [!UICONTROL View]</td> 
   <td> <p>Mostrar una lista de vistas y opciones adicionales para administrar vistas, incluido el proceso de crear una. </p> <p>En una pantalla pequeña, el nombre de la vista se reemplaza por el icono [!UICONTROL view]. S muestra un punto azul en el icono [!UICONTROL View] cuando se aplica cualquier vista que no sea “[!UICONTROL Standard]”.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menú desplegable [!UICONTROL Grouping]</td> 
   <td> <p>Mostrar una lista de agrupaciones y opciones adicionales para administrar agrupaciones, incluido el proceso de crear una. </p> <p>En una pantalla pequeña, el nombre de agrupación se reemplaza por el icono [!UICONTROL grouping]. Aparece un punto azul en el icono [!UICONTROL Grouping] cuando se aplica cualquier agrupación que no sea "[!UICONTROL Nothing]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL Plan mode]</p> </td> 
   <td> <p>Elija si desea guardar los cambios realizados en una lista de tareas de forma automática o manual. </p> <p>Para obtener información acerca de la edición de tareas en una lista, vea <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Editar tareas en una lista</a>. </p> <p>Esta opción solo está disponible para tareas.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[!UICONTROL Summary]</td> 
   <td> <p>Mostrar u ocultar el cuadro [!UICONTROL Summary] para el elemento seleccionado.</p> <p>Esta opción solo está disponible para tareas y problemas.</p> <p>Para obtener información acerca del panel [!UICONTROL Summary], consulte <a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Resumen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL Remove]</td> 
   <td>Quitar algo de la lista. Por ejemplo, como administrador de un grupo que administra los miembros de un grupo o subgrupo, quite un miembro de un grupo tal como se explica en <a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">Ver y administrar los miembros de un grupo</a>.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[!UICONTROL Comment] /[!UICONTROL Update]</td> 
   <td> <p>Escribir un comentario o una actualización.</p> </td> 
  </tr> 
 </tbody> 
</table>

## La diferencia entre listas e informes

Tanto las listas como los informes son cuadrículas que contienen información sobre un tipo de objeto.

En la tabla siguiente se describen las similitudes y diferencias entre las listas y los informes:

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
   <td> <p>Solamente un administrador y usuarios de [!DNL Workfront] con una licencia de [!UICONTROL Plan] pueden crearlos</p> </td> 
   <td> </td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td> <p>Hay disponible un conjunto predeterminado en [!DNL Workfront]</p> </td> 
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
   <td> <p>Pueden compartirse con otros usuarios</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puede compartirse en todo el sistema</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Pueden compartirse fuera del sistema</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Pueden exportarse a formatos .pdf, [!DNL Excel] y delimitado por tabuladores</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Pueden programarse para enviarse en un correo electrónico</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Pueden añadirse a una plantilla de diseño</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Puede añadirse a secciones personalizadas </p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Pueden añadirse a un panel de control</p> </td> 
   <td> ✓*** </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Pueden utilizarse indicadores para personalizar lo que muestran</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Pueden mostrarse en un gráfico</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Pueden editarse objetos en línea en ellos</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

* Debe tener acceso a filtros, vistas y agrupaciones para poder crearlos. Para obtener más información, consulte [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

**Debe tener acceso a filtros, vistas y agrupaciones, así como a informes, tableros y calendarios, para poder crearlos. Para obtener más información, consulte [Conceder acceso a informes, paneles de control y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

***Puede personalizar listas para informes que se colocan en un panel solo si el creador del informe ha configurado los elementos de la lista para que sean visibles en el panel.

>[!NOTE]
>
>No se puede añadir una lista a un panel de control sin crear un informe y añadirlo primero al panel de control.

Para obtener más información sobre cómo generar un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Para obtener información acerca de cómo crear secciones personalizadas , vea [Crear pestañas o secciones personalizadas](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## La diferencia entre las listas estándar y las mejoradas

Hay dos tipos de listas en [!DNL Workfront]:

* Listas estándar

  ![Lista de proyectos estándar](assets/standard-list-screen-shot-gray-groupings.png)

* Listas mejoradas

  ![Listas mejoradas](assets/enhanced-status-list.png)

Las capacidades de cada lista mejorada difieren según la página desde la que se acceda a ella.

Para obtener información acerca de las listas mejoradas, vea [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).



La tabla siguiente muestra algunas de las diferencias entre las listas estándar y las mejoradas de [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Listas estándar</b></td> 
   <td><b>Listas mejoradas</b></td> 
  </tr> 
  <tr>
  <td> <p>Se muestran <strong>Todos</strong> o hasta <strong>2000</strong> elementos de forma predeterminada</p> </td> 
   <td> Mostrar todos los elementos de la lista después de desplazarse manualmente </td> 
  </tr>

<tr> 
   <td>La interacción con los elementos de la lista es coherente en todos los tipos de objetos y se realiza mediante los iconos de la parte superior de la lista.  </td> 
   <td>La interacción con los elementos de la lista puede variar según el tipo de objeto y se realiza mediante los iconos de la parte superior de la lista, así como mediante la barra de herramientas azul activada después de seleccionar los elementos de la lista. </td> 
  </tr>

</td> 
  </tr> 
  <tr> 
   <td><p>Puede aplicar cambios de color de celda a los elementos de una lista</p></td>
   <td><p>No se pueden aplicar cambios de color de celda a los elementos de una lista. </p></td>
   </td> 
   <td></td> 
  </tr> 
 </tbody> 
</table>

<!--
consider adding things like adding fields on the fly in an enhanced list when we will be able to do this-->

<!--old table: 
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Legacy lists</b></td> 
   <td><b>Updated lists</b></td> 
  </tr> 
  <td> <p>Display <strong>100</strong> items by default</p> </td> 
   <td> <p>Display <strong>All</strong> or up to <strong>2000</strong> items by default</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Use CTRL+F to find items in a list</p> </td> 
   <td> <p>Use quick filters to quickly find information in a large list</p> <p>For information about using quick filters in lists, see <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Apply the quick filter to a list</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>You can't inline edit custom fields with rich text formatting.</td> 
   <td> <p>Text in custom fields with formatting can be configured to allow bold, italics, underline, bullets, numbering, hyperlinks, and block quotes.</p> <p>For more information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Conditional formatting can change the text color of links in a list</td> 
   <td>Cannot apply text color changes to links in a list</td> 
  </tr> 
 </tbody> 
</table>
-->
