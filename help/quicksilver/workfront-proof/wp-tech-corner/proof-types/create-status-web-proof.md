---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Crear una revisión de sitio web estático usando  [!DNL Workfront Proof]
description: Puede crear pruebas estáticas a partir de sus páginas web. Además, puede simular varios dispositivos definiendo la resolución de pantalla de las capturas.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Crear una revisión de sitio web estático usando [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Puede crear pruebas estáticas a partir de sus páginas web. Además, puede simular varios dispositivos definiendo la resolución de pantalla de las capturas.

## Creación de una revisión de sitio web estática

1. Abra la página [!UICONTROL Nueva revisión], tal como se describe en [Generar revisiones en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. Pegue o escriba la dirección URL en el cuadro **www.shareyourlink.com**.
1. Puede repetir este paso para agregar varias direcciones URL.
1. Justo debajo de este cuadro, haga clic en la resolución (el valor predeterminado es 1366x768) y, a continuación, seleccione las resoluciones que desee en el cuadro **[!UICONTROL Resolución de captura de pantalla]**.
Seleccione una resolución más pequeña si desea probar diseños para dispositivos móviles. Por lo general, los diseños se cargan según la resolución de pantalla/ventana del explorador.

1. Haga clic en **[!UICONTROL Buscar subpáginas]** si desea incluir páginas conectadas que se encuentran en el mismo dominio o subdominio que la dirección URL ingresada.
   [!DNL Workfront Proof] analiza las páginas conectadas y las enumera debajo de la opción **[!UICONTROL Buscar subpáginas]**. Puede seleccionar las páginas que desee incluir.

1. Con la función [!UICONTROL Combinar pruebas], puede enviar todas las páginas web como una sola revisión de varias páginas.
1. Haga clic en **[!UICONTROL Listo]** y luego termine de configurar la revisión como se explica en [Generar revisiones en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Páginas protegidas con contraseña y páginas que requieren autorización

[!DNL Workfront Proof] no puede capturar un sitio web protegido con contraseña como una revisión estática.

Para crear pruebas a partir de páginas que requieran autorización, su equipo de TI debe agregar una de las siguientes URL a la Lista de permitidos de su empresa a través de la cual se conecta nuestra herramienta de captura web:

**Clústeres de AWS en Estados Unidos**: webcapture.proofhq.com

**Clústeres GCP en EE. UU.**: webcapture.gcp.proofhq.com

**Clústeres de EMEA**: webcapture.proofhq.eu

>[!NOTE]
>
>Recomendamos la revisión interactiva en lugar de la revisión estática para las páginas internas que requieren autorización y sitios web protegidos por contraseña. Para obtener más información, consulte [Resumen de las pruebas de contenido interactivo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## Acerca del procesamiento de revisiones estáticas de sitios web

* Las animaciones, los vídeos incrustados, los scripts y las interacciones no se pueden incluir en las pruebas de sitio web estáticas. Si desea revisar el contenido interactivo, consulte [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) en [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* Las páginas de prueba se preparan generalmente y se capturan a una velocidad de unos 20 segundos por página. Sin embargo, el tiempo de preparación general depende también de los servidores en los que se alojan las páginas. La herramienta espera 60 segundos a que se cargue cada URL enviada. Si se supera este tiempo de espera, la prueba falla.
* En el caso de pruebas combinadas, si alguna de las direcciones URL no responde a la herramienta de captura, la prueba falla.
* [!DNL Workfront Proof] captura páginas web de hasta 195 pulgadas de longitud después de rasterizarlas. Si la página web es más larga, la prueba falla.
* La extracción de texto está disponible en todos los elementos de texto, pero el texto colocado como imágenes no se extrae.
* En las pruebas se puede hacer clic en los hipervínculos de texto, y las páginas vinculadas se abren en las nuevas pestañas del explorador.
* No se puede hacer clic en los hipervínculos de las imágenes si se utilizan los elementos style=&quot;display:block&quot; dentro de las etiquetas `<a>`. Se recomienda ajustar estas partes del diseño de página.
* Para obtener los mejores resultados, recomendamos crear las páginas utilizando las prácticas recomendadas de codificación y los estándares reconocidos.
