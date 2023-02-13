---
product-area: projects
navigation-topic: use-lists
title: Editar elementos en línea en una lista de [!DNL Adobe Workfront]
description: Los objetos se pueden editar en línea cuando se muestran en una lista o informe. Cuando edita la información sobre los objetos mostrados en una lista o informe, el objeto se actualiza inmediatamente.
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Editar elementos en línea en una lista de [!DNL Adobe Workfront]

Los objetos se pueden editar en línea cuando se muestran en una lista o informe. Cuando edita la información sobre los objetos mostrados en una lista o informe, el objeto se actualiza inmediatamente.

Cuando se edita en línea un campo contenido en un formulario personalizado que no está adjunto al objeto, el formulario personalizado se agrega automáticamente al objeto. Si el campo existe en varios formularios personalizados, el formulario personalizado que se actualizó más recientemente se adjunta al objeto.

Para obtener más información sobre las listas, consulte [Introducción a las listas en [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Mientras que la mayoría de los objetos mostrados en listas o informes se pueden editar en línea en [!DNL Adobe Workfront], hay algunas limitaciones, que incluyen:

* No se pueden editar los campos calculados ni [!DNL Workfront] campos integrados que son cálculos.
* Solo se pueden editar campos asociados directamente a los objetos de la lista. No se pueden editar campos que pertenezcan a objetos asociados a los objetos de la lista.\
   Por ejemplo, puede editar el estado de una tarea en un informe de tarea, pero no puede editar el nombre del proyecto al que está asociada la tarea en el mismo informe. Solo se puede editar el nombre del proyecto en un informe de proyecto.
* No se pueden editar campos en línea cuando la vista de una lista no muestra la moneda predeterminada.\
   Para obtener información sobre cómo mostrar la moneda predeterminada, consulte la sección [Editar informes con monedas únicas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) en el artículo [Crear informes de datos financieros con tipos de cambio únicos](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

* Los indicadores y los iconos que se muestran en una lista no se pueden editar.

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
   <td> <p>Acceso de [!UICONTROL Edit] al área en la que se encuentra la lista</p> <p>Por ejemplo, para editar tareas en línea en un proyecto, necesita acceso de [!UICONTROL Edit] a Proyectos.</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso.<br>Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>[!UICONTROL Administrar]</p> <p>También debe tener permisos para editar ciertos campos, como campos personalizados, estado, etc.</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Editar objetos en línea

1. Vaya a la lista de objetos que desea editar en línea.

   La lista debe mostrar los campos que pertenezcan a los objetos o campos que pertenezcan a objetos asociados a los objetos de la lista.

1. Busque el objeto que desea editar y, a continuación, haga clic dentro de cualquier campo de la lista.

   >[!TIP]
   >
   >Si tiene varias páginas, puede localizar un objeto utilizando:
   >
   >   
   >   
   >   * **Paginación**: Haga clic en las flechas hacia atrás y hacia adelante para desplazarse entre las páginas.\
      >     Situado en la esquina inferior derecha de la lista, la variable [!UICONTROL paginación] permanece fija mientras se desplaza por la lista.
   >   * **Filtro rápido**: Haga clic en el icono de filtro o escriba Alt+F para abrir el filtro rápido y, a continuación, escriba el texto para mostrar solo los elementos que contengan el texto introducido.\
      >     El filtro rápido se encuentra en la barra de herramientas de la lista. Para obtener más información, consulte [Aplicar el filtro rápido a una lista](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).



   Si se puede editar el campo, este convierte el campo y todos los demás campos mostrados en la lista en celdas editables.

   ![](assets/nwe-editable-cells-350x131.png)

1. Edite la información dentro de esta celda y luego presione [!UICONTROL Entrar].

   >[!NOTE]
   >
   >Si se ha configurado un campo personalizado para permitir el formato, puede aplicar negrita, cursiva o subrayado al editar el campo en línea en una lista actualizada.\
   >Para obtener información sobre la configuración del formato de un campo personalizado, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).\
   >Para obtener información sobre las listas actualizadas, consulte la sección &quot;La diferencia entre las listas actualizadas y las listas heredadas&quot; en el artículo [Introducción a las listas en [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Press [!UICONTROL Tabulación] para desplazarse a la siguiente celda editable.
1. (Condicional) Si no puede guardar las ediciones y la celda está delineada en rojo, haga clic dentro del campo para revisar el mensaje de validación que aparece junto a la celda y realizar las actualizaciones adecuadas.

   Lo más habitual es que esto ocurra cuando se utiliza un formato incorrecto o cuando se deja en blanco un campo obligatorio.

1. Después de finalizar la modificación de todas las celdas, presione [!UICONTROL Entrar] para guardar los cambios.
