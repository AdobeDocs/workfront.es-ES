---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Editar un informe de calendario existente
description: Es posible modificar calendarios existentes añadiendo o eliminando un vínculo a un proyecto. También se pueden modificar las agrupaciones de calendario asociadas a un informe de calendario.
author: Lisa
feature: Reports and Dashboards
exl-id: 494d040c-bd1d-4356-824f-a75890803617
source-git-commit: c8f4d8e460ed9247ca5d89c9a711ecb1ec5ed1e9
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 61%

---

# Editar un informe de calendario existente

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>

Es posible modificar calendarios existentes añadiendo o eliminando un vínculo a un proyecto. También se pueden modificar las agrupaciones de calendario asociadas a un informe de calendario.

>[!NOTE]
>
>Un informe de calendario tiene un límite máximo de 15 agrupaciones.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Nuevo: estándar</p>
       <p>o</p>
       <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso [!UICONTROL Edit] a [!UICONTROL Reports], [!UICONTROL Dashboards] y [!UICONTROL Calendars]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Acceso [!UICONTROL Manage] al informe de calendario</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar un informe de calendario existente en producción

{{step1-to-calendars}}

1. (Opcional) Para cambiar el nombre del informe de calendario, haga clic en el campo [!UICONTROL nombre de calendario] y realice los cambios que desee. Se recomienda utilizar solo caracteres UTF-8 para evitar problemas de compatibilidad.

   ![Cambiar el nombre del informe](assets/titlechange-250x230.png)

   Si compartió el informe de calendario con otros usuarios o equipos, el nombre del calendario modificado se actualizará automáticamente en la vista de calendario.

1. (Opcional) Para añadir un proyecto al informe de calendario:

   1. Haga clic en **[!UICONTROL Añadir al calendario].**
   1. En el campo **[!UICONTROL Nombre del proyecto]**, empiece a escribir el nombre del proyecto desde el que desea agregar eventos de calendario y, a continuación, haga clic en el nombre cuando se muestre en la lista desplegable.

      ![Seleccione el nombre del proyecto](assets/calendar-project-name.png)
Los elementos del proyecto y sus tareas y problemas asociados se añaden al informe de calendario.

1. (Opcional) Para añadir una agrupación de calendario o modificar una existente:

   1. Pase el ratón sobre el nombre del proyecto, haga clic en la flecha desplegable situada junto al nombre del proyecto y, a continuación, haga clic en **[!UICONTROL Editar]**.

      ![Editar agrupación de calendario](assets/editcalendergroup-350x126.png)

   1. Elija cómo quiere agrupar los elementos:

      * [Usar [!UICONTROL Fechas planificadas] en un informe de calendario](../../../reports-and-dashboards/reports/calendars/use-planned-dates.md)
      * [Usar [!UICONTROL Fechas proyectadas] en un informe de calendario](../../../reports-and-dashboards/reports/calendars/use-projected-dates.md)
      * [Usar campos de fecha personalizados en un informe de calendario](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md)


<div class="preview">

## Editar un informe de calendario existente en Vista previa

{{step1-to-calendars}}

1. (Opcional) Para cambiar el nombre del informe del calendario, haga clic en el menú **Más** y seleccione **Editar**.
   ![menú más](assets/new-more-menu-calendar.png)
Si ha compartido el informe de calendario con otros usuarios o equipos, el nombre del calendario modificado se actualiza automáticamente en su vista de calendario.

1. (Opcional) Para añadir un proyecto al informe de calendario:
   1. Haga clic en **[!UICONTROL Añadir al calendario].**
   1. Empiece a escribir el nombre del proyecto desde el que desea agregar eventos de calendario y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
   1. Haga clic en **Add**.
      ![agregar un proyecto a un calendario](assets/add-a-calendar-project.png)


1. (Opcional) Para añadir una agrupación de calendario o modificar una existente:
   1. Haga clic en el menú **Más** junto al nombre del proyecto y luego haga clic en **Editar**.
      ![editar proyecto en calendario](assets/edit-project-in-calendar.png)e

   1. Elija cómo quiere agrupar los elementos:

      * [Usar [!UICONTROL Fechas planificadas] en un informe de calendario](../../../reports-and-dashboards/reports/calendars/use-planned-dates.md)
      * [Usar [!UICONTROL Fechas proyectadas] en un informe de calendario](../../../reports-and-dashboards/reports/calendars/use-projected-dates.md)
      * [Usar campos de fecha personalizados en un informe de calendario](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md)


      </div>