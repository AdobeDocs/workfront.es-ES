---
user-type: administrator
product-area: system-administration;setup
title: Ver y administrar el historial de cambios
description: El historial de cambios permite ver un registro de los cambios realizados en los objetos y campos de Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 100b900bd7419d78a3135358026ec5e27755fdeb
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 6%

---

# Ver y administrar el historial de cambios

{{preview-fast-release-general}}

El historial de cambios le permite configurar y realizar un seguimiento de los cambios realizados en objetos y campos específicos de Adobe Workfront. La configuración flexible permite configurar qué objetos y campos exactamente desea rastrear.

El historial de cambios puede realizar un seguimiento de los siguientes tipos de datos definidos:

* Actividad en el área de Configuración, como crear o eliminar un nivel de acceso o un rol
* Actualizaciones de nivel de campo, como editar una descripción de proyecto o cambiar la plantilla de diseño de un usuario
* Actualizaciones de objetos, como actualizar el estado de un proyecto o adjuntar un formulario personalizado a una tarea
* <span class="preview">Actividad de flujo de trabajo de revisión y aprobación unificadas, que incluye participantes y decisiones</span>

Para obtener información sobre cómo definir qué objetos y campos se rastrean, vea [Configurar campos para rastrearlos en el historial de cambios](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md).

En la lista Historial de cambios, puede ver el registro de cambios realizados en los objetos de Workfront, incluidos atributos como:

* Nombre de objeto
* Tipo de objeto
* Tipo de cambio (operación)
* Fecha y hora del cambio
* Source del cambio, como usuarios específicos, API, Workfront Fusion, AI LLM o el sistema de Workfront

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td><span class="preview">Acceso administrativo al historial de cambios</span></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
## View the Configuration area for change tracking

>[!NOTE]
>
>In the Production environment, Configuration is currently available only as information and cannot be changed. The ability to change which fields are tracked will be available in the near future.

To view the types of changes that are tracked: 

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > Configuration**.
   
   Fields are displayed grouped by object type.

1. To display fields under a specific object, click the dropdown arrow next to the object type.
-->


## Ver la lista Historial de cambios

Puede ver los registros del historial de cambios en el área de Configuración.

La lista Historial de cambios es una lista mejorada que incluye filtros, columnas, altura de fila, un selector de fechas y una barra de búsqueda.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Seguimiento de cambios > Lista de historial de cambios**.

   Se abrirá la lista Historial de cambios.

1. Para ajustar las fechas para las que se muestran cambios, haga clic en el selector de fechas y seleccione las nuevas fechas.

   Los cambios están disponibles durante los últimos 90 días.

1. Para buscar un término específico, haga clic en el cuadro de búsqueda e introduzca el término. Los resultados se resaltan en la lista a medida que escribe.
1. (Opcional) Para filtrar por una columna, consulte [Filtrar elementos de una lista mejorada](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list) en el artículo [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Opcional) Para ocultar, mostrar o reordenar columnas, consulte [Personalizar columnas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns) en el artículo [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Opcional) Para agregar o quitar columnas, consulte [Agregar y quitar columnas con el Administrador de columnas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) en el artículo [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Opcional) Para ajustar el alto de fila, consulte [Cambiar el alto de fila en una vista](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view) en el artículo [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Exportar historial de cambios

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Seguimiento de cambios > Lista de historial de cambios**.
1. Filtre la lista para mostrar los elementos que desea exportar.
1. Haga clic en el icono **Exportar** ![Icono de exportar](assets/export-icon.png) y seleccione si desea guardar en formato XLSX o CSV.

   Se abrirá el cuadro Guardar archivo y podrá guardar el archivo exportado en el equipo.
   Termine de guardar el archivo exportado. Ahora puede encontrarlo en el equipo y compartirlo con otros usuarios.



