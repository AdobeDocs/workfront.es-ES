---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Historial de cambios
description: El historial de cambios permite ver un registro de los cambios realizados en los objetos Workfront
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: de1f426630b8c99cfaca07dafb9c2de0f16f263f
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 4%

---

# Ver y administrar el historial de cambios

{{preview-fast-release-general}}

Puede ver el historial de cambios, incluidos los registros de auditoría, en el área Seguimiento de cambios de Configuración.

* **Registros de auditoría** son cambios activados por los usuarios.
Para obtener más información sobre los registros de auditoría y el área de registros de auditoría, vea [Resumen de los registros de auditoría](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md) y [Ver y exportar registros de auditoría](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).
* **Configuración** muestra qué campos se están rastreando para la lista Historial de cambios.
  <span class="preview">Como administrador de Workfront, puede configurar qué acciones y campos de objeto rastrea Workfront. Por ejemplo, puede hacer que Workfront rastree todos los cambios que los usuarios realizan en los nombres de los problemas en todo el sistema. Cualquier cambio de nombre de problema aparecerá como una entrada en el registro del historial de cambios.</span>

* **Lista de historial de cambios** le permite ver un registro de los cambios realizados en los objetos de Workfront, incluidos atributos como:

  * Objeto
  * Tipo de objeto
  * Tipo de cambio (operación)
  * Source del cambio, como usuarios específicos, API, Workfront Fusion, AI LLM o el sistema de Workfront

  <span class="preview">La actividad de flujo de trabajo de revisión y aprobación unificadas se rastrea en Historial de cambios, incluidos los participantes y las decisiones.</span>

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
   <td><p>Administrador del sistema</p>
       <p><span class="preview">Para ver el historial de cambios: Acceso administrativo al historial de cambios</span></p>
       <p><span class="preview">Para configurar campos rastreados: Administrador del sistema</span></p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<div class="preview">

## Añada los campos que desee rastrear

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Seguimiento de cambios > Configuración**.
1. En la pantalla Configuración, haga clic en **Agregar campo**.
1. En el cuadro **Agregar campos**, seleccione un objeto. Puede empezar a escribir el nombre del objeto y, a continuación, seleccionarlo cuando aparezca en la lista.
1. A continuación, seleccione los nombres de campo que desea rastrear para ese objeto. Se puede escribir el nombre del campo y, a continuación, seleccionarlo cuando aparezca en la lista.

   Tanto los campos personalizados como los campos nativos están disponibles para el objeto.
   Los campos que ya se están rastreando se muestran como seleccionados en la lista.

   ![Agregar campos para el seguimiento de cambios](assets/change-history-config-add-fields.png)

1. Después de seleccionar todos los campos que desea rastrear, haga clic en **Agregar**.

   Los campos se agregan a la lista Campos rastreados.

## Elimine los campos de los que ya no desea realizar un seguimiento

Puede eliminar campos que no desee que el sistema rastree para un tipo particular de objeto en toda la interfaz de Workfront.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Seguimiento de cambios > Configuración**.
1. En la pantalla Configuración, seleccione el campo o campos sobre los que desea detener el seguimiento.

   Puede ver el mismo nombre de campo más de una vez. Los campos se agrupan por objeto para que pueda localizar el campo correcto. También puede utilizar el cuadro de búsqueda en la parte superior de la pantalla.

1. Seleccione **Eliminar** en la barra de acciones de la parte inferior de la pantalla.
1. Haz clic en **Quitar** en el mensaje de confirmación.

   Los campos se quitan de la lista Campos rastreados.

</div>

## Ver el área Configuración para el seguimiento de cambios

>[!NOTE]
>
>En el entorno de producción, la configuración solo está disponible como información y no se puede cambiar. La capacidad de cambiar los campos de los que se realiza un seguimiento estará disponible en un futuro próximo.

Para ver los tipos de cambios de los que se realiza un seguimiento:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Seguimiento de cambios >** Configuración**.

   Los campos se muestran agrupados por tipo de objeto.

1. Para mostrar campos debajo de un objeto específico, haga clic en la flecha desplegable situada junto al tipo de objeto.

## Ver la lista Historial de cambios

Los administradores de Workfront pueden ver el historial de cambios en el área de Configuración.

La lista Historial de cambios es una lista mejorada que incluye filtros, columnas, altura de fila, un selector de fechas y una barra de búsqueda.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Seguimiento de cambios > Lista de historial de cambios**.

   Se abrirá la lista Historial de cambios.

1. Para ajustar las fechas para las que se muestran cambios, haga clic en el selector de fechas y seleccione las nuevas fechas.

   Los cambios están disponibles durante los últimos 90 días.

1. Para buscar un término específico, haga clic en la barra de búsqueda e introduzca el término. Los resultados se resaltan en la lista a medida que escribe.
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



