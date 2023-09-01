---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Cargar pruebas desde Illustrator
description: Puede cargar sus tableros de arte como documentos para una revisión y aprobación rápidas o simplemente para almacenarlos en Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: e98f27d4-7c07-44cc-8df5-e04472ec946e
source-git-commit: 66186bb8af14e7ce86b3fb5e8bb1b07fe32dca7a
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Cargar pruebas desde [!DNL Illustrator]

Puede cargar sus tableros de arte como pruebas directamente en [!DNL Adobe Workfront] para una revisión y aprobación exhaustivas.

## Requisitos de acceso

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
   <td>Debe tener un [!DNL Adobe Creative Cloud] licencia además de una [!DNL Workfront] licencia.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>[!UICONTROL Manager] o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Editar acceso a documentos de [!UICONTROL]</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su [!DNL Workfront] o [!DNL Workfront Proof] administrador.

## Requisitos previos

* Debe instalar [!DNL Adobe Workfront for design and video] antes de poder cargar pruebas desde [!DNL Illustrator].

  Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for design and video]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-install-cc.md).

## Cargar una prueba básica

1. Haga clic en **[!UICONTROL Menú]** en la esquina superior derecha, y luego seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/go-back-to-work-list-350x314.png)

1. Vaya al elemento de trabajo en el que desea cargar una prueba.
1. Haga clic en **[!UICONTROL Documento]** icono ![](assets/documents.png) en la barra de navegación.
1. Clic **[!UICONTROL Nuevo archivo]** cerca de la parte inferior del complemento.
1. Habilite la **[!UICONTROL Creación de una prueba]** alternar.
1. (Opcional) Escriba un nombre para la prueba en la **[!UICONTROL Nombre de revisión]** cuadro de texto.
1. En el **[!UICONTROL Aprobaciones de revisión]** , seleccione **[!UICONTROL Básico]**.
1. (Opcional) Añada aprobadores.
1. (Opcional) Escriba un comentario en la **[!UICONTROL Actualizaciones]** área.

   ![](assets/add-comment.png)

1. Elija la **[!UICONTROL Tipo de recurso]** en el menú desplegable.

1. (Opcional) Seleccione **[!UICONTROL Añadir archivo externo]** para agregar un archivo desde el equipo.
1. Clic **[!UICONTROL Cargar]** A continuación, configure las opciones de exportación que desee en función del tipo de recurso elegido anteriormente.

   ![](assets/plugin-files-350x307.png)\
   El documento aparece en la [!UICONTROL Documentos] en el complemento y en la aplicación de escritorio.


## Cargar una revisión automatizada

1. Haga clic en **[!UICONTROL Menú]** en la esquina superior derecha, y luego seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/go-back-to-work-list-350x314.png)

1. Vaya al elemento de trabajo en el que desea cargar una prueba.
1. Haga clic en **[!UICONTROL Documento]** icono ![](assets/documents.png) en la barra de navegación.

1. Clic **[!UICONTROL Nuevo archivo]** cerca de la parte inferior del complemento.
1. Habilite la **[!UICONTROL Creación de una prueba]** alternar.
1. (Opcional) Escriba un nombre para la prueba en la **[!UICONTROL Nombre de revisión]** cuadro de texto.
1. En el **[!UICONTROL Aprobaciones de revisión]** , seleccione **[!UICONTROL Automatizado]**.
1. (Opcional) En el **[!UICONTROL Plantilla de flujo de trabajo]** , escriba el nombre de una plantilla de flujo de trabajo de prueba.

{{adjust-proof-settings}}

>[!NOTE]
>
> Si hay campos obligatorios en blanco en la plantilla de flujo de trabajo, la configuración de la prueba automatizada se abre automáticamente y es necesario rellenar esos campos para cargar la prueba.


1. (Opcional) Escriba un comentario en la **[!UICONTROL Actualizaciones]** área.

   ![](assets/add-comment-automated-approval.png)

1. Elija la **[!UICONTROL Tipo de recurso]** en el menú desplegable.
1. (Opcional) Seleccione **[!UICONTROL Añadir archivo externo]** para agregar un archivo desde el equipo.
1. Clic **[!UICONTROL Cargar]**A continuación, configure las opciones de exportación que desee en función del tipo de recurso elegido anteriormente.
El documento aparece en la [!UICONTROL Documentos] en el complemento y en la aplicación de escritorio.

## Cargar una nueva versión de revisión

Puede cargar una nueva versión de una prueba. El complemento recuerda el flujo de trabajo de revisión establecido en la versión anterior, pero puede cambiarlo si lo desea.

1. Haga clic en **[!UICONTROL Menú]** en la esquina superior derecha, y luego seleccione **[!UICONTROL Lista de trabajos]**. También puede utilizar el menú para desplazarse a los objetos principales.

   ![](assets/go-back-to-work-list-350x314.png)

1. Vaya al elemento de trabajo en el que debe cargar un documento.
1. Haga clic en **[!UICONTROL Documento]** icono ![](assets/documents.png)en la barra de navegación.

1. Clic **[!UICONTROL Nueva versión]** cerca de la parte inferior del complemento.
1. Habilite la **[!UICONTROL Creación de una prueba]** alternar.

1. En el *[!UICONTROL *Aprobaciones de pruebas]** sección, elija **[!UICONTROL Básico]** o **[!UICONTROL Automatizado]**.

1. Añadir **[!UICONTROL Revisores]** o una **[!UICONTROL Plantilla de flujo de trabajo]** en función del tipo de aprobación seleccionado en el paso 7.

1. (Opcional) Escriba un comentario en la **[!UICONTROL Actualizaciones]** área.
1. Elija la **[!UICONTROL Tipo de recurso]** en el menú desplegable.
1. Clic **[!UICONTROL Cargar]**A continuación, configure las opciones de exportación que desee en función del tipo de recurso elegido anteriormente.
El documento aparece en la [!UICONTROL Documentos] en el complemento y en la aplicación de escritorio.
