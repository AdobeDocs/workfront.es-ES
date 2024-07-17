---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Agregar un webhook a un escenario básico
description: Los webhooks, también conocidos como déclencheur instantáneos, son un tipo específico de módulo de déclencheur que puede iniciar un escenario cada vez que se realice un cambio, en lugar de hacerlo en una programación determinada.
author: Becky
feature: Workfront Fusion
exl-id: 6694b883-6f94-449c-bcfe-5a4053e8655a
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Agregar un webhook a un escenario básico en [!DNL Adobe Workfront Fusion]

Los webhooks, también conocidos como déclencheur instantáneos, son un tipo específico de módulo de déclencheur que puede iniciar un escenario cada vez que se realice un cambio, en lugar de hacerlo en una programación determinada.

En este ejemplo, agregará un webhook para iniciar un escenario en cuanto se haya enviado una solicitud a una cola específica. A continuación, el escenario convierte esas solicitudes en un proyecto.

Este ejemplo modifica el escenario creado en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Requisitos previos

Debe crear el escenario descrito en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) antes de seguir este procedimiento.

## Agregar y configurar el webhook

1. Abra el módulo Convertir objeto.
1. En el campo ID de problema, elimine el bloque de ID negro. El bloque es negro porque el módulo desde el que se asignó ya no está disponible.
1. Seleccione el bloque de ID bajo el primer módulo (Ver eventos) para asignarlo al segundo módulo.
1. Haga clic en **Aceptar**.

### Añadir el módulo webhook

1. Abra el escenario en el editor de escenarios.
1. Haga clic con el botón derecho en el primer módulo y seleccione **Eliminar módulo**.

   El módulo se elimina y se deja un marcador de posición en blanco.

1. Haga clic en el módulo en blanco y seleccione **Adobe Workfront** de la lista de aplicaciones.
1. Seleccione **Ver eventos**.
1. Haga clic en **Agregar** junto al campo Webhook.
1. en el campo Tipo de registro, seleccione **Problema**, de modo que el módulo se almacenará en déclencheur para los cambios en los problemas.
1. En el campo Estado, seleccione **Nuevo estado**. Este es un campo obligatorio que se utiliza para el filtro, que este ejemplo no cubre.
1. En el campo Origen de registro, seleccione **Solo nuevo registro**. Esto permite que el escenario entre en déclencheur cuando se agrega un problema, no cuando se actualiza o elimina uno.
1. Haga clic en **Guardar** para guardar la configuración del módulo.
