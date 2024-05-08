---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Añadir un filtro a un escenario básico
description: Los filtros le permiten asegurarse de que su escenario progresa solo si se cumplen ciertas condiciones.
author: Becky
feature: Workfront Fusion
source-git-commit: 5ba5b2e37e2ce58d96d11f24786feef57f8eb638
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Añadir un filtro a un escenario básico en [!DNL Adobe Workfront Fusion]

Los filtros le permiten asegurarse de que su escenario progresa solo si se cumplen ciertas condiciones.

En este ejemplo, agregará un filtro a su escenario que permite crear un nuevo proyecto a partir de una solicitud solo si la solicitud se envió a una cola de solicitudes específica.

Este ejemplo modifica el escenario creado en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Los módulos de déclencheur de Workfront incluyen filtros que permiten que un escenario se inicie solo si se cumplen determinadas condiciones. Sin embargo, dado que los filtros entre módulos se utilizan en todos los casos de uso que no sean de déclencheur o de Workfront, es importante aprender a utilizar filtros entre módulos. Este ejemplo utiliza un filtro entre módulos para la funcionalidad que se puede cumplir con un filtro en módulos.

## Requisitos previos

Debe crear el escenario descrito en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) antes de seguir este procedimiento.

## Añadir un filtro

### Preparación para añadir el filtro

1. Abra el primer escenario.
1. En el **Salidas** , seleccione `Project`.
Ahora debería tener `ID`, `Name`, y `Project` seleccionados.
1. Haga clic en Aceptar para guardar la configuración del módulo.
1. Abra Workfront.
1. En Workfront, busque el proyecto que representa la cola de solicitudes con la que trabajará el escenario de Fusion.

   Este proyecto debe estar en la misma cuenta de Workfront para la que está configurada la conexión Fusion.

1. Tome nota del ID del proyecto en la dirección URL.

   Ejemplo: https://\&lt;mydomain>.my.workfront.com/project/\&lt;projectid>/tasks

### Adición y configuración del filtro

1. Abra el escenario en el editor de escenarios.
1. Haga clic en el icono de llave inglesa ![Icono de llave inglesa](assets/wrench-icon.png) entre el primer y el segundo módulo y seleccione **Configuración de un filtro**.
1. En el campo Etiqueta, introduzca una etiqueta para este filtro, como &quot;Filtro para cola de solicitudes&quot;.
1. En el **Condición** , en el campo superior, asigne el `projectID` desde el primer módulo.

   ![Asignar ID de proyecto](assets/map-proj-id.png)
1. Deje el **Condición** operador as Equal to.
1. En el campo inferior de la **Condición** , pegue el ID del proyecto del que tomó nota en la dirección URL del proyecto en [Preparación para añadir el filtro](#prepare-to-add-the-filter).
1. Clic **OK** para guardar la configuración del filtro.

### Prueba y activación

1. Vaya al entorno de Workfront al que se está conectando Fusion y añada un problema al proyecto que especificó en el filtro. Agregar otro problema a un proyecto diferente.
1. Clic **[!UICONTROL Ejecutar una vez]** en la esquina inferior izquierda del editor de escenarios.
1. Examine el resultado para asegurarse de que el escenario se ejecutó según lo esperado.

   Ambos problemas deben aparecer en el resultado del primer escenario, pero solo el problema del proyecto especificado debe aparecer como entrada en el segundo escenario,
1. Cuando esté seguro de que el escenario funciona correctamente, haga clic en **Programación** en la parte inferior izquierda de la pantalla, seleccione **Activado**.

   Esto activa el escenario.
1. Entrada [!DNL Workfront Fusion], haga clic en **[!UICONTROL Guardar]** cerca de la esquina inferior izquierda para guardar el progreso del escenario.

   >[!IMPORTANT]
   >
   >Guarde con frecuencia mientras perfecciona y prueba un escenario.

## Recursos

* Para obtener más información sobre los filtros, consulte [Adición de un filtro a un escenario](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

