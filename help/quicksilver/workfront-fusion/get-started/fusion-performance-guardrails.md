---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: escenario,rendimiento
navigation-topic: get-started-with-workfront-fusion-2-0
title: Protecciones de rendimiento de Adobe Workfront Fusion
description: Adobe Workfront Fusion requiere una licencia de Adobe Workfront Fusion además de una licencia de Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 229fd48d604385a1bfcaba2fd34eb6f3bbdde7a7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] protecciones de rendimiento

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requiere un [!DNL Adobe Workfront Fusion] además de una [!DNL Adobe Workfront license].

La automatización de trabajo requiere un procesamiento rápido, por lo que [!DNL Adobe Workfront Fusion] está diseñado para ofrecer un alto rendimiento. Como los escenarios de larga duración pueden ralentizar el ritmo de su trabajo, hemos diseñado [!DNL Workfront Fusion] con protecciones que preservan el rendimiento y que limitan el tiempo de ejecución, el tamaño de los datos y otros parámetros de escenario. [!DNL Workfront Fusion] los diseñadores deben conocer estas barreras e incorporarlas en sus prácticas de diseño.

## Escenarios

* El tiempo de espera de ejecución del escenario predeterminado es **40 minutos**. Cuando la ejecución alcanza este tiempo de espera, [!DNL Workfront Fusion] interrumpe la ejecución del escenario después del siguiente ciclo u operación, según el escenario. Esto obliga al escenario a detenerse poco después de alcanzar el límite de 40 minutos
* El tamaño máximo de un modelo de escenario es **5 MB**, pero se recomienda mantener el tamaño del escenario en **3 MB**.

   Los módulos de aplicaciones que crean o actualizan datos con un gran número de campos pueden causar modelos muy grandes.

   * Al usar la variable [!DNL Workfront] , asegúrese de seleccionar solo los campos necesarios para los casos de uso de creación o actualización.
   * Cuando utilice otras aplicaciones, utilice módulos de API personalizados para interactuar con cualquier tipo de registro que tenga un gran número de campos.

* Aunque no hay límite para el número de módulos en un escenario, los escenarios con más de 150 módulos afectan negativamente al rendimiento de su [!DNL Workfront Fusion] sistema. Por este motivo, no se recomienda crear escenarios con más de 150 módulos.

## Operaciones

* El tiempo de espera predeterminado de la operación suele ser **40 segundos**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Archivos

* La capacidad total de procesamiento de archivos de Fusion es **1 GB**. El límite se basa en un coste total de memoria. Cada operación contribuye a ese costo. Si se descarga y carga un solo archivo de 400 MB, el costo total para la capacidad del archivo sería de 800 MB.

## Uso de memoria del servidor

* El uso de memoria del servidor para una sola ejecución se limita a **1 GB**.

   Muchos factores, como archivos grandes o módulos complejos, pueden afectar al uso de la memoria del servidor de maneras que son difíciles de predecir o controlar. Debido a esto, la ejecución del escenario puede superar el límite de 1 GB de memoria, incluso si el escenario sigue todas las demás protecciones de rendimiento. Si se supera el límite de memoria, se produce un error en la ejecución.

## Enlaces web

* El tamaño máximo predeterminado de una carga útil es **5 MB**.
* Los Webhooks están limitados a **100 solicitudes por segundo**. Cuando se alcanza este límite, Workfront Fusion envía un error 429 ([!UICONTROL Demasiadas solicitudes]).
* [!DNL Workfront Fusion] almacena cargas útiles de weblock durante 30 días. El acceso a una carga útil de weblock más de 30 días después de su recepción da como resultado el error &quot;[!UICONTROL No se pudo leer el archivo desde el almacenamiento.]&quot;
* Los Webhooks se desactivan automáticamente si se aplica cualquiera de las siguientes opciones:

   * El enlace web no ha estado conectado a ningún escenario durante más de 5 días
   * El enlace web solo se utiliza en escenarios inactivos, que han estado inactivos durante más de 30 días.

* Los enlaces web desactivados se eliminan y no se registran automáticamente si no están conectados a ningún escenario y han estado en estado desactivado durante más de 30 días.
