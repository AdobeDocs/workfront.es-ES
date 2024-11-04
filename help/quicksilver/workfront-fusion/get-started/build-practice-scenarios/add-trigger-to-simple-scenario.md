---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adición de un módulo de déclencheur a un escenario básico
description: Aprenda a añadir un módulo de déclencheur para permitir que el escenario busque periódicamente nuevas solicitudes y las convierta en proyectos.
author: Becky
feature: Workfront Fusion
exl-id: 067ee6a1-f4c1-4602-ac39-0283255cced8
source-git-commit: 7ad3fbcfa5be5074016f399560cca509d81f4714
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Adición de un módulo de déclencheur a un escenario básico

Los módulos de déclencheur se colocan al principio de un escenario. Estos módulos comienzan una ejecución de escenario cuando se cumplen criterios específicos cuando se ha producido un cambio en un servicio determinado. El cambio puede consistir en la creación de registros nuevos, la eliminación de registros, la actualización de registros, etc.

Los módulos de sondeo comprueban el servicio en un intervalo de tiempo establecido y devuelven información sobre los cambios que se produjeron durante ese intervalo de tiempo. Si no ha habido cambios, el déclencheur no ejecuta el escenario.

En este ejemplo, agregará un módulo de déclencheur que se ejecuta cada 15 minutos e inicia un escenario si se han enviado solicitudes a una cola específica. A continuación, el escenario convierte esas solicitudes en un proyecto.

Este ejemplo modifica el escenario creado en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Requisitos previos

Debe crear el escenario descrito en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) antes de seguir este procedimiento.

## Adición y configuración del módulo de déclencheur

### Añadir el módulo de déclencheur

1. Abra el escenario en el editor de escenarios.
1. Haga clic con el botón derecho en el primer módulo (Buscar) y seleccione **Eliminar módulo**.

   El módulo se elimina y se deja un marcador de posición en blanco.

1. Haga clic en el módulo en blanco y seleccione **Adobe Workfront** de la lista de aplicaciones.
1. Seleccionar **Registro de inspección**.
1. Asegúrese de que el módulo utiliza la misma conexión que el resto de módulos del escenario.
1. En el campo Filtro, seleccione **Solo registros nuevos**.
1. En el campo Tipo de registro, seleccione **Problema**.
1. En el cuadro Resultados, seleccione `ID`, `Name` y `Project ID`.
1. Haga clic en **Aceptar** para guardar la configuración del módulo.

   Aparece la ventana Elija por dónde comenzar.

1. Seleccionar **A partir de ahora**.

### Programación del módulo de déclencheur

1. Haga clic en el reloj del módulo Ver registros.

   Se abre la ventana Configuración de programación.

1. En el campo Ejecutar escenario, seleccione **A intervalos regulares**.

1. Haga clic en **Aceptar**.

### Actualización del segundo módulo

Dado que se ha reemplazado el primer módulo, el segundo debe asignarse al nuevo primer módulo.

1. Abra el módulo Convertir objeto.
1. En el campo ID de problema, elimine el bloque de ID negro. El bloque es negro porque el módulo desde el que se asignó ya no está disponible.
1. Seleccione el bloque de ID bajo el primer módulo (Ver registros) para asignarlo al segundo módulo.
1. Haga clic en **Aceptar**.

### Prueba y activación

1. Vaya al entorno de Workfront al que se está conectando Fusion y añada un problema.
1. Haga clic en **[!UICONTROL Ejecutar una vez]** en la esquina inferior izquierda del editor de escenarios.
1. Examine el resultado para asegurarse de que el escenario se ejecutó según lo esperado.
1. Cuando esté seguro de que el escenario funciona según lo esperado, haga clic en el botón de alternancia **Programando** en la parte inferior izquierda de la pantalla para **Activar**.

   Esto activa el escenario.
1. En [!DNL Workfront Fusion], haga clic en **[!UICONTROL Guardar]** cerca de la esquina inferior izquierda para guardar su progreso en el escenario.

   >[!IMPORTANT]
   >
   >Guarde con frecuencia mientras perfecciona y prueba un escenario.

## Recursos

* Para obtener más información sobre los webhooks, vea [déclencheur instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md).
