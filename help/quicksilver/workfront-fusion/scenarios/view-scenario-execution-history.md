---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ver el historial de ejecución de un escenario en Adobe Workfront Fusion
description: Puede mostrar información sobre todas las ejecuciones para un escenario o buscar datos específicos en todas las ejecuciones del escenario.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# Ver el historial de ejecución de un escenario en [!DNL Adobe Workfront Fusion]

Puede mostrar información sobre todas las ejecuciones para un escenario o buscar datos específicos en todas las ejecuciones del escenario.

El historial de ejecución de un escenario muestra todas las ejecuciones de un escenario durante los últimos 30 días.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ver todas las ejecuciones de un escenario

### Ver el historial de ejecución de escenario en la variable [!UICONTROL Detalle del escenario] página

1. Haga clic en el **[!UICONTROL Situación]** en el panel izquierdo y, a continuación, haga clic en el escenario.

   O

   Si está trabajando en el escenario en el editor de escenarios, haga clic en la flecha izquierda ![](assets/exit-editing-arrow.png) cerca de la esquina superior izquierda de la ventana.

1. Vea la información en la lista de la derecha.

   ![](assets/open-history-tab-350x202.png)

   C

   También puede hacer clic en para ver una vista de página completa de esta información. La vista de página completa le permite filtrar el historial para ver ejecuciones específicas.

   Se enumeran los siguientes detalles para cada ejecución del escenario:

   * Fecha en la que se ejecutó **[!UICONTROL Inicio]**
   * **[!UICONTROL Estado]** (éxito o error)
   * Ejecutar **[!UICONTROL Duración]**
   * Número de **[!UICONTROL Operaciones]**
   * Tamaño de **[!UICONTROL Transferencia de datos]**
   * Vincular a **[!UICONTROL Detalles]**

### Ver el historial de ejecución de escenario en la variable [!UICONTROL Historial] ficha

La variable [!UICONTROL Historial] muestra más detalles de los que están disponibles en la pestaña [!UICONTROL Detalles del escenario] página. También puede filtrar y ordenar las ejecuciones en la variable [!UICONTROL Historial] pestaña .

1. Haga clic en el **[!UICONTROL Situación]** en el panel izquierdo y, a continuación, haga clic en el escenario.

   O

   Si está trabajando en el escenario en el editor de escenarios, haga clic en la flecha izquierda ![](assets/exit-editing-arrow.png) cerca de la esquina superior izquierda de la ventana.

1. Haga clic en el **[!UICONTROL Historial]** cerca de la esquina superior izquierda de la página
1. (Opcional) Para obtener información detallada sobre un escenario seleccionado en ejecución, incluidos los paquetes que se procesaron, haga clic en el **[!UICONTROL Detalles]** vínculo.

   Para obtener más información sobre el procesamiento de paquetes, consulte [Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >La variable [!UICONTROL detalles] El vínculo solo está visible si la ejecución tiene detalles disponibles.

## Filtrar el historial de ejecución del escenario

Puede filtrar el historial de ejecución para ver solo las ejecuciones con los valores especificados.

1. Abra el historial de página completa de un escenario como se describe en [Ver el historial de ejecución de escenario en la variable [!UICONTROL Historial] ficha](#view-scenario-execution-history-on-the-history-tab) en este artículo.
1. Haga clic en el [!UICONTROL filter] icono ![](assets/fusion-scenario-filter-icon.png) en el encabezado de la columna por la que desea filtrar.
1. En el [!UICONTROL filter] , introduzca los valores por los que desea filtrar.
1. Haga clic en **[!UICONTROL Guardar]**.

El icono de filtro es naranja en las columnas con un filtro activo actualmente.

## Ordenar el historial de ejecución del escenario

Puede ordenar el historial de ejecución del escenario.

1. Abra el historial de página completa de un escenario como se describe en [Ver el historial de ejecución de escenario en la variable [!UICONTROL Historial] ficha](#view-scenario-execution-history-on-the-history-tab) en este artículo.
1. Haga clic en el [!UICONTROL Ordenar] en el encabezado de la columna por la que desea filtrar.
1. Opcional: Para invertir el orden de la clasificación, haga clic en el botón [!UICONTROL Ordenar] de nuevo.

## Buscar todas las ejecuciones de un escenario

1. Haga clic en el **[!UICONTROL Situación]** icono ![](assets/scenarios-icon.png) en el panel izquierdo, haga clic en el escenario.

   O

   Si está trabajando en el escenario en el editor de escenarios, haga clic en la flecha izquierda ![](assets/exit-editing-arrow.png) cerca de la esquina superior izquierda de la ventana.

1. Haga clic en el **[!UICONTROL Historial]** cerca de la esquina superior izquierda de la pantalla.
1. Haga clic en **[!UICONTROL Búsqueda de texto completo]** en la parte superior de la lista de ejecuciones.

   O

   Tipo **Ctrl + Mayús + F** (Windows) o **Cmd + Mayús + F** (Mac) El [!UICONTROL Búsqueda en el historial] se abre.

1. (Opcional) Para buscar ejecuciones que contengan texto específico, escriba el texto en la barra de búsqueda de la variable **[!UICONTROL Búsqueda en el historial]** ventana.

   Para buscar texto exacto, rodee el texto con comillas dobles (&quot;ejemplo&quot;).

   >[!INFO]
   >
   >**Ejemplo:** Si desea buscar la ejecución que creó un proyecto específico, introduzca el ID del proyecto en la variable [!UICONTROL Búsqueda de texto completo] barra.
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. (Opcional) Para limitar la búsqueda por intervalo de fechas, seleccione las fechas de inicio y finalización de la búsqueda deseada en la [!UICONTROL Por intervalo de fechas] .

   >[!NOTE]
   >
   >* Las ejecuciones solo están disponibles para los 30 días anteriores.
   >
   >* [!DNL Workfront Fusion] almacena cargas útiles de weblock durante 30 días. El acceso a una carga útil de weblock más de 30 días después de su creación da como resultado el error &quot;[!UICONTROL No se pudo leer el archivo desde el almacenamiento.]&quot;



1. (Opcional) Para limitar la búsqueda por estado, seleccione el estado deseado en la **[!UICONTROL Por estado]** lista desplegable.


   Los estados disponibles son:

   * [!UICONTROL Todos]

   * [!UICONTROL Error]

   * [!UICONTROL Advertencia]

   * [!UICONTROL Correcto]

1. (Opcional) Cambie el orden en que aparecen los resultados en la **[!UICONTROL Ordenar por fechas]** lista desplegable.

1. (Opcional) Para copiar un ID de ejecución de escenario, haga clic en el botón **[!UICONTROL Copiar ID de ejecución]** icono <img src="assets/copy-fusion-execution-id-icon.png"> en la fila de la ejecución deseada

1. (Opcional) Haga clic en un resultado de la [!UICONTROL Búsqueda de texto completo] para examinar el paquete de salida del módulo de escenario que contiene la información.
