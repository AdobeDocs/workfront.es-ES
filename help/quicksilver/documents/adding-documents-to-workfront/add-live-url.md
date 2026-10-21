---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Adición de un vínculo web como documento
description: Puede agregar un sitio web a Adobe Workfront como vínculo web y solicitar su aprobación.
author: Courtney
feature: Digital Content and Documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
source-git-commit: 05f148f2c28555e37fb415f606e314a5df564047
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 8%
---
# Adición de un vínculo web como documento

Puede agregar un sitio web a Adobe Workfront como vínculo web desde la nueva área Documentos. Después de agregarlo, puede solicitar la aprobación en la página web activa del mismo modo que solicita la aprobación de un archivo cargado.

Si su organización utiliza el almacenamiento en la nube de Adobe, verá la nueva área Documentos al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento en la nube de Adobe, consulte [Información general sobre el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquier paquete de Workfront para administrar documentos mediante el almacenamiento heredado de Workfront</p>
<p>Cualquier paquete de flujo de trabajo para administrar documentos mediante Adobe Cloud Storage.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior</p> 
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Almacenamiento de Workfront heredado: Editar acceso a documentos</p> 
   <p>Almacenamiento en la nube de Adobe: Editar acceso a documentos está habilitado de forma predeterminada y no se puede cambiar</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adición de un vínculo web como documento

Puede cargar una página web HTML en Workfront como vínculo web. Después de agregarlo, puede solicitar la aprobación en la página web activa del mismo modo que solicita la aprobación de un archivo cargado. Para obtener más información sobre cómo Frame.io administra los vínculos web, consulte [Revisión de HTML para Frame.io](https://support.frame.io/hc/en-us/articles/360041187574-Frame-io-Web-Links).


>[!IMPORTANT]
>
>* Las direcciones URL son compatibles si el sitio permite incrustaciones de iFrame.
>* Se admiten direcciones URL web privadas, pero es posible que ciertos flujos de autenticación no funcionen según la configuración del servidor.
>* Las direcciones URL de YouTube y Figma no son compatibles actualmente.<br>
>Para obtener más información, consulte [Revisión de HTML para Frame.io](https://help.frame.io/en/articles/12893213-html-review-for-frame-io).


Para añadir un vínculo web:

1. Vaya al proyecto, tarea o problema donde desee agregar el sitio web y, a continuación, seleccione **Documentos** en el panel izquierdo.
1. Haga clic en **Nuevo** y, a continuación, seleccione **vínculo web**.
1. Escriba un nombre en el campo **Nombre del documento** y luego ingrese la dirección del sitio web en el campo **URL**.
1. Haga clic en **Añadir**.
   ![Agregar un vínculo web como documento](assets/web-url.png)

Para solicitar aprobación en el vínculo web, consulte [Crear un flujo de trabajo de aprobación de documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

## Limitaciones conocidas

* Hay un problema temporal con los documentos de vínculo web creados en Frame.io. Si crea un vínculo web en Frame.io y, a continuación, crea una aprobación para él en Workfront, el documento no se abrirá en Frame.io. Los vínculos web creados en Workfront no se ven afectados. Hasta que se resuelva, cree documentos de vínculo web en Workfront antes de iniciar una aprobación.
* Actualmente no se pueden crear versiones nuevas de documentos de vínculos web en Frame.io. Si necesita crear una nueva versión de un documento de vínculo web, cree la nueva versión en Workfront.