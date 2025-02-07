---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Carga de pruebas desde InDesign
description: Puede cargar sus tableros de arte como documentos para una revisión y aprobación rápidas o simplemente para almacenarlos en Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: ee3dc446-6886-4285-a942-4f44f5c0ac31
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 92%

---

# Carga de pruebas desde [!DNL InDesign]

Puede cargar sus tableros de arte como pruebas directamente a [!DNL Adobe Workfront] para una revisión y aprobación exhaustivas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Plan actual: [!UICONTROL Pro] o superior</p> <p>o</p> <p>Plan heredado: [!UICONTROL Premium]</p> <p>Para obtener más información sobre el acceso de revisión con los diferentes planes, consulte .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>Plan actual: [!UICONTROL Work] o [!UICONTROL Proof]</p> <p>Plan heredado: cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
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

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, comuníquese con el administrador de [!DNL Workfront] o [!DNL Workfront Proof].

+++

## Requisitos previos

* Debe instalar el complemento [!DNL Adobe Workfront for design and video] para poder cargar pruebas desde [!DNL InDesign].

  Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for design and video]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-install-cc.md).

## Carga de una prueba básica

1. Haga clic en el icono **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![Volver a la lista de trabajos](assets/go-back-to-work-list-350x314.png)

1. Vaya al elemento de trabajo en el que desea cargar una prueba.
1. Haga clic en el icono **[!UICONTROL Documento]** ![Icono del documento](assets/documents.png) en la barra de navegación.
1. Haga clic en **[!UICONTROL Nuevo archivo]**, cerca de la parte inferior del complemento.
1. Habilite el conmutador **[!UICONTROL Crear una prueba]**.
1. (Opcional) Escriba un nombre para la prueba en el cuadro de texto **[!UICONTROL Nombre de la revisión]**.
1. En la sección **[!UICONTROL Aprobaciones de prueba]**, seleccione **[!UICONTROL Básico]**.
1. (Opcional) Añada aprobadores.
1. (Opcional) Escriba un comentario en el área **[!UICONTROL Actualizaciones]**.

   ![Agregar un comentario](assets/add-comment.png)

1. Elija el **[!UICONTROL Tipo de recurso]** en el menú desplegable.

1. (Opcional) Seleccione **[!UICONTROL Añadir archivo externo]** para añadir un archivo desde el equipo.
1. Haga clic en **[!UICONTROL Cargar]** y, a continuación, configure las opciones de exportación que desee en función del tipo de recurso elegido antes.

   ![Archivos en el complemento](assets/plugin-files-350x307.png)\
   El documento aparece en el área [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.


## Carga de una prueba automatizada

1. Haga clic en el icono **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![Volver a la lista de trabajos](assets/go-back-to-work-list-350x314.png)

1. Vaya al elemento de trabajo en el que desea cargar una prueba.
1. Haga clic en el icono **[!UICONTROL Documento]** ![Icono del documento](assets/documents.png) en la barra de navegación.

1. Haga clic en **[!UICONTROL Nuevo archivo]**, cerca de la parte inferior del complemento.
1. Habilite el conmutador **[!UICONTROL Crear una prueba]**.
1. (Opcional) Escriba un nombre para la prueba en el cuadro de texto **[!UICONTROL Nombre de la revisión]**.
1. En la sección **[!UICONTROL Aprobaciones de prueba]**, seleccione **[!UICONTROL Automatizado]**.
1. (Opcional) En el cuadro **[!UICONTROL Plantilla de flujo de trabajo]**, escriba el nombre de una plantilla de flujo de trabajo de prueba.

{{adjust-proof-settings}}

>[!NOTE]
>
> Si hay campos obligatorios en blanco en la plantilla de flujo de trabajo, la configuración de la prueba automatizada se abre de forma automática y es necesario rellenar esos campos para cargar la prueba.


1. (Opcional) Escriba un comentario en el área **[!UICONTROL Actualizaciones]**.

   ![Agregar aprobación automatizada de comentario](assets/add-comment-automated-approval.png)

1. Elija el **[!UICONTROL Tipo de recurso]** en el menú desplegable.
1. (Opcional) Seleccione **[!UICONTROL Añadir archivo externo]** para añadir un archivo desde el equipo.
1. Haga clic en **[!UICONTROL Cargar]** y, a continuación, configure las opciones de exportación que desee en función del tipo de recurso elegido antes.
El documento aparece en el área [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.

## Carga de una nueva versión de prueba

Puede cargar una nueva versión de una prueba. El complemento recuerda el flujo de trabajo de revisión establecido en la versión anterior, pero puede cambiarlo si lo desea.

1. Haga clic en el icono de **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![Volver a la lista de trabajos](assets/go-back-to-work-list-350x314.png)

1. Vaya al elemento de trabajo en el que debe cargar un documento.
1. Haga clic en el icono **[!UICONTROL Documento]** ![Icono del documento](assets/documents.png)en la barra de navegación.

1. Haga clic en **[!UICONTROL Nueva versión]** cerca de la parte inferior del complemento.
1. Habilite el conmutador **[!UICONTROL Crear una revisión]**.

1. En la sección *[!UICONTROL *Aprobaciones de revisión]**, elija **[!UICONTROL Básico]** o **[!UICONTROL Automatizado]**.

1. Añada **[!UICONTROL Revisores]** o una **[!UICONTROL Plantilla de flujo de trabajo]** según el tipo de aprobación que seleccionó en el paso 7.

1. (Opcional) Escriba un comentario en el área **[!UICONTROL Actualizaciones]**.
1. Elija el **[!UICONTROL Tipo de recurso]** en el menú desplegable.
1. Haga clic en **[!UICONTROL Cargar]** y, a continuación, configure las opciones de exportación que desee en función del tipo de recurso elegido antes.
El documento aparece en el área [!UICONTROL Documentos] del complemento y de la aplicación de escritorio.
