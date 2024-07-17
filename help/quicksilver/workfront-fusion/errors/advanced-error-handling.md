---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Tratamiento de errores avanzado en  [!DNL Adobe] Workfront Fusion
description: Las técnicas avanzadas de gestión de errores incluyen filtrado y anidamiento.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# Tratamiento de errores avanzado en [!DNL Adobe Workfront Fusion]

Las técnicas avanzadas de gestión de errores incluyen filtrado y anidamiento.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Filtrando

Existen dos tipos de filtrado que pueden realizarse en una ruta de tratamiento de errores.

* [Adición de un filtro a la ruta del controlador de error](#adding-a-filter-to-the-error-handler-route)
* [Agregar un enrutador seguido de filtros a la ruta del controlador de errores](#adding-a-router-followed-by-filters-to-the-error-handler)

### Adición de un filtro a la ruta del controlador de error

Puede utilizar un filtro para controlar qué errores gestiona la ruta del controlador de errores. Esto le permite procesar únicamente tipos de errores específicos. Si un error no pasa a través del filtro, se tratará como si no hubiera una ruta de controlador de error definida para el módulo determinado.

>[!INFO]
>
>**Ejemplo:**
>
>![](assets/filter-error-handling-350x238.png)

### Agregando un [!UICONTROL enrutador] seguido de filtros al controlador de errores

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>En este ejemplo, el error tiene lugar en el módulo [!UICONTROL Crear una carpeta] (A), que tiene una ruta normal y una ruta de controlador de error. A este último le sigue un enrutador con una ruta que tiene un filtro que define un tipo específico de error (Error de datos) y la otra que es la ruta predeterminada para todos los demás errores. La primera ruta termina con la directiva [!UICONTROL Resume], que contiene valores sustitutos para que el escenario se reanude desde el módulo A ([!UICONTROL Crear una carpeta]), mientras que la segunda ruta termina con la directiva [!UICONTROL Rollback], que detiene la ejecución del escenario inmediatamente.

Consulte [Procesamiento de errores en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) para obtener más información sobre varios tipos de errores y sobre cómo [!DNL Workfront Fusion] los procesa y evalúa.

### El escenario de ejemplo

Puede configurar esta situación de ejemplo para comprender cómo funcionan estos filtros para la gestión de errores.

Utilice una carpeta [!DNL Dropbox] existente para cargar un archivo en lugar de crear una nueva

Si usa el módulo [!UICONTROL Crear una carpeta] en [!DNL Dropbox] y ya existe una carpeta con el mismo nombre, el módulo generará un error de datos como se muestra a continuación:

![](assets/dropbox-350x276.png)

El escenario completo:

![](assets/dropbox-scenario-350x190.png)

1. El módulo [!UICONTROL Herramientas] > [!UICONTROL Establecer variable] contiene el nombre de la carpeta
1. El módulo [!UICONTROL HTTP] >[!UICONTROL Obtener un archivo] recupera el archivo que debe cargarse en la carpeta
1. El módulo [!UICONTROL Dropbox] >[!UICONTROL Crear una carpeta] genera un error si ya existe una carpeta con el mismo nombre que la asignada en el módulo
1. La ruta del controlador de errores (burbujas transparentes) contiene un enrutador para filtrar los errores
1. La primera ruta es para un tipo de error especificado llamado Error de datos, tal como lo conocemos ya:

   1. Si se produce un error de datos y los detalles del error pasan a través del filtro, [!UICONTROL Dropbox] >[!UICONTROL Enumerar todos los archivos/subcarpetas de un módulo de carpetas] enumera todas las carpetas de [!DNL Dropbox]
   1. El filtro siguiente coincide con los nombres de carpeta
   1. La directiva [!UICONTROL Resume] especifica el ID de carpeta y la ruta de la carpeta existente, y la ejecución del escenario se reanuda desde el módulo [!UICONTROL Dropbox] >[!UICONTROL Crear una carpeta], pero en lugar de intentar crear una nueva carpeta, esta vez usa los valores de la directiva [!UICONTROL Resume] para pasar al siguiente módulo y cargar el archivo en la carpeta existente

1. La segunda ruta es para todos los demás errores y termina con la directiva [!UICONTROL Rollback], lo que hace que se detenga el escenario inmediatamente

A continuación se ofrece una explicación detallada de la quinta declaración:

Para usar la carpeta existente en los módulos subsiguientes ([!UICONTROL Cargar un archivo] más abajo), debe agregar una ruta de controlador de error al módulo y recuperar la ruta de carpeta que se asignará al módulo de directiva [!UICONTROL Reanudar] que sigue:

![](assets/add-error-handler-route-350x113.png)

El filtro de la primera ruta está configurado para controlar únicamente el error concreto (Error de datos) que aparece cuando ya existe una carpeta con el mismo nombre:

![](assets/condition-350x327.png)

El módulo [!UICONTROL Dropbox] >[!UICONTROL Enumerar todos los archivos de una carpeta] está configurado para devolver todas las carpetas de la carpeta de destino. El siguiente filtro solo pasa el que estábamos intentando crear originalmente (el nombre de la carpeta se almacena en el 33. Nombre de carpeta (elemento):

![](assets/condition2-350x193.png)

Finalmente, la directiva [!UICONTROL Resume] proporciona la ruta de la carpeta como salida para el módulo con error. Tenga en cuenta que el ID de carpeta se ha dejado en blanco porque el módulo &#39;[!UICONTROL Cargar un archivo]&#39; no lo necesita:

![](assets/flow-control-350x190.png)

## Anidado

Independientemente de dónde se encuentre un módulo, se pueden crear e implementar rutas de controladores de errores en todos los módulos, excepto en los enrutadores. Por lo tanto, es posible crear una ruta de controlador de error para un módulo que ya forme parte de una ruta de controlador de error existente creada para otro módulo.

Este es un ejemplo de una ruta anidada del controlador de error:

![](assets/nested-error-handling-route-350x174.png)

En este escenario, la segunda ruta del controlador de errores está anidada en la primera ruta del controlador de errores. Por lo tanto, si [!UICONTROL Dropbox] >[!UICONTROL Crear un módulo de carpetas] encuentra un error, la ejecución pasa a la Ruta 1, si se pasa el filtro [!UICONTROL Error de datos], el siguiente módulo se ejecuta seguido del módulo de directiva [!UICONTROL Reanudar] si no se produce un error con el [!UICONTROL Dropbox] >[!UICONTROL Enumerar todos los archivos/subcarpetas] en un módulo de carpetas.

Sin embargo, si se produce un error con este módulo [!DNL Dropbox], la ejecución se mueve a la Ruta 2 del controlador de errores y termina con la directiva [!UICONTROL Ignore]. El módulo [!UICONTROL Reanudar directiva] no se ejecuta en este caso.

Se trata de una combinación de controladores de error de filtrado y anidación.

