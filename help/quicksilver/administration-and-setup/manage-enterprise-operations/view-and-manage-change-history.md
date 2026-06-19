---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Historial de cambios
description: El historial de cambios permite ver un registro de los cambios realizados en los objetos Workfront
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 44292bc9cf8654d1ecfb398b0f118a6c001f544f
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 8%

---

# Ver y administrar el historial de cambios

Puede ver el historial de cambios, incluidos los registros de auditoría, en el área Seguimiento de cambios de Configuración.

* **Registros de auditoría** son cambios activados por los usuarios.
Para obtener más información sobre los registros de auditoría y el área de registros de auditoría, consulte [Resumen de los registros de auditoría](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md)
* **Configuración** muestra qué campo se está rastreando para la lista Historial de cambios.
Actualmente, la configuración solo está disponible como información y no se puede cambiar. La capacidad de cambiar los campos de los que se realiza un seguimiento estará disponible en un futuro próximo.
* La lista Historial de cambios permite ver un registro de los cambios realizados en los objetos de Workfront, incluidos atributos como:

   * Objeto
   * Tipo de objeto
   * Tipo de cambio (operación)
   * Source del cambio, como usuarios específicos, API, Workfront Fusion, AI LLM o el sistema de Workfront

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de Workfront para ver el historial de cambios</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver y administrar registros de auditoría

Para ver y administrar registros de auditoría, vea [Ver y exportar registros de auditoría](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Ver el área Configuración para el seguimiento de cambios

>[!NOTE]
>
>Actualmente, la configuración solo está disponible como información y no se puede cambiar. La capacidad de cambiar los campos de los que se realiza un seguimiento estará disponible en un futuro próximo.

Para ver los tipos de cambios de los que se realiza un seguimiento:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Seguimiento de cambios** ![Icono de historial de cambios](assets/change-history-icon.png).
1. Haga clic en **Configuración**.

   Los campos se muestran agrupados por tipo de objeto.

1. Para mostrar campos debajo de un objeto específico, haga clic en la flecha desplegable situada junto al tipo de objeto.

## Ver la lista Historial de cambios

Los administradores de Workfront pueden ver el historial de cambios en el área de Configuración.

La lista Historial de cambios es una lista mejorada que incluye filtros, columnas, altura de fila, un selector de fechas y una barra de búsqueda.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Seguimiento de cambios** ![Icono de historial de cambios](assets/change-history-icon.png).
1. Haga clic en **Cambiar lista de historial**.

   Se abrirá la lista Historial de cambios.

1. Para ajustar las fechas para las que se muestran cambios, haga clic en el selector de fechas y seleccione las nuevas fechas.

   Los cambios están disponibles durante los últimos 90 días.
1. Para buscar un término específico, haga clic en la barra de búsqueda e introduzca el término. Los resultados se filtran a medida que escribe.
1. (Opcional) Para filtrar por una columna, consulte [Filtrar elementos de una lista mejorada](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list) en el artículo Usar listas mejoradas.
1. (Opcional) Para ocultar, mostrar o reordenar columnas, consulte [Personalizar columnas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns) en el artículo Usar listas mejoradas.
1. Para agregar o quitar columnas, vea [Agregar y quitar columnas con el Administrador de columnas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) en el artículo Usar listas mejoradas.
1. Para ajustar el alto de fila, vea [Cambiar el alto de fila en una vista](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view) en el artículo Usar listas mejoradas.





