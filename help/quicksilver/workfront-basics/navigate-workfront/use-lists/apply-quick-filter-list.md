---
navigation-topic: use-lists
title: Aplicar el filtro rápido a una lista
description: Puede utilizar el filtro rápido en una lista de objetos para que sólo le ayude a localizar los elementos que son importantes para usted, de modo que pueda revisarlos, actualizarlos o compartirlos rápidamente con otras personas.
feature: Get Started with Workfront
author: Nolan
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 261ac44eb0d13ffbd61a2c70213adb591bf018aa
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Aplicar el filtro rápido a una lista

<!--Audited:11/2024-->

Puede utilizar el filtro rápido en una lista de objetos para que sólo le ayude a localizar los elementos que son importantes para usted, de modo que pueda revisarlos, actualizarlos o compartirlos rápidamente con otras personas.

>[!IMPORTANT]
>
>Puede buscar elementos que contengan una palabra de búsqueda mediante filtros rápidos, tanto si el elemento se ha mostrado físicamente en la pantalla como si se mostrará después de desplazarse hasta la parte inferior de la página. Cuando utiliza las capacidades de búsqueda del explorador, solo puede encontrar elementos que se muestran físicamente en la pantalla. Si la lista tiene varias páginas, los filtros rápidos no encuentran elementos que se encuentren en páginas que no se muestran.

Si desea guardar un filtro rápido, le recomendamos que cree un filtro permanente para la lista.\
Para obtener información acerca de cómo generar filtros en [!DNL Adobe Workfront], vea el artículo [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

El filtro rápido está disponible actualmente en las siguientes áreas


Puede utilizar filtros rápidos temporales en todas las listas, excepto en las siguientes:

* El área [!UICONTROL Informes]
* Listas de documentos e informes
* Varias áreas de [!UICONTROL instalación]

  >[!NOTE]
  >
  >Los filtros rápidos están disponibles en las siguientes áreas de configuración: [!UICONTROL Grupos], [!UICONTROL Equipos], [!UICONTROL Compañías], [!UICONTROL Horarios], [!UICONTROL Plantillas de diseño] y [!UICONTROL Forms personalizado].


Tenga en cuenta lo siguiente al aplicar filtros rápidos a una lista:

* Puede utilizar palabras clave para filtrar cualquier campo que se muestre en la vista de la lista. Esto incluye campos personalizados o campos complejos como [!UICONTROL Predecesoras], [!UICONTROL Asignaciones], [!UICONTROL Asignación] y [!UICONTROL Estado], [!UICONTROL Aprobador] y [!UICONTROL Estado], etc.
* Si la lista tiene agrupaciones contraídas, se expanden automáticamente al utilizar filtros rápidos. Al eliminar el filtro rápido, las agrupaciones se contraen de nuevo.
* Las agrupaciones conservan la información agregada de la lista original independientemente de los filtros rápidos aplicados o de los cambios realizados en los objetos de la lista.
* Los filtros rápidos son temporales. Al cambiar la agrupación, la vista, el filtro o el orden de la lista, se eliminan los criterios de filtro rápido.
* No se puede guardar un filtro rápido. Si desea guardar un filtro para utilizarlo de nuevo, considere la posibilidad de crear un filtro permanente para la lista.
* Si tiene más de una agrupación en la lista y el filtro rápido encuentra elementos en una única agrupación, sólo se mostrará esa agrupación con los elementos encontrados. Todas las demás agrupaciones están ocultas.
* En una tarea o lista de subtareas, la jerarquía de tareas se quita cuando se muestran los resultados del filtro rápido.

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
   <td> <p>Ver el acceso al área en la que se encuentra la lista</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de [!UICONTROL View] para el objeto en el que se encuentra la lista</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Aplicación de un filtro rápido a una lista

1. Vaya a una lista o informe que admita filtros rápidos y luego haga clic en el icono **[!UICONTROL Filtro rápido]** ![](assets/qs-quick-filter-icon.png) de la barra de herramientas.

   O

   Según el sistema operativo o el navegador y cuando utilice un teclado QWERTY estándar, pulse el siguiente conjunto de comandos para iniciar el filtro rápido:

   * ALT+F para [!DNL Windows] equipos
   * ALT/ Opción + F para [!DNL Mac] equipos

     >[!TIP]
     >
     >Si presiona CTRL+F o CMD+F, aparece información sobre herramientas junto al filtro rápido para recordarle estos comandos. Los comandos también se muestran dentro del cuadro de búsqueda de filtro rápido.

1. En el cuadro **[!UICONTROL Filtrar página]**, escriba la palabra clave por la que desee filtrar.

   Puede utilizar cualquier palabra que se muestre actualmente en la vista de la lista.

   >[!NOTE]
   >
   >Si utiliza una palabra que podría mostrarse en otra página de la lista, el filtro rápido no encuentra ningún resultado.

   Una lista de elementos que coinciden con los criterios de búsqueda se muestra dinámicamente en la lista a medida que escribe y todos los demás elementos están ocultos. La palabra clave utilizada en la búsqueda se resaltará en amarillo en todos los campos independientes y complejos. Algunos ejemplos de campos complejos son columnas compartidas o cualquiera de los siguientes: [!UICONTROL Asignaciones], [!UICONTROL Asignaciones] y [!UICONTROL Estado], [!UICONTROL Porcentaje completado], [!UICONTROL Predecesoras], [!UICONTROL Aprobadores y estado], [!UICONTROL Administradores de recursos], [!UICONTROL Categorías], [!UICONTROL Condición], [!UICONTROL Actualización de condición], etc.

1. (Opcional) Para editar de forma masiva los elementos encontrados por el filtro rápido:

   1. Seleccione todos o varios de los elementos de la lista y, a continuación, haga clic en **[!UICONTROL Editar]** para editar los elementos en lote.
   1. Después de completar las ediciones, haga clic en **[!UICONTROL Guardar cambios]**.

1. (Opcional) Para exportar los elementos encontrados por el filtro rápido, seleccione todos o varios de los elementos de la lista y, a continuación, haga clic en el icono **[!UICONTROL Exportar]** ![](assets/export.png).

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Solo los elementos que encontró en la búsqueda de filtro rápido se exportan al archivo seleccionado. Si no selecciona ningún elemento antes de exportar la lista, se exporta la lista completa sin filtrar.\
   >Para obtener más información, vea [Exportar una lista](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Opcional) Para borrar los resultados filtrados, haga clic en el icono **[!UICONTROL Filtro rápido]** en la esquina superior derecha de la ventana.
O
Actualice la página.
