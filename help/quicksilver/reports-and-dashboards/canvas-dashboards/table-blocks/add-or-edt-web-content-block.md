---
title: Adición o edición de un bloque de contenido web en el lienzo de informes
description: Los bloques de contenido web permiten mostrar información de sitios web externos directamente en el informe.
hidefromtoc: true
hide: true
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# Adición o edición de un bloque de contenido web en el lienzo de informes

Los bloques de contenido web permiten mostrar información de sitios web externos directamente en el informe.

## Requisitos previos

Antes de empezar, debe inscribirse en la versión beta del lienzo de informes. Para obtener más información, consulte [Resumen de Lienzo de informes beta](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Adición o edición de un bloque de contenido web

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Informes**.
1. Clic **Nuevo informe**.

   O

   Vaya a un informe existente y haga clic en **Más** icono ![](assets/more-icon-27x15.png) en el encabezado del informe, haga clic en **Editar**.

1. En el lado derecho de la pantalla, debajo de **Agregar un bloque**, bien:

   Arrastre el **Contenido web** en el lienzo directamente a la ubicación deseada.

   O

   Haga doble clic en **Contenido web** para añadir un bloque a la parte superior del lienzo.

   >[!TIP]
   >
   >Se puede cambiar el tamaño del bloque una vez colocado arrastrando sus puntos de control de esquina.

1. Clic **Contenido web sin título** en el encabezado del bloque, escriba un título para el bloque.
1. Haga clic en **Editar** icono ![](assets/edit-icon.png) en el encabezado del bloque.

   ![](assets/web-content-block-header-350x76.png)

1. En el **Configuración** Cuando se abra, introduzca la dirección URL completa de la página que desea mostrar (incluido &quot;https://&quot;) en el **URL** field.

   >[!NOTE]
   >
   >Actualmente, solo se pueden mostrar los sitios de dominios seleccionados. Los dominios que se pueden utilizar actualmente son:
   >   
   >   * workfront.com
   >   * google.com
   >   * sharepoint.com
   >   * attask-ondemand.om
   >   * powerbi.com
   >   * domo.com
   >   * looker.com

   Aparece una advertencia debajo de la dirección URL introducida si no se puede incrustar. Estas advertencias incluyen:

   | Nombre de advertencia | Motivo |
   |---|---|
   | Dirección URL no válida | La dirección URL introducida no devuelve un sitio válido. |
   | Restricciones del sitio del proveedor | El sitio que está intentando incrustar no está permitido. |

   {style="table-layout:auto"}

1. (Opcional) Haga clic en **Pasar parámetros** active esta opción para abrir una lista de los parámetros de pase disponibles.

   >[!WARNING]
   >
   >Los parámetros de paso están desactivados actualmente.

1. Clic **Incrustar URL** para guardar las selecciones y volver al informe.
