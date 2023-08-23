---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Personalizar los campos que se muestran en una tarjeta
description: Puede personalizar los campos que se muestran en una tarjeta deshabilitando un campo para que no se muestre en la vista de tarjeta completa o en la vista condensada, u ocultando un campo en la vista de tarjeta condensada.
author: Lisa
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: 0beb96dc3869e6f913d87f699aa9a51c5aaa8f79
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

# Personalizar los campos que se muestran en una tarjeta

De forma predeterminada, todos los campos disponibles se muestran en una tarjeta, tanto en la vista completa cuando la tarjeta está abierta como en la vista de tarjeta condensada del tablero. Puede personalizar los campos que se muestran mediante lo siguiente:

* Desactivación de un campo para que no se muestre en ninguna vista
* Ocultar un campo en la vista de tarjeta condensada

Si un campo contiene un valor y lo desactiva, el valor se conserva si vuelve a habilitar el campo más adelante.

Las secciones (que aparecen como opciones de navegación izquierda en los detalles de la tarjeta) también están disponibles para mostrarlas y ocultarlas.

También puede mostrar campos personalizados creados anteriormente. No se pueden diseñar y crear nuevos campos personalizados dentro de un tablero.

>[!NOTE]
>
>Las personalizaciones de campo que realice solo se aplican al tablero en el que esté trabajando.

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

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Tableros]**.
1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Clic [!UICONTROL **Configurar**] a la derecha del tablero para abrir el panel Configurar.
1. Expandir [!UICONTROL **Tarjetas**].

   La mayoría de los campos y secciones están habilitados de forma predeterminada.

1. Desactive un campo o una sección para deshabilitarlo en ambas vistas de tarjeta.
1. Haga clic en el icono Ocultar ![Icono Ocultar](assets/eye-hide-icon.png) situado junto a un campo o sección para ocultarlo en la vista condensada.
1. Para mostrar todos los campos y secciones de ambas vistas, haga clic en [!UICONTROL **Restaurar todos los campos a los valores predeterminados**].
1. Clic [!UICONTROL **Ocultar configuración**] para cerrar el panel Configurar.

## Agregar campos personalizados a las tarjetas

Los campos personalizados están disponibles en las tarjetas conectadas. Solo son visibles en la vista de tarjeta completa, no en la vista condensada del tablero.

>[!NOTE]
>
>Cuando se agrega un campo personalizado a las tarjetas, los datos de la tarjeta son de solo lectura.

1. Acceda a un tablero y haga clic en [!UICONTROL **Configurar**] para abrir el panel Configurar.
1. Expandir [!UICONTROL **Tarjetas**].
1. En [!UICONTROL Campos de tarjeta], haga clic en [!UICONTROL **Añadir campo personalizado**].
1. Seleccionar [!UICONTROL **Tarea**] o [!UICONTROL **Problema**].

   Aparecerán las categorías de los campos disponibles para tareas o problemas. Expanda una categoría para ver todos los campos. También puede buscar un campo.

   ![Buscar campo personalizado](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Los siguientes tipos de campo no están disponibles para añadirlos a las tarjetas: Adobe XD, Imagen, PDF, Vídeo.

1. Seleccione el nombre del campo.
1. (Opcional) Haga clic en el icono **[!UICONTROL Valor de campo]** para cambiar este campo personalizado por otro diferente.
1. (Opcional) Cambie el **[!UICONTROL Etiqueta de campo]** al nombre de campo que desee que aparezca en las tarjetas.
1. Cuando haya terminado de realizar los cambios, haga clic en [!UICONTROL **Guardar campo**].

   ![Valor de campo personalizado y etiqueta](assets/save-custom-field-value-label.png)

   El campo personalizado se añade a la lista de campos disponibles y se activa de forma predeterminada. Puede deshabilitar el campo personalizado siguiendo los pasos de la [Configuración de tarjetas](customize-fields-on-card.md#configure-cards) en la sección anterior, edite el campo o elimínelo de todas las tarjetas.

>[!NOTE]
>
>Si posteriormente cambia el nombre del campo personalizado en Workfront, debe editar la etiqueta del campo en el panel Configuración para que coincida o el campo no se mostrará en las tarjetas.
