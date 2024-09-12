---
title: Personalización de filtros, vistas y agrupaciones mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador de Workfront, puede utilizar una plantilla de diseño para especificar qué controles de lista aparecen en los menús desplegables Filtrar, Ver y Agrupar. Estos menús aparecen encima de las listas en Workfront, como la lista de tareas de un proyecto.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: e9b61da8-2eca-4d88-969b-ae337e402540
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Personalización de filtros, vistas y agrupaciones mediante una plantilla de diseño

Como administrador de Adobe Workfront, puede utilizar una plantilla de diseño para especificar qué controles de lista aparecen en los menús desplegables Filtrar, Ver y Agrupar. Estos menús aparecen encima de las listas en Workfront, como la lista de tareas de un proyecto:

![](assets/filter-view-grouping-layout-templates.png)

Para obtener más información acerca de las plantillas de diseño, vea [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Para obtener información acerca de las plantillas de diseño para grupos, vea [Crear y modificar plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Después de configurar una plantilla de diseño, debe asignarla a usuarios para que los cambios que ha realizado sean visibles para otros. Para obtener información acerca de cómo asignar una plantilla de diseño a los usuarios, vea [Asignar usuarios a una plantilla de diseño](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td><p>Nuevo: estándar</p>
  <p> Actual: plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.
Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar controles de lista de filtro, vista y agrupación:

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Haga clic en la flecha abajo ![](assets/down-arrow-blue.png) bajo **Personalizar lo que ven los usuarios** y, a continuación, haga clic en **Listas** en el menú desplegable que se muestra.

   ![](assets/customize-what-users-see-dropdown-on-pg-adobe-branding.png)

1. Haga clic en la flecha abajo ![](assets/down-arrow-blue.png) bajo **Seleccione una lista para personalizar** y, a continuación, seleccione el tipo de objeto de Workfront para el que desea personalizar los controles de lista Filtrar, Ver y Agrupar.

   ![](assets/select-a-list-to-customize-menu-on-pg-adobe-branding.png)

   >[!NOTE]
   >
   >Si selecciona Proyectos como la lista que desea personalizar y, a continuación, deshabilita Proyectos en los que participo o Proyectos de mi propiedad en la sección Filtro, los usuarios ya no podrán ver ni utilizar ese filtro:
   >
   >* En la lista de filtros que se muestra al hacer clic en el icono de filtro ![](assets/filter-nwepng.png) sobre una lista:
   >   
   >  ![](assets/disable-filters-projects-im-on-or-own.png)
   >   
   >* En el encabezado del área Proyectos:
   >   
   >  ![](assets/disable-filter-pills.png)

1. (Opcional) Si desea cambiar el filtro, la vista o la agrupación predeterminados de la plantilla de diseño, pase el ratón sobre el filtro, la vista o la agrupación y, a continuación, haga clic en **Establecer como predeterminado**.

   Los valores predeterminados que elija determinan qué filtro, vista y agrupación verán los usuarios en las listas de Workfront cuando se les asigne la plantilla de diseño. Si no cambia estos valores predeterminados, los usuarios verán todas las listas de la siguiente manera:

   * **Filtros**: Todos
   * **Vista**: Estándar (donde corresponda; algunas listas no tienen esta vista)
   * **Agrupación**: Nada

   Puede ocultar las opciones Todos, Estándar y Nada después de seleccionar diferentes valores predeterminados (consulte el Paso 5), pero no se pueden eliminar.

   Puede eliminar cualquier otra opción que se utilice como predeterminada, pero primero debe seleccionar una predeterminada diferente.

   Para obtener información acerca de cómo eliminar filtros, vistas y agrupaciones, vea [Crear, editar y compartir filtros, vistas y agrupaciones predeterminados](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

1. Ocultar y agregar controles de lista como se indica a continuación:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ocultar un control de lista</td> 
      <td> <p>Desactive o marque la casilla situada junto al control de lista que desee ocultar o mostrar.</p> <p>Si una casilla de verificación está atenuada, no se puede ocultar ese control de lista. La configuración predeterminada <img src="assets/default-pill.png"> para cada control de lista está atenuada porque no se puede ocultar la configuración que está configurada actualmente como predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agregar un control de lista personalizado</td> 
      <td> <p> 
        <ol> 
         <li value="1"> Haga clic en <strong>Agregar filtro</strong>, <strong>Agregar vista</strong> o <strong>Agregar agrupación</strong> en la parte inferior de la lista Filtro, Vista o Agrupación. En el cuadro que aparece, empiece a escribir el nombre de un control de lista personalizado existente creado anteriormente para su organización y, a continuación, haga clic en el nombre cuando aparezca.</li> 
         <li value="2"> Si desea que el nuevo control de lista personalizado se establezca como filtro, vista o agrupación predeterminados para la plantilla de diseño, haga clic en <strong>Establecer como predeterminado</strong>. </li> 
         <li value="3"> <p>Haga clic en <strong>Agregar</strong> cuando haya terminado.</p> <p><b>NOTA</b>: <p>Los usuarios pueden agregar controles de lista personalizados a sus propias listas. Si agrega controles de lista personalizados a una plantilla de diseño, los controles de la lista se agregan y los suyos se mueven al final del panel; los suyos no reemplazan a los suyos.</p> <p>Esto también se cumple si asigna al usuario una nueva plantilla de diseño que tiene controles de lista personalizados. </p> <p>Para obtener información acerca de cómo personalizar los controles de lista, vea <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Resumen de filtros</a>, <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Resumen de vistas en Adobe Workfront</a> y <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Resumen de agrupaciones en Adobe Workfront</a>.</p> </p> </li> 
        </ol> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Siga personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **Guardar**.

   >[!TIP]
   >
   >Puede hacer clic en Guardar en cualquier momento para guardar el progreso y seguir modificando la plantilla más adelante.
