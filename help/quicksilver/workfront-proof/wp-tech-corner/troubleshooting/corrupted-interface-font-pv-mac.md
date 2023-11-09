---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 'Solución de problemas: fuente de interfaz dañada en el visor de pruebas en Mac'
description: Solución de problemas de fuente de interfaz dañada en el visor de pruebas en Mac
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Solución de problemas: fuente de interfaz dañada en el visor de pruebas en Mac

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Si observa que el visor de revisión no muestra correctamente la fuente de la interfaz, podría deberse a algunos problemas con las fuentes del equipo con Mac. Para resolver el problema, pruebe las siguientes soluciones:

## Eliminar duplicados de fuentes

Compruebe si hay fuentes duplicadas en el sistema.

1. Cierre el explorador que está utilizando.
1. Abra la aplicación Libro de fuentes en la carpeta Aplicaciones.
1. Clic **[!UICONTROL Todas las fuentes]** (1).
1. Clic **[!UICONTROL Editar]** > **[!UICONTROL Buscar duplicados habilitados]**.

1. Clic **[!UICONTROL Sí]** para resolver duplicados.
1. Si ve una advertencia sobre las fuentes dañadas, haga clic en **[!UICONTROL Sí]**.
1. Reinicie el equipo.
1. Vuelva a intentar la prueba.

## Borrar la caché de fuentes

A veces, las cachés de fuentes en Mac OS X se dañan. Por ejemplo, cuando se vuelve a instalar una fuente o una familia de fuentes varias veces o si se ha actualizado o reinstalado una aplicación. Aparte de los archivos de caché de fuentes del sistema operativo, algunas aplicaciones pueden tener su propia caché de fuentes. Eliminar estos archivos de caché de fuentes puede resolver el problema con texto ilegible.

En primer lugar, tendrá que iniciar Libro de fuentes, seleccionar la fuente o la familia con la que está teniendo problemas y pulsar el botón Eliminar en el teclado. También puede hacer clic con el botón derecho y seleccionar [!UICONTROL Quitar familia]. Si no está seguro de qué fuente o familia está causando los problemas, es posible que desee intentar eliminar primero los duplicados como se ha descrito anteriormente.

El segundo paso sería borrar la caché de fuentes y hay varias formas de lograrlo.

La primera es simplemente reiniciar en Modo Seguro manteniendo pulsada la tecla Mayús inmediatamente cuando oiga el timbre de arranque durante el arranque. Cuando se carga este modo, debería aparecer una barra de progreso, durante la cual el sistema ejecutará varias comprobaciones y rutinas de mantenimiento, una de las cuales es borrar la caché de fuentes.

El segundo enfoque es utilizar el terminal, que se puede hacer ejecutando el siguiente comando desde una cuenta administrativa: *sudo atsutil bases de datos -remove*

>[!NOTE]
>
>Este comando requiere que escriba la contraseña, que no se mostrará cuando la escriba. Recomendamos consultar con su departamento de TI, ya que esto puede requerir permisos de administrador en su equipo.

Otro método sería utilizar una utilidad de caché de fuentes como, por ejemplo, FontNuke y borrar la caché con su ayuda.

Muchos estudios de preimpresión y diseño también usan el software Universal Type Server para administrar licencias y distribución de fuentes. A veces, puede producirse un problema con la caché de fuentes del servidor de tipo universal, que puede causar lo siguiente [!DNL Workfront Proof] anotaciones que deben desaparecer.

Para solucionarlo, borre la caché de fuentes del servidor de tipo universal y reinicie el servidor de tipo universal.

## Fix [!DNL Flash] conflicto de fuentes

Es posible que no tenga acceso a esta funcionalidad porque es compatible con [!DNL Flash], que ha quedado obsoleta en la mayoría de los entornos.

El visor de revisión de elementos heredados se basa en [!DNL Flash Player] y a veces, cuando falta el texto en el visor de pruebas, es posible que haya un conflicto de fuentes entre OS X y [!DNL Flash Player]. Pruebe lo siguiente:

1. Abra el buscador y abra **[!UICONTROL Ir]** pestaña.
1. Pulse la tecla Opción (⌥ Alt) para abrir [!UICONTROL Biblioteca] en la lista desplegable.
1. Mientras mantiene pulsada la tecla Opción, haga clic en [!UICONTROL Biblioteca] carpeta.
1. Después del [!UICONTROL Biblioteca] se abre la carpeta, vaya a [!UICONTROL Fuentes] carpeta ubicada en.
1. Mueva todas las fuentes ubicadas en el [!UICONTROL Fuentes] carpeta en otra carpeta, tal vez en el escritorio (no cree otra carpeta dentro de la carpeta Fuentes).
1. Esta acción oculta todas las fuentes personalizadas; aún debe tener las fuentes del sistema estándar guardadas en su ubicación independiente.
1. Salir y reiniciar [!DNL Safari].
1. Vuelva a abrir la prueba.

Ahora debería ver las fuentes. Si no necesita ninguna de las fuentes que ha eliminado del directorio de inicio, puede eliminarlas con seguridad. De lo contrario, revíselos por lotes, cópielos de nuevo en la carpeta Biblioteca/Fuentes y vea cuál es la causa del problema.
