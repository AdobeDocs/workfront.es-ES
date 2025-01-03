---
navigation-topic: use-lists
title: Introducción a las listas en  [!DNL Adobe Workfront]
description: Puede ver listas de objetos en  [!DNL Adobe Workfront]  para obtener información sobre ellos, como sus fechas de inicio y vencimiento, los usuarios asignados a ellos y otros objetos asociados a ellos.
feature: Get Started with Workfront
author: Nolan
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 261ac44eb0d13ffbd61a2c70213adb591bf018aa
workflow-type: tm+mt
source-wordcount: '2284'
ht-degree: 0%

---

# Introducción a las listas de [!DNL Adobe Workfront]

<!--Audited: 11/2024-->

Puede ver listas de objetos en [!DNL Adobe Workfront] para obtener información sobre ellos, como sus fechas de inicio y vencimiento, los usuarios asignados a ellos y otros objetos asociados a ellos.

Las siguientes son algunas características de las listas de [!DNL Workfront]:

* Las listas se actualizan automáticamente cada cinco minutos para actualizar la información que otros usuarios del sistema están actualizando en otra parte.
* Algunas áreas de [!DNL Workfront] están preconfiguradas con listas predeterminadas de objetos.

  Puede personalizar la mayoría de estas listas preconfiguradas.

* Un administrador de [!DNL Workfront] puede crear listas personalizadas para aplicarlas a varias áreas de [!DNL Workfront].

  Para obtener más información acerca de cómo crear listas de nivel de sistema, vea el artículo [Crear, editar y compartir filtros, vistas y agrupaciones predeterminados](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
    <p>Nuevo:</p>
   <ul><li><p>Colaborador o superior </p></li>
   </ul>

<p>Actual:</p>
   <ul><li><p>Solicitud o superior</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a filtros, vistas y agrupaciones </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores de un filtro, vista o agrupación con acceso para compartir </p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
>* Esta lista no es completa. Cada una de estas listas de objetos también puede aparecer en un informe o en un tablero. Por ejemplo, un informe de proyecto o un tablero que contenga un informe de proyecto también mostrará una lista de proyectos.
>* En esta lista, &quot;seleccionar&quot; significa que debe hacer clic en el nombre del elemento, no en la casilla de verificación situada a la izquierda del nombre.


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
     <li> <p>[!UICONTROL Portfolio]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de programas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolio] &gt;[!UICONTROL seleccionar un portafolio] &gt;[!UICONTROL Programas]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL Programas]</p> </li> 
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
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar un proyecto] &gt; [!UICONTROL Tareas]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL seleccionar una tarea] &gt;[!UICONTROL Subtareas]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL seleccionar una tarea] &gt; [!UICONTROL Predecesores*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de problemas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt; [!UICONTROL seleccionar] un proyecto &gt;[!UICONTROL Problemas]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL seleccionar una tarea] &gt; [!UICONTROL Problemas]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL seleccionar una tarea] &gt;[!UICONTROL Subtareas] &gt;[!UICONTROL seleccionar una tarea] &gt; [!UICONTROL Problemas]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de informes</td> 
   <td> 
    <ul> 
     <li> <p>  [!UICONTROL Informes]  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de paneles</td> 
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
     <li> <p>[!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Portfolio] &gt;[!UICONTROL seleccionar un portafolio] &gt; [!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Portfolio] &gt; [!UICONTROL seleccionar un portafolio] &gt;[!UICONTROL Programas] &gt;[!UICONTROL seleccionar un programa] &gt;[!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL seleccionar una tarea] &gt; [!UICONTROL Documentos]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt; [!UICONTROL seleccionar] un proyecto &gt; [!UICONTROL Problemas] &gt;[!UICONTROL seleccionar un problema] &gt; [!UICONTROL Documentos]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de hojas de horas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Hoja de horas] s &gt; [!UICONTROL Todas las hojas de horas]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de tarifas de facturación</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tarifas de facturación*]</p> </li> 
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
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar] un proyecto &gt;[!UICONTROL Gastos]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt; [!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL seleccionar una tarea] &gt;[!UICONTROL Gastos]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de entradas de horas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar] un proyecto</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar un proyecto] &gt;[!UICONTROL Tareas] &gt;[!UICONTROL seleccionar una tarea] &gt;[!UICONTROL Horas]</p> </li> 
     <li> <p>[!UICONTROL Proyectos] &gt;[!UICONTROL seleccionar] un proyecto &gt;[!UICONTROL Problemas] &gt;[!UICONTROL seleccionar] un problema &gt;[!UICONTROL Horas]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de formularios personalizados</td> 
   <td> 
    <ul> 
     <li>[!UICONTROL Configuración] &gt;[!UICONTROL Forms personalizado] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>Lista de grupos o subgrupos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuración] &gt;[!UICONTROL Grupos]</p> </li>
     <li> <p>[!UICONTROL Configuración] &gt;[!UICONTROL Grupos] &gt;[!UICONTROL seleccionar el grupo principal] &gt;[!UICONTROL Subgrupos] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Lista de equipos</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuración] &gt;[!UICONTROL Equipos]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de empresas</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuración] &gt;[!UICONTROL Compañías]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de horarios</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuración] &gt;[!UICONTROL Programaciones]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Lista de plantillas de diseño</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Configuración] &gt;[!UICONTROL Plantillas de diseño]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

No se puede personalizar la lista en el área especificada. Un administrador de [!DNL Workfront] puede generar una lista personalizada en el sistema o puede generar un informe para este objeto si su nivel de acceso le permite tener acceso para editar informes.

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
   <td><strong>[!UICONTROL Filtro]</strong></td> 
   <td> <p>Los filtros mantienen la información innecesaria fuera de una lista, según los criterios especificados. </p> <p>Para obtener más información, vea <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Resumen de filtros</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Ver]</strong></td> 
   <td> <p>Las vistas definen qué campos (columnas) se muestran en la pantalla.</p> <p>Para obtener más información, vea <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Información general sobre vistas en [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Agrupación]</strong></td> 
   <td> <p>Las agrupaciones separan los objetos de la lista en áreas basadas en los criterios especificados.</p> <p>Por ejemplo, los problemas de una lista pueden mostrarse en secciones por estado o prioridad.</p> <p>Puede tener hasta tres capas de agrupaciones en una agrupación estándar y puede agregar una cuarta capa si configura una agrupación en modo de texto.</p> <p>Para obtener más información acerca de las agrupaciones, vea <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Información general sobre agrupaciones en [!DNL Adobe Workfront]</a>.</p> <p>Para obtener más información acerca del modo de texto, vea <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Información general sobre el modo de texto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Estos elementos se muestran en la parte superior de cada lista de forma predeterminada. Son fijas y no se mueven a medida que se desplaza por la lista. Pase el ratón sobre el icono de cada elemento para identificarlos.

![](assets/nwe-list-elements.png)

Puede personalizar los elementos de la lista en las siguientes áreas y compartirlos con otros usuarios:

* Se encontró cualquier lista predeterminada del sistema en la sección [Introducción a las listas en [!DNL Adobe Workfront]](#default-workfront-lists) en este artículo
* Cualquier informe que se comparta con usted

Los elementos de creación para las listas son los mismos que para los informes.

Para obtener más información acerca de cómo crear y personalizar los elementos de creación de listas e informes, vea [Elementos de informes: filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

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
   <td> <p>Editar objetos y su información directamente en la lista.</p> <p>Para obtener más información, vea <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">Editar elementos en línea en una lista de [!DNL Adobe Workfront]</a>.</p> 
   <p><b>NOTA:</b></p>
   <p>La edición en línea no es posible en una agrupación.</p>

</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>Actualización con el [!UICONTROL Summary]</strong> </td> 
   <td> <p>Actualizar tareas y problemas en el nivel de proyecto mediante el panel [!UICONTROL Summary].</p> <p><b>SUGERENCIA:</b></p> <p>El resumen no está disponible para todos los objetos y no está disponible en los informes de Tareas o Problemas.</p> <p>Para obtener más información, consulte <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Resumen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Personalizar visualización de lista</strong> </td> 
   <td> <p>Personalice el aspecto de una lista, la disposición de columnas, el orden de clasificación de los elementos o el número de elementos que se muestran.</p> <p><b>NOTA:</b></p> <p>Los cambios que realice en el número de elementos que se mostrarán en una página se revertirán cuando cierre la sesión de [!DNL Workfront] o el explorador. Los cambios también se pueden revertir después de un período de 8 horas.</p> <p>Para obtener más información, vea <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">Modificar la presentación de una lista</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Filtro rápido</strong> </td> 
   <td> <p>Aplique un filtro rápido para buscar sólo los elementos que son importantes para usted, de modo que pueda revisarlos, actualizarlos o compartirlos rápidamente con otros.</p> <p><b>IMPORTANTE:</b></p> <p> Puede buscar elementos que contengan una palabra de búsqueda mediante el filtro rápido, independientemente de si ese elemento está visible en la pantalla o se mostrará después de desplazarse hasta la parte inferior de la página. Cuando utiliza las funciones de búsqueda del explorador, solo puede encontrar elementos que ya están visibles en la pantalla. Si la lista tiene varias páginas, los filtros rápidos sólo encontrarán los elementos de la página actual.</p> <p>Para obtener más información, vea <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Aplicar el filtro rápido a una lista</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Exportar</strong> </td> 
   <td> <p>Exportar una lista de objetos de [!DNL Workfront]. Cuando una lista contiene más de 2000 elementos, exportar la lista es la única manera de revisar todos los elementos de una página.</p> <p>Para obtener más información acerca de cómo exportar una lista, vea <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">Exportar una lista</a>. Para obtener más información sobre los formatos y límites de exportación, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportar datos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Barra de herramientas Lista

En la tabla siguiente se enumeran muchos de los iconos disponibles en la barra de herramientas y se indica lo que sucede cuando se hace clic en ellos:

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
   <td>Abra más opciones, incluido agregar un nuevo elemento o usuario.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insertar tarea arriba]</td> 
   <td> <p>Insertar una tarea encima de la tarea seleccionada.</p> <p>Esto solo está disponible para tareas. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insertar tarea debajo]</td> 
   <td> <p>Insertar una tarea debajo de la tarea seleccionada.</p> <p>Esto solo está disponible para tareas. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[!UICONTROL Editar]</td> 
   <td>Editar el elemento seleccionado.</td> 
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
   <td>[!UICONTROL Sangrar y anular sangría de tareas] </td> 
   <td> <p>Aplicar sangría o anular sangría a la tarea seleccionada. </p> <p>Esto solo está disponible para tareas. </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[!UICONTROL Más]</td> 
   <td>Abrir opciones adicionales para el elemento seleccionado.</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[!UICONTROL Filtro rápido] </p> </td> 
   <td> <p>Abra el cuadro de búsqueda de filtros rápidos para buscar elementos en la lista mostrada.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[!UICONTROL Export]</td> 
   <td>Exporte la lista a archivos de PDF, Excel o delimitados por tabuladores.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Vista de Agile]</td> 
   <td>Mostrar la lista en la vista de Agile.<br>Esto solo está disponible para tareas.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>Diagrama de Gantt de [!UICONTROL]</td> 
   <td> <p>Mostrar la lista en la vista [!UICONTROL Gantt Chart].</p> <p>Esto solo está disponible para proyectos y tareas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>Menú desplegable [!UICONTROL Filtro]</td> 
   <td> <p>Mostrar una lista de filtros y opciones adicionales para administrar filtros, incluido el proceso de creación de uno. </p> <p>En una pantalla pequeña, el nombre del filtro se reemplaza por el icono de filtro. Aparece un punto azul en el icono Filtro cuando se aplica cualquier filtro que no sea "[!UICONTROL All]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menú desplegable de [!UICONTROL View]</td> 
   <td> <p>Mostrar una lista de vistas y opciones adicionales para administrar vistas, incluida la creación de una. </p> <p>En una pantalla pequeña, el nombre de la vista se reemplaza por el icono [!UICONTROL view]. Aparece un punto azul en el icono [!UICONTROL View] cuando se aplica cualquier vista distinta de "[!UICONTROL Standard]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menú desplegable [!UICONTROL Grouping]</td> 
   <td> <p>Mostrar una lista de agrupaciones y opciones adicionales para administrar agrupaciones, incluida la creación de una. </p> <p>En una pantalla pequeña, el nombre de agrupación se reemplaza por el icono [!UICONTROL grouping]. Aparece un punto azul en el icono [!UICONTROL Agrupación] cuando se aplica cualquier agrupación que no sea "[!UICONTROL Nada]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL Modo de plan]</p> </td> 
   <td> <p>Elija si desea guardar los cambios realizados en una lista de tareas de forma automática o manual. </p> <p>Para obtener información acerca de la edición de tareas en una lista, vea <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Editar tareas en una lista</a>. </p> <p>Esto solo está disponible para tareas.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[!UICONTROL Resumen]</td> 
   <td> <p>Muestra u oculta el cuadro [!UICONTROL Summary] para el elemento seleccionado.</p> <p>Esto solo está disponible para tareas y problemas.</p> <p>Para obtener información acerca del panel [!UICONTROL Summary], consulte <a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Resumen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL Quitar]</td> 
   <td>Elimine algo de la lista. Por ejemplo, como administrador de un grupo que administra las pertenencias a grupos o subgrupos, quite un miembro del grupo como se explica en <a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">Ver y administrar las pertenencias a grupos</a>.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[!UICONTROL Comentario] /[!UICONTROL Actualización]</td> 
   <td> <p>Escriba un comentario o una actualización.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Diferencia entre listas e informes

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
   <td>✓ <span>*</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Solamente un administrador de [!DNL Workfront] y usuarios con una licencia de [!UICONTROL Plan] pueden crearlos</p> </td> 
   <td> </td> 
   <td>✓ ** de</td> 
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
   <td> <p>Puede compartirlos con otros usuarios</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puede compartirlos en todo el sistema</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Puede compartirlos fuera del sistema</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Puede exportar a los formatos .pdf, [!DNL Excel] y Delimitado por tabuladores</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Puede programarlos para su envío en un correo electrónico</p> </td> 
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
   <td> <p>Puede agregarlos a un panel</p> </td> 
   <td> ✓ *** de </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puede utilizar indicadores para personalizar lo que muestran</p> </td> 
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

Debe tener acceso a los filtros, vistas y agrupaciones para poder crearlos. Para obtener más información, consulte [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

Debe tener acceso a los filtros, vistas y agrupaciones, así como a los informes, tableros y calendarios, para poder crearlos. Para obtener más información, consulte [Conceder acceso a informes, paneles y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Puede personalizar listas para informes que se colocan en un panel solo si el creador del informe ha configurado los elementos de la lista para que sean visibles en el panel.

>[!NOTE]
>
>No puede agregar una lista a un panel sin crear un informe y agregarlo primero al panel.

Para obtener más información sobre cómo generar un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Para obtener información acerca de cómo crear secciones personalizadas , vea [Crear fichas o secciones personalizadas](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## La diferencia entre las listas actualizadas y las heredadas

Hay dos tipos de listas en [!DNL Workfront]:

* Listas heredadas

  ![](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* Listas actualizadas

  ![](assets/updated-list-screen-shot-gray-groupings-350x71.png)

La tabla siguiente muestra algunas de las diferencias entre las listas heredadas y actualizadas de [!DNL Workfront]:

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
  <td> <p>Mostrar <strong>100</strong> elementos de forma predeterminada</p> </td> 
   <td> <p>Mostrar <strong>Todos</strong> o hasta <strong>2000</strong> elementos de forma predeterminada</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilice CTRL+F para buscar elementos en una lista</p> </td> 
   <td> <p>Utilice filtros rápidos para buscar información rápidamente en una lista grande</p> <p>Para obtener información acerca del uso de filtros rápidos en listas, vea <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Aplicar el filtro rápido a una lista</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>No puede editar en línea campos personalizados con formato de texto enriquecido.</td> 
   <td> <p>El texto de los campos personalizados con formato se puede configurar para que incluya negrita, cursiva, subrayado, viñetas, numeración, hipervínculos y comillas de bloque.</p> <p>Para obtener más información, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Crear un formulario personalizado</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>El formato condicional puede cambiar el color del texto de los vínculos de una lista</td> 
   <td>No se pueden aplicar cambios de color de texto a los vínculos de una lista</td> 
  </tr> 
 </tbody> 
</table>
