---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adición de un módulo de activador a un escenario básico
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: f4588063-024f-4520-986e-45342a6b6777
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 85%

---

# Utilizar una función para actualizar un proyecto en un escenario simple en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Use una función para actualizar un proyecto en un escenario básico](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/use-function-to-build-practice-scenario.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

La actualización de un elemento de trabajo de Workfront es un caso de uso común para Workfront Fusion. En este ejemplo, utilizará una función para cambiar el nombre de un proyecto para que esté en mayúsculas.

Fusion incluye muchos tipos de funciones que le permiten transformar y realizar lógica condicional en sus datos. Para obtener más información sobre cómo usar las funciones, consulte [Asignar información de un módulo a otro en Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

Este ejemplo modifica el escenario creado en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Requisitos previos

Debe crear el escenario descrito en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) antes de seguir este procedimiento.

## Utilizar una función para actualizar un proyecto

### Añada el módulo Actualizar registro a su escenario

1. Abra el escenario en el editor de escenarios.
1. Pase el puntero por encima del círculo parcial a la derecha del módulo y luego haga clic en **[!UICONTROL Añadir otro módulo]**.
1. Seleccione [!DNL Adobe Workfront] de la lista de aplicaciones y luego elija el módulo **[!UICONTROL Actualizar registro]**.
1. en el campo ID, seleccione el bloque ID que se encuentra en el módulo Convertir objeto. Este es el ID del proyecto que ese módulo generó.

   ![ID de Convertir objeto](assets/id-convert-object.png)

1. En el campo Tipo de registro, seleccione Proyecto, ya que el objeto que se va a actualizar es un proyecto.
1. En el área Seleccionar campos para asignar, seleccione Nombre.

   Se abrirá un campo Nombre.

### Asignación de la función para la actualización del nombre

Cuando este escenario convierte una solicitud en un proyecto, el nombre del proyecto es el mismo que la solicitud. La función toma ese nombre y pone en mayúsculas todas las letras que contiene.

1. Haga clic en el campo **Nombre**.

   Se abrirá el panel de asignación.
1. En el panel de asignación, haga clic en el icono **Funciones binarias y de texto**. ![Icono de funciones de texto](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. Seleccione la función **superior**.

   La función aparece en el campo Nombre, incluido el formato de la entrada que espera.

   La entrada para este ejemplo es el nombre del problema desde el que se convirtió el proyecto.

1. Mueva el cursor entre los paréntesis, ya que aquí es donde irá la entrada.
1. En el panel de asignación, haga clic en el icono **salida del módulo**. ![Icono de salida del módulo](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. Seleccione el bloque de nombres que generó el primer módulo.

   El bloque de nombres aparece en la función.

   ![Bloque de nombres en la función](assets/map-name.png)

1. Haga clic en Aceptar para guardar la configuración del módulo.

### Prueba y activación

1. Pruebe el escenario haciendo clic en **Ejecutar una vez** en la esquina inferior izquierda de la pantalla.
1. Examine el resultado para asegurarse de que el escenario se ejecutó según lo esperado.
1. Cuando esté seguro de que el escenario funciona según lo esperado, haga clic en el conmutador **Programando** en la parte inferior izquierda de la pantalla para **activarlo**.

   Esto activará el escenario. Los escenarios activos se ejecutan según la programación establecida en el módulo del activador.
1. En [!DNL Workfront Fusion], haga clic en **[!UICONTROL Guardar]** cerca de la esquina inferior izquierda para guardar su progreso en el escenario.

   >[!IMPORTANT]
   >
   >Se recomienda guardar con frecuencia mientras se perfeccionan y prueban escenarios.

## Recursos:

* [Asignar elementos usando funciones en  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
