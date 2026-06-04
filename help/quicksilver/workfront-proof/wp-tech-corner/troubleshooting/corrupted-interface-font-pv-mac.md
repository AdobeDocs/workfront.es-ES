---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 'Solución de problemas: fuente de la interfaz corrupta en el visor de revisiones en Mac.'
description: Solucionar fuente de la interfaz corrupta en el visor de revisiones en Mac
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
TQID: https://experienceleague.adobe.com/t6MNg6tX6QJ2v3SCwu7NhiXcMaYq8CYQrvSi-ng-HWY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 660
ht-degree: 97%

---

# Solución de problemas: fuente de la interfaz corrupta en el visor de revisiones en Mac.

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Si nota que el visor de revisiones no muestra correctamente la fuente de la interfaz, esto podría deberse a algunos problemas con las fuentes en tu Mac. Para resolver el problema, pruebe las siguientes soluciones:

## Eliminar duplicados de fuentes

Compruebe si hay fuentes duplicadas en el sistema.

1. Cierre el explorador que está utilizando.
1. Abra la aplicación Libro de fuentes en la carpeta Aplicaciones.
1. Haga clic en **[!UICONTROL Todas las fuentes]** (1).
1. Haga clic en **[!UICONTROL Editar]** > **[!UICONTROL Buscar duplicados habilitados]**.

1. Haga clic en **[!UICONTROL Sí]** para resolver duplicados.
1. Si ve una advertencia sobre las fuentes dañadas, haga clic en **[!UICONTROL Sí]**.
1. Reinicie su ordenador.
1. Vuelva a intentar la prueba.

## Borrar la caché de fuentes

A veces, las cachés de fuentes en Mac OS X se dañan. Por ejemplo, cuando se vuelve a instalar una fuente o una familia de fuentes varias veces o si se ha actualizado o reinstalado una aplicación. Aparte de los archivos de caché de fuentes del sistema operativo, algunas aplicaciones pueden tener su propia caché de fuentes. Eliminar estos archivos de caché de fuentes puede resolver el problema con texto ilegible.

En primer lugar, tendrá que iniciar libro de fuentes, seleccionar la fuente o la familia con la que está teniendo problemas y pulsar el botón Eliminar en el teclado. También puede hacer clic con el botón derecho y seleccionar [!UICONTROL Quitar familia]. Si no está seguro de qué fuente o familia está causando los problemas, es posible que desee intentar eliminar primero los duplicados como se ha descrito anteriormente.

El segundo paso sería borrar la caché de fuentes y hay varias formas de lograrlo.

La primera es simplemente reiniciar en Modo Seguro manteniendo pulsada la tecla Mayús inmediatamente cuando oiga el timbre de arranque durante el arranque. Cuando se carga este modo, debería aparecer una barra de progreso, durante la cual el sistema ejecutará varias comprobaciones y rutinas de mantenimiento, una de las cuales es borrar la caché de fuentes.

El segundo método consiste en usar el Terminal, que se puede realizar ejecutando el siguiente comando desde una cuenta administrativa: *sudo atsutil database -remove*

>[!NOTE]
>
>Este comando requiere que escriba la contraseña, que no se mostrará cuando la escriba. Recomendamos que consulte con tu departamento de TI, ya que esto podría requerir permisos de Administrador en tu equipo.

Otro enfoque sería utilizar una utilidad de caché de fuentes como, por ejemplo, FontNuke y borrar la caché con su ayuda.

Muchos estudios de preimpresión y diseño también usan el software Universal Type Server para administrar licencias y distribución de fuentes. A veces, puede ocurrir un problema con la caché de fuentes de Universal Type Server, lo que puede hacer que las [!DNL Workfront Proof] anotaciones desaparezcan.

Para solucionarlo, borre la caché de fuentes del servidor de tipo universal y reinicie el servidor de tipo universal.

## Corregir conflicto de fuentes de [!DNL Flash]

Es posible que no tenga acceso a esta funcionalidad porque es compatible con [!DNL Flash], que ha quedado obsoleta en la mayoría de los entornos.

El Visualizador de revisiones heredadas está basado en [!DNL Flash Player] y, a veces, cuando falta el texto en el visor de revisiones, es posible que haya un conflicto de fuentes entre OS X y [!DNL Flash Player]. Intente lo siguiente:

1. Abra Finder y la pestaña **[!UICONTROL Ir]**.
1. Presione la tecla Opción (⌥ Alt) para abrir la carpeta [!UICONTROL Library] en la lista desplegable.
1. Mientras mantiene la tecla Opción, haga clic en la carpeta [!UICONTROL Biblioteca].
1. Después de que se abra la carpeta [!UICONTROL biblioteca] vaya a la carpeta [!UICONTROL Fuentes] que se encuentra dentro.
1. Mueva todas las fuentes ubicadas en la carpeta [!UICONTROL Fuentes] a otra carpeta, quizás en su Escritorio (no cree otra carpeta dentro de la carpeta Fuentes).
1. Esta acción oculta todas sus fuentes personalizadas; aún debería tener las fuentes estándar del sistema guardadas en su ubicación separada.
1. Salga y reinicie [!DNL Safari].
1. Vuelva a abrir la prueba.

Ahora debería ver las fuentes. Si no necesita ninguna de las fuentes que eliminó de su directorio personal, puede borrarla de forma segura. De lo contrario, revíselos por lotes, cópielos de nuevo en la carpeta Biblioteca/Fuentes y vea cuál es la causa del problema.
