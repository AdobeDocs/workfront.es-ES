---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Administrar tarjetas de tarifa
description: Las tarjetas de tarifas le permiten definir varias tarifas de facturación por rol, según la ubicación.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---

# Administrar tarjetas de tarifa

{{highlighted-preview-article-level}}

Las tarjetas de tarifas le permiten definir varias tarifas de facturación por rol, según la ubicación. Podría tener una función laboral de Designer con sede en París y una segunda Designer con sede en Nueva York, cada una con diferentes tarifas de facturación. Sin embargo, no se requiere una ubicación para los roles en una tarjeta de tarifas. Una tarifa de facturación para un rol (y posiblemente una ubicación) en una tarjeta de tarifas también puede incluir fechas efectivas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Nuevo: [!UICONTROL Standard]</p>
   O
   <p>Actual: [!UICONTROL plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Editar acceso a [!UICONTROL Financial Data]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Para editar una tarjeta de tarifas compartida con usted, debe tener permisos de administración en la tarjeta de tarifas.</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agregar una tarjeta de tarifa

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifa**].
1. Haga clic en [!UICONTROL **Nueva tarjeta de tarifa**] y, a continuación, escriba un nombre para la tarjeta de tarifa en el cuadro [!UICONTROL Nueva tarjeta de tarifa], para reemplazar &quot;Tarjeta de tarifa sin título&quot;.
1. (Opcional) En la pantalla Detalles de la tarjeta de tarifas, agregue una [!UICONTROL **Descripción**].
1. (Opcional) Para adjuntar un formulario personalizado a la tarjeta de tarifas, haga clic en el campo [!UICONTROL **Agregar formulario personalizado**] en la esquina superior derecha y seleccione un formulario personalizado de la lista que se muestra.

   Para obtener más información sobre cómo adjuntar un formulario personalizado, vea [Agregar un formulario personalizado a un objeto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Haga clic en [!UICONTROL **Funciones y tarifas del puesto**] en el panel de navegación izquierdo.
1. En la pantalla Tasas y roles de la tarjeta Tasas, haz clic en [!UICONTROL **Agregar rol**].
1. En el cuadro de diálogo, seleccione un [!UICONTROL **Rol**] para definir las tarifas de facturación de.

   La tarifa de facturación predeterminada muestra la tarifa en el nivel del sistema para este rol, si se ha definido uno.

   ![Cuadro de diálogo Nueva tarifa de facturación](assets/location-rate-for-rate-card.png)

1. Seleccione una [!UICONTROL **Moneda**] para el rol.
1. (Opcional) Seleccione una [!UICONTROL **ubicación**] para el rol.
1. En el campo [!UICONTROL **Tarifa de facturación 1**], escriba la tarifa de facturación para esta ubicación. A continuación, haga clic en [!UICONTROL **Guardar**] para anular la tarifa de facturación una vez.

   O

   Haz clic en [!UICONTROL **Agregar tarifa**] para agregar más tarifas de facturación específicas de la ubicación con fechas de vigencia.

1. (Condicional) Si agrega más de una tarifa de facturación para esta ubicación, introduzca la siguiente información:

   * **[!UICONTROL Tarifa de facturación 1], 2, etc.:** El valor de la tarifa de facturación para el período de tiempo.
   * **[!UICONTROL Fecha de inicio]:** La fecha en la que comienza la anulación de tarifa.
   * **[!UICONTROL Fecha de finalización]:** La fecha en la que finaliza la anulación de tarifa.

     La tarifa de facturación 1 no tendrá una fecha de inicio y la última tarifa de facturación no tendrá una fecha de finalización. Algunas fechas se añaden automáticamente. Por ejemplo, si la Tarifa de facturación 1 no tiene una fecha de finalización y agrega la Tarifa de facturación 2 con una fecha de inicio del 1 de mayo de 2023, se agrega la fecha de finalización del 30 de abril de 2023 a la Tarifa de facturación 1 para que no existan lagunas.

1. Haga clic en [!UICONTROL **Guardar**].
1. (Opcional) Para agregar otra tarifa de facturación, ya sea para el mismo rol en otra ubicación o para un rol separado, haga clic en [!UICONTROL **Agregar rol**].
1. (Opcional) Para editar una tarjeta de tarifa, haga clic en el nombre de la tarjeta de tarifa en la lista Tarjetas de tarifa de Configuración. Para editar una tarifa de facturación, haga clic en [!UICONTROL **Funciones y tarifas del puesto**] en el panel de navegación izquierdo de la tarjeta de tarifas. A continuación, seleccione la tarifa y haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png).

## Copiar una tarjeta de tarifas

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifa**].
1. Seleccione la casilla de verificación situada junto a la tarjeta de tarifa de la lista y haga clic en el icono **Copiar** ![Copiar icono](assets/copy-icon.png).
1. Escriba un nombre para la tarjeta de tarifa en el cuadro [!UICONTROL Copiar tarjeta de tarifa], para reemplazar &quot;Tarjeta de tarifa sin título&quot;. A continuación, haga clic en **Guardar**.

   Se guardará la nueva tarjeta de tarifas. Edite los detalles de la tarjeta de tarifas, los roles y las tarifas según sea necesario.

## Eliminar una tarjeta de tarifa completa

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifa**].
1. Seleccione la casilla de verificación situada junto a la tarjeta de tarifa de la lista y haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete.png).

   >[!NOTE]
   >
   >Se eliminará del proyecto una tarjeta de tarifas adjunta a un proyecto.
