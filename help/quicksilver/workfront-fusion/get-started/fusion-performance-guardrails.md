---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: escenario, rendimiento
navigation-topic: get-started-with-workfront-fusion-2-0
title: Protecciones de rendimiento de Adobe Workfront Fusion
description: Adobe Workfront Fusion requiere una licencia Adobe Workfront Fusion además de una licencia Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 7c27dc98c4ce59d598be537a1f09c6eddf9bce42
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] protecciones de rendimiento

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requiere una licencia de [!DNL Adobe Workfront Fusion] además de [!DNL Adobe Workfront license].

La automatización del trabajo requiere un procesamiento rápido, por lo que [!DNL Adobe Workfront Fusion] está diseñado para un alto rendimiento. Dado que los escenarios de larga duración pueden ralentizar el ritmo de trabajo, hemos diseñado [!DNL Workfront Fusion] con protecciones que preservan el rendimiento y limitan el tiempo de ejecución, el tamaño de los datos y otros parámetros de escenario. Los diseñadores de [!DNL Workfront Fusion] deben tener en cuenta estas protecciones e incorporarlas en sus prácticas de diseño.

## Navegadores

* Workfront Fusion solo admite exploradores basados en Chrome.

## Escenarios

* El tiempo de espera de ejecución del escenario predeterminado es de **40 minutos**. Cuando la ejecución alcanza este tiempo de espera, [!DNL Workfront Fusion] interrumpe la ejecución del escenario después del siguiente ciclo u operación, según el escenario. Esto obliga al escenario a detenerse poco después de alcanzar el límite de 40 minutos
* El tamaño máximo de un modelo de escenario es de **5 MB**, pero se recomienda mantener el tamaño de escenario por debajo de **3 MB**.

  Los módulos de aplicaciones que crean o actualizan datos con una gran cantidad de campos pueden causar modelos muy grandes.

   * Al usar la aplicación [!DNL Workfront], asegúrese de seleccionar solo los campos necesarios para los casos de uso de creación o actualización.
   * Cuando utilice otras aplicaciones, utilice módulos de API personalizados para interactuar con cualquier tipo de registro que tenga un gran número de campos.

* Aunque no hay límite para el número de módulos en un escenario, los escenarios con más de 150 módulos afectan negativamente al rendimiento del sistema [!DNL Workfront Fusion]. Por este motivo, no se recomienda crear escenarios con más de 150 módulos.

## Operaciones

* El tiempo de espera de operación predeterminado suele ser de **40 segundos**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Archivos

* La capacidad total de procesamiento de archivos de Fusion es de **1 GB**. El límite se basa en el coste total de la memoria. Cada operación contribuye a ese coste. Si se descarga y carga un solo archivo de 400 MB, el coste total de la capacidad del archivo sería de 800 MB.
* Las organizaciones con el plan Workfront Ultimate tienen acceso a un mayor procesamiento de archivos que supera los 1 GB. La plataforma Fusion puede admitir archivos individuales de hasta 15 GB para una sola acción (por ejemplo, cargar archivo), pero hay otros factores que afectan a la transferencia de datos. El límite de tamaño de archivo de una sola acción depende del servicio web al que se conecte Fusion. La transferencia de datos es el procesamiento total de una sola ejecución. Esto significa que varias acciones en una sola ejecución contribuyen a la transferencia total de datos. Fusion procesará archivos hasta que se alcance el límite de ejecución de 40 minutos.

  Para obtener más información, consulte [Uso de archivos grandes en Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/fusion-large-files.md).


## Uso de memoria del servidor

* El uso de memoria del servidor para una sola ejecución está limitado a **1 GB**.

  Muchos factores, como los archivos grandes o los módulos complejos, pueden afectar al uso de la memoria del servidor de formas difíciles de predecir o controlar. Debido a esto, la ejecución del escenario puede superar el límite de memoria de 1 GB, incluso si el escenario sigue todas las demás protecciones de rendimiento. Si se supera el límite de memoria, la ejecución falla.

## Webhooks

* El tamaño máximo predeterminado de una carga útil es **5 MB**.
* Los enlaces web están limitados a **100 solicitudes por segundo**. Cuando se alcanza este límite, Workfront Fusion envía un estado 429 ([!UICONTROL Demasiadas solicitudes]).
* [!DNL Workfront Fusion] almacena cargas útiles de ganchos web durante 30 días. Acceder a una carga útil de gancho web más de 30 días después de recibirla provoca el error &quot;[!UICONTROL No se pudo leer el archivo desde el almacenamiento.]&quot;
* Los webhooks se desactivan automáticamente si se aplica cualquiera de las siguientes opciones:

   * El webhook no ha estado conectado a ningún escenario durante más de 5 días
   * El webhook solo se utiliza en escenarios inactivos, que han estado inactivos durante más de 30 días.

* Los webhooks desactivados se borran y no se registran automáticamente si no están conectados a ningún escenario y han estado en estado desactivado durante más de 30 días.

## Historial de ejecución

* Los registros del historial de ejecución están limitados a un tamaño de **100 MB**. Si el historial de ejecución supera este tamaño, solo se mostrarán los primeros 100 MB.
* Si un escenario tiene varias ejecuciones simultáneas. solo se muestran 5 ejecuciones en el área Ejecuciones de la página de detalles del escenario. Esto ocurre incluso cuando se están ejecutando más de 5 ejecuciones.

## Ejecuciones incompletas

* Las ejecuciones incompletas están limitadas a un tamaño total de **500 MB**. Si se alcanza el límite de 500 MB, no se almacenarán más ejecuciones incompletas.

## Reintentos

* Al utilizar el módulo Break y especificar la directiva Retry, si un escenario falla consecutivamente 10 veces dentro de un intervalo de tiempo de 2 minutos, el escenario se desactiva automáticamente.

