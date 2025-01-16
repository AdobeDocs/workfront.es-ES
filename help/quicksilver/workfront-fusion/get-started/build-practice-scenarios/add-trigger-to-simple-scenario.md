---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adición de un módulo de activador a un escenario básico
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 067ee6a1-f4c1-4602-ac39-0283255cced8
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 84%

---

# Adición de un módulo de activador a un escenario básico

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Agregar un módulo de déclencheur a un escenario básico](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-trigger-to-basic-scenario.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Los módulos de activador se colocan al principio de un escenario. Estos módulos comienzan una ejecución de escenario al cumplirse criterios específicos cuando se produce un cambio en un servicio determinado. El cambio puede consistir en la creación de registros nuevos, la eliminación de registros, la actualización de registros, etc.

Los módulos de sondeo comprueban el servicio en un intervalo de tiempo establecido y devuelven información sobre los cambios producidos durante ese intervalo de tiempo. Si no se produjeron cambios, el activador no ejecutará el escenario.

En este ejemplo, añadirá un módulo de activador que se ejecute cada 15 minutos e inicie un escenario si se enviaron solicitudes a una cola específica. A continuación, el escenario convertirá esas solicitudes en un proyecto.

En este ejemplo se modifica el escenario que se creó en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Requisitos previos

Es necesaria la creación del escenario descrito en [Crear un escenario básico](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) antes de seguir con este procedimiento.

## Adición y configuración del módulo de activador

### Añadir el módulo de activador

1. Abra el escenario en el editor de escenarios.
1. Haga clic con el botón derecho en el primer módulo (Búsqueda) y seleccione **Eliminar módulo**.

   El módulo se eliminará y quedará un marcador de posición en blanco.

1. Haga clic en el módulo en blanco y seleccione **Adobe Workfront** de la lista de aplicaciones.
1. Seleccione **Ver registro**.
1. Asegúrese de que el módulo utilice la misma conexión que el resto de módulos del escenario.
1. En el campo Filtro, seleccione **Solo registros nuevos**.
1. En el campo Tipo de registro, seleccione **Problema**.
1. En el cuadro Resultados, seleccione `ID`, `Name` y `Project ID`.
1. Haga clic en **Aceptar** para guardar la configuración del módulo.

   Aparecerá la ventana Elegir por dónde comenzar.

1. Seleccione **A partir de ahora**.

### Programación del módulo de activador

1. Haga clic en el reloj del módulo Ver registros.

   Se abrirá la ventana Configuración de la programación.

1. En el campo Ejecutar escenario, seleccione **A intervalos regulares**.

1. Haga clic en **Aceptar**.

### Actualización del segundo módulo

Como se reemplazó el primer módulo, el segundo deberá asignarse al nuevo primer módulo.

1. Abra el módulo Convertir objeto.
1. En el campo ID del problema, elimine el bloque de ID negro. El bloque es negro porque el módulo desde el que se asignó ya no está disponible.
1. Seleccione el bloque de ID situado bajo el primer módulo (Ver registros) para asignarlo al segundo módulo.
1. Haga clic en **Aceptar**.

### Prueba y activación

1. Vaya al entorno de Workfront al que se conecte Fusion y añada un problema.
1. Haga clic en **[!UICONTROL Ejecutar una vez]**, en la esquina inferior izquierda del editor de escenarios.
1. Examine el resultado para asegurarse de que el escenario se ejecutó según lo esperado.
1. Cuando esté seguro de que el escenario funciona según lo esperado, haga clic en el conmutador **Programando** de la parte inferior izquierda de la pantalla para **Activar**.

   Esto activará el escenario.
1. En [!DNL Workfront Fusion], haga clic en **[!UICONTROL Guardar]** cerca de la esquina inferior izquierda para guardar su progreso en el escenario.

   >[!IMPORTANT]
   >
   >Se recomienda guardar con frecuencia mientras se perfeccionan y prueban escenarios.

## Recursos

* Para obtener más información sobre los webhooks, consulte [Activadores instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md).
