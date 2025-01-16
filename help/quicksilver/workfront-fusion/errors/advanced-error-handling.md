---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gestión avanzada de errores en [!DNL Adobe] Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 92%

---

# Tratamiento avanzado de errores en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Agregar filtrado y anidamiento a las rutas de control de errores](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/advanced-error-handling.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Las técnicas avanzadas de tratamiento de errores incluyen el filtrado y el anidamiento.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td role="rowheader">Licencia** de [!UICONTROL Adobe Workfront Fusion]</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere la licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Filtrando

Hay dos tipos de filtrado que pueden tener lugar en una ruta del controlador de errores.

* [Añadir un filtro a la ruta del controlador de errores](#adding-a-filter-to-the-error-handler-route)
* [Añadir un enrutador seguido de filtros a la ruta del controlador de errores](#adding-a-router-followed-by-filters-to-the-error-handler)

### Añadir un filtro a la ruta del controlador de errores

Puede utilizar un filtro para controlar qué errores gestiona la ruta del controlador de errores. Esto le permite procesar solamente tipos específicos de errores. Si un error no pasa el filtro, se tratará como si no hubiera ninguna ruta del controlador de errores definida para el módulo dado.

>[!INFO]
>
>**Ejemplo:**
>
>![](assets/filter-error-handling-350x238.png)

### Añadir un [!UICONTROL Router] seguido de filtros al controlador de errores

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>En este ejemplo, el error tiene lugar en el módulo [!UICONTROL Crear una carpeta] (A), que tiene una ruta normal y una ruta de controlador de errores. Una ruta tiene un filtro que define un tipo específico de error (Error de datos), y la otra es la ruta por defecto para todos los demás errores. La primera ruta termina con la directiva [!UICONTROL Reanudar] que contiene valores sustitutivos para que el escenario se reanude desde el módulo A ([!UICONTROL Crear una carpeta]), mientras que la segunda ruta termina con la directiva [!UICONTROL Reversión] que detiene inmediatamente la ejecución del escenario.

Consulte [Procesamiento de errores en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) para obtener más información sobre varios tipos de errores y sobre cómo [!DNL Workfront Fusion] los procesa y evalúa.

### El escenario de ejemplo

Puede configurar esta escena de ejemplo para entender cómo funcionan estos filtros para la gestión de errores.

Utilizar una carpeta [!DNL Dropbox] existente para subir un archivo en lugar de crear una nueva

Si utiliza el módulo [!UICONTROL Crear una carpeta] en [!DNL Dropbox] y ya existe una carpeta con el mismo nombre, el módulo arrojará un error de datos como se muestra a continuación:

![](assets/dropbox-350x276.png)

El escenario completo:

![](assets/dropbox-scenario-350x190.png)

1. El módulo [!UICONTROL Herramientas] > [!UICONTROL Establecer variable] contiene el nombre de la carpeta
1. El módulo [!UICONTROL HTTP] >[!UICONTROL Obtener un archivo] recupera el archivo que debe cargarse en la carpeta
1. El módulo [!UICONTROL Dropbox] >[!UICONTROL Crear una carpeta] genera un error si ya existe una carpeta con el mismo nombre que la asignada en el módulo
1. La ruta del controlador de errores (burbujas transparentes) contiene un enrutador para filtrar los errores
1. La primera ruta es para un tipo de error especificado llamado Error de datos, tal como lo conocemos ya:

   1. Si se produce un Error de datos y los detalles del error pasan por el filtro, el módulo [!UICONTROL Dropbox] >[!UICONTROL Lista todos los archivos/subcarpetas de una carpeta] lista todas las carpetas de [!DNL Dropbox]
   1. El filtro siguiente coincide con los nombres de las carpetas
   1. La directiva [!UICONTROL Reanudar] especifica el ID de la carpeta y la ruta de la carpeta existente y la ejecución del escenario se reanuda desde el módulo [!UICONTROL Dropbox] >[!UICONTROL Crear una carpeta] pero en lugar de intentar crear una nueva carpeta, esta vez utiliza los valores de la directiva [!UICONTROL Resume] para pasar al siguiente módulo y cargar el archivo en la carpeta existente

1. La segunda ruta es para todos los demás errores y termina con la directiva [!UICONTROL Rollback], lo que hace que se detenga el escenario inmediatamente

A continuación se ofrece una explicación detallada de la quinta declaración:

Con el fin de utilizar la carpeta existente en sus módulos posteriores ([!UICONTROL Subir un archivo] a continuación), es necesario añadir una ruta del controlador de errores al módulo y obtener la ruta de la carpeta que se asignará en el módulo directivo [!UICONTROL Reanudar] que sigue:

![](assets/add-error-handler-route-350x113.png)

El filtro de la primera ruta está configurado para gestionar únicamente el error concreto (Data Error) que aparece cuando ya existe una carpeta con el mismo nombre:

![](assets/condition-350x327.png)

El módulo [!UICONTROL Dropbox] >[!UICONTROL Lista todos los archivos de una carpeta] está configurado para devolver todas las carpetas de la carpeta de destino. El siguiente filtro solo pasa el que estábamos intentando crear originalmente (el nombre de la carpeta se almacena en el 33. Elemento nombre de carpeta):

![](assets/condition2-350x193.png)

Finalmente, la directiva [!UICONTROL Reanudar] proporciona la ruta de la carpeta como salida para el módulo que ha fallado. Tenga en cuenta que el ID de carpeta se ha dejado en blanco porque el módulo “[!UICONTROL Subir un archivo]” no lo necesita:

![](assets/flow-control-350x190.png)

## Anidado

Independientemente de la ubicación de un módulo, se pueden crear e implementar rutas de controlador de errores en todos los módulos, excepto en los enrutadores. Por lo tanto, es posible crear una ruta de controlador de errores para un módulo que ya forme parte de una ruta de controlador de errores existente creada para otro módulo.

Este es un ejemplo de una ruta anidada del controlador de errores:

![](assets/nested-error-handling-route-350x174.png)

En este escenario, la segunda ruta del controlador de errores está anidada en la primera ruta del controlador de errores. Así, si el módulo [!UICONTROL Dropbox] >[!UICONTROL Crear una carpeta] encuentra un error, la ejecución pasa a la ruta 1, si se pasa el filtro [!UICONTROL Error de Datos], se ejecuta el siguiente módulo seguido del módulo directivo [!UICONTROL Reanudar] si no se produce un error con el módulo [!UICONTROL Dropbox] >[!UICONTROL Listar todos los ficheros/subcarpetas] de una carpeta.

Sin embargo, si se produce un error con este módulo [!DNL Dropbox], la ejecución se mueve a la Ruta 2 del controlador de errores y termina con la directiva [!UICONTROL Ignorar]. El módulo [!UICONTROL Reanudar directiva] no se ejecuta en este caso.

Se trata de una combinación de controladores de error de filtrado y anidación.

