---
product-area: documents
navigation-topic: approvals
title: Configuración de marcas para el revisor de IA
description: Configuración de marcas para el revisor de IA
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: cd2a5560fdf446e8e971afcb640af38b4d301d40
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 10%

---

# Configuración de marcas para el revisor de IA

>[!IMPORTANT]
>
>Esta función se encuentra actualmente en fase beta.

El revisor de IA utiliza directrices de marca para evaluar el contenido durante el proceso de revisión. Puede crear marcas en Workfront cargando archivos de PDF que contengan las directrices de marca o introduciendo manualmente elementos de marca.

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
   <td role="rowheader">Permisos de Admin Console</td> 
   <td> <p>Debe utilizar GenStudio Brand Manager.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Requisitos previos

* Su organización debe haber migrado a Adobe IMS (sistema Identity Management).
* La instancia de Workfront debe tener habilitadas las aprobaciones unificadas.
* Su organización debe tener GenStudio Foundation.
* Adobe debe tener registrado un acuerdo de Adobe Gen AI.
Para obtener más información sobre la firma del acuerdo, consulte [Firmar el acuerdo de Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).

## Crear una marca con un PDF

{{step-1-to-setup}}

1. En el panel izquierdo, vaya a **Revisar y aprobar** > **Marcas**.
1. Haz clic en **Agregar marca** en la esquina superior derecha de la pantalla.
1. Nombre la marca.
1. Haga clic en Cargar PDF para cargar archivos de marca.
   ![cargar pdf de marca](assets/upload-PDF.png)
1. Haga clic en **Continuar**.
1. Suba uno o más archivos PDF que contengan las directrices de marca y luego haga clic en **Agregar marca**.
1. Una vez cargados los archivos, revise los elementos de marca extraídos para asegurarse de que se alinean con las directrices de marca.

   >[!IMPORTANT]
   >
   >Las directrices se generan mediante los archivos y la tecnología de IA generativa y pueden ser inexactas. Revise las directrices extraídas para ver los detalles que faltan o son incorrectos y edítelas antes de publicar esta marca.

1. Cuando termine, haga clic en **Publicar** para que la marca esté disponible para el Revisor de IA.

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
        <td>logos</td>
        <td>Incluya los logotipos oficiales asociados a la marca.</td>
    </tr>
    <tr>
        <td>Colores</td>
        <td>Especifique la paleta de colores de la marca.</td>
    </tr>
    </table>

   ![agregar elementos de marca manualmente](assets/brand-elements.png)


1. Cuando termine, haga clic en **Publicar** para que la marca esté disponible para el Revisor de IA.
