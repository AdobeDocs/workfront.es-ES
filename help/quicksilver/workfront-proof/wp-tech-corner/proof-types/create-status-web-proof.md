---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Creación de una prueba de sitio web estática mediante [!DNL Workfront Proof]
description: Puede crear pruebas estáticas desde las páginas web. Además, puede simular varios dispositivos definiendo la resolución de pantalla de las capturas.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Creación de una prueba de sitio web estática mediante [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Puede crear pruebas estáticas desde las páginas web. Además, puede simular varios dispositivos definiendo la resolución de pantalla de las capturas.

## Creación de una prueba de sitio web estática

1. Abra el [!UICONTROL Nueva prueba] como se describe en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. Pegue o escriba la dirección URL en la **www.shareyourlink.com** en la ventana
1. Puede repetir este paso para agregar varias direcciones URL.
1. Justo debajo de este cuadro, haga clic en la resolución (el valor predeterminado es 1366 x 768) y, a continuación, seleccione las resoluciones que desee en la **[!UICONTROL Resolución de pantalla]** en la ventana
Seleccione una resolución más pequeña si desea probar los diseños para dispositivos móviles. Por lo general, los diseños se cargan según la resolución de la ventana de pantalla/explorador.

1. Haga clic en **[!UICONTROL Buscar subpáginas]** si desea incluir páginas conectadas que están en el mismo dominio o subdominio que la dirección URL ingresada.
   [!DNL Workfront Proof] explora las páginas conectadas y las enumera debajo de la variable **[!UICONTROL Buscar subpáginas]** . Puede seleccionar las páginas que desee incluir.

1. Con la variable [!UICONTROL Combinación de pruebas] puede enviar todas las páginas web como una única prueba de varias páginas.
1. Haga clic en **[!UICONTROL Listo]** y, a continuación, termine de configurar la prueba como se explica en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Acerca de las páginas protegidas con contraseña y las páginas que requieren autorización

[!DNL Workfront Proof] no puede capturar un sitio web protegido con contraseña como una prueba estática.

Para crear pruebas a partir de páginas que requieran autorización, su equipo de TI debe agregar una de las siguientes URL a la Lista de permitidos de su empresa a través de la cual se conecta nuestra herramienta de captura web:

**Clústeres de AWS en EE. UU.**: webcapture.proofhq.com

**Clústeres GCP en EE. UU.**: webcaptura.gcp.proofhq.com

**Clústeres de EMEA**: webcapture.proofhq.eu

>[!NOTE]
>
>Recomendamos las pruebas interactivas en lugar de las estáticas para las páginas internas que requieren autorización y los sitios web protegidos con contraseña. Para obtener más información, consulte [Información general sobre pruebas de contenido interactivo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## Acerca del procesamiento de pruebas de sitio web estáticas

* Las animaciones, los vídeos incrustados, los scripts y las interacciones no se pueden incluir en las pruebas estáticas del sitio web. Si desea probar contenido interactivo, consulte [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* Las páginas de prueba se preparan generalmente a una velocidad de unos 20 segundos por página. Sin embargo, el tiempo de preparación general también depende de los servidores en los que se alojen las páginas. La herramienta espera 60 segundos a que se cargue cada URL enviada. Si se supera este tiempo de espera, la prueba falla.
* En el caso de pruebas combinadas, si alguna de las URL no responde a la herramienta de captura, la prueba falla.
* [!DNL Workfront Proof] captura páginas web de hasta 195 pulgadas de largo después de la rasterización. Si la página web es más larga que esto, la prueba falla.
* La extracción de texto está disponible en todos los elementos de texto, pero el texto colocado como imágenes no se extrae.
* Se puede hacer clic en los hipervínculos de texto en las pruebas y las páginas vinculadas se abren en las nuevas pestañas del explorador.
* No se puede hacer clic en los hipervínculos de las imágenes si los elementos style=&quot;display:block&quot; se utilizan dentro del `<a>` etiquetas. Se recomienda ajustar estas partes del diseño de página.
* Para obtener los mejores resultados, recomendamos crear las páginas utilizando las prácticas de codificación recomendadas y los estándares reconocidos.
