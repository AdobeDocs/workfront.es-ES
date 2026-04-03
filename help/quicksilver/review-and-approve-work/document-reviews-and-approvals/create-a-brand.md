---
product-area: documents
navigation-topic: approvals
title: Crear y administrar marcas para el Revisor de contenido
description: Crear y administrar marcas para el Revisor de contenido
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b2788f3f-43d2-46f3-8502-bb833f8a0970
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 2b3e2ac00126facab9cc45ba8fb193d8951a37ec
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 9%

---

# Crear y administrar marcas para el Revisor de contenido

{{highlighted-preview-article-level}}

El revisor de contenido utiliza directrices de marca para evaluar el contenido durante el proceso de revisión. Puede crear marcas en Workfront cargando archivos de PDF que contengan las directrices de marca o introduciendo manualmente elementos de marca.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador del sistema.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de Admin Console*</td> 
   <td> <p>Debe ser administrador de marca de GenStudio.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos

* La instancia de Workfront debe tener habilitadas las aprobaciones unificadas.

* Su organización debe tener GenStudio Foundation.
   * El Revisor de contenido de Workfront proporciona la funcionalidad disponible en GenStudio Foundation para los flujos de trabajo de revisión y aprobación de recursos. No es necesario que acceda directamente a GenStudio Foundation para completar su trabajo. El acceso a la funcionalidad de GenStudio Foundation a través del Revisor de contenido se encuentra dentro de los términos del contrato de Workfront.
* Adobe debe tener registrado un acuerdo de Adobe Gen AI.
Para obtener más información sobre la firma del acuerdo, consulte [Firmar el acuerdo de Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Requisitos previos

1. Debe conceder acceso a los permisos de marca en los niveles de acceso de Admin Console y Workfront para poder crear marcas. Para obtener instrucciones, consulte [Conceder acceso a los permisos de marca](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md).


## Crear una marca con un PDF

{{step-1-to-setup}}

1. En el panel izquierdo, vaya a **Revisar y aprobar** > **Marcas**.
1. Haz clic en **Agregar marca** en la esquina superior derecha de la pantalla.
1. Nombre la marca.
1. Haga clic en **Cargar PDF** para cargar archivos de marca.
   ![cargar pdf de marca](assets/upload-PDF.png)
1. Haga clic en **Continuar**.
1. Suba uno o más archivos PDF que contengan las directrices de marca y luego haga clic en **Agregar marca**.
1. Una vez cargados los archivos, revise los elementos de marca extraídos para asegurarse de que se alinean con las directrices de marca.

   >[!IMPORTANT]
   >
   >Las directrices se generan mediante los archivos y la tecnología de IA generativa y pueden ser inexactas. Revise las directrices extraídas para ver los detalles que faltan o son incorrectos y edítelas antes de publicar esta marca.

1. Cuando termine, haga clic en **Publicar** para que la marca esté disponible para el Revisor de contenido.

## Crear una marca manualmente

{{step-1-to-setup}}

1. En el panel izquierdo, vaya a **Revisar y aprobar** > **Marcas**.
1. Haz clic en **Agregar marca** en la esquina superior derecha de la pantalla.
1. Nombre la marca.
1. Haga clic en **Agregar manualmente** para crear una marca con elementos individuales.
1. Rellene los detalles de la marca según sea necesario. Puede añadir los siguientes elementos:

   <table>
    <tr>
        <td>Cuándo usar</td>
        <td>Informe a los especialistas en marketing cuándo utilizar esta marca.</td>
    </tr>
    <tr>
        <td>Directrices de voz</td>
        <td>Proporcionar orientación sobre el tono y el estilo de la voz de la marca.</td>
    </tr>
    <tr>
        <td>Directrices de imagen</td>
        <td>Especifique los tipos de imágenes que se alinean con la identidad de la marca.</td>
    </tr>
    <tr>
        <td>Directrices de canal</td>
        <td>Describa los canales adecuados para la comunicación de la marca.</td>
    </tr>
    <tr>
        <td>Logotipos</td>
        <td>Incluya los logotipos oficiales asociados a la marca.</td>
    </tr>
    <tr>
        <td>Colores</td>
        <td>Especifique la paleta de colores de la marca.</td>
    </tr>
    </table>

   ![agregar elementos de marca manualmente](assets/brand-elements.png)


1. Cuando termine, haga clic en **Publicar** para que la marca esté disponible para el Revisor de contenido.
