---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Flujo de ejecución de escenarios en Adobe Workfront Fusion
description: Este artículo explica cómo se ejecuta un escenario y cómo fluyen los datos a través de él. También explica dónde puede encontrar información sobre los datos procesados y cómo leerlos.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '797'
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

## Flujo de ejecución de escenario

Una vez que un escenario se configura correctamente y se activa, se ejecuta según su programación definida.

Cuando comienza el escenario, el primer módulo responde a un evento que se ha configurado para inspeccionar. Si devuelve algún paquete (datos), pasa al siguiente módulo y el escenario continúa, pasando los paquetes a través de cada módulo sucesivo, uno a uno.

Si los paquetes se procesan correctamente en todos los módulos, el escenario se marca como un éxito en el área de detalles del escenario, como se explica en [Detalles del escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* Para obtener más información sobre la configuración de un escenario, consulte [Configuración básica de escenarios en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* Para obtener más información sobre la activación de un escenario, consulte [Activación o desactivación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* Para obtener más información sobre cómo programar un escenario, consulte [Programar un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* Para obtener más información sobre los módulos, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

### Ejemplo: [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]

>[!INFO]
>
>**Ejemplo:** En un escenario que observa las solicitudes entrantes en [!DNL Workfront] y, a continuación, los convierte a [!DNL Workfront] proyectos, los datos fluirían de la siguiente manera.
>
>El primer paso del escenario, realizado por el primer módulo, es inspeccionar las solicitudes. Cada solicitud que se incluye se considera un paquete. Si el módulo se ejecuta sin encontrar ningún paquete, el escenario finaliza después del primer módulo.
>
>Si el primer módulo devuelve un paquete, este pasará por el resto del escenario. En este ejemplo, el resto del escenario está formado por el segundo y el último módulo, que convierten la solicitud en un proyecto.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### Ejemplo: [!UICONTROL [!DNL Workfront Fusion] para la automatización e integración del trabajo]

>[!INFO]
>
>**Ejemplo:** En un escenario que descarga documentos de [!DNL Adobe Workfront] y los envía a una carpeta en [!DNL Dropbox], los datos fluirían de la siguiente manera.
>
>El primer paso del escenario, realizado por el primer módulo, es inspeccionar los paquetes (documentos). En este ejemplo, el módulo observa los paquetes en [!DNL Workfront]. Si no devuelve un paquete, el escenario finaliza después del primer módulo.
>
>Si se devuelve un paquete, este pasa por el resto del escenario. En este ejemplo, el resto del escenario consiste en el segundo y último módulo, que carga el paquete en [!DNL Dropbox] carpeta.
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>Si el primer módulo devuelve varios paquetes, el primer paquete se carga en [!DNL Dropbox] antes de cargar el segundo paquete. Luego se carga el segundo paquete, luego el tercero, etc.

## Información sobre paquetes procesados

Para cada módulo, el paquete pasa por un proceso de 4 pasos antes de pasar al siguiente módulo o llegar a su destino final. El proceso de 4 pasos es Inicialización, Operación, Confirmar/Revertir y Finalización. Esto se denomina procesamiento de transacciones y ayuda a explicar cómo se procesaron los datos en un módulo.

Una vez finalizada la ejecución de un escenario, cada módulo muestra un icono con el número de operaciones realizadas. Puede hacer clic en este icono para mostrar la información detallada sobre los paquetes procesados, en el formato descrito anteriormente. Puede ver qué configuración de módulos se utilizó y qué paquetes devolvió cada módulo.

![](assets/info-processed-bundles-350x396.png)

Un módulo recibió información de entrada como:

* Imagen convertida
* Carpeta seleccionada donde se cargará la imagen
* Nombre original de [!DNL Facebook] imagen

Después del procesamiento, el módulo devolvió esta información de salida:

* ID de imagen asignado por [!DNL Dropbox]
* Ruta completa en la que [!DNL Dropbox] [!DNL Workfront Fusion] subió el archivo

La información anterior se captura para cada paquete por separado, tal como indican los cuadros desplegables [!UICONTROL Operación 1] y [!UICONTROL Operación 2] en la imagen.

Para obtener más información sobre el procesamiento de transacciones, consulte [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Error al ejecutar un escenario

Se puede producir un error durante la ejecución del escenario. Por ejemplo, si elimina el [!DNL Dropbox] carpeta que ha establecido como carpeta de destino en la configuración del módulo, el escenario termina con un mensaje de error. Para obtener más información sobre cómo gestionar errores, consulte [Error de procesamiento en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
