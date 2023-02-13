---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Administración de versiones de prueba en [!DNL Workfront Proof]
description: Administrar comentarios en varias versiones o revisiones de un trabajo puede ser un gran desafío. [!DNL Workfront Proof] simplifica este proceso al permitirle crear y comparar varias versiones de una prueba.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d1bee64d-c091-40d3-a9c1-847c7f645b96
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 0%

---

# Administración de versiones de prueba en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Administrar comentarios en varias versiones o revisiones de un trabajo puede ser un gran desafío. [!DNL Workfront Proof] simplifica este proceso al permitirle crear y comparar varias versiones de una prueba.

No hay límite en el número de versiones de una prueba que puede crear. Por lo tanto, si necesita revisar muchas versiones con un cliente para obtener una aprobación final, todas las versiones creadas se pueden ver y administrar fácilmente en [!DNL Workfront Proof].

Los permisos son específicos de una versión, por lo que puede conceder a una persona permiso para ver una versión pero no otra. Por el contrario, si comparte una versión posterior con una persona, no podrán ver versiones anteriores a menos que vuelva atrás y las añada explícitamente también a esas versiones anteriores.

Para crear una nueva versión de una prueba, debe tener derechos de edición en la prueba.

Consulte [Administrar funciones de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) para obtener más información sobre quién tiene derechos de edición en una prueba. Consulte para obtener más información sobre la creación de versiones.

## Visualización de versiones de prueba en el visor de pruebas

El nombre completo de la versión que está viendo se muestra en la parte superior izquierda del visor de pruebas. Cualquier otra versión de la prueba se mostrará como números de versión solamente.

1. Abra una prueba en el visor de pruebas, tal como se describe en [Apertura de una prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/open-proof.md).
1. En el visor de pruebas, haga clic en el número de versión a la derecha del nombre de la prueba.
1. Para ver la otra versión, haga clic en su nombre en el menú que aparece al hacer clic en el número de versión.
1. Para comparar dos versiones, haga clic en el botón **[!UICONTROL Comparar pruebas]** icono.\
   ![Compare_Proofs_button.png](assets/compare-proofs-button.png)\
   Si hay varias versiones de la prueba, puede seleccionar qué dos versiones desea comparar haciendo clic en el número de versión correspondiente en cada lado de la pantalla de división del modo de comparación.

Para obtener información sobre la revisión de pruebas en un visor de pruebas, consulte [Revisar una prueba](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).

## Acceso a las versiones de prueba a través de la página Detalles de prueba

Puede acceder a todas las versiones de una prueba a través de la página Detalles de la prueba .

1. Abra la página Detalles de la prueba para ver una prueba, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Haga clic en la pestaña de las pestañas de la versión en la parte superior de la página y haga clic en **[!UICONTROL Vaya a la prueba]** para abrir la versión que desee en el visor de pruebas.\
   ![Version_tabs_on_Proof_Details_page.png](assets/version-tabs-on-proof-details-page-350x205.png)

## Vinculación de versiones de prueba

Si la prueba tiene varias versiones, la versión anterior de la prueba se conoce comúnmente como prueba principal.

Si desea cambiar la prueba principal (versión anterior) a otra prueba de la cuenta o conectar una sola prueba a otra prueba de la cuenta (como una nueva versión de la otra prueba), puede hacerlo fácilmente siguiendo estos pasos:

1. Abra la página Detalles de la prueba para ver una prueba, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Haga clic en **[!UICONTROL Más]** > **[!UICONTROL Cambiar versión anterior]**.

1. En el **[!UICONTROL Cambiar versión anterior]** que aparece, seleccione la prueba que desea establecer como prueba principal (versión anterior).\
   Si necesita ayuda para encontrar la prueba en la lista, puede ordenar las columnas haciendo clic en el encabezado de la columna.

1. Haga clic en **[!UICONTROL Cambiar versión anterior]** en la parte inferior del cuadro para conectar versiones.

>[!NOTE]
>
>Cuando conecta una prueba a otra prueba de su cuenta (como una versión nueva), [!DNL Workfront Proof] bloquea la prueba que ahora es la versión anterior.

## Desvinculación de versiones de prueba

Puede desvincular la prueba que está viendo de su prueba principal (versión anterior) sin vincularla a otra prueba de su cuenta:

1. Abra la página Detalles de la prueba para ver una prueba, tal como se describe en [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Haga clic en **[!UICONTROL Más]** > **[!UICONTROL Eliminar vínculo a la versión anterior]**.

   * Solo se puede desvincular (desconectar) la última versión del conjunto completo de versiones. Luego se convertirá en una única prueba.
   * Si necesita insertar una versión en entre dos versiones existentes, puede desvincular todas las versiones de la misma prueba y volver a vincularlas en el orden correcto.

## Acerca de los conjuntos de versiones y los límites de prueba

Cada conjunto de cinco versiones contará como una prueba con respecto al límite total de pruebas.

Por ejemplo, si carga cinco versiones de un diseño (incluida la versión original), eso cuenta como una prueba. Si carga seis versiones de un diseño, eso cuenta como dos pruebas. Once versiones contarían como tres pruebas y así sucesivamente.

Para los archivos visuales de audio, cada nueva versión cuenta como una nueva prueba.
