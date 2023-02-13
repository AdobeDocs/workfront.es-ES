---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestión de errores avanzada en [!DNL Adobe] Workfront Fusion
description: Las técnicas avanzadas de gestión de errores incluyen el filtrado y el anidado.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# Gestión de errores avanzada en [!DNL Adobe Workfront Fusion]

Las técnicas avanzadas de gestión de errores incluyen el filtrado y el anidado.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Filtrando

Existen dos tipos de filtrado que pueden realizarse en una ruta de controlador de errores.

* [Adición de un filtro a la ruta del controlador de errores](#adding-a-filter-to-the-error-handler-route)
* [Adición de un router seguido de filtros a la ruta del controlador de error](#adding-a-router-followed-by-filters-to-the-error-handler)

### Adición de un filtro a la ruta del controlador de errores

Puede utilizar un filtro para controlar qué errores gestiona la ruta del controlador de errores. Esto le permite procesar solo tipos específicos de errores. Si un error no pasa a través del filtro, se tratará como si no hubiera ninguna ruta de controlador de errores definida para el módulo dado.

>[!INFO]
>
>**Ejemplo:**
>
>![](assets/filter-error-handling-350x238.png)

### Adición de un [!UICONTROL Enrutador] seguido de filtros al controlador de error

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>En este ejemplo, el error se produce en la [!UICONTROL Crear una carpeta] módulo (A), que tiene una ruta regular y una ruta de controlador de errores. Este último va seguido de un router con una ruta que tiene un filtro que define un tipo específico de error (se produce un error de datos) y el otro es la ruta predeterminada para todos los demás errores. La primera ruta termina con el [!UICONTROL Reanudar] directiva que contiene valores sustitutivos para que el escenario se reanude desde el módulo A ([!UICONTROL Crear una carpeta]), mientras que la segunda ruta termina con el [!UICONTROL Reversión] que detiene la ejecución del escenario inmediatamente.

Consulte [Error de procesamiento en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) para obtener más información sobre varios tipos de error y sobre cómo [!DNL Workfront Fusion] los procesa y evalúa.

### El escenario de ejemplo

Puede configurar esta situación de ejemplo para comprender cómo funcionan estos filtros para la gestión de errores.

Usar una [!DNL Dropbox] carpeta para cargar un archivo en lugar de crear uno nuevo

Si usa la variable [!UICONTROL Crear una carpeta] módulo activado [!DNL Dropbox] y ya existe una carpeta con el mismo nombre, el módulo generará un error de datos como se muestra a continuación:

![](assets/dropbox-350x276.png)

El escenario completo:

![](assets/dropbox-scenario-350x190.png)

1. La variable [!UICONTROL Herramientas] > [!UICONTROL Establecer variable] El módulo contiene el nombre de la carpeta
1. La variable [!UICONTROL HTTP] >[!UICONTROL Obtener un archivo] recupera el archivo que debe cargarse en la carpeta
1. La variable [!UICONTROL Dropbox] >[!UICONTROL Crear una carpeta] genera un error si ya existe una carpeta con el mismo nombre que la asignada en el módulo
1. La ruta del controlador de errores (burbujas transparentes) contiene un router para filtrar los errores
1. La primera ruta es para un tipo de error especificado llamado Error de datos como ya sabemos:

   1. Si se produce un error de datos y los detalles del error pasan por el filtro, la variable [!UICONTROL Dropbox] >[!UICONTROL Enumerar todos los archivos/subcarpetas en un módulo de carpetas] enumera todas las carpetas de [!DNL Dropbox]
   1. El filtro siguiente coincide con los nombres de carpeta
   1. La variable [!UICONTROL Reanudar] especifica el ID de la carpeta y la ruta de la carpeta de la carpeta existente y la ejecución del escenario se reanuda desde la [!UICONTROL Dropbox] >[!UICONTROL Crear una carpeta] pero en lugar de intentar crear una carpeta nueva, esta vez utiliza los valores de la variable [!UICONTROL Reanudar] directiva para pasar al siguiente módulo y cargar el archivo en la carpeta existente

1. La segunda ruta es para todos los demás errores y termina con el [!UICONTROL Reversión] directiva que resulta en detener el escenario inmediatamente

A continuación, una explicación detallada de la quinta declaración:

Para utilizar la carpeta existente en los módulos siguientes ([!UICONTROL Cargar un archivo] a continuación), debe añadir una ruta de controlador de error al módulo y recuperar la ruta de carpeta que se va a asignar a la variable [!UICONTROL Reanudar] módulo de directiva que sigue:

![](assets/add-error-handler-route-350x113.png)

El filtro de la primera ruta se configura para controlar solo el error en particular (error de datos) que aparece cuando ya existe una carpeta con el mismo nombre:

![](assets/condition-350x327.png)

La variable [!UICONTROL Dropbox] >[!UICONTROL Enumerar todos los archivos en una carpeta] está configurado para devolver todas las carpetas de la carpeta de destino. El siguiente filtro solo pasa al que originalmente intentamos crear (el nombre de la carpeta se almacena en el 33). Elemento Nombre de carpeta):

![](assets/condition2-350x193.png)

Al final, la variable [!UICONTROL Reanudar] proporciona la ruta de acceso Folder como salida para el módulo fallido. Tenga en cuenta que el ID de carpeta se ha dejado en blanco porque no lo necesita el[!UICONTROL Cargar un archivo]Módulo &#39;:

![](assets/flow-control-350x190.png)

## Anidado

Independientemente de dónde se encuentre un módulo, las rutas de tratamiento de errores se pueden crear e implementar en todos los módulos, excepto en los enrutadores. Por lo tanto, es posible crear una ruta de controlador de errores para un módulo que ya forma parte de una ruta de controlador de errores existente creada para otro módulo.

Este es un ejemplo de una ruta de controlador de error anidada:

![](assets/nested-error-handling-route-350x174.png)

En esta situación, la segunda ruta del controlador de errores está anidada en la primera ruta del controlador de errores. Si la variable [!UICONTROL Dropbox] >[!UICONTROL Creación de un módulo de carpetas] encuentra un error, la ejecución se mueve a Route 1, si la variable [!UICONTROL Error de datos] , se ejecuta el siguiente módulo seguido del [!UICONTROL Reanudar] módulo de directiva si no se produce un error con la variable [!UICONTROL Dropbox] >[!UICONTROL Enumerar todos los archivos/subcarpetas] en un módulo de carpetas.

Sin embargo, si se produce un error con esto [!DNL Dropbox] , luego la ejecución se mueve a la ruta 2 del controlador de errores y finaliza con el [!UICONTROL Ignorar] directiva. La variable [!UICONTROL Reanudar directiva] no se ejecuta en este caso.

Es una combinación de filtrado y anidación de controladores de error.

