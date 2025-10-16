---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Cargar mesas de trabajo de XD como documentos a Workfront
description: Puede cargar las mesas de trabajo como documentos para su rápida revisión y aprobación, o simplemente para almacenarlos en Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 38%

---


# Cargar [!DNL XD] mesas de trabajo como documentos en [!DNL Workfront]

Puede cargar las mesas de trabajo como documentos para revisarlos y aprobarlos rápidamente o simplemente para almacenarlos en [!DNL Adobe Workfront].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> 
   <p>Standard</p>
   <p>Work or higher</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">Productos adicionales</td> 
   <td>Debe tener una licencia [!DNL Adobe Creative Cloud] además de una licencia [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a [!UICONTROL Documents]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso de [!UICONTROL View] o superior al objeto donde desea cargar un documento.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

* Debe instalar el complemento [!DNL Adobe Workfront for XD] para poder cargar tableros de arte de XD como documentos en Workfront.

Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Agregar un nuevo documento

1. Haga clic en el icono de **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![Icono de menú](assets/menu-350x440.png)

1. Vaya al elemento de trabajo donde desea cargar un documento.
1. Haga clic en el icono **[!UICONTROL Documento]** ![Icono del documento](assets/documents.png) en la barra de navegación.

1. Haga clic en **[!UICONTROL Nuevo archivo]** cerca de la parte inferior del complemento.
1. Seleccione la mesa de trabajo que desee cargar.

   >[!TIP]
   >
   >Para seleccionar más de una mesa de trabajo, haga clic y arrastre el ratón sobre las mesas de trabajo que desee.
1. (Opcional) Escriba un comentario en el área de **[!UICONTROL Actualizaciones]**.
1. Elija **[!UICONTROL Tipo de recurso]** del menú desplegable:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL Formato de exportación]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>Las mesas de trabajo se cargan como un PNG en la ficha [!UICONTROL Documents] del elemento de trabajo en [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>Las mesas de trabajo se cargan como un JPG en la ficha [!UICONTROL Documents] del elemento de trabajo en [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Las mesas de trabajo se cargan como un SVG en la ficha [!UICONTROL Documents] del elemento de trabajo en [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>Elija si desea que las mesas de trabajo seleccionadas se carguen como <strong>un solo archivo de PDF</strong> o <strong>varios archivos de PDF</strong>. Las mesas de trabajo se cargan como un PDF en la ficha [!UICONTROL Documents] del elemento de trabajo de [!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. Haga clic en **[!UICONTROL Cargar]**\
   El documento aparece en el área de [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.

## Añadir una nueva versión

1. Haga clic en el icono de **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![Icono de menú](assets/menu-350x440.png)

1. Vaya al elemento de trabajo donde desea cargar un documento.
1. Haga clic en el icono **[!UICONTROL Documento]** ![Icono del documento](assets/documents.png)en la barra de navegación.

1. Haga clic en el documento al que desea agregar una nueva versión.
1. Haga clic en **[!UICONTROL Nueva versión]** cerca de la parte inferior del complemento.
1. Seleccione las mesas de trabajo que desee cargar.

   >[!NOTE]
   >
   >Si desea cargar una nueva versión de un SVG, PNG o JPG, solo puede cargar una mesa de trabajo.

1. (Opcional) Escriba un comentario en el área de **[!UICONTROL Actualizaciones]**.

1. Elija **[!UICONTROL Tipo de recurso]** del menú desplegable:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">Formato de exportación</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>La mesa de trabajo se carga como un PNG en la ficha [!UICONTROL Documents] del elemento de trabajo de [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>La mesa de trabajo se carga como un JPG en la ficha [!UICONTROL Documents] del elemento de trabajo de [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>La mesa de trabajo se carga como un SVG en la ficha [!UICONTROL Documents] del elemento de trabajo de [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>Las mesas de trabajo se cargan como un PDF en la ficha [!UICONTROL Documents] del elemento de trabajo en [!DNL Workfront].</p>
      <p><strong>Nota</strong>: solo puede cargar una mesa de trabajo para una nueva versión del documento.</p>
      </td>
     </tr>
    </tbody>
   </table>

1. Haga clic en **[!UICONTROL Cargar]**\
   El documento aparece en el área [!UICONTROL Documentos] en el complemento y en la aplicación de escritorio.
