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
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 1%

---

# Configurar integraciones de documentos

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como administrador de [!DNL Adobe Workfront], puede configurar integraciones de documentos para administrar documentos en [!UICONTROL Workfront]. También puede configurar [!UICONTROL Workfront] para que los documentos se almacenen únicamente en aplicaciones de servicios de documentos y no en el propio [!UICONTROL Workfront]. Para obtener más información, consulte [Actualizar y vincular un documento de [!UICONTROL Workfront] a un proveedor de nube externo](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) en [Vincular documentos de aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Para permitir la comunicación abierta entre [!DNL Workfront Proof] y los servidores [!DNL Workfront], es posible que tenga que agregar ciertas direcciones IP a la lista de permitidos. Para obtener más información, consulte [Configuración de la lista de permitidos del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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

  Vincular pruebas de [!DNL Workfront Proof] le permite hacer que las pruebas creadas originalmente en [!DNL Workfront Proof] estén disponibles en [!DNL Workfront]. Para los planes actuales, se requiere un plan [!UICONTROL Pro] [!DNL Workfront] o superior para usar esta característica. Para los nuevos planes, esta función está disponible con todos los planes. Para obtener más información sobre los diversos planes disponibles, consulte [Planes de Workfront](https://www.workfront.com/plans).

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

     <!--Quip-->

  >[!TIP]
  >
  >Puede revisar y aprobar documentos enlazados desde un proveedor de nube externo de la misma manera que revisa y aprueba documentos cargados directamente en [!DNL Workfront].

* Otros proveedores de documentos (mediante integraciones de documentos personalizadas).

  Para los planes actuales, se requiere un plan [!UICONTROL Pro] [!DNL Workfront] o superior para usar esta característica. Para los nuevos planes, esta función está disponible con todos los planes. Para obtener más información sobre los diversos planes disponibles, consulte [Planes de Workfront](https://www.workfront.com/plans).

Además, puede mejorar su experiencia con los documentos de [!DNL Workfront] con un sistema nativo de administración de activos digitales (DAM) o con integraciones DAM de terceros. Los administradores deben habilitar estas características para que los usuarios puedan vincular el servicio a su cuenta de [!DNL Workfront]. Para obtener más información acerca de Workfront DAM, vea [Administrar documentos con [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Configurar integraciones para administrar documentos

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Proveedores de nube].**

1. (Opcional) Para almacenar documentos en una aplicación de servicios de documentos y no en [!DNL Workfront], seleccione **[!UICONTROL Impedir que los usuarios almacenen documentos en [!DNL Workfront]].**

1. Seleccione las integraciones que desee activar.
1. Haga clic en **[!UICONTROL Guardar]**.

Si está configurando integraciones con [!DNL Workfront DAM], puede permitir que [!DNL Workfront] incluya metadatos con los documentos. Para obtener información acerca de la asignación de metadatos, vea [Configurar la asignación de metadatos](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configurar integraciones de documentos personalizadas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Una integración de documentos personalizada permite a los usuarios de [!DNL Workfront] vincular archivos a [!DNL Workfront] prácticamente desde cualquier sistema, siempre que el sistema funcione con [!DNL Workfront].

Para que la integración personalizada esté disponible para los usuarios de, primero debe crear la integración de. Para obtener información acerca de cómo generar integraciones para usarlas con [!DNL Workfront], consulte [API de Document Webhooks](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Una vez creada la integración de documentos personalizada, puede ponerla a disposición de los usuarios de su sitio.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Integración personalizada]**.

1. Haga clic en **[!UICONTROL Agregar integración personalizada]**.
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

1. (Condicional) Si seleccionó la autenticación **[!UICONTROL OAuth]** para el **[!UICONTROL Tipo de autenticación]**, escriba la siguiente información:

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
   >El URI de redireccionamiento [!DNL Workfront] que aparece en la parte inferior de la página [!UICONTROL Integración personalizada] enumera el URI usado para registrar esta integración con el proveedor de documentos externo.

1. (Condicional) Si seleccionó la autenticación **[!UICONTROL ApiKey]** para el **[!UICONTROL Tipo de autenticación]**, escriba la clave de API que emitió el proveedor de documentos personalizados.

   [!DNL Workfront] utiliza esta clave de API para realizar llamadas de API autorizadas al proveedor de documentos.

1. Haga clic en **[!UICONTROL Guardar]** para crear la integración.

## Uso de integraciones de documentos

Para obtener información acerca de cómo los usuarios pueden usar [!DNL Workfront DAM], vea [Administrar documentos con [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

Para obtener información acerca de cómo los usuarios pueden utilizar la revisión, vea [Crear revisiones](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

Para obtener información sobre cómo los usuarios pueden usar integraciones de documentos de terceros después de configurarlas, consulte [Enlazar documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configurar [!DNL Workfront] para enviar metadatos a [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Al enviar un documento de [!DNL Workfront] a [!DNL Workfront DAM], también puede enviar información asociada con ese documento. La información sobre el documento se ha asignado a [!DNL Workfront DAM] como metadatos.

La información se asigna en una sola dirección, de [!DNL Workfront] a [!DNL Workfront DAM] y se transfiere solamente cuando el documento se carga a [!DNL Workfront DAM]. Cualquier cambio futuro en los campos de Workfront no actualizará los campos de metadatos en [!DNL Workfront DAM] después de que ya se haya cargado el documento.\
Puede asignar el mismo campo [!DNL Workfront] a varios campos [!DNL Workfront DAM], pero no puede usar el mismo campo [!DNL Workfront DAM] para varios campos [!DNL Workfront].

Si debe configurar varios campos [!DNL Workfront] para exportarlos a un campo [!DNL Workfront DAM], cree primero un campo personalizado calculado en [!DNL Workfront] para mostrar todos los campos personalizados individuales de un objeto. A continuación, asigne el campo [!DNL Workfront] calculado a un campo [!DNL Workfront DAM].\
Para obtener más información sobre los campos personalizados calculados, vea [Agregar campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

La asignación afecta a todos los documentos cargados por cualquier usuario de [!DNL Workfront] a [!UICONTROL Workfront] DAM.

Como administrador de [!DNL Workfront], debe habilitar [!DNL Workfront DAM] en Workfront para poder asignar los campos para el proceso de asignación de metadatos.

Para configurar [!DNL Workfront] para enviar metadatos a [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Asignación de metadatos]**.

1. En el campo **[!UICONTROL Seleccionar campo de Source para asignación]**, empiece a escribir el nombre del campo de Workfront que desea asignar a [!DNL Workfront DAM] y, a continuación, selecciónelo cuando lo vea en la lista.
1. En **[!UICONTROL Seleccionar campo de destino para asignación]**, seleccione el campo [!DNL Workfront DAM] que desee rellenar con la información del campo [!DNL Workfront] seleccionado.

   >[!NOTE]
   >
   > Todos los documentos enviados a [!DNL Workfront DAM] por usuarios que tienen derechos para hacerlo tienen sus metadatos actualizados con los campos de [!DNL Workfront] asignados aquí, cuando se cargan en [!DNL Workfront DAM].

1. Haga clic en **[!UICONTROL Agregar asignación]**.

1. Continúe agregando más [!UICONTROL campos de Workfront] y los [!DNL Workfront DAM] campos correspondientes.

### Eliminar campos asignados

{{step-1-to-setup}}

1. Expanda **[!UICONTROL Documentos]** y, a continuación, haga clic en **[!UICONTROL Asignación de metadatos]**.

1. En la lista de campos, seleccione cualquiera de los campos que desee eliminar de la asignación de metadatos.
1. Haga clic en **[!UICONTROL Eliminar]**.

   Los campos se quitan de la asignación de metadatos y la información que contienen no se transfiere a [!DNL Workfront DAM] con los documentos cargados.
