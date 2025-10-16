---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: Cargar mesas de trabajo XD como pruebas en Workfront
description: Puede cargar las mesas de trabajo como pruebas directamente en Adobe Workfront para una revisión y aprobación exhaustivas.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 93%

---

# Cargar mesas de trabajo [!DNL XD] como pruebas en [!DNL Workfront]

Puede cargar las mesas de trabajo como pruebas directamente en [!DNL Adobe Workfront] para una revisión y aprobación exhaustivas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquete</td> 
   <td>Cualquiera </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>Estándar</p> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Productos adicionales</td> 
   <td>Debe tener una licencia [!DNL Adobe Creative Cloud] además de una licencia [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de prueba </td> 
   <td>[!UICONTROL Manager] o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Editar acceso a [!UICONTROL Documents]</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Requisitos previos

* Debe instalar el complemento de [!DNL Adobe Workfront for XD] para poder cargar las pruebas en [!DNL Adobe XD].

  Para obtener instrucciones, consulte [Instalar  [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Cargar una prueba estática

1. Haga clic en el icono de **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![Icono de menú](assets/menu-350x440.png)

1. Vaya al elemento de trabajo donde desea cargar una prueba estática.
1. Haga clic en el icono **[!UICONTROL Documento]** ![Icono del documento](assets/documents.png) en la barra de navegación.

1. Haga clic en **[!UICONTROL Nuevo archivo]** cerca de la parte inferior del complemento.
1. Seleccione las mesas de trabajo que desee cargar.

   >[!TIP]
   >
   >* Las mesas de trabajo aparecerán en la prueba en el orden en que se seleccionaron. La primera mesa de trabajo seleccionada será la primera página de la prueba, etc.
   >* Para seleccionar rápidamente más de una mesa de trabajo, haga clic y arrastre el ratón sobre las mesas de trabajo que desee. Esto no le permite controlar el orden de las mesas de trabajo en la prueba.

1. Habilite **[!UICONTROL Crear una prueba]**.

1. Asigne un nombre a la prueba.

1. Elija el tipo de aprobación de prueba que desee:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>Los procesos de aprobación básicos son ad hoc y pueden incluir diferentes revisores según sea necesario: </p> 
       <ul> 
        <li> <p>(Opcional) Añada <strong>Aprobadores</strong> en el cuadro.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Los administradores generan previamente los procesos de aprobación automatizados, que incluyen revisores y fases específicos. Para más información, consulte <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Información general sobre el flujo de trabajo automatizado</a>.</p> 
       <ul> 
        <li> <p>Elija una [!UICONTROL Workflow Template] en el menú desplegable.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Opcional) Escriba un comentario en el área de **[!UICONTROL Actualizaciones]**.

   ![Aprobaciones de revisión en XD](assets/proof-approvals-xd-350x396.png)

1. Elija el formato de exportación en el menú desplegable **[!UICONTROL Tipo de recurso]**.


1. (Opcional) Si selecciona PDF como tipo de recurso y tiene más de una mesa de trabajo seleccionada, elija si desea exportar las mesas de trabajo como un **[!UICONTROL solo archivo PDF]** o **[!UICONTROL varios archivos PDF]**.

1. (Opcional) Asigne un nombre al PDF.

   ![Opciones de PDF](assets/pdf-options.png)

1. Haga clic en **[!UICONTROL Cargar]**\
   El documento aparece en el área de [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.

## Cargar una prueba interactiva {#upload-an-interactive-proof}

Puede crear una prueba interactiva para las mesas de trabajo con el complemento de [!DNL Workfront for Adobe]. Es un proceso de 2 pasos. Primero debe crear un vínculo interactivo y luego cargar la prueba en un elemento de trabajo.

### Crear un vínculo interactivo para la mesa de trabajo  {#create-an-interactive-link-for-your-art-board}

1. Abra la mesa de trabajo y haga clic en **[!UICONTROL Compartir]** en el área superior izquierda de la pantalla.
1. Especifique la configuración del vínculo:

   1. Asigne un nombre al grupo.
   1. Elija una configuración para la vista.
   1. En la sección **[!UICONTROL Acceso al vínculo]**, asegúrese de que ha seleccionado **[!UICONTROL Cualquiera con el vínculo]**.

      Debe habilitar este tipo de acceso para poder generar una prueba interactiva.

   1. Haga clic en **[!UICONTROL Crear vínculo]**.

1. Vuelva a hacer clic en **[!UICONTROL Diseño]** en el área superior izquierda de la pantalla. Vaya hasta la sección [Cargar una prueba interactiva](#upload-an-interactive-proof) que se describe a continuación.

   >[!NOTE]
   >
   >Es posible que tenga que volver a abrir el panel del complemento en la esquina inferior izquierda de la pantalla.

### Cargar una prueba interactiva

1. Haga clic en el icono de **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![Icono de menú](assets/menu-350x440.png)

1. Vaya al elemento de trabajo en el que desea cargar una prueba interactiva.
1. Haga clic en el icono **[!UICONTROL Documento]** ![Icono del documento](assets/documents.png) en la barra de navegación.

1. Haga clic en **[!UICONTROL Nuevo archivo]** cerca de la parte inferior del complemento.
1. Habilite **[!UICONTROL Crear una prueba]**.

1. Elija el tipo de aprobación de prueba que desee:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>Los procesos de aprobación básicos son ad hoc y pueden incluir diferentes revisores según sea necesario: </p> 
       <ul> 
        <li> <p>(Opcional) Añada <strong>Aprobadores</strong> en el cuadro.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Los administradores generan previamente los procesos de aprobación automatizados, que incluyen revisores y fases específicos. Para más información, consulte <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Información general sobre el flujo de trabajo automatizado</a>.</p> 
       <ul> 
        <li> <p>Elija una [!UICONTROL Workflow Template] en el menú desplegable.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Opcional) Escriba un comentario en el área de **[!UICONTROL Actualizaciones]**.

   ![Aprobaciones de revisión en XD](assets/proof-approvals-xd-350x396.png)

1. En el menú desplegable **[!UICONTROL Tipo de recurso]**, elija el vínculo que acaba de crear en la pestaña **Vínculos compartidos**. Para obtener más información, consulte [Crear un vínculo interactivo para la mesa de trabajo](#create-an-interactive-link-for-your-artboard).\
   ![Vínculos compartidos en XDS](assets/shared-links-xd-350x870.png)

1. Haga clic en **[!UICONTROL Cargar]**

   El documento aparece en el área de [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.

   >[!IMPORTANT]
   >
   >Los usuarios deben tener acceso al [!UICONTROL Visor de corrección de escritorio] para revisar y aprobar las pruebas interactivas. Para obtener más información, consulte [Instalación del [!UICONTROL visor de corrección de escritorio]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## Carga de una nueva versión de prueba

Puede cargar una nueva versión de una prueba. El complemento recuerda el flujo de trabajo de revisión establecido en la versión anterior, pero puede cambiarlo si lo desea.

1. Haga clic en el icono de **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![Icono de menú](assets/menu-350x440.png)

1. Vaya al elemento de trabajo en el que debe cargar un documento.
1. Haga clic en el icono **[!UICONTROL Documento]** ![Icono del documento](assets/documents.png)en la barra de navegación.

1. Haga clic en **[!UICONTROL Nueva versión]** cerca de la parte inferior del complemento.
1. Habilite **[!UICONTROL Crear una prueba]**.
1. Seleccione las mesas de trabajo que desee cargar.

   >[!NOTE]
   >
   >Si desea subir una nueva versión de un archivo .svg, .png o .jpg, solo puede cargar una mesa de trabajo.

1. Elija el tipo de aprobación de prueba que desee:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>Los procesos de aprobación básicos son ad hoc y pueden incluir diferentes revisores según sea necesario: </p> 
       <ul> 
        <li> <p>(Opcional) Añada <strong>Aprobadores</strong> en el cuadro.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Los administradores generan previamente los procesos de aprobación automatizados, que incluyen revisores y fases específicos. Para más información, consulte <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Información general sobre el flujo de trabajo automatizado</a>.</p> 
       <ul> 
        <li> <p>Elija una [!UICONTROL Workflow Template] en el menú desplegable.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. Elija el formato de exportación en el menú desplegable **[!UICONTROL Tipo de recurso]**.

   ![Crear una revisión en XD](assets/create-a-proof-xd-350x202.png)

1. (Opcional) Escriba un comentario en el área de **[!UICONTROL Actualizaciones]**.

   ![Aprobaciones de revisión en XD](assets/proof-approvals-xd-350x396.png)

1. (Opcional) Si selecciona PDF como tipo de recurso y tiene más de una mesa de trabajo seleccionada, elija si desea exportar las mesas de trabajo como un **[!UICONTROL solo archivo PDF]** o **[!UICONTROL varios archivos PDF]**.

1. (Opcional) Asigne un nombre al PDF.

   Opciones de PDF

1. Haga clic en **[!UICONTROL Cargar]**\
   El documento aparece en el área [!UICONTROL Documentos] en el complemento y en la aplicación de escritorio.
