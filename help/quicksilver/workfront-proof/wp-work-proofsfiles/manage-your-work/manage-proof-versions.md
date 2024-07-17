---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Administrar versiones de revisión en  [!DNL Workfront Proof]
description: Gestionar los comentarios en varias versiones o revisiones de una parte del trabajo puede ser un gran desafío. [!DNL Workfront Proof] simplifica este proceso al permitirle crear y comparar varias versiones de una revisión.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d1bee64d-c091-40d3-a9c1-847c7f645b96
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---

# Administrar versiones de revisión en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Gestionar los comentarios en varias versiones o revisiones de una parte del trabajo puede ser un gran desafío. [!DNL Workfront Proof] simplifica este proceso al permitirle crear y comparar varias versiones de una revisión.

No hay límite en el número de versiones de una prueba que puede crear. Por lo tanto, si necesita pasar por muchas revisiones con un cliente para obtener una aprobación final, todas las versiones creadas se pueden ver y administrar fácilmente dentro de [!DNL Workfront Proof].

Los permisos son específicos de una versión, por lo que puede conceder a una persona permiso para ver una versión, pero no otra. Por el contrario, si comparte una versión posterior con una persona, no podrá ver las versiones anteriores a menos que vuelva atrás y las agregue explícitamente también a esas versiones anteriores.

Para crear una nueva versión de una prueba, debe tener derechos de edición sobre la prueba.

Consulte [Administrar roles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) para obtener más información sobre quién tiene derechos de edición en una prueba. Consulte para obtener más información sobre la creación de versiones.

## Visualización de versiones de prueba en el visor de pruebas

El nombre completo de la versión que está viendo se muestra en la parte superior izquierda del visor de pruebas. Las demás versiones de la revisión solo se mostrarán como números de versión.

1. Abra una revisión en el visor de revisiones, tal como se describe en [Abrir una revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/open-proof.md).
1. En el visor de revisión, haga clic en el número de versión que aparece a la derecha del nombre de la revisión.
1. Para ver la otra versión, haga clic en su nombre en el menú que aparece al hacer clic en el número de versión.
1. Para comparar dos versiones, haga clic en el icono **[!UICONTROL Comparar pruebas]**.\
   ![Botón_Comparar_Pruebas.png](assets/compare-proofs-button.png)\
   Si hay varias versiones de la prueba, puede seleccionar qué dos versiones desea comparar haciendo clic en el número de versión correspondiente a cada lado de la pantalla de división del modo de comparación.

Para obtener información acerca de cómo revisar pruebas en un visor de pruebas, vea [Revisar una prueba](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).

## Acceso a las versiones de prueba mediante la página de detalles de prueba

Puede acceder a todas las versiones de una prueba a través de la página de detalles de la prueba.

1. Abra la página de detalles de una revisión para una revisión, como se describe en [Administrar detalles de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Haga clic en la pestaña de las pestañas de versión en la parte superior de la página y haga clic en **[!UICONTROL Ir a la revisión]** para abrir la versión que desee en el visor de revisión.\
   ![Version_tabs_on_Proof_Details_page.png](assets/version-tabs-on-proof-details-page-350x205.png)

## Vinculación de versiones de revisión

Si la prueba tiene varias versiones, la versión anterior de la prueba se conoce comúnmente como la prueba principal.

Si desea cambiar la prueba principal (versión anterior) a otra prueba de su cuenta o conectar una sola prueba a otra prueba de su cuenta (como una nueva versión de la otra prueba), puede hacerlo fácilmente siguiendo estos pasos:

1. Abra la página de detalles de una revisión para una revisión, como se describe en [Administrar detalles de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Haga clic en **[!UICONTROL Más]** > **[!UICONTROL Cambiar la versión anterior]**.

1. En el cuadro **[!UICONTROL Cambiar versión anterior]** que aparece, seleccione la revisión que desee establecer como revisión principal (versión anterior).\
   Si necesita ayuda para encontrar la prueba en la lista, puede ordenar las columnas haciendo clic en el encabezado de la columna.

1. Haga clic en **[!UICONTROL Cambiar versión anterior]** en la parte inferior del cuadro para conectar versiones.

>[!NOTE]
>
>Cuando conecta una revisión a otra revisión de su cuenta (como una nueva versión), [!DNL Workfront Proof] bloquea la revisión que ahora es la versión anterior.

## Desvincular versiones de revisión

Puede desvincular la revisión que está viendo actualmente de su revisión principal (versión anterior) sin vincularla a otra revisión de su cuenta:

1. Abra la página de detalles de una revisión para una revisión, como se describe en [Administrar detalles de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Haga clic en **[!UICONTROL Más]** > **[!UICONTROL Quitar vínculo a la versión anterior]**.

   * Solo la última versión se puede desvincular (desconectar) de todo el conjunto de versiones. A continuación, se convierte en una sola prueba.
   * Si necesita insertar una versión entre dos versiones existentes, puede desvincular todas las versiones de la misma prueba y volver a vincularlas en el orden correcto.

## Acerca de los conjuntos de versiones y límites de prueba

Cada conjunto de cinco versiones contará como una prueba contra su límite total de pruebas.

Por ejemplo, si carga cinco versiones de un diseño (incluida la versión original), eso cuenta como una prueba. Si sube seis versiones de un diseño, eso cuenta como dos pruebas. Once versiones contarían como tres pruebas, etc.

En el caso de los archivos audiovisuales, cada nueva versión se cuenta como una nueva prueba.
