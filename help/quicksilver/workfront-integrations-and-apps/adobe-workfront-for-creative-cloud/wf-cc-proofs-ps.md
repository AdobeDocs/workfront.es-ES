---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Cargar pruebas desde Adobe Photoshop
description: Puede cargar los tableros de arte como pruebas directamente en Adobe Workfront para una revisión y aprobación exhaustivas.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: cbb12ee7-949e-44a1-9340-3ef93c003b21
source-git-commit: 4256e1ecd16179d0a2aa8e623b05be754d8bbd2d
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 0%

---

# Cargar pruebas de [!DNL Photoshop]

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
   <td> <p>Editar acceso a documentos de [!UICONTROL]</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Requisitos previos

* Debe instalar [!DNL Adobe Workfront for Photoshop] para poder cargar pruebas desde [!DNL Adobe Photoshop].

  Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for Photoshop]](../../workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md).

## Cargar una prueba básica

1. Haga clic en el icono **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/go-back-to-work-list-350x314.png)

1. Vaya al elemento de trabajo en el que desea cargar una prueba.
1. Haga clic en el icono **[!UICONTROL Documento]** ![](assets/documents.png) en la barra de navegación.
1. Haga clic en **[!UICONTROL Nuevo archivo]** cerca de la parte inferior del panel [!DNL Workfront].
1. Habilite la opción **[!UICONTROL Crear una revisión]**.
1. (Opcional) Escriba un nombre para la revisión en el cuadro de texto **[!UICONTROL Nombre de revisión]**.
1. En la sección **[!UICONTROL Aprobaciones de revisión]**, seleccione **[!UICONTROL Básico]**.
1. (Opcional) Añada aprobadores.
1. (Opcional) Escriba un comentario en el área **[!UICONTROL Actualizaciones]**.

   ![](assets/add-comment.png)

1. Elija **[!UICONTROL Tipo de recurso]** en el menú desplegable.

1. (Opcional) Seleccione **[!UICONTROL Agregar archivo externo]** para agregar un archivo desde el equipo.
1. Haga clic en **[!UICONTROL Cargar]** y, a continuación, configure las opciones de exportación que desee en función del tipo de recurso elegido anteriormente.

   ![](assets/plugin-files-350x307.png)\
   El documento aparece en el área [!UICONTROL Documentos] del panel [!DNL Workfront] en [!DNL Photoshop] y en la aplicación de escritorio [!DNL Workfront].


## Cargar una revisión automatizada

1. Haga clic en el icono **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/go-back-to-work-list-350x314.png)

1. Vaya al elemento de trabajo en el que desea cargar una prueba.
1. Haga clic en el icono **[!UICONTROL Documento]** ![](assets/documents.png) en la barra de navegación.

1. Haga clic en **[!UICONTROL Nuevo archivo]** cerca de la parte inferior del panel [!DNL Workfront].
1. Habilite la opción **[!UICONTROL Crear una revisión]**.
1. (Opcional) Escriba un nombre para la revisión en el cuadro de texto **[!UICONTROL Nombre de revisión]**.
1. En la sección **[!UICONTROL Aprobaciones de revisión]**, seleccione **[!UICONTROL Automatizado]**.
1. (Opcional) En el cuadro **[!UICONTROL Plantilla de flujo de trabajo]**, escriba el nombre de una plantilla de flujo de trabajo de revisión.

{{adjust-proof-settings}}

>[!NOTE]
>
> Si hay campos obligatorios en blanco en la plantilla de flujo de trabajo, la configuración de la prueba automatizada se abre automáticamente y es necesario rellenar esos campos para cargar la prueba.


1. (Opcional) Escriba un comentario en el área **[!UICONTROL Actualizaciones]**.

   ![](assets/add-comment-automated-approval.png)

1. Elija **[!UICONTROL Tipo de recurso]** en el menú desplegable.
1. (Opcional) Seleccione **[!UICONTROL Agregar archivo externo]** para agregar un archivo desde el equipo.
1. Haga clic en **[!UICONTROL Cargar]** y, a continuación, configure las opciones de exportación que desee en función del tipo de recurso elegido anteriormente.
El documento aparece en el área [!UICONTROL Documentos] del panel [!DNL Workfront] en [!DNL Photoshop] y en la aplicación de escritorio [!DNL Workfront].

## Cargar una nueva versión de revisión

Puede cargar una nueva versión de una prueba. El complemento recuerda el flujo de trabajo de revisión establecido en la versión anterior, pero puede cambiarlo si lo desea.

1. Haga clic en el icono **[!UICONTROL Menú]** en la esquina superior derecha y seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/go-back-to-work-list-350x314.png)

1. Vaya al elemento de trabajo en el que debe cargar un documento.
1. Haga clic en el icono **[!UICONTROL Documento]** ![](assets/documents.png)de la barra de navegación.

1. Haga clic en **[!UICONTROL Nueva versión]** cerca de la parte inferior del panel [!DNL Workfront].
1. Habilite la opción **[!UICONTROL Crear una revisión]**.

1. En la sección *[!UICONTROL *Aprobaciones de revisión]**, elija **[!UICONTROL Básico]** o **[!UICONTROL Automatizado]**.

1. Agregue **[!UICONTROL Revisores]** o una **[!UICONTROL plantilla de flujo de trabajo]** según el tipo de aprobación que seleccionó en el paso 7.

1. (Opcional) Escriba un comentario en el área **[!UICONTROL Actualizaciones]**.
1. Elija **[!UICONTROL Tipo de recurso]** en el menú desplegable.
1. Haga clic en **[!UICONTROL Cargar]** y, a continuación, configure las opciones de exportación que desee en función del tipo de recurso elegido anteriormente.
El documento aparece en el área [!UICONTROL Documentos] del panel [!DNL Workfront] en [!DNL Photoshop] y en la aplicación de escritorio [!DNL Workfront].
