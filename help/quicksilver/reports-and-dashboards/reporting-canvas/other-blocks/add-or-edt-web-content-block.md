---
product-area: reporting
navigation-topic: other-blocks
title: Añadir o editar un bloque de contenido web en el Lienzo de informes
description: Los bloques de contenido web permiten mostrar información de sitios web externos directamente dentro del informe.
author: Nolan
feature: Reports and Dashboards
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---


# Añadir o editar un bloque de contenido web en el Lienzo de informes

Los bloques de contenido web permiten mostrar información de sitios web externos directamente dentro del informe.

## Requisitos previos

Antes de comenzar, debe inscribirse en la versión beta del lienzo de informes. Para obtener más información, consulte [Reporting Canvas beta: información general](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Añadir o editar un bloque de contenido web

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Informes**.
1. Haga clic en **Nuevo informe**.

   O

   Vaya a un informe existente y haga clic en el botón **Más** icono ![](assets/more-icon-27x15.png) en el encabezado del informe y, a continuación, haga clic en **Editar**.

1. En el lado derecho de la pantalla, debajo de **Agregar un bloque**, ya sea:

   Arrastre el **Contenido web** en el lienzo directamente a la ubicación deseada.

   O

   Haga doble clic en el botón **Contenido web** para añadir un bloque a la parte superior del lienzo.

   >[!TIP]
   >
   >Puede cambiar el tamaño del bloque después de colocarlo arrastrando sus controladores de esquina.

1. Haga clic en **Contenido web sin título** en el encabezado de bloque, escriba un título para el bloque.
1. Haga clic en el **Editar** icono ![](assets/edit-icon.png) en el encabezado de bloque.

   ![](assets/web-content-block-header-350x76.png)

1. En el **Configuración** que se abre, introduzca la dirección URL completa de la página que desea mostrar (incluido &quot;https://&quot;) en la **URL** campo .

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


   Si no se puede incrustar, aparece una advertencia debajo de la dirección URL introducida. Estas advertencias incluyen:

   | Nombre de advertencia | Razón |
   |---|---|
   | Dirección URL no válida | La dirección URL introducida no devuelve un sitio válido. |
   | Restricciones del sitio del proveedor | No se permite el sitio que está intentando incrustar. |

   {style="table-layout:auto"}

1. (Opcional) Haga clic en el **Pasar parámetros** para abrir una lista de parámetros de paso disponibles.

   >[!WARNING]
   >
   >Pasar parámetros está deshabilitado actualmente.

1. Haga clic en **Incrustar URL** para guardar las selecciones y volver al informe.
