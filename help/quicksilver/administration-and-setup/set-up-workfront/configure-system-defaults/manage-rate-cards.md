---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Administrar tarjetas de tarifas
description: Según la ubicación, las tarjetas de tarifas le permiten definir varias tarifas de facturación por función.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 99%

---

# Administrar tarjetas de tarifas

{{highlighted-preview-article-level}}

Según la ubicación, las tarjetas de tarifas le permiten definir varias tarifas de facturación por función. Podría tener una función de diseñador con sede en París y un segundo diseñador con sede en Nueva York, cada uno con diferentes tarifas de facturación. Sin embargo, no se requiere una ubicación para las funciones en una tarjeta de tarifas. Una tarifa de facturación para una función (y posiblemente una ubicación) en una tarjeta de tarifas también puede incluir fechas efectivas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Añadir una tarjeta de tarifas

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifas**].
1. Haga clic en [!UICONTROL **Nueva tarjeta de tarifas**] y, a continuación, escriba un nombre en el cuadro [!UICONTROL Nueva tarjeta de tarifas], para reemplazar “Tarjeta de tarifas sin título”.
1. (Opcional) En la pantalla Detalles de la tarjeta de tarifas, añada una [!UICONTROL **Descripción**].
1. (Opcional) Para adjuntar un formulario personalizado a la tarjeta de tarifas, haga clic en el campo [!UICONTROL **Añadir formulario personalizado**] en la esquina superior derecha y seleccione un formulario personalizado de la lista que se muestra.

   Para obtener más información sobre cómo adjuntar un formulario personalizado, vea [Añadir un formulario personalizado a un objeto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Haga clic en [!UICONTROL **Funciones y tarifas**] en el panel de navegación izquierdo.
1. En la pantalla Funciones de tarjeta de tarifas y Tarjeta de tarifas, haga clic en [!UICONTROL **Añadir función**].
1. En el cuadro de diálogo, seleccione una [!UICONTROL **Función**] para la cual definir las tarifas de facturación.

   La tarifa de facturación predeterminada muestra la tarifa en el nivel del sistema para esta función si hay una definida.

   ![Cuadro de diálogo Nueva tarifa de facturación](assets/location-rate-for-rate-card.png)

1. Seleccione una [!UICONTROL **moneda**] para la función.
1. (Opcional) Seleccione una [!UICONTROL **ubicación**] para la función.
1. En el campo [!UICONTROL **Tarifa de facturación 1**], escriba la tarifa de facturación para esta ubicación. A continuación, haga clic en [!UICONTROL **Guardar**] para anular la tarifa de facturación una vez.

   O

   Haga clic en [!UICONTROL **Añadir tarifa**] para añadir más tarifas de facturación específicas de la ubicación con fechas de vigencia.

1. (Condicional) Si añade más de una tarifa de facturación para esta ubicación, introduzca la siguiente información:

   * **[!UICONTROL Tarifa de facturación 1], 2, etc.:** el valor de la tarifa de facturación para el período de tiempo.
   * **[!UICONTROL Fecha de inicio]:** la fecha en la que comienza la anulación de tarifa.
   * **[!UICONTROL Fecha de finalización]:** la fecha en la que finaliza la anulación de tarifa.

     La tarifa de facturación 1 no tendrá una fecha de inicio y la última tarifa de facturación no tendrá una fecha de finalización. Algunas fechas se añaden automáticamente. Por ejemplo, si la tarifa de facturación 1 no tiene una fecha de finalización y añade la tarifa de facturación 2 con una fecha de inicio del 1 de mayo de 2023, se añade la fecha de finalización del 30 de abril de 2023 a la tarifa de facturación 1 para que no existan lagunas.

1. Haga clic en [!UICONTROL **Guardar**].
1. (Opcional) Para añadir otra tarifa de facturación, ya sea para la misma función en otra ubicación o para una función separada, haga clic en [!UICONTROL **Añadir función**].
1. (Opcional) Para editar una tarjeta de tarifas, haga clic en el nombre de la tarjeta de tarifas de la lista de tarjetas de tarifas en Configuración. Para editar una tarifa de facturación, haga clic en [!UICONTROL **Roles de trabajo y tarifas**] en el panel de navegación izquierdo de la tarjeta de tarifas. A continuación, seleccione la tarifa y haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png).

## Copiar una tarjeta de tarifas

{{step-1-to-setup}}

1. El panel de navegación izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifas**].
1. Seleccione la casilla de verificación situada junto a la tarjeta de tarifas de la lista y haga clic en el icono **Copiar** ![Copiar icono](assets/copy-icon.png).
1. Escriba un nombre para la tarjeta de tarifa en el cuadro [!UICONTROL Copiar tarjeta de tarifas], para reemplazar “Tarjeta de tarifa sin título”. A continuación, haga clic en **Guardar**.

   Se guardará la nueva tarjeta de tarifas. Edite los detalles de la tarjeta de tarifas, las funciones y las tarifas, según sea necesario.

## Eliminar una tarjeta de tarifas

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifas**].
1. Seleccione la casilla de verificación situada junto a la tarjeta de tarifas de la lista y haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete.png).

   >[!NOTE]
   >
   >Una tarjeta de tarifas adjunta se eliminará del proyecto.
