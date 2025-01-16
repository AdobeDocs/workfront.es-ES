---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Operaciones en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 80%

---

# Operaciones en [!DNL Adobe Workfront Fusion]



>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Operaciones](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/operations-in-workfront-fusion.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Una operación en [!DNL Adobe Workfront Fusion] es una tarea realizada por un módulo. Para fines de seguimiento, cualquier acción correcta realizada por un módulo es una operación.

## Consideraciones al contar el número de operaciones

* En general, cualquier ejecución correcta de la etapa de acción se considera una operación.

* El primer módulo de un escenario se ejecuta solo una vez y siempre se cuenta como una operación, aunque no devuelva un paquete.

* El número de veces que se ejecuta el resto de los módulos depende del número de paquetes que deben procesar.  Una ejecución de un módulo para un paquete es una operación. Una excepción es el módulo del agregador, que se cuenta como una operación por cada conjunto de paquetes que se procesa.

* Las operaciones se cuentan en la fase [!UICONTROL Finalización] de la ejecución de un escenario.

* Los siguientes **no** se cuentan como operaciones:

   * Cualquier paso del filtro.

   * Cualquier acción que falle o se detenga.

   * Cualquier ruta que no se ejecute porque no se cumplen las reglas de la ruta, como las rutas de reserva o deshabilitadas.

   * Cualquier acción que no se ejecute, ya sea porque un filtro no ha permitido el paso de datos o porque el escenario se ha detenido debido a un error.

## Límites de operación

Es posible que su organización tenga un límite mensual de operaciones. Esto se basa en el plan de [!DNL Workfront] que compró su organización. El plan [!UICONTROL Ultimate] de [!DNL Workfront] ofrece operaciones ilimitadas.

Si su organización tiene un límite mensual, se le notificará cuando se aproxime a él. Si sobrepasa el límite, [!DNL Workfront] se pondrá en contacto con su organización para asegurarse de que el plan cumpla con sus necesidades.

## Visualización del número de operaciones realizadas en los últimos 30 días

Se pueden ver gráficos que muestran el número de operaciones realizadas. Estos gráficos están disponibles en las siguientes ubicaciones:

* **Panel de organización**: operaciones utilizadas por toda la organización
* **Panel de equipo**: operaciones utilizadas por los escenarios propiedad de este equipo ([!DNL Adobe Experience Cloud] solo)
* **Página de detalles del escenario**: operaciones utilizadas por este escenario ([!DNL Adobe Experience Cloud] solo)
