---
title: Adición o edición de un bloque de contenido web en el lienzo de informes
description: Los bloques de contenido web permiten mostrar información de sitios web externos directamente en el informe.
hidefromtoc: true
hide: true
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 17%

---

# Adición o edición de un bloque de contenido web en el lienzo de informes

Los bloques de contenido web permiten mostrar información de sitios web externos directamente en el informe.

## Requisitos previos

Antes de empezar, debe inscribirse en la versión beta del lienzo del sistema de informes. Para obtener más información, consulte la [Versión beta del lienzo del sistema de informes: descripción general](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Adición o edición de un bloque de contenido web

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Informes**.
1. Haga clic en **Nuevo informe**.

   O

   Vaya a un informe existente, haga clic en el icono **Más** ![Más iconos](assets/more-icon-27x15.png) en el encabezado del informe y, a continuación, haga clic en **Editar**.

1. En el lado derecho de la pantalla, en **Añadir un bloque**, efectúe lo siguiente:

   Arrastre el icono **Contenido web** al lienzo directamente a la ubicación que desee.

   O

   Haga doble clic en el icono **Contenido web** para agregar un bloque a la parte superior del lienzo.

   >[!TIP]
   >
   >Puede cambiar el tamaño del bloque una vez colocado arrastrando sus controladores de esquina.

1. Haga clic en **Contenido web sin título** en el encabezado del bloque y, a continuación, escriba un título para el bloque.
1. Haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png) del encabezado del bloque.

   ![Editar icono en el encabezado del bloque](assets/web-content-block-header-350x76.png)

1. En el panel **Configuración** que se abre, escriba la dirección URL completa de la página que desea mostrar (incluyendo &quot;https://&quot;) en el campo **URL**.

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

1. (Opcional) Haga clic en el botón de alternancia **Pasar parámetros** para abrir una lista de parámetros de paso disponibles.

   >[!WARNING]
   >
   >Los parámetros de paso están desactivados actualmente.

1. Haga clic en **Incrustar dirección URL** para guardar las selecciones y volver al informe.
