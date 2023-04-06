---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Personalización de los campos que se muestran en una tarjeta
description: Puede personalizar los campos que se muestran en una tarjeta desactivando un campo para que no se muestre en la tarjeta completa o en la vista condensada, o ocultando un campo en la vista de tarjeta condensada.
author: Lisa
feature: Agile
source-git-commit: 48dc1bcbaa5755888c45fdafbd6471c9ee073a45
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---


# Personalización de los campos que se muestran en una tarjeta

De forma predeterminada, todos los campos disponibles se muestran en una tarjeta, tanto en la vista completa cuando la tarjeta está abierta como en la vista de tarjeta condensada en el tablero. Puede personalizar los campos que se muestran:

* Desactivación de un campo para que no se muestre en ninguna de las vistas
* Ocultar un campo en la vista de tarjeta condensada

Si un campo contiene un valor y desactiva el campo, el valor se conserva si vuelve a habilitar el campo más adelante.

También puede mostrar campos personalizados que se hayan creado anteriormente. No se pueden diseñar ni crear nuevos campos personalizados dentro de un tablero.

>[!NOTE]
>
>Las personalizaciones de campo que realice solo se aplicarán al tablero en el que esté trabajando.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Request] o superior</p> </td> 
  </tr>
   </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Configuración de tarjetas {#configure-cards}

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Tableros]**.
1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en [!UICONTROL **Configurar**] a la derecha del tablero para abrir el panel Configurar .
1. Expandir [!UICONTROL **Tarjetas**].

   La mayoría de los campos están habilitados de forma predeterminada.

1. Desactive un campo para desactivarlo en ambas vistas de tarjeta.
1. Haga clic en el icono Ocultar ![Ocultar icono](assets/eye-hide-icon.png) junto a un campo para ocultarlo en la vista condensada.
1. Para mostrar todos los campos en ambas vistas, haga clic en [!UICONTROL **Restaurar todos los campos de forma predeterminada**].
1. Haga clic en [!UICONTROL **Ocultar configurar**] para cerrar el panel Configurar .

## Añadir campos personalizados a tarjetas

Los campos personalizados están disponibles en tarjetas conectadas. Solo son visibles en la vista completa de la tarjeta, no en la vista condensada del tablero.

>[!NOTE]
>
>Cuando agrega un campo personalizado a las tarjetas, los datos de la tarjeta son de solo lectura.

1. Acceda a un tablero y haga clic en [!UICONTROL **Configurar**] para abrir el panel Configurar .
1. Expandir [!UICONTROL **Tarjetas**].
1. En [!UICONTROL Campos de tarjeta], haga clic en [!UICONTROL **Añadir campo personalizado**].
1. Select [!UICONTROL **Tarea**] o [!UICONTROL **Problema**].

   Aparecen las categorías de campos disponibles para tareas o problemas. Expanda una categoría para ver todos los campos. También puede buscar un campo.

   ![Buscar campo personalizado](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Los siguientes tipos de campos no están disponibles para agregarlos a las tarjetas: Adobe XD, Imagen, PDF, Vídeo.

1. Seleccione el nombre del campo.
1. (Opcional) Haga clic en la **[!UICONTROL Valor de campo]** para cambiar este campo personalizado por otro.
1. (Opcional) Cambie el **[!UICONTROL Etiqueta de campo]** al nombre del campo que desea que aparezca en las tarjetas.
1. Cuando haya terminado de realizar cambios, haga clic en [!UICONTROL **Guardar campo**].

   ![Etiqueta y valor de campo personalizado](assets/save-custom-field-value-label.png)

   El campo personalizado se añade a la lista de campos disponibles y se activa de forma predeterminada. Puede desactivar el campo personalizado siguiendo los pasos de la sección [Configuración de tarjetas](customize-fields-on-card.md#configure-cards) , edite el campo o elimínelo de todas las tarjetas.

