---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adición de un módulo de déclencheur a un escenario básico
description: Aprenda a añadir un módulo de déclencheur para permitir que el escenario busque periódicamente nuevas solicitudes y las convierta en proyectos.
author: Becky
feature: Workfront Fusion
exl-id: f4588063-024f-4520-986e-45342a6b6777
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Usar una función para actualizar un proyecto en un escenario simple de [!DNL Adobe Workfront Fusion]

La actualización de un elemento de trabajo de Workfront es un caso de uso común para Workfront Fusion. En este ejemplo, utilizará una función para cambiar el nombre de un proyecto a mayúsculas.

Fusion incluye muchos tipos de funciones que le permiten transformar y realizar lógica condicional en sus datos. Para obtener más información sobre cómo usar las funciones, vea [Asignar información de un módulo a otro en Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

Este ejemplo modifica el escenario creado en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Requisitos previos

Debe crear el escenario descrito en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) antes de seguir este procedimiento.

## Usar una función para actualizar un proyecto

### Agregue el módulo Actualizar registro a su escenario

1. Abra el escenario en el editor de escenarios.
1. Pase el ratón sobre el círculo parcial a la derecha del del módulo y luego haga clic en **[!UICONTROL Agregar otro módulo]**.
1. Seleccione [!DNL Adobe Workfront] de la lista de aplicaciones y luego elija el módulo **[!UICONTROL Actualizar registro]**.
1. en el campo ID, seleccione el bloque ID que se encuentra en el módulo Convertir objeto. Este es el ID del proyecto que ese módulo generó.

   ![ID del objeto Convert](assets/id-convert-object.png)

1. En el campo Tipo de registro, seleccione Proyecto, ya que el objeto que se va a actualizar es un proyecto.
1. En el área Seleccionar campos para asignar, seleccione Nombre.

   Se abrirá un campo Nombre.

### Asignación de la función para la actualización de nombres

Cuando este escenario convierte una solicitud en un proyecto, el nombre del proyecto es el mismo que la solicitud. La función toma ese nombre y pone en mayúsculas todas las letras que contiene.

1. Haga clic en el campo **Nombre**.

   Se abrirá el panel Asignación.
1. En el panel de asignación, haga clic en el icono **Funciones binarias y de texto**. ![Icono de funciones de texto](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. Seleccione la función **upper**.

   La función aparece en el campo Nombre, incluido el formato de la entrada que espera.

   La entrada para este ejemplo es el nombre del problema desde el que se convirtió el proyecto.

1. Mueva el cursor entre los paréntesis, ya que aquí es donde irá la entrada.
1. En el panel de asignación, haga clic en el icono **salida del módulo**. ![Icono de salida de módulo](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. Seleccione el bloque de nombre que generó el primer módulo.

   El bloque de nombre aparece en la función.

   ![Bloque de nombres en la función](assets/map-name.png)

1. Haga clic en Aceptar para guardar la configuración del módulo.

### Prueba y activación

1. Pruebe el escenario haciendo clic en **Ejecutar una vez** en la esquina inferior izquierda de la pantalla.
1. Examine el resultado para asegurarse de que el escenario se ejecutó según lo esperado.
1. Cuando esté seguro de que el escenario funciona según lo esperado, haga clic en el botón de alternancia **Programando** en la parte inferior izquierda de la pantalla para **Activar**.

   Esto activa el escenario. Los escenarios activos se ejecutan según la programación establecida en el módulo de déclencheur.
1. En [!DNL Workfront Fusion], haga clic en **[!UICONTROL Guardar]** cerca de la esquina inferior izquierda para guardar su progreso en el escenario.

   >[!IMPORTANT]
   >
   >Guarde con frecuencia mientras perfecciona y prueba un escenario.

## Recursos:

* [Asignar elementos usando funciones en  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
