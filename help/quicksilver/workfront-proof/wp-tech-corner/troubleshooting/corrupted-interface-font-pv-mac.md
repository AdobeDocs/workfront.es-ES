---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 'Solución de problemas: fuente de interfaz dañada en el visor de pruebas en Mac'
description: 'Si nota que el visor de pruebas no muestra correctamente la fuente de la interfaz, esto puede deberse a algunos problemas con las fuentes en el equipo Mac. Para resolver el problema, pruebe las siguientes soluciones: EDITAR.'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Solución de problemas: fuente de interfaz dañada en el visor de pruebas en Mac

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Si nota que el visor de pruebas no muestra correctamente la fuente de la interfaz, esto puede deberse a algunos problemas con las fuentes en el equipo Mac. Para resolver el problema, pruebe las siguientes soluciones:

## Eliminar duplicados de fuentes

Compruebe si hay fuentes duplicadas en el sistema.

1. Cierre el explorador que esté usando.
1. Abra la aplicación Libro de fuentes en la carpeta Aplicaciones .
1. Haga clic en **[!UICONTROL Todas las fuentes]** (1)
1. Haga clic en **[!UICONTROL Editar]** > **[!UICONTROL Buscar duplicados habilitados]**.

1. Haga clic en **[!UICONTROL Sí]** para resolver duplicados.
1. Si ve una advertencia sobre fuentes dañadas, haga clic en **[!UICONTROL Sí]**.
1. Reinicie el equipo.
1. Vuelva a intentar la prueba.

## Borrar la caché de fuentes

A veces, las cachés de fuentes en Mac OS X se corrompen. Por ejemplo, cuando se vuelve a instalar una fuente o una familia de fuentes varias veces o si se ha actualizado o reinstalado una aplicación. Aparte de los archivos de caché de fuentes del sistema operativo, algunas aplicaciones pueden tener su propia caché de fuentes. La eliminación de estos archivos de caché de fuentes puede resolver el problema con el texto ilegible.

En primer lugar, deberá iniciar la Libreta de fuentes, seleccionar la fuente o la familia con la que tenga problemas y pulsar el botón Eliminar del teclado. También puede hacer clic con el botón derecho y seleccionar [!UICONTROL Quitar familia]. Si no está seguro de qué fuente o familia está causando los problemas, es posible que desee intentar eliminar primero los duplicados, tal como se describe más arriba.

El segundo paso sería borrar la caché de fuentes y hay varias maneras de lograrlo.

El primero es simplemente reiniciarlo en el modo a prueba de errores manteniendo pulsada la tecla Mayús inmediatamente cuando se oye el inicio. Cuando se carga este modo, debería aparecer una barra de progreso, durante la cual el sistema ejecutará varias comprobaciones y rutinas de mantenimiento, una de las cuales es borrar la caché de fuentes.

El segundo método es usar el terminal, que se puede hacer ejecutando el siguiente comando desde una cuenta administrativa: *sudo atsutil database -remove*

>[!NOTE]
>
>Este comando requiere que introduzca su contraseña, que no se mostrará cuando se escriba. Recomendamos consultar con su departamento de TI, ya que esto puede requerir permisos de administrador en su equipo.

Otro método sería usar una utilidad de caché de fuentes como, por ejemplo, FontNuke y borrar la caché con su ayuda.

Muchos estudios de preimpresión y diseño/diseño también utilizan el software Universal Type Server para administrar las licencias y la distribución de fuentes. A veces, se puede producir un problema con la caché de fuentes del servidor de tipo universal, que puede causar la [!DNL Workfront Proof] anotaciones para desaparecer.

Para solucionarlo, borre la caché de fuentes del servidor de tipo universal y reinicie el servidor de tipo universal.

## Corrección [!DNL Flash] conflicto de fuentes

Es posible que no tenga acceso a esta funcionalidad porque es compatible con [!DNL Flash], que ha quedado obsoleto en la mayoría de los entornos.

El visor de pruebas heredado se basa en [!DNL Flash Player] y a veces, cuando falta el texto en el visor de pruebas, es posible que haya un conflicto de fuentes entre OS X y [!DNL Flash Player]. Pruebe lo siguiente:

1. Abra el Buscador y abra el **[!UICONTROL Ir]** pestaña .
1. Pulse la tecla Opción ( ⌥ Alt) para abrir el [!UICONTROL Biblioteca] en la lista desplegable.
1. Mientras mantiene pulsada la tecla Opción, haga clic en el botón [!UICONTROL Biblioteca] carpeta.
1. Después de la [!UICONTROL Biblioteca] se abre la carpeta, vaya a [!UICONTROL Fuentes] carpeta ubicada dentro de.
1. Mueva todas las fuentes ubicadas en la [!UICONTROL Fuentes] carpeta en otra carpeta, tal vez en el escritorio (no cree otra carpeta dentro de la carpeta Fuentes).
1. Esta acción oculta todas las fuentes personalizadas; las fuentes estándar del sistema se deben guardar en su ubicación separada.
1. Salir y reiniciar [!DNL Safari].
1. Vuelva a abrir la prueba.

Ahora debería ver sus fuentes. Si no necesita ninguna de las fuentes que ha eliminado del directorio de inicio, puede eliminarlas con seguridad. De lo contrario, revise los lotes, cópielos de nuevo en la carpeta Biblioteca/Fuentes y vea cuál de ellos está causando el problema.
