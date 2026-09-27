---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Configurar ubicaciones
description: Puede configurar las ubicaciones predeterminadas disponibles para asignar como atributos a los roles en las tarjetas de tasas.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 69233499-fbcb-44a4-a247-d5051f9bc8b9
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 27%
---
# Configurar ubicaciones

{{preview-fast-release-general}}

Puede configurar las ubicaciones predeterminadas disponibles para asignar como atributos a los roles en las tarjetas de tasas. Esto garantiza que las tarjetas de tarifas reflejen con precisión las tarifas de mercado en cada ubicación.

Las tarjetas de tarifas permiten a su organización administrar fácilmente las tarifas de facturación para los proyectos. Para obtener más información, consulte [Administrar tarjetas de tarifas](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md) y [Definir atributos de tarifas](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Añadir una ubicación

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en [!UICONTROL **Ubicaciones**].
1. En el entorno Producción, haga clic en [!UICONTROL **Agregar más ubicaciones**] al final de la lista.
   <span class="preview">En el entorno de vista previa, haga clic en [!UICONTROL **Nueva fila**] en la parte inferior de la lista.</span>

1. Introduzca el nombre de la ubicación y la descripción.
1. Haga clic fuera de la fila para guardar la ubicación.
1. Para eliminar una ubicación en el entorno Producción, selecciónela en la lista y haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete.png).
   <span class="preview">Para eliminar una ubicación en el entorno de vista previa, selecciónela en la lista y haga clic en [!UICONTROL **Eliminar**] en la barra de acciones de la parte inferior de la pantalla.</span>

>[!NOTE]
>
>No se pueden eliminar las ubicaciones asociadas con funciones en una tarjeta de tarifas.

## Añadir una sububicación

Puede agregar una sububicación a una ubicación existente. Por ejemplo, si ya tiene una ubicación de Reino Unido, Londres podría ser una sububicación.

Se permiten tres niveles de sububicaciones. El país, el estado o la provincia y la ciudad son usos comunes de las sububicaciones.

Cada sububicación se puede agregar como atributo en una tarjeta de tasa de la misma manera que una ubicación de nivel superior, para definir la tasa para un rol específico en esa ubicación.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en [!UICONTROL **Ubicaciones**].
1. En el entorno Producción, seleccione una ubicación existente en la lista y haga clic en [!UICONTROL **Agregar ubicación secundaria**].
   <span class="preview">En el entorno de vista previa, seleccione una ubicación existente en la lista y haga clic en [!UICONTROL **Agregar ubicación secundaria**] en la barra de acciones de la parte inferior de la pantalla.</span>

1. Introduzca el nombre de la ubicación y la descripción.
1. Haga clic fuera del área de entrada para guardar la ubicación.

   La sububicación tiene sangría debajo de la ubicación de nivel superior.

   Imagen de muestra en el entorno de producción:
   ![Ubicaciones y sububicaciones](assets/locations-sublocations.png)

   <span class="preview">Imagen de muestra en el entorno de vista previa:</span>
   ![Ubicaciones y sububicaciones](assets/locations-sublocations-082526.png)


