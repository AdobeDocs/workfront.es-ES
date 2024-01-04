---
navigation-topic: use-lists
title: Aplicar el filtro rápido a una lista
description: Puede utilizar el filtro rápido en una lista de objetos para que sólo le ayude a localizar los elementos que son importantes para usted, de modo que pueda revisarlos, actualizarlos o compartirlos rápidamente con otras personas.
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# Aplicar el filtro rápido a una lista

<!--
{{highlighted-preview}}
-->

Puede utilizar el filtro rápido en una lista de objetos para que sólo le ayude a localizar los elementos que son importantes para usted, de modo que pueda revisarlos, actualizarlos o compartirlos rápidamente con otras personas.

>[!IMPORTANT]
>
>Puede buscar elementos que contengan una palabra de búsqueda mediante filtros rápidos, tanto si el elemento se ha mostrado físicamente en la pantalla como si se mostrará después de desplazarse hasta la parte inferior de la página. Cuando utiliza las capacidades de búsqueda del explorador, solo puede encontrar elementos que se muestran físicamente en la pantalla. Si la lista tiene varias páginas, los filtros rápidos no encuentran elementos que se encuentren en páginas que no se muestran.

Si desea guardar un filtro rápido, le recomendamos que cree un filtro permanente para la lista.\
Para obtener información sobre cómo generar filtros en [!DNL Adobe Workfront], consulte el artículo [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

El filtro rápido está disponible actualmente en las siguientes áreas


Puede utilizar filtros rápidos temporales en todas las listas, excepto en las siguientes:

* El [!UICONTROL Informes] área
* Listas de documentos e informes
* Varios [!UICONTROL Configurar] áreas
  >[!NOTE]
  >
  >Los filtros rápidos están disponibles en las siguientes áreas de configuración: [!UICONTROL Grupos], [!UICONTROL Equipos], [!UICONTROL Compañías], [!UICONTROL Horarios], [!UICONTROL Plantillas de diseño], y [!UICONTROL Forms personalizado].


Tenga en cuenta lo siguiente al aplicar filtros rápidos a una lista:

* Puede utilizar palabras clave para filtrar cualquier campo que se muestre en la vista de la lista. Esto incluye campos personalizados o campos complejos como [!UICONTROL Predecesoras], [!UICONTROL Asignaciones], [!UICONTROL Asignación] y [!UICONTROL Estado], [!UICONTROL Aprobador] y [!UICONTROL Estado], etc.
* Si la lista tiene agrupaciones contraídas, se expanden automáticamente al utilizar filtros rápidos. Al eliminar el filtro rápido, las agrupaciones se contraen de nuevo.
* Las agrupaciones conservan la información agregada de la lista original independientemente de los filtros rápidos aplicados o de los cambios realizados en los objetos de la lista.
* Los filtros rápidos son temporales. Al cambiar la agrupación, la vista, el filtro o el orden de la lista, se eliminan los criterios de filtro rápido.
* No se puede guardar un filtro rápido. Si desea guardar un filtro para utilizarlo de nuevo, considere la posibilidad de crear un filtro permanente para la lista.
* Si tiene más de una agrupación en la lista y el filtro rápido encuentra elementos en una única agrupación, sólo se mostrará esa agrupación con los elementos encontrados. Todas las demás agrupaciones están ocultas.
* En una tarea o lista de subtareas, la jerarquía de tareas se quita cuando se muestran los resultados del filtro rápido.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] plan*</b></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] licencia*</b></td> 
   <td> <p>[!UICONTROL Request] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Configuraciones de nivel de acceso*</b></td> 
   <td> <p>Ver el acceso al área en la que se encuentra la lista</p> <p>Por ejemplo, para aplicar un filtro rápido a un proyecto, necesita el acceso de [!UICONTROL View] a Proyectos.</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso.<br>Para obtener información sobre cómo [!DNL Workfront] El administrador puede cambiar su nivel de acceso. Consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Permisos de objeto</b></td> 
   <td> <p>[!UICONTROL Ver]</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Aplicación de un filtro rápido a una lista

1. Vaya a una lista o informe que admita filtros rápidos y haga clic en el botón **[!UICONTROL Filtro rápido] icono** ![](assets/qs-quick-filter-icon.png) en la barra de herramientas.

   O

   Según el sistema operativo o el navegador y cuando utilice un teclado QWERTY estándar, pulse el siguiente conjunto de comandos para iniciar el filtro rápido:

   * ALT+F para [!DNL Windows] ordenadores
   * ALT/ Opción + F para [!DNL Mac] ordenadores

     >[!TIP]
     >
     >Si presiona CTRL+F o CMD+F, aparece información sobre herramientas junto al filtro rápido para recordarle estos comandos. Los comandos también se muestran dentro del cuadro de búsqueda de filtro rápido.

1. En el **[!UICONTROL Página de filtro]** , escriba la palabra clave por la que desea filtrar.

   Puede utilizar cualquier palabra que se muestre actualmente en la vista de la lista.

   >[!NOTE]
   >
   >Si utiliza una palabra que podría mostrarse en otra página de la lista, el filtro rápido no encuentra ningún resultado.

   Una lista de elementos que coinciden con los criterios de búsqueda se muestra dinámicamente en la lista a medida que escribe y todos los demás elementos están ocultos. La palabra clave utilizada en la búsqueda se resaltará en amarillo en todos los campos independientes y complejos. Algunos ejemplos de campos complejos son columnas compartidas o cualquiera de los siguientes: [!UICONTROL Asignaciones], [!UICONTROL Asignaciones] y [!UICONTROL Estado], [!UICONTROL Porcentaje completado], [!UICONTROL Predecesoras], [!UICONTROL Aprobadores y estado], [!UICONTROL Gerentes de recursos], [!UICONTROL Categorías], [!UICONTROL Condición], [!UICONTROL Actualización de condición], etc.

1. (Opcional) Para editar de forma masiva los elementos encontrados por el filtro rápido:

   1. Seleccione todos o varios de los elementos de la lista y haga clic en **[!UICONTROL Editar]** para editar los elementos de forma masiva.
   1. Una vez finalizadas las ediciones, haga clic en **[!UICONTROL Guardar cambios]**.

1. (Opcional) Para exportar los elementos encontrados por el filtro rápido, seleccione todos o varios de los elementos de la lista y haga clic en **[!UICONTROL Exportar]**.

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Solo los elementos que encontró en la búsqueda de filtro rápido se exportan al archivo seleccionado. Si no selecciona ningún elemento antes de exportar la lista, se exporta la lista completa sin filtrar.\
   >Para obtener más información, consulte [Exportar una lista](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Opcional) Para borrar los resultados filtrados, haga clic en **[!UICONTROL Filtro rápido]** en la esquina superior derecha de la ventana.\
   O\
   Actualice la página.
