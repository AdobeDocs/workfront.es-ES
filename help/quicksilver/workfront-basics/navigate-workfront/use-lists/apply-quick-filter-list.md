---
navigation-topic: use-lists
title: Aplicar el filtro rápido a una lista
description: Puede utilizar el filtro rápido en una lista de objetos para localizar solo elementos que sean importantes para usted, de modo que pueda revisarlos, actualizarlos o compartirlos rápidamente con otros usuarios.
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# Aplicar el filtro rápido a una lista

<!--
{{highlighted-preview}}
-->

Puede utilizar el filtro rápido en una lista de objetos para localizar solo elementos que sean importantes para usted, de modo que pueda revisarlos, actualizarlos o compartirlos rápidamente con otros usuarios.

>[!IMPORTANT]
>
>Puede encontrar elementos que contengan una palabra de búsqueda mediante filtros rápidos, tanto si el elemento se ha mostrado físicamente en la pantalla como si se mostrará después de desplazarse hasta la parte inferior de la página. Al utilizar las funciones de búsqueda del explorador, solo puede encontrar los elementos que se muestran físicamente en la pantalla. Si la lista tiene varias páginas, los filtros rápidos no encuentran elementos que estén en páginas que no se muestran.

Si desea guardar un filtro rápido, le recomendamos que cree un filtro permanente para la lista.\
Para obtener información sobre cómo crear filtros en [!DNL Adobe Workfront], consulte el artículo [Información general sobre filtros en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

El filtro rápido está disponible actualmente en las siguientes áreas


Puede utilizar filtros rápidos temporales en todas las listas, excepto en las siguientes:

* La variable [!UICONTROL Informes] area
* Listas de documentos e informes
* Varios [!UICONTROL Configuración] áreas
   >[!NOTE]
   >
   >Los filtros rápidos están disponibles en las siguientes áreas de configuración: [!UICONTROL Grupos], [!UICONTROL Equipos], [!UICONTROL Compañías], [!UICONTROL Programaciones], [!UICONTROL Plantillas de diseño]y [!UICONTROL Forms personalizado].


Tenga en cuenta lo siguiente al aplicar filtros rápidos a una lista:

* Puede utilizar palabras clave para filtrar por cualquier campo que se muestre en la vista de la lista. Esto incluye campos personalizados o campos complejos como [!UICONTROL Predecesores], [!UICONTROL Asignaciones], [!UICONTROL Asignación] y [!UICONTROL Estado], [!UICONTROL Aprobador] y [!UICONTROL Estado], etc.
* Si la lista ha contraído agrupaciones, estas se expanden automáticamente cuando utiliza filtros rápidos. Al quitar el filtro rápido, las agrupaciones se contraen de nuevo.
* Los grupos conservan la información agregada de la lista original independientemente de los filtros rápidos aplicados o de los cambios realizados en los objetos de la lista.
* Los filtros rápidos son temporales. Si se cambia la agrupación, la vista, el filtro o el orden de la lista, se eliminarán los criterios de filtro rápido.
* No puede guardar un filtro rápido. Si desea guardar un filtro para volver a utilizarlo, considere la posibilidad de crear un filtro permanente para la lista.
* Si tiene más de una agrupación en la lista y el filtro rápido encuentra elementos en una sola agrupación, solo esa agrupación se muestra con los elementos encontrados. Todas las demás agrupaciones están ocultas.
* En una lista de tareas o subtareas, la jerarquía de tareas se elimina cuando se muestran los resultados del filtro rápido.

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
   <td> <p>Ver acceso al área en la que se encuentra la lista</p> <p>Por ejemplo, para aplicar un filtro rápido a un proyecto, necesita acceso de [!UICONTROL View] a Proyectos.</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso.<br>Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Permisos de objeto</b></td> 
   <td> <p>[!UICONTROL View]</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Aplicar un filtro rápido a una lista

1. Vaya a una lista o informe que admita filtros rápidos y, a continuación, haga clic en el **[!UICONTROL Filtro rápido] icono** ![](assets/qs-quick-filter-icon.png) en la barra de herramientas.

   O

   Según el sistema operativo o navegador y cuando utilice un teclado QWERTY estándar, presione el siguiente conjunto de comandos para iniciar el filtro rápido:

   * ALT+F para [!DNL Windows] equipos
   * ALT/ Opción+F para [!DNL Mac] equipos

      >[!TIP]
      >
      >Si pulsa CTRL+F o CMD+F, aparece una información sobre herramientas junto al filtro rápido para recordarle estos comandos. Los comandos también se muestran dentro del cuadro de búsqueda de filtro rápido.

1. En el **[!UICONTROL Filtrar página]** , introduzca la palabra clave por la que desea filtrar.

   Puede utilizar cualquier palabra que se muestre actualmente en la vista de la lista.

   >[!NOTE]
   >
   >Si utiliza una palabra que podría aparecer en otra página de la lista, el filtro rápido no encontrará ningún resultado.

   Una lista de elementos que coinciden con los criterios de búsqueda se muestra en la lista de forma dinámica a medida que escribe y el resto de elementos están ocultos. La palabra clave utilizada en la búsqueda se resalta en amarillo en todos los campos independientes y complejos. Algunos ejemplos de campos complejos son columnas compartidas o cualquiera de los siguientes: [!UICONTROL Asignaciones], [!UICONTROL Asignaciones] y [!UICONTROL Estado], [!UICONTROL Porcentaje completado], [!UICONTROL Predecesores], [!UICONTROL Aprobadores y estado], [!UICONTROL Administradores de recursos], [!UICONTROL Categorías], [!UICONTROL Condición], [!UICONTROL Actualización de condición], etc.

1. (Opcional) Para editar de forma masiva los elementos que encuentra el filtro rápido:

   1. Seleccione todos o varios elementos de la lista y haga clic en **[!UICONTROL Editar]** para editar los elementos de forma masiva.
   1. Después de completar las ediciones, haga clic en **[!UICONTROL Guardar cambios]**.

1. (Opcional) Para exportar los elementos que encuentra el filtro rápido, seleccione todos o varios de los elementos de la lista y haga clic en **[!UICONTROL Exportar]**.

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Solo los elementos que haya encontrado en la búsqueda de filtro rápido exportan al archivo seleccionado. Si no selecciona ningún elemento antes de exportar la lista, se exporta la lista completa sin filtrar.\
   >Para obtener más información, consulte [Exportación de una lista](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Opcional) Para borrar los resultados filtrados, haga clic en el **[!UICONTROL Filtro rápido]** en la esquina superior derecha de la ventana.\
   O\
   Actualice la página.
