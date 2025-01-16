---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Agregar un webhook a un escenario básico
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 6694b883-6f94-449c-bcfe-5a4053e8655a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 26%

---

# Agregar un webhook a un escenario básico en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Agregar un webhook a un escenario básico](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-a-webhook-to-basic-scenario.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Los webhooks, también conocidos como déclencheur instantáneos, son un tipo específico de módulo de déclencheur que puede iniciar un escenario cada vez que se realice un cambio, en lugar de hacerlo en una programación determinada.

En este ejemplo, agregará un webhook para iniciar un escenario en cuanto se haya enviado una solicitud a una cola específica. A continuación, el escenario convertirá esas solicitudes en un proyecto.

En este ejemplo se modifica el escenario que se creó en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Requisitos previos

Debe crear el escenario descrito en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) antes de seguir este procedimiento.

## Agregar y configurar el webhook

1. Abra el módulo Convertir objeto.
1. En el campo ID del problema, elimine el bloque de ID negro. El bloque es negro porque el módulo desde el que se asignó ya no está disponible.
1. Seleccione el bloque de ID bajo el primer módulo (Ver eventos) para asignarlo al segundo módulo.
1. Haga clic en **OK**.

### Añadir el módulo webhook

1. Abra el escenario en el editor de escenarios.
1. Haga clic con el botón derecho en el primer módulo y seleccione **Eliminar módulo**.

   El módulo se eliminará y quedará un marcador de posición en blanco.

1. Haga clic en el módulo en blanco y seleccione **Adobe Workfront** de la lista de aplicaciones.
1. Seleccione **Ver eventos**.
1. Haga clic en **Agregar** junto al campo Webhook.
1. en el campo Tipo de registro, seleccione **Problema**, de modo que el módulo se almacenará en déclencheur para los cambios en los problemas.
1. En el campo Estado, seleccione **Nuevo estado**. Este es un campo obligatorio que se utiliza para el filtro, que este ejemplo no cubre.
1. En el campo Origen de registro, seleccione **Solo nuevo registro**. Esto permite que el escenario entre en déclencheur cuando se agrega un problema, no cuando se actualiza o elimina uno.
1. Haga clic en **Guardar** para guardar la configuración del módulo.
