---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Operaciones en Adobe Workfront Fusion
description: Una operación en Adobe Workfront Fusion es una tarea realizada por un módulo. Para fines de seguimiento, cualquier acción correcta realizada por un módulo es una operación.
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Operaciones en [!DNL Adobe Workfront Fusion]

Una operación en [!DNL Adobe Workfront Fusion] es una tarea realizada por un módulo. Para fines de seguimiento, cualquier acción correcta realizada por un módulo es una operación.

## Consideraciones al contar el número de operaciones

* En general, cualquier ejecución correcta de la etapa de acción se considera una operación.

* El primer módulo de un escenario se ejecuta solo una vez y siempre se cuenta como una operación, aunque no devuelva un paquete.

* El número de veces que se ejecuta el resto de los módulos depende del número de paquetes que deben procesar.  Una ejecución de un módulo para un paquete es una operación. Una excepción es el módulo del acumulador, que se cuenta como una operación por cada conjunto de paquetes que se procesa.

* Las operaciones se cuentan en la fase [!UICONTROL Finalización] de la ejecución de un escenario.

* Los siguientes **no** se cuentan como operaciones:

   * Cualquier paso del filtro.

   * Cualquier acción que falle o se detenga.

   * Cualquier ruta que no se ejecute porque no se cumplen las reglas de la ruta, como las rutas de reserva o deshabilitadas.

   * Cualquier acción que no se ejecute, ya sea porque un filtro no permitió el paso de datos o porque el escenario se detuvo debido a un error.

## Límites de operación

Es posible que su organización tenga un límite mensual de operaciones. Esto se basa en el plan [!DNL Workfront] que su organización compró. El plan [!UICONTROL Ultimate] [!DNL Workfront] ofrece operaciones ilimitadas.

Si su organización tiene un límite mensual, se le notificará cuando se aproxime al límite. Si sobrepasa el límite, [!DNL Workfront] se pondrá en contacto con su organización para asegurarse de que su plan cumpla con sus necesidades.

## Ver el número de operaciones realizadas en los últimos 30 días

Se pueden ver gráficos que muestran el número de operaciones realizadas. Estos gráficos están disponibles en las siguientes ubicaciones:

* **Panel de organización**: operaciones utilizadas por toda la organización
* **Panel del equipo**: operaciones utilizadas por los escenarios propiedad de este equipo ([!DNL Adobe Experience Cloud] solamente)
* **Página de detalles del escenario**: operaciones utilizadas por este escenario ([!DNL Adobe Experience Cloud] solamente)
