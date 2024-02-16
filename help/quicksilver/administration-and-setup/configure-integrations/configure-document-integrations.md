---
title: Configurar integraciones de documentos
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Como administrador de Adobe Workfront, puede configurar integraciones de documentos para administrar documentos en Workfront.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 1%

---

# Configurar integraciones de documentos

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como un [!DNL Adobe Workfront] administrador, puede configurar integraciones de documentos para administrar documentos en [!UICONTROL Workfront]. También puede configurar [!UICONTROL Workfront] para que los documentos se almacenen únicamente en aplicaciones de servicios de documentos y no en [!UICONTROL Workfront] sí mismo. Para obtener más información, consulte [Actualizar y vincular un documento desde [!UICONTROL Workfront] a un proveedor de nube externo](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) in [Vinculación de documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Para permitir la comunicación abierta entre [!DNL Workfront Proof] y el [!DNL Workfront] servidores, es posible que tenga que añadir determinadas direcciones IP a la lista de permitidos. Para obtener más información, consulte [Configuración de la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

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
       <p>Actual: [!UICONTROL plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser un [!DNL Workfront] administrador.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Integraciones compatibles

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Puede configurar las siguientes integraciones para administrar documentos:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  Vinculación de pruebas desde [!DNL Workfront Proof] permite realizar pruebas que se crearon originalmente en [!DNL Workfront Proof] disponible en [!DNL Workfront]. Para los planes actuales, un [!UICONTROL Pro] [!DNL Workfront] Se requiere planificación o superior para utilizar esta función. Para los nuevos planes, esta función está disponible con todos los planes. Para obtener más información sobre los distintos planes disponibles, consulte [Planes de Workfront](https://www.workfront.com/plans).

* [!DNL Microsoft SharePoint]

  Para obtener información sobre la integración de con [!DNL SharePoint], consulte [Configure las variables [!DNL SharePoint] integración](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Proveedores de documentos de nube de terceros:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google Drive]

     <!--Quip-->
  >[!TIP]
  >
  >Puede probar y aprobar documentos vinculados desde un proveedor de nube externo del mismo modo que prueba y aprueba documentos cargados directamente en [!DNL Workfront].

* Otros proveedores de documentos (mediante integraciones de documentos personalizadas).

  Para los planes actuales, un [!UICONTROL Pro] [!DNL Workfront] Se requiere planificación o superior para utilizar esta función. Para los nuevos planes, esta función está disponible con todos los planes. Para obtener más información sobre los distintos planes disponibles, consulte [Planes de Workfront](https://www.workfront.com/plans).

Además, puede mejorar su [!DNL Workfront] Documente la experiencia con un sistema nativo de administración de activos digitales (DAM) o con integraciones DAM de terceros. Los administradores deben habilitar estas funciones para que los usuarios puedan vincular el servicio a su [!DNL Workfront] cuenta. Para obtener más información sobre Workfront DAM, consulte [Administrar documentos con [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Configurar integraciones para administrar documentos

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Proveedores de nube].**

1. (Opcional) Para almacenar documentos en una aplicación de servicios de documentos y no en [!DNL Workfront], seleccione **[!UICONTROL Impedir que los usuarios almacenen documentos en [!DNL Workfront]].**

1. Seleccione las integraciones que desee activar.
1. Haga clic en **[!UICONTROL Guardar]**.

Si configura integraciones con [!DNL Workfront DAM], puede habilitar [!DNL Workfront] para incluir metadatos en documentos. Para obtener información sobre la asignación de metadatos, consulte [Configurar asignación de metadatos](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configurar integraciones de documentos personalizadas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Una integración de documentos personalizada permite [!DNL Workfront] usuarios a los que vincular archivos [!DNL Workfront] de prácticamente cualquier sistema, siempre que el sistema esté diseñado para funcionar con [!DNL Workfront].

Para que la integración personalizada esté disponible para los usuarios de, primero debe crear la integración de. Para obtener información sobre cómo crear integraciones para utilizarlas con [!DNL Workfront], consulte [API de webhooks de documentos](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Una vez creada la integración de documentos personalizada, puede ponerla a disposición de los usuarios de su sitio.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Integración personalizada]**.

1. Clic **[!UICONTROL Añadir integración personalizada]**.
1. Introduzca la siguiente información para configurar la integración:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre]</td> 
      <td>Nombre de la integración personalizada. Este es el nombre que los usuarios ven al utilizar la integración en Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL de API base] </td> 
      <td>La dirección URL HTTP base o HTTP segura para llamadas a la API. Por ejemplo, <code>https://documentprovider.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de autenticación]</td> 
      <td> <p>El método de autenticación que se utiliza al realizar llamadas de API autorizadas a la integración personalizada.</p> 
       <ul> 
        <li>Si elige <strong>[!UICONTROL OAuth]</strong>, continúe con el paso 5.</li> 
        <li>Si elige <strong>[!UICONTROL ApiKey]</strong>, continúe con el paso 6.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Si ha seleccionado **[!UICONTROL OAuth]** autenticación para el **[!UICONTROL Tipo de autenticación]**, introduzca la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL de autenticación]</td> 
      <td>Dirección URL completa que se utiliza para la autenticación de usuarios. [!DNL Workfront] desplaza a los usuarios a esta dirección como parte del proceso de aprovisionamiento de OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Endpoint URL]</td> 
      <td>Dirección de URL de API completa que sirve para recuperar tokens de OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID de cliente]</td> 
      <td>El ID de cliente de OAut para esta integración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Secreto de cliente]</td> 
      <td>Secreto de cliente de OAut para esta integración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parámetros de solicitud]</td> 
      <td> <p>Introduzca valores opcionales que se añadirán a la cadena de consulta de cada llamada de API. Por ejemplo, access_type=offline.</p> <p>Para agregar varios parámetros de solicitud, haga clic en <strong>+Agregar parámetro de solicitud</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >El [!DNL Workfront] URI de redireccionamiento que se muestra en la parte inferior de [!UICONTROL Integración personalizada] Esta página enumera el URI utilizado para registrar esta integración con el proveedor de documentos externo.

1. (Condicional) Si ha seleccionado **[!UICONTROL ApiKey]** autenticación para el **[!UICONTROL Tipo de autenticación]**, introduzca la clave de API emitida por el proveedor de documentos personalizados.

   [!DNL Workfront] utiliza esta clave API para realizar llamadas de API autorizadas al proveedor de documentos.

1. Clic **[!UICONTROL Guardar]** para crear la integración.

## Uso de integraciones de documentos

Para obtener información sobre cómo pueden utilizar los usuarios [!DNL Workfront DAM], consulte [Administrar documentos con [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

Para obtener información sobre cómo los usuarios pueden utilizar la revisión, consulte [Creación de pruebas](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

Para obtener información sobre cómo los usuarios pueden utilizar las integraciones de documentos de terceros después de configurarlas, consulte [Vinculación de documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configurar [!DNL Workfront] para enviar metadatos a [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Al enviar un documento desde [!DNL Workfront] hasta [!DNL Workfront DAM], también puede enviar información asociada a ese documento. La información sobre el documento está asignada a [!DNL Workfront DAM] como metadatos.

La información se asigna en una sola dirección, desde [!DNL Workfront] hasta [!DNL Workfront DAM] y solo se transfiere cuando el documento se carga en [!DNL Workfront DAM]. Cualquier cambio futuro en los campos de Workfront no actualizará los campos de metadatos en [!DNL Workfront DAM] después de que el documento ya se haya cargado.\
Puede asignar lo mismo [!DNL Workfront] campo a varios [!DNL Workfront DAM] campos, pero no puede utilizar los mismos [!DNL Workfront DAM] campo para varios [!DNL Workfront] campos.

Si debe configurar varias [!DNL Workfront] campos para exportar a uno [!DNL Workfront DAM] , cree primero un campo personalizado calculado en [!DNL Workfront] para mostrar todos los campos personalizados individuales de un objeto. A continuación, asigne el [!DNL Workfront] Campo a uno [!DNL Workfront DAM] field.\
Para obtener más información sobre los campos personalizados calculados, consulte [Añadir datos calculados a un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

La asignación afecta a todos los documentos cargados por cualquier usuario de [!DNL Workfront] hasta [!UICONTROL Workfront] DAM.

As a [!DNL Workfront] administrador, debe habilitar [!DNL Workfront DAM] en Workfront antes de poder asignar los campos para el proceso de asignación de metadatos.

Para configurar [!DNL Workfront] para enviar metadatos a [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. Clic **[!UICONTROL Documentos]** > **[!UICONTROL Asignación de metadatos]**.

1. En el **[!UICONTROL Seleccionar el campo de origen de la asignación]** , empiece a escribir el nombre del campo de Workfront al que desee asignar [!DNL Workfront DAM]y, a continuación, selecciónelo cuando lo vea en la lista.
1. En el **[!UICONTROL Seleccionar el campo de destino de la asignación]**, seleccione la [!DNL Workfront DAM] que desee rellenar con la información del campo seleccionado [!DNL Workfront] field.

   >[!NOTE]
   >
   > Todos los documentos enviados a [!DNL Workfront DAM] de los usuarios que tengan derechos para hacerlo, actualicen sus metadatos con la variable [!DNL Workfront] campos asignados aquí, cuando se cargan en [!DNL Workfront DAM].

1. Clic **[!UICONTROL Agregar asignación]**.

1. Continuar añadiendo más [!UICONTROL Workfront] campos y correspondientes [!DNL Workfront DAM] campos.

### Eliminar campos asignados

{{step-1-to-setup}}

1. Expandir **[!UICONTROL Documentos]**, luego haga clic en **[!UICONTROL Asignación de metadatos]**.

1. En la lista de campos, seleccione cualquiera de los campos que desee eliminar de la asignación de metadatos.
1. Clic **[!UICONTROL Eliminar]**.

   Los campos se eliminan de la asignación de metadatos y la información que contienen no se transfiere a [!DNL Workfront DAM] con los documentos cargados.
