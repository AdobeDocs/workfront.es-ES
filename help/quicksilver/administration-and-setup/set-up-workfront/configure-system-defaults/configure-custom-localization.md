---
user-type: administrator
product-area: system-administration;setup
title: Configurar la localización personalizada
description: La localización personalizada le permite definir términos y frases personalizados en diferentes idiomas. A continuación, Workfront muestra estos términos en el idioma establecido en la configuración del explorador.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: b077c95d8bb795fcd7c0983c78b7533cb8167270
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 18%
---
# Configuración de la localización personalizada

{{highlighted-preview}}

La localización personalizada le permite <span class="preview"> usar AI</span> para definir términos y frases personalizados en diferentes idiomas. A continuación, Workfront muestra estos términos en el idioma establecido en la configuración de Adobe Identity Management (IMS) del usuario.

Por ejemplo, la etiqueta &quot;Audiencia objetivo&quot; se puede localizar con la palabra alemana &quot;Zielgruppe&quot;. Cualquier usuario con el alemán seleccionado como idioma principal del navegador ve la palabra &quot;Zielgruppe&quot; como una etiqueta para cualquier campo etiquetado como &quot;Audiencia objetivo&quot; en inglés.

Puede configurar las traducciones a varios idiomas. Los idiomas disponibles actualmente incluyen:

* Chino (tradicional)
* Chino (simplificado)
* Francés
* Alemán
* Italiano
* Japonés
* Coreano
* Portugués (Brasil)
* Español

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Flujo de trabajo Prime o superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront para configurar las traducciones.</p>  </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al configurar la localización

Tenga en cuenta lo siguiente al configurar la localización:

* Puede configurar un término para traducirlo a varios idiomas.
* La localización se aplica a las etiquetas de campo personalizado (incluso cuando se utiliza como encabezado de columna) y a la información sobre herramientas.
* La localización personalizada puede aplicarse a mensajes generados a partir de reglas de negocio, pero debe habilitarse en la regla de negocio.

  Para obtener instrucciones, vea [Habilitar la localización en una regla de negocio](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md#using-custom-localization-with-business-rules) en el artículo Crear y editar reglas de negocio.

## Configuración de traducciones

Las traducciones se configuran en el área de Configuración.

1. Haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o, si está disponible, haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Setup]** ![Icono de Configuración](/help/_includes/assets/gear-icon-setup.png).
1. En el área Configuración, haga clic en **Localización** en el panel de navegación izquierdo.
1. Para agregar una nueva traducción, haga clic en **Nueva fila**.
1. En la columna **English**, escriba el término en inglés que se debe traducir.
1. En la columna del idioma al que desee traducir el término, introduzca el término en el idioma de destino.
1. (Opcional) Para traducir la palabra a otros idiomas, añada la traducción a la columna de idioma correspondiente.
1. (Opcional) Para reordenar las columnas de idioma, haga clic en el encabezado de la columna que desee mover y arrástrela a la ubicación deseada.
1. (Opcional) Para eliminar traducciones de un término, haga clic en la casilla de verificación que hay junto al término y, a continuación, haga clic en **Eliminar** en la barra azul de la parte inferior de la página.

<div class="preview">

## Localizar texto personalizado sin traducir mediante traducciones de IA

Puede utilizar IA para localizar texto personalizado. Selecciona el término y los idiomas, y puede aprobar las traducciones antes de que se apliquen.

1. Haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o, si está disponible, haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Setup]** ![Icono de Configuración](/help/_includes/assets/gear-icon-setup.png).
1. En el área Configuración, haga clic en **Localización** en el panel de navegación izquierdo.
1. En el área Localización, seleccione la ficha **Texto personalizado sin traducir**.

   Aparecerá una lista de texto personalizado sin traducir. Esto incluye texto como etiquetas de campo y mensajes de reglas personalizadas.

1. Seleccione uno o varios términos que desee localizar.
1. En la barra azul de la parte inferior de la pantalla, selecciona **Traducir con IA**.

   Se abre la ventana Generar traducciones.

1. Haga clic en los idiomas a los que desee traducir el término o términos. Para seleccionar rápidamente todos los idiomas, haga clic en **Seleccionar todos**.
1. (Opcional) Para proporcionar una orientación más específica para la traducción, introduzca instrucciones en el campo &quot;Instrucciones para IA&quot;.
1. Haga clic en **Generar**.

   AI comienza a generar traducciones.

   Se abre la ventana Revisar traducciones.

1. (Opcional) Para ajustar las traducciones o añadir su propia traducción, haga clic en el cuadrado correspondiente de la tabla y escriba la traducción deseada.
1. Haga clic en **Guardar**.

## Traducir un término localizado a otros idiomas

Puede traducir un término previamente localizado a nuevos idiomas mediante IA o proporcionar su propia traducción.

1. Haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o, si está disponible, haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Setup]** ![Icono de Configuración](/help/_includes/assets/gear-icon-setup.png).
1. En el área Configuración, haga clic en **Localización** en el panel de navegación izquierdo.
1. En el área Localización, seleccione la ficha **Traducciones**.

   Se muestra una lista de los términos traducidos anteriormente y sus traducciones.

1. (Opcional) Para editar o introducir directamente una traducción, haga clic en el cuadro correspondiente de la tabla y escriba la traducción que desee.
1. Seleccione los términos para los que desea generar traducciones adicionales haciendo clic en las casillas de verificación situadas junto a esos términos.
1. En la barra azul de la parte inferior de la página, haz clic en **Rellenar con IA**.


   Se abre la ventana Generar traducciones.

1. Haga clic en los idiomas a los que desee traducir el término o términos. Para seleccionar rápidamente todos los idiomas, haga clic en **Seleccionar todos**.
1. (Opcional) Para proporcionar una orientación más específica para la traducción, introduzca instrucciones en el campo &quot;Instrucciones para IA&quot;.
1. Haga clic en **Generar**.

   AI comienza a generar traducciones.

   Se abre la ventana Revisar traducciones.

1. (Opcional) Para ajustar las traducciones o añadir su propia traducción, haga clic en el cuadrado correspondiente de la tabla y escriba la traducción deseada.
1. Haga clic en **Guardar**.
1. (Opcional) Para eliminar todas las traducciones de un término, haga clic en la casilla de verificación que hay junto al término y, a continuación, haga clic en **Eliminar** en la barra azul de la parte inferior de la página.


</div>
