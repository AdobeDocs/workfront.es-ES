---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Flujo de ejecución de escenario en Adobe Workfront Fusion
description: Este artículo explica cómo se ejecuta un escenario y cómo fluyen los datos a través de él. También explica dónde puede encontrar información sobre los datos procesados y cómo leerlos.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]

Este artículo explica cómo se ejecuta un escenario y cómo fluyen los datos a través de él. También explica dónde puede encontrar información sobre los datos procesados y cómo leerlos.

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

## Flujo de ejecución del escenario

Una vez configurado y activado correctamente un escenario, se ejecuta según su programación definida.

A medida que comienza el escenario, el primer módulo responde a un evento que se ha configurado para observar. Si devuelve paquetes (datos), se transfieren al siguiente módulo y el escenario continúa, pasando los paquetes a través de cada módulo sucesivo, uno por uno.

Si los paquetes se procesan correctamente en todos los módulos, el escenario se marca como un éxito en el área de detalles del escenario, tal como se explica en [Detalles del escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* Para obtener más información sobre la configuración de un escenario, consulte [Configuración básica de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* Para obtener más información sobre la activación de un escenario, consulte [Activar o desactivar un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* Para obtener más información sobre cómo programar un escenario, consulte [Programar un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* Para obtener más información sobre los módulos, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

### Ejemplo: [!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]

>[!INFO]
>
>**Ejemplo:** En un escenario que observa solicitudes entrantes en [!DNL Workfront] y luego los convierte en [!DNL Workfront] proyectos, los datos fluirían de la siguiente manera.
>
>El primer paso del escenario, realizado por el primer módulo, es observar las solicitudes. Cada solicitud que ingresa se considera un paquete. Si el módulo se ejecuta sin encontrar ningún paquete, el escenario finaliza después del primer módulo.
>
>Si el primer módulo devuelve un paquete, el paquete pasa por el resto del escenario. En este ejemplo, el resto del escenario consta del segundo y último módulo, que convierte la solicitud en un proyecto.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### Ejemplo: [!UICONTROL [!DNL Workfront Fusion] para la automatización e integración del trabajo]

>[!INFO]
>
>**Ejemplo:** En una situación en la que se descargan documentos de [!DNL Adobe Workfront] y los envía a una carpeta de [!DNL Dropbox], los datos fluirían de la siguiente manera.
>
>El primer paso del escenario, realizado por el primer módulo, es buscar paquetes (documentos). En este ejemplo, el módulo observa los paquetes de [!DNL Workfront]. Si no devuelve un paquete, el escenario finaliza después del primer módulo.
>
>Si se devuelve un paquete, el paquete pasa por el resto del escenario. En este ejemplo, el resto del escenario consiste en el segundo y último módulo, que carga el paquete en el [!DNL Dropbox] carpeta.
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>Si el primer módulo devuelve varios paquetes, el primer paquete se carga en [!DNL Dropbox] antes de que se cargue el segundo paquete. A continuación, se carga el segundo paquete, luego el tercero, etc.

## Información sobre paquetes procesados

Para cada módulo, el paquete pasa por un proceso de 4 pasos antes de pasar al siguiente módulo o alcanzar su destino final. El proceso de 4 pasos es Inicialización, Operación, Confirmación/Reversión y Finalización. Esto se denomina procesamiento de transacciones y ayuda a explicar cómo se procesaron los datos en un módulo.

Una vez finalizada la ejecución de un escenario, cada módulo muestra un icono con el número de operaciones realizadas. Puede hacer clic en este icono para mostrar la información detallada sobre los paquetes procesados, en el formato descrito anteriormente. Puede ver qué configuración de módulos se usó y qué paquetes fueron devueltos por cada módulo.

![](assets/info-processed-bundles-350x396.png)

Un módulo recibió información de entrada como:

* Imagen convertida
* Carpeta seleccionada en la que se cargará la imagen
* Nombre original del [!DNL Facebook] image

Tras el procesamiento, el módulo devolvió esta información de salida:

* ID de imagen asignado por [!DNL Dropbox]
* Ruta completa donde [!DNL Dropbox] [!DNL Workfront Fusion] cargado el archivo

La información anterior se captura para cada paquete por separado, como se indica en los cuadros desplegables [!UICONTROL Operación 1] y [!UICONTROL Operación 2] en la imagen.

Para obtener más información sobre el procesamiento de transacciones, consulte [Ejecución del escenario, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Error al ejecutar un escenario

Podría producirse un error durante la ejecución del escenario. Por ejemplo, si elimina la variable [!DNL Dropbox] carpeta que ha establecido como carpeta de destino en la configuración del módulo, el escenario termina con un mensaje de error. Para obtener más información sobre cómo gestionar errores, consulte [Error de procesamiento en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
