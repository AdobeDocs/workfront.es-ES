---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Administrar tarjetas de tarifa
description: Las tarjetas de tarifas le permiten definir varias tarifas de facturación por rol, según la ubicación.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 961e0451ce9011a8a9f511d7d5da99368d22d6fb
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# Administrar tarjetas de tarifa

{{highlighted-preview-article-level}}

Las tarjetas de tarifas le permiten definir varias tarifas de facturación por rol, según la ubicación. Podría tener una función de Designer con sede en París y una segunda función de Designer con sede en Nueva York, cada una con diferentes tarifas de facturación. Sin embargo, no se requiere una ubicación para los roles en una tarjeta de tarifas. Una tarifa de facturación para un rol (y posiblemente una ubicación) en una tarjeta de tarifas también puede incluir fechas efectivas.

## Requisitos de acceso

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
   <td><p>Plan heredado: [!UICONTROL Plan]</p>
       <p>Plan actual: [!UICONTROL Standard]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a [!UICONTROL Financial Data]</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Para editar una tarjeta de tarifas compartida con usted, debe tener permisos de administración en la tarjeta de tarifas.</td> 
  </tr> 
 </tbody> 
</table>

## Agregar una tarjeta de tarifa

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en [!UICONTROL **Valorar tarjetas**].
1. Clic [!UICONTROL **Nueva tarjeta de tarifa**], luego escriba un nombre para la tarjeta de tarifa en la [!UICONTROL **Tarjeta de tarifa**] , para reemplazar &quot;Tarjeta Tarifa sin título&quot;.
1. En la pantalla de la tarjeta, haga clic en [!UICONTROL **Agregar rol**].
1. En el cuadro de diálogo, seleccione una [!UICONTROL **Rol**] para definir tarifas de facturación para.

   La tarifa de facturación predeterminada muestra la tarifa en el nivel del sistema para este rol, si se ha definido uno.

   ![Cuadro de diálogo Nueva tarifa de facturación](assets/location-rate-for-rate-card.png)

1. Seleccione una [!UICONTROL **Moneda**] para el rol.
1. (Opcional) Seleccione una [!UICONTROL **Ubicación**] para el rol.
1. En el [!UICONTROL **Tarifa de facturación 1**] , introduzca la tarifa de facturación para esta ubicación. A continuación, haga clic en [!UICONTROL **Guardar**] para anular la tarifa de facturación una vez.

   O

   Clic [!UICONTROL **Agregar tarifa**] para agregar tarifas de facturación más específicas de la ubicación con fechas efectivas.

1. (Condicional) Si agrega más de una tarifa de facturación para esta ubicación, introduzca la siguiente información:

   * **[!UICONTROL Tarifa de facturación 1], 2, etc.:** El valor de la tarifa de facturación para el período de tiempo.
   * **[!UICONTROL Fecha de inicio]:** La fecha en la que comienza la anulación de tarifa.
   * **[!UICONTROL Fecha de finalización]:** La fecha en la que finaliza la anulación de tarifa.

     La tarifa de facturación 1 no tendrá una fecha de inicio y la última tarifa de facturación no tendrá una fecha de finalización. Algunas fechas se añaden automáticamente. Por ejemplo, si la Tarifa de facturación 1 no tiene una fecha de finalización y agrega la Tarifa de facturación 2 con una fecha de inicio del 1 de mayo de 2023, se agrega la fecha de finalización del 30 de abril de 2023 a la Tarifa de facturación 1 para que no existan lagunas.

1. Haga clic en [!UICONTROL **Guardar**].
1. (Opcional) Para agregar otra tasa de facturación, ya sea para el mismo rol en otra ubicación o para un rol separado, haga clic en [!UICONTROL **Agregar rol**].
1. (Opcional) Para editar una tarifa de facturación, seleccione la tarifa en la tarjeta de tarifas y haga clic en **Editar** icono.

## Copiar una tarjeta de tarifas

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en [!UICONTROL **Valorar tarjetas**].
1. Seleccione la casilla de verificación situada junto a la tarjeta de tarifa de la lista y haga clic en **Copiar** icono ![Icono Copiar](assets/copy-icon.png).

   Se ha añadido una tarjeta de tarifa duplicada. Haga clic en el nombre de la tarjeta de tarifa en la lista para cambiar su nombre.

## Eliminar una tarjeta de tarifa completa

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en [!UICONTROL **Valorar tarjetas**].
1. Seleccione la casilla de verificación situada junto a la tarjeta de tarifa de la lista y haga clic en **Eliminar** icono ![Icono Eliminar](assets/delete.png).

   >[!NOTE]
   >
   >Se eliminará del proyecto una tarjeta de tarifas adjunta a un proyecto.
