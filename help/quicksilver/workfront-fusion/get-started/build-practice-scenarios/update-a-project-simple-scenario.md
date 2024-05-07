---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adición de un módulo de déclencheur a un escenario básico
description: Aprenda a añadir un módulo de déclencheur para permitir que el escenario busque periódicamente nuevas solicitudes y las convierta en proyectos.
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Utilice una función para actualizar un proyecto en un escenario simple en [!DNL Adobe Workfront Fusion]

La actualización de un elemento de trabajo de Workfront es un caso de uso común para Workfront Fusion. En este ejemplo, utilizará una función para cambiar el nombre de un proyecto a mayúsculas.

Fusion incluye muchos tipos de funciones que le permiten transformar y realizar lógica condicional en sus datos. Para obtener más información sobre el uso de funciones, consulte [Asignación de información de un módulo a otro en Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

Este ejemplo modifica el escenario creado en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Requisitos previos

Debe crear el escenario descrito en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) antes de seguir este procedimiento.

## Usar una función para actualizar un proyecto

### Agregue el módulo Actualizar registro a su escenario

1. Abra el escenario en el editor de escenarios.
1. Pase el ratón sobre el círculo parcial a la derecha del del módulo y haga clic en **[!UICONTROL Añadir otro módulo]**.
1. Seleccionar [!DNL Adobe Workfront] en la lista de aplicaciones, elija el módulo **[!UICONTROL Actualizar registro]**.
1. en el campo ID, seleccione el bloque ID que se encuentra en el módulo Convertir objeto. Este es el ID del proyecto que ese módulo generó.

   ![ID del objeto Convert](assets/id-convert-object.png)

1. En el campo Tipo de registro, seleccione Proyecto, ya que el objeto que se va a actualizar es un proyecto.
1. En el área Seleccionar campos para asignar, seleccione Nombre.

   Se abrirá un campo Nombre.

### Asignación de la función para la actualización de nombres

Cuando este escenario convierte una solicitud en un proyecto, el nombre del proyecto es el mismo que la solicitud. La función toma ese nombre y pone en mayúsculas todas las letras que contiene.

1. Haga clic en **Nombre** field.

   Se abrirá el panel Asignación.
1. En el panel de asignación, haga clic en **Funciones de texto y binarias** icono. ![Icono de funciones de texto](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. Seleccione la función **upper**.

   La función aparece en el campo Nombre, incluido el formato de la entrada que espera.

   La entrada para este ejemplo es el nombre del problema desde el que se convirtió el proyecto.

1. Mueva el cursor entre los paréntesis, ya que aquí es donde irá la entrada.
1. En el panel de asignación, haga clic en **salida del módulo** icono. ![Icono de salida de módulo](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. Seleccione el bloque de nombre que generó el primer módulo.

   El bloque de nombre aparece en la función.

   ![Bloque de nombres en la función](assets/map-name.png)

1. Haga clic en Aceptar para guardar la configuración del módulo.

### Prueba y activación

1. Pruebe el escenario haciendo clic en **Ejecutar una vez** en la esquina inferior izquierda de la pantalla.
1. Examine el resultado para asegurarse de que el escenario se ejecutó según lo esperado.
1. Cuando esté seguro de que el escenario funciona correctamente, haga clic en **Programación** en la parte inferior izquierda de la pantalla, seleccione **Activado**.

   Esto activa el escenario. Los escenarios activos se ejecutan según la programación establecida en el módulo de déclencheur.
1. Entrada [!DNL Workfront Fusion], haga clic en **[!UICONTROL Guardar]** cerca de la esquina inferior izquierda para guardar el progreso del escenario.

   >[!IMPORTANT]
   >
   >Guarde con frecuencia mientras perfecciona y prueba un escenario.

## Recursos:

* [Asignación de elementos mediante funciones en [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
