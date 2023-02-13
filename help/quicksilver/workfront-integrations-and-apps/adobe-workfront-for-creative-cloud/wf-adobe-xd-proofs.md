---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: Cargar XD tableros como pruebas a Workfront
description: Puede cargar las mesas de trabajo como pruebas directamente en Adobe Workfront para una revisión y aprobación exhaustivas.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: 4a7fb18674b399b138fd981907f3a9da8e0bb30e
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---

# Cargar [!DNL XD] tableros como pruebas para [!DNL Workfront]

Puede cargar las mesas de trabajo como pruebas directamente en [!DNL Adobe Workfront] para una revisión y aprobación exhaustivas.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Plan actual: [!UICONTROL Pro] o superior</p> <p>o</p> <p>Plan heredado: [!UICONTROL Premium]</p> <p>Para obtener más información sobre la prueba del acceso con los diferentes planes, consulte .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>Plan actual: [!UICONTROL Work] o [!UICONTROL Proof]</p> <p>Plan heredado: Cualquiera (debe tener las pruebas habilitadas para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Debe tener un [!DNL Adobe Creative Cloud] además de una [!DNL Workfront] licencia.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>[!UICONTROL Manager] o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Editar acceso a [!UICONTROL Documents]</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con su [!DNL Workfront] o [!DNL Workfront Proof] administrador.

## Requisitos previos

* Debe instalar el [!DNL Adobe Workfront for XD] antes de poder cargar pruebas en [!DNL Adobe XD].

   Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Cargar una prueba estática

1. Haga clic en el **[!UICONTROL Menú]** en la esquina superior derecha y, a continuación, seleccione **[!UICONTROL Lista de trabajo]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/menu-350x440.png)

1. Vaya al elemento de trabajo en el que desea cargar una prueba estática.
1. Haga clic en el **[!UICONTROL Documento]** icono ![](assets/documents.png) en la barra de navegación.

1. Haga clic en **[!UICONTROL Nuevo archivo]** cerca de la parte inferior del complemento.
1. Seleccione las mesas de trabajo que desee cargar.

   >[!TIP]
   >
   >Para seleccionar más de una mesa de trabajo, haga clic y arrastre el ratón sobre las mesas de trabajo que desee.

1. Habilitar **[!UICONTROL Crear una prueba]**.

1. Asigne un nombre a la prueba.

1. Elija el tipo de aprobación de prueba que desea:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Básico]: </td> 
      <td> <p>Los procesos de aprobación básicos son ad hoc y pueden incluir diferentes revisores según sea necesario: </p> 
       <ul> 
        <li> <p>(Opcional) Agregue <strong>Aprobadores</strong> en la casilla .</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automatizado]</td> 
      <td> <p>Los procesos de aprobación automatizada están pregenerados por los administradores e incluyen revisores y etapas específicos. Para obtener más información, consulte <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Resumen del flujo de trabajo automatizado</a>.</p> 
       <ul> 
        <li> <p>Elija una [!UICONTROL Workflow Template] en el menú desplegable.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Escriba un comentario en el **[!UICONTROL Actualizaciones]** .

   ![](assets/proof-approvals-xd-350x396.png)

1. Elija el formato de exportación en la **[!UICONTROL Tipo de recurso]** menú desplegable.


1. (Opcional) Si selecciona PDF como tipo de recurso y tiene más de una mesa de trabajo seleccionada, elija si desea exportar las mesas de trabajo como **[!UICONTROL Archivo de PDF único]s** o **M[!UICONTROL varios archivos PDF]**.

1. (Opcional) Asigne un nombre al PDF.

   ![](assets/pdf-options.png)

1. Haga clic en **[!UICONTROL Cargar]**.\
   El documento aparece en la [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.

## Cargar una prueba interactiva {#upload-an-interactive-proof}

Puede crear una prueba interactiva para las mesas de trabajo con la variable [!DNL Workfront for Adobe] plugin. Es un proceso de 2 pasos. Primero debe crear un vínculo interactivo y luego cargar la prueba en un elemento de trabajo.

### Crear un vínculo interactivo para la mesa de trabajo  {#create-an-interactive-link-for-your-art-board}

1. Abra la mesa de trabajo y haga clic en **[!UICONTROL Compartir]** en el área superior izquierda de la pantalla.
1. Especifique la configuración del vínculo:

   1. Asigne un nombre al vínculo.
   1. Elija una configuración de vista.
   1. En el **[!UICONTROL Acceso a vínculos]** , asegúrese de que **[!UICONTROL Cualquiera con este vínculo]** está seleccionado.

      Debe habilitar este tipo de acceso para generar una prueba interactiva.

   1. Haga clic en **[!UICONTROL Crear vínculo]**.

1. Haga clic en **[!UICONTROL Diseño]** en el área superior izquierda de la pantalla. Continúe con el [Cargar una prueba interactiva](#upload-an-interactive-proof) a continuación.

   >[!NOTE]
   >
   >Es posible que tenga que volver a abrir el panel del complemento en la esquina inferior izquierda de la pantalla.

### Cargar una prueba interactiva

1. Haga clic en el **[!UICONTROL Menú]** en la esquina superior derecha y, a continuación, seleccione **[!UICONTROL Lista de trabajo]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/menu-350x440.png)

1. Vaya al elemento de trabajo en el que desea cargar una prueba interactiva.
1. Haga clic en el **[!UICONTROL Documento]** icono ![](assets/documents.png) en la barra de navegación.

1. Haga clic en **[!UICONTROL Nuevo archivo]** cerca de la parte inferior del complemento.
1. Habilitar **[!UICONTROL Crear una prueba]**.

1. Elija el tipo de aprobación de prueba que desea:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Básico]: </td> 
      <td> <p>Los procesos de aprobación básicos son ad hoc y pueden incluir diferentes revisores según sea necesario: </p> 
       <ul> 
        <li> <p>(Opcional) Agregue <strong>Aprobadores</strong> en la casilla .</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automatizado]</td> 
      <td> <p>Los procesos de aprobación automatizada están pregenerados por los administradores e incluyen revisores y etapas específicos. Para obtener más información, consulte <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Resumen del flujo de trabajo automatizado</a>.</p> 
       <ul> 
        <li> <p>Elija una [!UICONTROL Workflow Template] en el menú desplegable.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Escriba un comentario en el **[!UICONTROL Actualizaciones]** .

   ![](assets/proof-approvals-xd-350x396.png)

1. En el **[!UICONTROL Tipo de recurso]** menú desplegable, elija el vínculo que acaba de crear en la **Vínculos compartidos** pestaña . Para obtener más información, consulte [Crear un vínculo interactivo para la mesa de trabajo](#create-an-interactive-link-for-your-artboard).\
   ![](assets/shared-links-xd-350x870.png)

1. Haga clic en **[!UICONTROL Cargar]**.

   El documento aparece en la [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.

   >[!IMPORTANT]
   >
   >Los usuarios deben tener acceso al [!UICONTROL Visor de prueba de escritorio] para revisar y aprobar pruebas interactivas. Para obtener más información, consulte [Instale el [!UICONTROL Visor de prueba de escritorio]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## Cargar una nueva versión de prueba

Puede cargar una nueva versión de una prueba. El complemento recuerda el flujo de trabajo de pruebas establecido en la versión anterior, pero puede cambiarlo si lo desea.

1. Haga clic en el **[!UICONTROL Menú]** en la esquina superior derecha y, a continuación, seleccione **[!UICONTROL Lista de trabajo]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/menu-350x440.png)

1. Vaya al elemento de trabajo al que debe cargar un documento.
1. Haga clic en el **[!UICONTROL Documento]** icono ![](assets/documents.png)en la barra de navegación.

1. Haga clic en **[!UICONTROL Nueva versión]** cerca de la parte inferior del complemento.
1. Habilitar **[!UICONTROL Crear una prueba]**.
1. Seleccione las mesas de trabajo que desee cargar.

   >[!NOTE]
   >
   >Si desea cargar una nueva versión de un .svg, .png o .jpg, solo puede cargar una mesa de trabajo.

1. Elija el tipo de aprobación de prueba que desea:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Básico]: </td> 
      <td> <p>Los procesos de aprobación básicos son ad hoc y pueden incluir diferentes revisores según sea necesario: </p> 
       <ul> 
        <li> <p>(Opcional) Agregue <strong>Aprobadores</strong> en la casilla .</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automatizado]</td> 
      <td> <p>Los procesos de aprobación automatizada están pregenerados por los administradores e incluyen revisores y etapas específicos. Para obtener más información, consulte <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Resumen del flujo de trabajo automatizado</a>.</p> 
       <ul> 
        <li> <p>Elija una [!UICONTROL Workflow Template] en el menú desplegable.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Elija el formato de exportación en la **[!UICONTROL Tipo de recurso]** menú desplegable.

   ![](assets/create-a-proof-xd-350x202.png)

1. (Opcional) Escriba un comentario en el **[!UICONTROL Actualizaciones]** .

   ![](assets/proof-approvals-xd-350x396.png)

1. (Opcional) Si selecciona PDF como tipo de recurso y tiene más de una mesa de trabajo seleccionada, elija si desea exportar las mesas de trabajo como **[!UICONTROL Archivo de PDF único]s** o **M[!UICONTROL varios archivos PDF]**.

1. (Opcional) Asigne un nombre al PDF.

   ![](assets/pdf-options.png)

1. Haga clic en **[!UICONTROL Cargar]**.\
   El documento aparece en la [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.
