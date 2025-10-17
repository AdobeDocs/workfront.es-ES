---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Personalizar los campos que se muestran en una tarjeta
description: Personalice los campos que se mostrarán en una tarjeta deshabilitando campos para que no se muestren en la vista de tarjeta completa o en la vista condensada, o bien ocultando campos en la vista de tarjeta condensada.
author: Jenny
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 97%

---

# Personalizar los campos que se muestran en una tarjeta

De forma predeterminada, todos los campos disponibles se mostrarán en una tarjeta, tanto en la vista completa cuando la tarjeta esté abierta como en la vista de tarjeta condensada del tablero. Es posible personalizar los campos que se mostrarán mediante lo siguiente:

* La desactivación de un campo para que no se muestre en ninguna vista
* La ocultación de un campo en la vista de tarjeta condensada

Si un campo contiene un valor y se desactiva, el valor se conservará al volver a habilitar el campo más adelante.

Las secciones (que aparecen como opciones de navegación izquierda en los detalles de la tarjeta) también están disponibles para mostrarse y ocultarse.

También es posible mostrar campos personalizados creados anteriormente. No se pueden diseñar y crear nuevos campos personalizados dentro de un tablero.

>[!NOTE]
>
>Las personalizaciones de campos que se realicen solo se aplicarán al tablero en el que se esté trabajando.

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
   <p>Colaborador o superior</p> 
   <p>Solicitud o superior</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuración de tarjetas {#configure-cards}

{{step1-to-boards}}

1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en [!UICONTROL **Configurar**], a la derecha del tablero, para abrir el panel Configurar.
1. Expanda las [!UICONTROL **tarjetas**].

   La mayoría de los campos y secciones están habilitados de forma predeterminada.

1. Desactive un campo o una sección para deshabilitarlo en ambas vistas de tarjeta.
1. Haga clic en el ![icono Ocultar](assets/eye-hide-icon.png) que verá junto a un campo o sección para ocultarlo en la vista resumida.
1. Para mostrar todos los campos y secciones de ambas vistas, haga clic en [!UICONTROL **Restaurar todos los campos al valor predeterminado**].
1. Haga clic en [!UICONTROL **Ocultar configuración**] para cerrar el panel Configurar.

## Adición de campos personalizados a las tarjetas

Los campos personalizados están disponibles en las tarjetas conectadas. Solo son visibles en la vista de tarjeta completa, no en la vista condensada del tablero.

Es posible editar los datos de los campos personalizados en la tarjeta, aunque algunos elementos personalizados solo están disponibles para su edición en el campo original y no en la tarjeta.

1. Acceda a un tablero y haga clic en [!UICONTROL **Configurar**] para abrir el panel Configurar.
1. Expanda las [!UICONTROL **tarjetas**].
1. En [!UICONTROL Campos de la tarjeta], haga clic en [!UICONTROL **Añadir campo personalizado**].
1. Seleccione [!UICONTROL **Tarea**] o [!UICONTROL **Problema**].

   Aparecerán las categorías de los campos disponibles para tareas o problemas. Expanda una categoría para ver todos los campos. También es posible buscar un campo.

   ![Buscar un campo personalizado](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >No están disponibles los siguientes tipos de campo para que se añadan a las tarjetas: Adobe XD, Imagen, PDF y Vídeo.

1. Seleccione el nombre del campo.
1. (Opcional) Haga clic en el campo **[!UICONTROL Valor del campo]** para cambiar este campo personalizado por otro diferente.
1. (Opcional) Cambie **[!UICONTROL Etiqueta del campo]** por el nombre del campo que quiera que aparezca en las tarjetas.
1. Cuando haya terminado de realizar cambios, haga clic en [!UICONTROL **Guardar campo**].

   ![Etiqueta y valor del campo personalizado](assets/save-custom-field-value-label.png)

   El campo personalizado se añade a la lista de campos disponibles y se habilita de forma predeterminada. Es posible deshabilitar el campo personalizado siguiendo los pasos de la sección [Configurar tarjetas](customize-fields-on-card.md#configure-cards) anterior, editar el campo o eliminarlo de todas las tarjetas.

>[!NOTE]
>
>Si posteriormente cambia el nombre del campo personalizado en Workfront, debe editar la etiqueta del campo en el panel Configuración para que coincida o el campo no se mostrará en las tarjetas.

## Mostrar u ocultar tarjetas archivadas

Debe activar un ajuste de configuración para mostrar las tarjetas archivadas en un tablero.

1. Acceda a un tablero y haga clic en [!UICONTROL **Configurar**] para abrir el panel Configurar.
1. Expanda [!UICONTROL **Tarjetas**].
1. Active [!UICONTROL **Mostrar tarjetas archivadas en el tablero**].

   Ahora, puede filtrar el tablero para mostrar cualquier tarjeta que se haya archivado. Para obtener más información, consulte [Filtrar y buscar en un tablero](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

1. Haga clic en [!UICONTROL **Ocultar configuración**] para cerrar el panel Configurar.

## Configurar la caída de tarjetas

Para quitar tarjetas del tablero automáticamente después de un período de tiempo, consulte [Configurar caída de tarjetas](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).
