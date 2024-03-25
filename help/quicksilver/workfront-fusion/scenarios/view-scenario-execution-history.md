---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Visualización del historial de ejecución de un escenario en Adobe Workfront Fusion
description: Puede mostrar información sobre todas las ejecuciones de un escenario o puede buscar datos específicos en todas las ejecuciones del escenario.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: ae57c38149bf6db3bbbb471fad8f3567b7d712a7
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# Visualización del historial de ejecución de un escenario en [!DNL Adobe Workfront Fusion]

Puede mostrar información sobre todas las ejecuciones de un escenario o puede buscar datos específicos en todas las ejecuciones del escenario.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ver todas las ejecuciones de un escenario

### Ver historial de ejecución de escenario en [!UICONTROL Detalles del escenario] página

1. Haga clic en **[!UICONTROL Escenario]** en el panel izquierdo y, a continuación, haga clic en el escenario.

   O

   Si está trabajando en el escenario en el Editor de escenarios, haga clic en la flecha izquierda ![](assets/exit-editing-arrow.png) cerca de la esquina superior izquierda de la ventana.

1. Vea la información en la lista de la derecha.

   ![](assets/open-history-tab-350x202.png)

   También puede hacer clic en para ver una vista de página completa de esta información. La vista de página completa permite filtrar el historial para ver ejecuciones específicas.

   Se enumeran los siguientes detalles para cada ejecución del escenario:

   * Fecha en la que se realizó la ejecución **[!UICONTROL Iniciado]**
   * **[!UICONTROL Estado]** (correcto o fallido)
   * Ejecutar **[!UICONTROL Duración]**
   * Número de **[!UICONTROL Operaciones]**
   * Tamaño de **[!UICONTROL Transferencia de datos]**
   * Vincular a **[!UICONTROL Detalles]**

>[!NOTE]
>
>El historial de escenarios muestra un **Procesando** junto a los escenarios que se han ejecutado recientemente, mientras los detalles de ejecución se escriben en el almacenamiento. El procesamiento se produce inmediatamente después de que se ejecute el escenario. y no debe durar más de unos minutos. Es posible que los detalles de la ejecución del escenario no estén visibles mientras se procesa la ejecución.

### Ver historial de ejecución de escenario en [!UICONTROL Historial] pestaña

El [!UICONTROL Historial] La pestaña muestra más detalles de los que están disponibles en [!UICONTROL Detalles del escenario] página. También puede filtrar y ordenar las ejecuciones en [!UICONTROL Historial] pestaña.

1. Haga clic en **[!UICONTROL Escenario]** en el panel izquierdo y, a continuación, haga clic en el escenario.

   O

   Si está trabajando en el escenario en el Editor de escenarios, haga clic en la flecha izquierda ![](assets/exit-editing-arrow.png) cerca de la esquina superior izquierda de la ventana.

1. Haga clic en **[!UICONTROL Historial]** pestaña cerca de la esquina superior izquierda de la página
1. (Opcional) Para obtener información detallada sobre la ejecución de un escenario seleccionado, incluidos los paquetes que se procesaron, haga clic en **[!UICONTROL Detalles]** vínculo.

   Para obtener más información sobre el procesamiento de paquetes, consulte [Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >* El [!UICONTROL detalles] El vínculo de solo es visible si la ejecución tiene detalles disponibles.
   >
   >* El historial de escenarios muestra un **Historial de procesamiento** junto a los escenarios que se han ejecutado recientemente, mientras los detalles de ejecución se escriben en el almacenamiento. El procesamiento se produce inmediatamente después de que se ejecute el escenario. y no debe durar más de unos minutos. Es posible que los detalles de la ejecución del escenario no estén visibles mientras se procesa la ejecución.

## Filtrado del historial de ejecución del escenario

Puede filtrar el historial de ejecución para ver solo las ejecuciones con los valores especificados.

1. Abra el historial de página completa de un escenario como se describe en [Ver historial de ejecución de escenario en [!UICONTROL Historial] pestaña](#view-scenario-execution-history-on-the-history-tab) en este artículo.
1. Haga clic en [!UICONTROL filter] icono ![](assets/fusion-scenario-filter-icon.png) en el encabezado de la columna por la que desea filtrar.
1. En el [!UICONTROL filter] , introduzca los valores por los que desea filtrar.
1. Haga clic en **[!UICONTROL Guardar]**.

El icono de filtro es de color naranja en las columnas con un filtro activo actualmente.

## Ordenar el historial de ejecución del escenario

Puede ordenar el historial de ejecución del escenario.

1. Abra el historial de página completa de un escenario como se describe en [Ver historial de ejecución de escenario en [!UICONTROL Historial] pestaña](#view-scenario-execution-history-on-the-history-tab) en este artículo.
1. Haga clic en [!UICONTROL Ordenar] en el encabezado de la columna por la que desea filtrar.
1. Opcional: para invertir el orden, haga clic en [!UICONTROL Ordenar] icono de nuevo.

## Buscar todas las ejecuciones de un escenario

1. Haga clic en **[!UICONTROL Escenario]** icono ![](assets/scenarios-icon.png) en el panel izquierdo, haga clic en el escenario.

   O

   Si está trabajando en el escenario en el Editor de escenarios, haga clic en la flecha izquierda ![](assets/exit-editing-arrow.png) cerca de la esquina superior izquierda de la ventana.

1. Haga clic en **[!UICONTROL Historial]** pestaña cerca de la esquina superior izquierda de la pantalla.
1. Clic **[!UICONTROL Búsqueda de texto completo]** en la parte superior de la lista de ejecuciones.

   O

   Tipo **Ctrl + Mayús + F** (Windows) o **Cmd + Mayús + F** (Mac) El [!UICONTROL Buscar en el historial] se abre.

1. (Opcional) Para buscar ejecuciones que contengan texto específico, introduzca el texto en la barra de búsqueda de **[!UICONTROL Buscar en el historial]** ventana.

   Para buscar texto exacto, escriba el texto entre comillas dobles (&quot;ejemplo&quot;).

   >[!INFO]
   >
   >**Ejemplo:** Si desea encontrar la ejecución que creó un proyecto específico, introduzca el ID de proyecto en la variable [!UICONTROL Búsqueda de texto completo] barra.
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. (Opcional) Para limitar la búsqueda por intervalo de fechas, seleccione las fechas de inicio y finalización de la búsqueda deseada en la [!UICONTROL Por intervalo de fechas] área.

   >[!NOTE]
   >
   >* Las ejecuciones solo están disponibles durante los 30 días anteriores.
   >
   >* [!DNL Workfront Fusion] almacena cargas útiles de webhook durante 30 días. Acceder a una carga útil de gancho web más de 30 días después de crearla provoca el error &quot;[!UICONTROL Error al leer el archivo desde el almacenamiento.]&quot;


1. (Opcional) Para limitar la búsqueda por estado, seleccione el estado deseado en la **[!UICONTROL Por estado]** desplegable.


   Los estados disponibles son:

   * [!UICONTROL Todo]

   * [!UICONTROL Error]

   * [!UICONTROL Advertencia]

   * [!UICONTROL Correcto]

1. (Opcional) Cambie el orden en que se muestran los resultados en la **[!UICONTROL Ordenar por fechas]** desplegable.

1. (Opcional) Para copiar un ID de ejecución de escenario, haga clic en **[!UICONTROL Copiar ID de ejecución]** icono <img src="assets/copy-fusion-execution-id-icon.png"> en la fila de la ejecución deseada

1. (Opcional) Haga clic en un resultado del [!UICONTROL Búsqueda de texto completo] para examinar el paquete de salida del módulo de escenario que contiene la información.
