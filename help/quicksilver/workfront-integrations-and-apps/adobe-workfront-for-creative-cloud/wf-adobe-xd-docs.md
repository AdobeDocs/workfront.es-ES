---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Cargar XD tableros como documentos a Workfront
description: Puede cargar las mesas de trabajo como documentos para una revisión y aprobación rápidas o simplemente para almacenarlas en Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: bf47ae15d2972e8ee11f76741f8e5c676d79e626
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---


# Cargar [!DNL XD] tableros como documentos para [!DNL Workfront]

Puede cargar las mesas de trabajo como documentos para una revisión y aprobación rápidas o simplemente para almacenarlas en [!DNL Adobe Workfront].

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">Product</td> 
   <td>Debe tener un [!DNL Adobe Creative Cloud] además de una [!DNL Workfront] licencia.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a [!UICONTROL Documents]</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>[!UICONTROL View] tiene acceso o superior al objeto en el que desea cargar un documento.</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

* Debe instalar el [!DNL Adobe Workfront for XD] antes de poder cargar XD tableros de arte como documentos en Workfront.

Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Agregar un nuevo documento

1. Haga clic en el **[!UICONTROL Menú]** en la esquina superior derecha y, a continuación, seleccione **[!UICONTROL Lista de trabajo]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/menu-350x440.png)

1. Vaya al elemento de trabajo en el que desea cargar un documento.
1. Haga clic en el **[!UICONTROL Documento]** icono ![](assets/documents.png) en la barra de navegación.

1. Haga clic en **[!UICONTROL Nuevo archivo]** cerca de la parte inferior del complemento.
1. Seleccione la mesa de trabajo que desee cargar.

   >[!TIP]
   >
   >Para seleccionar más de una mesa de trabajo, haga clic y arrastre el ratón sobre las mesas de trabajo que desee.
1. (Opcional) Escriba un comentario en el **[!UICONTROL Actualizaciones]** .
1. Elija la **[!UICONTROL Tipo de recurso]** en el menú desplegable:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL Formato de exportación]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>Las mesas de trabajo se cargan como PNG a la ficha [!UICONTROL Documents] del elemento de trabajo en [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>Las mesas de trabajo se cargan como JPG en la ficha [!UICONTROL Documents] del elemento de trabajo [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Las mesas de trabajo se cargan como SVG en la ficha [!UICONTROL Documents] del elemento de trabajo [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>Elija si desea que las mesas de trabajo seleccionadas se carguen como <strong>Archivo de PDF único</strong> o <strong>Varios archivos de PDF</strong>. Las mesas de trabajo se cargan como PDF a la ficha [!UICONTROL Documents] del elemento de trabajo en [!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. Haga clic en **[!UICONTROL Cargar]**.\
   El documento aparece en la [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.

## Agregar una nueva versión

1. Haga clic en el **[!UICONTROL Menú]** en la esquina superior derecha y, a continuación, seleccione **[!UICONTROL Lista de trabajo]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/menu-350x440.png)

1. Vaya al elemento de trabajo en el que desea cargar un documento.
1. Haga clic en el **[!UICONTROL Documento]** icono ![](assets/documents.png)en la barra de navegación.

1. Haga clic en el documento al que desee agregar una versión nueva.
1. Haga clic en **[!UICONTROL Nueva versión]** cerca de la parte inferior del complemento.
1. Seleccione las mesas de trabajo que desee cargar.

   >[!NOTE]
   >
   >Si desea cargar una nueva versión de un SVG, PNG o JPG, solo puede cargar una mesa de trabajo.

1. (Opcional) Escriba un comentario en el **[!UICONTROL Actualizaciones]** .

1. Elija la **[!UICONTROL Tipo de recurso]** en el menú desplegable:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">Formato de exportación</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>La mesa de trabajo se carga como PNG a la ficha [!UICONTROL Documents] del elemento de trabajo en [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>La mesa de trabajo se carga como JPG a la ficha [!UICONTROL Documents] del elemento de trabajo en [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>La mesa de trabajo se carga como SVG a la ficha [!UICONTROL Documents] del elemento de trabajo en [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>Las mesas de trabajo se cargan como PDF en la ficha [!UICONTROL Documents] del elemento de trabajo [!DNL Workfront].</p>
      <p><strong>Nota</strong>: Solo se puede cargar una mesa de trabajo para una nueva versión del documento.</p>
      </td>
     </tr>
    </tbody>
   </table>

1. Haga clic en **[!UICONTROL Cargar]**.\
   El documento aparece en la [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.
