---
title: Configurar integraciones de documentos
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Configurar integraciones de documentos
author: Courtney, Caroline
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 1%

---

# Configurar integraciones de documentos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como [!DNL Adobe Workfront] administrador, puede configurar integraciones de documentos para administrar documentos en [!UICONTROL Workfront]. También puede configurar [!UICONTROL Workfront] para que los documentos se almacenen únicamente en aplicaciones de servicios de documentos y no en [!UICONTROL Workfront] en sí. Para obtener más información, consulte [Actualizar y vincular un documento desde [!UICONTROL Workfront] a un proveedor de nube externo](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) en [Vincular documentos de aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Para permitir una comunicación abierta entre [!DNL Workfront Proof] y [!DNL Workfront] , es posible que tenga que agregar ciertas direcciones IP a la lista de permitidos. Para obtener más información, consulte [Configurar la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Integraciones compatibles

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Puede configurar las siguientes integraciones para administrar documentos:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

   Vinculación de pruebas desde [!DNL Workfront Proof] permite realizar pruebas que se crearon originalmente en [!DNL Workfront Proof] disponible dentro de [!DNL Workfront]. A [!UICONTROL Pro] [!DNL Workfront] Se requiere un plan o superior para utilizar esta función. Para obtener más información sobre los distintos planes disponibles, consulte [Planes de Workfront.](https://www.workfront.com/plans)

* [!DNL Microsoft SharePoint]

   Para obtener información sobre la integración con [!DNL SharePoint], consulte [Configure las variables [!DNL SharePoint] integración](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Proveedores de documentos de nube de terceros:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!UICONTROL Google Drive]

      <!--Quip-->
   >[!TIP]
   >
   >Puede probar y aprobar documentos vinculados desde un proveedor de nube externo del mismo modo que realiza la prueba y la aprobación de documentos cargados directamente en [!DNL Workfront].

* Otros proveedores de documentos (a través de integraciones de documentos personalizadas).

   A [!UICONTROL Pro] [!DNL Workfront] Se requiere un plan o superior para utilizar esta función. Para obtener más información sobre los distintos planes disponibles, consulte [[!DNL Workfront] Planes.](https://www.workfront.com/plans)

Además, puede mejorar su [!DNL Workfront] documentar la experiencia con un sistema nativo de administración de recursos digitales (DAM) o con integraciones DAM de terceros. Los administradores deben habilitar estas funciones para que los usuarios puedan vincular el servicio a sus [!DNL Workfront] cuenta. Para obtener más información sobre Workfront DAM, consulte [Administración de documentos con [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Configuración de integraciones para administrar documentos

1. Iniciar sesión en [!DNL Workfront] como administrador.
1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Proveedores de nube].**

1. (Opcional) Para almacenar documentos en una aplicación de servicios de documentos y no en [!DNL Workfront], seleccione **[!UICONTROL Impedir que los usuarios almacenen documentos en [!DNL Workfront]].**

1. Seleccione las integraciones que desee habilitar.
1. Haga clic en **[!UICONTROL Guardar]**.

Si está configurando integraciones con [!DNL Workfront DAM], puede activar [!DNL Workfront] para incluir metadatos con documentos. Para obtener información sobre la asignación de metadatos, consulte [Configuración de la asignación de metadatos](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configurar integraciones de documentos personalizadas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Una integración de documento personalizada permite [!DNL Workfront] usuarios para vincular archivos a [!DNL Workfront] de prácticamente cualquier sistema, siempre que el sistema esté diseñado para funcionar con [!DNL Workfront].

Para que la integración personalizada esté disponible para los usuarios, primero debe crear la integración. Para obtener información sobre cómo crear integraciones para utilizar con [!DNL Workfront], consulte [API de Document Webhooks](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Una vez creada la integración de documentos personalizada, puede ponerla a disposición de los usuarios del sitio.

1. Iniciar sesión en [!DNL Workfront] como administrador.
1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Integración personalizada].**

1. Haga clic en **[!UICONTROL Añadir integración personalizada]**.
1. Especifique la siguiente información para configurar la integración:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Nombre de la integración personalizada. Este es el nombre que ven los usuarios al utilizar la integración en Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Base API URL] </td> 
      <td>URL HTTP base o segura para llamadas API. Por ejemplo, <a class="link-https" title="https://documentprovider.com/api/v2" href="https://documentprovider.com/api/v2">https://documentprovider.com/api/v2</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de autenticación]</td> 
      <td> <p>Método de autenticación que se utiliza al realizar llamadas de API autorizadas a la integración personalizada.</p> 
       <ul> 
        <li>Si elige <strong>[!UICONTROL OAuth]</strong>, continúe con el paso 6.</li> 
        <li>Si elige <strong>[!UICONTROL ApiKey]</strong>, continúe con el paso 7.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Si ha seleccionado **[!UICONTROL OAuth]** autenticación para **[!UICONTROL Tipo de autenticación]**, especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL de autenticación]</td> 
      <td>La dirección URL completa utilizada para la autenticación de usuarios. [!DNL Workfront] navega a los usuarios a esta dirección como parte del proceso de aprovisionamiento de OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Endpoint URL]</td> 
      <td>Dirección de URL de API completa que sirve para recuperar tokens de OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>El ID de cliente OAut para esta integración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Secreto del cliente OAut para esta integración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parámetros de solicitud]</td> 
      <td> <p>Especifique valores opcionales para anexarlos a la cadena de consulta de cada llamada a la API. Por ejemplo, access_type=offline.</p> <p>Para añadir varios parámetros de solicitud, haga clic en <strong>+Agregar parámetro de solicitud</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >La variable [!DNL Workfront] URI de redireccionamiento que aparece en la parte inferior del [!UICONTROL Integración personalizada] lista el URI utilizado para registrar esta integración con el proveedor de documentos externo.

1. (Condicional) Si ha seleccionado **[!UICONTROL ApiKey]** autenticación para **[!UICONTROL Tipo de autenticación]**, especifique la clave de API que emitió el proveedor de documentos personalizado.

   [!DNL Workfront] utiliza esta clave de API para realizar llamadas de API autorizadas al proveedor de documentos.

1. Haga clic en **[!UICONTROL Guardar]** para crear la integración.

## Usar integraciones de documentos

Para obtener información sobre cómo pueden usar los usuarios [!DNL Workfront DAM], consulte [Administración de documentos con [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

Para obtener información sobre cómo pueden utilizar las pruebas los usuarios, consulte [Crear pruebas](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).

Para obtener información sobre cómo los usuarios pueden utilizar integraciones de documentos de terceros después de configurarlas, consulte [Vincular documentos de aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configurar [!DNL Workfront] para enviar metadatos a [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Al enviar un documento desde [!DNL Workfront] a [!DNL Workfront DAM], también puede enviar información asociada a ese documento. La información sobre el documento está asignada a [!DNL Workfront DAM] como metadatos.

La información solo se asigna de forma unidireccional, desde [!DNL Workfront] a [!DNL Workfront DAM] y se transfiere únicamente cuando el documento se carga en [!DNL Workfront DAM]. Los cambios futuros en los campos de Workfront no actualizarán los campos de metadatos en [!DNL Workfront DAM] después de cargar el documento.\
Puede asignar lo mismo [!DNL Workfront] campo a varios [!DNL Workfront DAM] campos, pero no puede utilizar el mismo [!DNL Workfront DAM] campo para varios [!DNL Workfront] campos.

Si debe configurar varias [!DNL Workfront] campos para exportar a uno [!DNL Workfront DAM] , cree primero un campo personalizado calculado en [!DNL Workfront] para mostrar todos los campos personalizados individuales de un objeto. A continuación, asigne el valor calculado [!DNL Workfront] campo a uno [!DNL Workfront DAM] campo .\
Para obtener más información sobre los campos personalizados calculados, consulte [Agregar datos calculados a un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

La asignación afecta a todos los documentos cargados por cualquier usuario desde [!DNL Workfront] a [!UICONTROL Workfront] DAM.

Como [!DNL Workfront] administrador, debe activar [!DNL Workfront DAM] en Workfront para poder asignar los campos del proceso de asignación de metadatos. Para obtener más información sobre cómo habilitar [!DNL Workfront DAM], consulte [Configuración de Workfront para enviar metadatos a [!DNL Workfront DAM]](#configure-workfront-to-send-metadata-to-workfront-dam).

Para configurar [!DNL Workfront] para enviar metadatos a [!DNL Workfront DAM]:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Asignación de metadatos]**.

1. En el **[!UICONTROL Seleccionar campo de origen para asignación]** , empiece a escribir el nombre del campo de Workfront al que desea asignar [!DNL Workfront DAM]y, a continuación, selecciónela cuando la vea en la lista.
1. En el **[!UICONTROL Seleccionar campo de destino para asignación]**, seleccione [!DNL Workfront DAM] campo que desea rellenar con la información del [!DNL Workfront] campo .

   >[!NOTE]
   >
   > Todos los documentos enviados a [!DNL Workfront DAM] los usuarios que tengan derechos para hacerlo tendrán sus metadatos actualizados con la variable [!DNL Workfront] campos asignados aquí, cuando se cargan a [!DNL Workfront DAM].

1. Haga clic en **[!UICONTROL Agregar asignación]**.

1. Continuar agregando más [!UICONTROL Workfront] campos y correspondientes [!DNL Workfront DAM] campos.

### Eliminar campos asignados

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Expandir **[!UICONTROL Documentos]** y haga clic en **[!UICONTROL Asignación de metadatos]**.

1. En la lista de campos, seleccione cualquiera de los campos que desee eliminar de la asignación de metadatos.
1. Haga clic en **[!UICONTROL Eliminar]**.

   Los campos se eliminan de la asignación de metadatos y la información que contienen no se transfiere a [!DNL Workfront DAM] con los documentos cargados.
