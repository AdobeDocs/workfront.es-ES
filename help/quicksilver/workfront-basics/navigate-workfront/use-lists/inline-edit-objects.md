---
product-area: projects
navigation-topic: use-lists
title: Editar elementos en línea en una lista en  [!DNL Adobe Workfront]
description: Puede editar objetos en línea cuando se muestren en una lista o informe. Cuando se edita la información sobre los objetos mostrados en una lista o informe, el objeto se actualiza inmediatamente.
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: f0912e4ef29d682ae3e6dd0e543b8e77fb7f29b6
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# Editar elementos en línea en una lista de [!DNL Adobe Workfront]

Puede editar objetos en línea cuando se muestren en una lista o informe. Cuando se edita la información sobre los objetos mostrados en una lista o informe, el objeto se actualiza inmediatamente.

Cuando se edita en línea un campo contenido en un formulario personalizado que no está adjunto al objeto, el formulario personalizado se agrega automáticamente al objeto. Si el campo existe en varios formularios personalizados, el formulario personalizado que se haya actualizado más recientemente se adjuntará al objeto.

Para obtener más información sobre las listas, vea [Introducción a las listas en [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Aunque la mayoría de los objetos mostrados en listas o informes se pueden editar en línea en [!DNL Adobe Workfront], existen algunas limitaciones, entre las que se incluyen:

* No puede editar campos calculados o [!DNL Workfront] campos integrados que sean cálculos.
* Solo se pueden editar campos asociados directamente a los objetos de la lista. No se pueden editar campos que pertenezcan a objetos asociados con los objetos de la lista.\
   Por ejemplo, puede editar el estado de una tarea en un informe de tareas, pero no puede editar el nombre del proyecto con el que está asociada la tarea en el mismo informe. Solo se puede editar el nombre del proyecto en un informe de proyecto.
* No puede editar campos en línea cuando la vista de una lista no muestra la moneda predeterminada.\
   Para obtener información sobre cómo mostrar la moneda predeterminada, consulte la sección [Editar informes con monedas únicas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) en el artículo [Crear informes de datos financieros con tasas de cambio únicas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).
* No se pueden editar los indicadores e iconos mostrados en una lista.
* No puede editar en línea campos de informe que procedan de otros informes.

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
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Acceso de [!UICONTROL Edit] al área donde se encuentra la lista</p> <p>Por ejemplo, para editar en línea las tareas de un proyecto, necesita el acceso de [!UICONTROL Edit] a Proyectos.</p> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso.<br>Para obtener información sobre cómo un administrador de [!DNL Workfront] puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>[!UICONTROL Administrar]</p> <p>También debe tener permisos para editar ciertos campos, como campos personalizados, estado, etc.</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Edición de objetos en línea

1. Vaya a la lista de objetos que desea editar en línea.

   La lista debe mostrar campos que pertenecen a los objetos o campos que pertenecen a objetos asociados con los objetos de la lista.

1. Busque el objeto que desea editar y, a continuación, haga clic dentro de cualquier campo de la lista.

   >[!TIP]
   >
   >Si tiene varias páginas, puede localizar un objeto mediante:
   >
   >   
   >   
   >   * **Paginación**: haga clic en las flechas hacia atrás y hacia adelante para desplazarse entre las páginas.\
   >     Ubicado en la esquina inferior derecha de la lista, el área de [!UICONTROL paginación] permanece fija mientras se desplaza por la lista.
   >   * **Filtro rápido**: haga clic en el icono de filtro o escriba Alt+F para abrir el filtro rápido y, a continuación, escriba texto para mostrar sólo los elementos que contienen el texto escrito.\
   >     El filtro rápido se encuentra en la barra de herramientas de la lista. Para obtener más información, vea [Aplicar el filtro rápido a una lista](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).


   Si el campo se puede editar, esto convierte el campo y todos los demás campos mostrados en la lista en celdas editables.

   ![](assets/nwe-editable-cells-350x131.png)

1. Edita la información dentro de esta celda y luego presiona [!UICONTROL Intro].

   >[!NOTE]
   >
   >Si se ha configurado un campo personalizado para permitir el formato, puede aplicar negrita, cursiva o subrayado al editar en línea el campo en una lista actualizada.\
   >Para obtener información sobre cómo configurar el formato de un campo personalizado, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).\
   >Para obtener información acerca de las listas actualizadas, vea la sección &quot;La diferencia entre las listas actualizadas y las heredadas&quot; en el artículo [Introducción a las listas en [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Presione [!UICONTROL Tab] para pasar a la siguiente celda editable.
1. (Condicional) Si no puede guardar las ediciones y la celda está delineada en rojo, haga clic dentro del campo para revisar el mensaje de validación que se muestra junto a la celda y realizar las actualizaciones adecuadas.

   Lo habitual es que esto ocurra cuando se utiliza un formato incorrecto o cuando se deja en blanco un campo obligatorio.

1. Cuando termine de modificar todas las celdas, presione [!UICONTROL Entrar] para guardar los cambios.
