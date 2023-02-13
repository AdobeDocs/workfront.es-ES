---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 'Problemas Con La Visualización De Pruebas: Explicación De Objetos Compartidos De Flash'
description: 'Nota: La información de este artículo hace referencia a funcionalidades que actualmente están en desuso y que se eliminarán de [!DNL Workfront] en 2018. Se recomienda utilizar el nuevo visor de prueba web (tal como se describe en Revisión de pruebas en el visor de prueba web) o el visor de prueba de escritorio (tal como se describe en Revisión de pruebas en el visualizador de prueba de escritorio).'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f1f3561e-8660-4c1e-b48f-446eb0eaac06
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Problemas Con La Visualización De Pruebas: [!DNL Flash] Objetos compartidos explicados

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

>[!NOTE]
>
>La información de este artículo hace referencia a funcionalidades que actualmente están en desuso y que se eliminarán de [!DNL Workfront] en 2018. Le recomendamos que utilice el nuevo visor de prueba web (tal como se describe en [Revisión de pruebas en el visor de pruebas web](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer)) o el Visor de prueba de escritorio (tal como se describe en [Revisión de pruebas en el visualizador de pruebas de escritorio](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer)).

## [!DNL Flash] Objetos compartidos

Un objeto compartido local, a veces llamado &quot;[!DNL Flash] ,&quot; es un archivo de datos que los sitios que visita pueden crear en su equipo. Los objetos compartidos se utilizan habitualmente para mejorar su experiencia de navegación web. A [!DNL Flash] es un mensaje que se usa en [!DNL Adobe Flash] que se envía desde un servidor web a un explorador web y, a continuación, se almacena como archivo de datos en el explorador.

Dado que la variable [!DNL Workfront Proof] El visor se basa en [!DNL Flash], vale la pena comprobar para qué almacenamiento está permitido [!DNL Flash] aplicaciones en el equipo.

## [!DNL Flash] Objetos compartidos: problemas conocidos

Si la variable [!DNL Flash] el almacenamiento está establecido en 0 KB o tiene otra configuración que bloquea [!DNL Flash] que no guarden los datos localmente, puede causar algunos problemas conocidos en la variable [!DNL Workfront Proof] Visor:

* La ventana emergente del tour &quot;Primeros pasos&quot; sigue apareciendo, aunque se eligió la opción de no volver a mostrarlo
* [!DNL Workfront Proof] El rendimiento del visor se ralentiza debido al creciente número de comentarios agregados a las pruebas
* Las pruebas no se cargan y se obtiene la &quot;pantalla gris&quot; en lugar de una imagen real

## Permitir [!DNL Flash] Objetos compartidos

Asegúrese de que el [!DNL Flash] Los objetos compartidos están permitidos en el equipo y el límite de almacenamiento no es 0.

Para comprobar si los objetos compartidos están permitidos:

1. Haga clic con el botón derecho en la variable [!DNL Workfront Proof] Visor.
1. Select **[!UICONTROL Configuración global]** en el menú contextual.
1. Vaya a la **[!UICONTROL Almacenamiento]** pestaña .
1. Asegúrese de que **[!UICONTROL Permitir que los sitios guarden información en este equipo]** está seleccionado (1).
1. ![2017-06-09_1929.png](assets/2017-06-09-1929-350x267.png)

## Aumento [!DNL Flash] almacenamiento

De forma predeterminada [!DNL Flash] las aplicaciones pueden almacenar hasta 100 KB de datos en la unidad del usuario, pero los usuarios pueden modificarlos fácilmente. La solución para muchos [!DNL Flash] problemas relacionados es aumentar el [!DNL Flash] almacenamiento. Esto se puede hacer directamente desde el [!DNL Workfront Proof] Visor:

1. Abra una prueba.
1. Abra el menú contextual de la prueba.
1. Haga clic en **[!UICONTROL Configuración]** para abrir el [!DNL Flash] configuración emergente.
1. Vaya a la **[!UICONTROL Local]** pestaña de almacenamiento.
1. Aumente el almacenamiento hasta, por ejemplo, 100 KB (1).
1. Cierre la ventana emergente de configuración y vuelva a abrir la prueba .

![2017-06-09_1926.png](assets/2017-06-09-1926-350x274.png)
