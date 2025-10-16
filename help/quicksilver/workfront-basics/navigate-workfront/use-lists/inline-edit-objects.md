---
product-area: projects
navigation-topic: use-lists
title: Editar elementos en línea en una lista en  [!DNL Adobe Workfront]
description: Puede editar objetos en línea cuando se muestren en una lista o un informe. Cuando se edita la información sobre los objetos mostrados en una lista o un informe, el objeto se actualiza inmediatamente.
feature: Get Started with Workfront
author: Nolan
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: f0b3b8aa64fa0b03a196bbcc2bdd037eeeb0f89e
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 95%

---

# Editar elementos en línea en una lista de [!DNL Adobe Workfront]

<!--Audited: 11/2024-->

Puede editar objetos en línea cuando se muestren en una lista o un informe. Cuando se edita la información sobre los objetos mostrados en una lista o un informe, el objeto se actualiza inmediatamente.

Cuando se edita en línea un campo contenido en un formulario personalizado que no está adjunto al objeto, el formulario personalizado se añade automáticamente al objeto. Si el campo existe en varios formularios personalizados, el formulario personalizado que se haya actualizado más recientemente se adjuntará al objeto.

Para obtener más información sobre las listas, consulte [Introducción a las listas en [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Aunque la mayoría de los objetos mostrados en listas o informes se pueden editar en línea en [!DNL Adobe Workfront], existen algunas limitaciones, entre las que se incluyen:

* No es posible editar campos calculados o [!DNL Workfront] campos integrados que sean cálculos.
* Únicamente se pueden editar campos asociados directamente a los objetos de la lista. No es posible editar campos que pertenezcan a objetos asociados a los objetos de la lista.

  Por ejemplo, puede editar el estado de una tarea en un informe de tareas, pero no puede editar el nombre del proyecto al que está asociada la tarea en el mismo informe. Únicamente se puede editar el nombre del proyecto en un informe de proyecto.
* No es posible editar campos en línea cuando la vista de una lista no muestra la moneda predeterminada.

  Para obtener más información sobre cómo mostrar la moneda predeterminada, consulte la sección [Editar informes con monedas únicas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) en el artículo [Crear informes de datos financieros con tasas de cambio únicas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).
* No es posible editar los indicadores e iconos mostrados en una lista.
* No es posible editar en línea campos de informe que procedan de otros informes.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior </p>
   <p>Solicitud o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de [!UICONTROL Edit] al área donde se encuentra la lista</p> <p>Por ejemplo, para editar en línea las tareas de un proyecto, necesita el acceso de [!UICONTROL Edit] a Proyectos.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>[!UICONTROL Manage]</p> <p>También debe tener permisos para editar ciertos campos, como campos personalizados, estado, etc.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar objetos en línea

1. Vaya a la lista de objetos que desea editar en línea.

   La lista debería mostrar campos que pertenecen a los objetos o a objetos asociados a los objetos de la lista.

1. Localice el objeto que desea editar y, a continuación, haga clic dentro de cualquier campo de la lista.

   >[!TIP]
   >
   >Si tiene varias páginas, puede localizar un objeto mediante lo siguiente:
   >
   >   * **Paginación**: haga clic en las flechas hacia atrás y hacia adelante para desplazarse entre las páginas.
   >     En la esquina inferior derecha de la lista, el área de [!UICONTROL paginación] permanece fija mientras se desplaza por la lista.
   >   * **Filtro rápido**: haga clic en el icono de filtro o escriba Alt+F para abrir el filtro rápido y, a continuación, escriba texto para mostrar únicamente los elementos que contienen dicho texto.
   >     El filtro rápido se encuentra en la barra de herramientas de la lista. Para obtener más información, consulte [Aplicar el filtro rápido a una lista](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

   Si el campo se puede editar, esto convierte el campo y todos los demás campos mostrados en la lista en celdas editables.

   ![Celdas editables](assets/nwe-editable-cells-350x131.png)

1. Edite la información dentro de esta celda y pulse [!UICONTROL Intro].

   >[!NOTE]
   >
   >Si se ha configurado un campo personalizado para permitir el formato, puede aplicar negrita, cursiva o subrayado al editar en línea el campo en una lista actualizada.
   >Para obtener información sobre cómo configurar el formato de un campo personalizado, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
   >Para obtener más información sobre las listas actualizadas, consulte la sección “Diferencia entre las listas actualizadas y las heredadas” en el artículo [Introducción a las listas en [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Pulse [!UICONTROL Pestaña] para pasar a la siguiente celda editable.
1. (Condicional) Si no puede guardar las ediciones y la celda está delineada en rojo, haga clic dentro del campo para revisar el mensaje de validación que se muestra junto a la celda y realizar las actualizaciones adecuadas.

   Lo habitual es que esto ocurra cuando se utiliza un formato incorrecto o cuando se deja en blanco un campo obligatorio.

1. Cuando termine de modificar todas las celdas, pulse [!UICONTROL Intro] para guardar los cambios.
