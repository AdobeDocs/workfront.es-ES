---
title: Configurar integraciones de documentos
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Como administrador de Adobe Systems Workfront, puede configurar integraciones de documento para administrar documentos en Workfront.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: 5ff071a6e0af93f5280225355edad1d0dde42b3f
workflow-type: tm+mt
source-wordcount: '1125'
ht-degree: 12%

---

# Configurar integraciones de documentos

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como administrador de [!DNL Adobe Workfront], puede configurar integraciones de documentos para administrar documentos en [!UICONTROL Workfront]. También puede configurar [!UICONTROL Workfront] para que los documentos se almacenen únicamente en aplicaciones de servicios de documentos y no en el propio [!UICONTROL Workfront]. Para obtener más información, consulte [Actualizar y vincular un documento de [!UICONTROL Workfront] a un proveedor de nube externo](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) en [Vincular documentos de aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Para permitir la comunicación abierta entre [!DNL Workfront Proof] y los servidores [!DNL Workfront], es posible que tenga que agregar ciertas direcciones IP a la lista de permitidos. Para obtener más información, consulte [Configurar la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Para realizar los pasos de este artículo, debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Nuevo: [!UICONTROL Standard]</p>
       <p>o</p>
       <p>Actual: [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Integraciones compatibles

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Puede configurar las siguientes integraciones para administrar documentos:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  Vincular pruebas de [!DNL Workfront Proof] le permite hacer que las pruebas que se crearon originalmente estén [!DNL Workfront Proof] disponibles en [!DNL Workfront]. Para los planes actuales, se requiere un [!UICONTROL Pro] [!DNL Workfront] plan o superior para usar esta función. Para los nuevos planes, esta función está disponible con todos los planes. Para obtener más información sobre los diversos planes disponibles, consulte [Planes de Workfront](https://www.workfront.com/plans).

* [!DNL Microsoft SharePoint]

  Para obtener información sobre la integración con [!DNL SharePoint], consulte [Configurar la [!DNL SharePoint] integración](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Proveedores de documentos de nube de terceros:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Unidad Google]
   * Quip

  >[!TIP]
  >
  >Puede revisar y aprobar documentos enlazados desde un proveedor de nube externo de la misma manera que revisa y aprueba documentos cargados directamente en [!DNL Workfront].

* Otros proveedores de documentos (mediante integraciones de documentos personalizadas).

  Para los planes actuales, se requiere un [!UICONTROL Pro] [!DNL Workfront] plan o superior para usar esta función. Para los nuevos planes, esta función está disponible con todos los planes. Para obtener más información sobre los diversos planes disponibles, consulte [Planes de Workfront](https://www.workfront.com/plans).

Además, puede mejorar su [!DNL Workfront] experiencia documento con una terceros DAM integraciones. Los administradores deben habilitar estas funciones para que los usuarios puedan vincular el servicio a sus [!DNL Workfront] cuenta.

## Configurar integraciones para administrar documentos

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL proveedores] de nube.**

1. (Opcional) Para almacenar documentos en una aplicación de servicios de documento y no en [!DNL Workfront], seleccione **[!UICONTROL Impedir que los usuarios almacenen documentos en [!DNL Workfront]].**

1. Seleccione las integraciones que desea activar.
1. Haga clic en **[!UICONTROL Guardar]**.

Si está configurando integraciones con [!DNL Workfront DAM], puede activar [!DNL Workfront] la inclusión de metadatos con documentos. Para obtener información sobre la asignación de metadatos, consulte [Configuración de la asignación](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md) metadatos.

## Configurar integraciones de documento personalizadas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Una integración de documentos personalizada permite a los usuarios de [!DNL Workfront] vincular archivos a [!DNL Workfront] prácticamente desde cualquier sistema, siempre que el sistema funcione con [!DNL Workfront].

Para que la integración personalizada esté disponible para los usuarios, primero debe versión la integración. Para obtener información acerca de cómo versión integraciones que se utilizarán con [!DNL Workfront], vea [Document Webhooks API.](../../wf-api/doc-wbhks-api/docu-webhook-api.md)

Una vez creada la integración de documento personalizada, puede ponerla a disposición de los usuarios de su sitio.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL integración personalizada]**.

1. Haga clic en **[!UICONTROL añadir Integración]** personalizada.
1. Introduzca la siguiente información para configurar la integración:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>El nombre de la integración personalizada. Es el nombre que ven los usuarios cuando utilizan la integración en Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[! UICONTROL Base API URL] </td> 
      <td>La URL HTTP base o HTTP segura para llamadas a la API. Por ejemplo: <code>https://&lt;documentprovider&gt;.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[! Tipo de Authentication UICONTROL]</td> 
      <td> <p>El método de autenticación que se utiliza al realizar llamadas de API autorizadas a la integración personalizada.</p> 
       <ul> 
        <li>Si elige <strong>[! UICONTROL OAuth]</strong>, continúe con el paso 5.</li> 
        <li>Si elige <strong>[! UICONTROL ApiKey]</strong>, continúe con el paso 6.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Si seleccionó **[!UICONTROL la autenticación OAuth]** para el Tipo ]**de**[!UICONTROL  Authentication, introduzca la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication URL]</td> 
      <td>Todas las URL utilizadas para usuario autenticación. [!DNL Workfront] desplaza a los usuarios a esta dirección como parte del proceso de aprovisionamiento de OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[! Punto final del token de UICONTROL URL]</td> 
      <td>Dirección de URL de API completa que sirve para recuperar tokens de OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>El ID de cliente de OAut para esta integración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Secreto de cliente de OAut para esta integración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parámetros de solicitud]</td> 
      <td> <p>Introduzca valores opcionales que se añadirán a la cadena de consulta de cada llamada de API. Por ejemplo, access_type=offline.</p> <p>Para añadir varios parámetros solicitud, haga clic en <strong>+añadir Parámetro</strong> de solicitud.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >El [!DNL Workfront] URI de redirección que se muestra en la parte inferior del [!UICONTROL Página de integración] personalizada enumera el URI utilizado para registrar esta integración con el proveedor de documento externo.

1. (Condicional) Si seleccionó **[!UICONTROL la autenticación de ApiKey]** para el Tipo de **[!UICONTROL Authentication]**, escriba la clave de API emitida por el proveedor de documento personalizado.

   [!DNL Workfront] utiliza esta clave de API para realizar llamadas de API autorizadas al proveedor de documento.

1. Haga clic en **[!UICONTROL Guardar]** para crear la integración.

## Usar integraciones de documento

Para obtener más información sobre cómo los usuarios pueden utilizar las correcciones, consulte [Crear pruebas](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

Para obtener información sobre cómo pueden usar los usuarios terceros integraciones de documento después de haberlas configurado, consulte [Vincular documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configurar [!DNL Workfront] para enviar metadatos a [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Al enviar un documento desde [!DNL Workfront] a [!DNL Workfront DAM], también puede enviar información asociada a ese documento. La información sobre la documento se asigna como [!DNL Workfront DAM] metadatos.

La información se asigna solo en un sentido, desde [!DNL Workfront] a [!DNL Workfront DAM] y se transfiere solo cuando el documento se carga en [!DNL Workfront DAM]. Cualquier cambio futuro en los campos de Workfront no actualizará los campos de metadatos en [!DNL Workfront DAM] después de que ya se haya cargado el documento.\
Puede asignar el mismo [!DNL Workfront] campo a varios [!DNL Workfront DAM] campos, pero no puede utilizar el mismo [!DNL Workfront DAM] campo para varios [!DNL Workfront] campos.

Si debe configurar varios [!DNL Workfront] campos para exportar a un [!DNL Workfront DAM] solo campo, cree primero un campo personalizado calculado para [!DNL Workfront] mostrar todos los campos personalizados individuales de un objeto. A continuación, asigne el campo calculado [!DNL Workfront] a un [!DNL Workfront DAM] campo.\
Para obtener más información sobre los campos personalizados calculados, consulte [Añadir campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

La asignación afecta a todos los documentos cargados por cualquier usuario en [!UICONTROL la DAM de [!DNL Workfront] Workfront].

Como administrador de [!DNL Workfront], debe habilitar [!DNL Workfront DAM] en Workfront para poder asignar los campos para el proceso de asignación de metadatos.

Para configurar [!DNL Workfront] para enviar metadatos a [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Asignación de metadatos]**.

1. En el campo **[!UICONTROL Seleccionar campo de Source para asignación]**, empiece a escribir el nombre del campo de Workfront que desea asignar a [!DNL Workfront DAM] y, a continuación, selecciónelo cuando lo vea en la lista.
1. En **[!UICONTROL Seleccionar campo de destino para asignación]**, seleccione el campo [!DNL Workfront DAM] que desee rellenar con la información del campo [!DNL Workfront] seleccionado.

   >[!NOTE]
   >
   > Todos los documentos enviados a [!DNL Workfront DAM] por usuarios que tienen derechos para hacerlo tienen sus metadatos actualizados con los campos de [!DNL Workfront] asignados aquí, cuando se cargan en [!DNL Workfront DAM].

1. Haga clic en **[!UICONTROL Add Mapping]**.

1. Continuar agregar más [!UICONTROL campos de Workfront] y los campos correspondientes [!DNL Workfront DAM] .

### Eliminar campos asignados

{{step-1-to-setup}}

1. Expanda **[!UICONTROL Documentos]** y, a continuación, haga clic en **[!UICONTROL Asignación de metadatos]**.

1. En la lista de campos, seleccione cualquiera de los campos que desee quitar de metadatos asignación.
1. Haga clic **[!UICONTROL eliminar]**.

   Los campos se eliminan de metadatos asignación y la información contenida en ellos no se transfiere con [!DNL Workfront DAM] el documentos cargado.


## Limitaciones

* La integración de Google Drive documento admite agregar carpetas e imágenes desde el área My Drive de tu Google Drive. No puedes añadir carpetas ni imágenes desde una unidad compartida. Obtén más información sobre [Google Shared Drives](https://support.google.com/a/users/answer/7212025?hl=en).