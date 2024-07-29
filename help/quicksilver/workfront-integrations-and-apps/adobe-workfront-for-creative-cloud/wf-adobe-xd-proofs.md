---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: XD Cargar tableros de trabajo de como pruebas en Workfront
description: Puede cargar las mesas de trabajo como pruebas directamente en Adobe Workfront para una revisión y aprobación exhaustivas.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: 4256e1ecd16179d0a2aa8e623b05be754d8bbd2d
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 0%

---

# Cargar [!DNL XD] mesas de trabajo como pruebas en [!DNL Workfront]

Puede cargar las mesas de trabajo como pruebas directamente en [!DNL Adobe Workfront] para una revisión y aprobación exhaustivas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Plan actual: [!UICONTROL Pro] o superior</p> <p>o</p> <p>Plan heredado: [!UICONTROL Premium]</p> <p>Para obtener más información sobre la revisión del acceso con los diferentes planes, consulte .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>Plan actual: [!UICONTROL Work] o [!UICONTROL Proof]</p> <p>Plan heredado: Cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Debe tener una licencia [!DNL Adobe Creative Cloud] además de una licencia [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>[!UICONTROL Manager] o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Editar acceso a documentos de [!UICONTROL]</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, rol o perfil de permiso de revisión tiene, comuníquese con el administrador de [!DNL Workfront] o [!DNL Workfront Proof].

+++

## Requisitos previos

* Debe instalar el complemento [!DNL Adobe Workfront for XD] para poder cargar las pruebas en [!DNL Adobe XD].

  Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Cargar una prueba estática

1. Haga clic en el icono **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/menu-350x440.png)

1. Vaya al elemento de trabajo donde desea cargar una prueba estática.
1. Haga clic en el icono **[!UICONTROL Documento]** ![](assets/documents.png) en la barra de navegación.

1. Haga clic en **[!UICONTROL Nuevo archivo]** cerca de la parte inferior del complemento.
1. Seleccione las mesas de trabajo que desee cargar.

   >[!TIP]
   >
   >* Las mesas de trabajo aparecerán en la prueba en el orden en que se seleccionaron. La primera mesa de trabajo seleccionada será la primera página de la prueba, etc.
   >* Para seleccionar rápidamente más de una mesa de trabajo, haga clic y arrastre el ratón sobre las mesas de trabajo que desee. Esto no permite controlar el orden de las mesas de trabajo en la prueba.

1. Habilitar **[!UICONTROL Crear una revisión]**.

1. Asigne un nombre a la prueba.

1. Elija el tipo de aprobación de prueba que desee:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Básico]: </td> 
      <td> <p>Los procesos de aprobación básicos son ad hoc y pueden incluir diferentes revisores según sea necesario: </p> 
       <ul> 
        <li> <p>(Opcional) Agregue <strong>Aprobadores</strong> en el cuadro.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automatizado]</td> 
      <td> <p>Los administradores generan previamente los procesos de aprobación automatizados, que incluyen revisores y etapas específicos. Para obtener más información, consulte <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Resumen del flujo de trabajo automatizado</a>.</p> 
       <ul> 
        <li> <p>Elija una [!UICONTROL Plantilla de flujo de trabajo] en el menú desplegable.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Opcional) Escriba un comentario en el área **[!UICONTROL Actualizaciones]**.

   ![](assets/proof-approvals-xd-350x396.png)

1. Elija el formato de exportación en el menú desplegable **[!UICONTROL Tipo de recurso]**.


1. (Opcional) Si selecciona PDF como tipo de recurso y tiene más de una mesa de trabajo seleccionada, elija si desea exportar las mesas de trabajo como **[!UICONTROL archivo de un solo PDF]s** o **M[!UICONTROL varios archivos de PDF]**.

1. (Opcional) Asigne un nombre al PDF.

   ![](assets/pdf-options.png)

1. Haga clic en **[!UICONTROL Cargar]**.\
   El documento aparece en el área [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.

## Cargar una prueba interactiva {#upload-an-interactive-proof}

Puede crear una prueba interactiva para las mesas de trabajo con el complemento [!DNL Workfront for Adobe]. Es un proceso de 2 pasos. Primero debe crear un vínculo interactivo y luego cargar la prueba en un elemento de trabajo.

### Creación de un vínculo interactivo para la mesa de trabajo  {#create-an-interactive-link-for-your-art-board}

1. Abra la mesa de trabajo y haga clic en **[!UICONTROL Compartir]** en el área superior izquierda de la pantalla.
1. Especifique la configuración del vínculo:

   1. Asigne un nombre al vínculo.
   1. Elija una configuración de vista.
   1. En la sección **[!UICONTROL Acceso a vínculos]**, asegúrese de que está seleccionado **[!UICONTROL Cualquier persona que tenga este vínculo]**.

      Debe habilitar este tipo de acceso para generar una prueba interactiva.

   1. Haga clic en **[!UICONTROL Crear vínculo]**.

1. Vuelva a hacer clic en **[!UICONTROL Diseño]** en el área superior izquierda de la pantalla. Continúe a la sección [Cargar una prueba interactiva](#upload-an-interactive-proof) a continuación.

   >[!NOTE]
   >
   >Es posible que tenga que volver a abrir el panel del complemento en la esquina inferior izquierda de la pantalla.

### Cargar una prueba interactiva

1. Haga clic en el icono **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/menu-350x440.png)

1. Vaya al elemento de trabajo en el que desea cargar una prueba interactiva.
1. Haga clic en el icono **[!UICONTROL Documento]** ![](assets/documents.png) en la barra de navegación.

1. Haga clic en **[!UICONTROL Nuevo archivo]** cerca de la parte inferior del complemento.
1. Habilitar **[!UICONTROL Crear una revisión]**.

1. Elija el tipo de aprobación de prueba que desee:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Básico]: </td> 
      <td> <p>Los procesos de aprobación básicos son ad hoc y pueden incluir diferentes revisores según sea necesario: </p> 
       <ul> 
        <li> <p>(Opcional) Agregue <strong>Aprobadores</strong> en el cuadro.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automatizado]</td> 
      <td> <p>Los administradores generan previamente los procesos de aprobación automatizados, que incluyen revisores y etapas específicos. Para obtener más información, consulte <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Resumen del flujo de trabajo automatizado</a>.</p> 
       <ul> 
        <li> <p>Elija una [!UICONTROL Plantilla de flujo de trabajo] en el menú desplegable.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Opcional) Escriba un comentario en el área **[!UICONTROL Actualizaciones]**.

   ![](assets/proof-approvals-xd-350x396.png)

1. En el menú desplegable **[!UICONTROL Tipo de recurso]**, elija el vínculo que acaba de crear en la ficha **Vínculos compartidos**. Para obtener más información, consulte [Crear un vínculo interactivo para la mesa de trabajo](#create-an-interactive-link-for-your-artboard).\
   ![](assets/shared-links-xd-350x870.png)

1. Haga clic en **[!UICONTROL Cargar]**.

   El documento aparece en el área [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.

   >[!IMPORTANT]
   >
   >Los usuarios deben tener acceso al [!UICONTROL Visor de corrección de escritorio] para revisar y aprobar las pruebas interactivas. Para obtener más información, consulte [Instalar el [!UICONTROL Visor de corrección de escritorio]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## Cargar una nueva versión de revisión

Puede cargar una nueva versión de una prueba. El complemento recuerda el flujo de trabajo de revisión establecido en la versión anterior, pero puede cambiarlo si lo desea.

1. Haga clic en el icono **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/menu-350x440.png)

1. Vaya al elemento de trabajo en el que debe cargar un documento.
1. Haga clic en el icono **[!UICONTROL Documento]** ![](assets/documents.png)de la barra de navegación.

1. Haga clic en **[!UICONTROL Nueva versión]** cerca de la parte inferior del complemento.
1. Habilitar **[!UICONTROL Crear una revisión]**.
1. Seleccione las mesas de trabajo que desee cargar.

   >[!NOTE]
   >
   >Si desea cargar una nueva versión de un archivo .svg, .png o .jpg, solo puede cargar una mesa de trabajo.

1. Elija el tipo de aprobación de prueba que desee:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Básico]: </td> 
      <td> <p>Los procesos de aprobación básicos son ad hoc y pueden incluir diferentes revisores según sea necesario: </p> 
       <ul> 
        <li> <p>(Opcional) Agregue <strong>Aprobadores</strong> en el cuadro.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automatizado]</td> 
      <td> <p>Los administradores generan previamente los procesos de aprobación automatizados, que incluyen revisores y etapas específicos. Para obtener más información, consulte <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Resumen del flujo de trabajo automatizado</a>.</p> 
       <ul> 
        <li> <p>Elija una [!UICONTROL Plantilla de flujo de trabajo] en el menú desplegable.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. Elija el formato de exportación en el menú desplegable **[!UICONTROL Tipo de recurso]**.

   ![](assets/create-a-proof-xd-350x202.png)

1. (Opcional) Escriba un comentario en el área **[!UICONTROL Actualizaciones]**.

   ![](assets/proof-approvals-xd-350x396.png)

1. (Opcional) Si selecciona PDF como tipo de recurso y tiene más de una mesa de trabajo seleccionada, elija si desea exportar las mesas de trabajo como **[!UICONTROL archivo de un solo PDF]s** o **M[!UICONTROL varios archivos de PDF]**.

1. (Opcional) Asigne un nombre al PDF.

   ![](assets/pdf-options.png)

1. Haga clic en **[!UICONTROL Cargar]**.\
   El documento aparece en el área [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.
