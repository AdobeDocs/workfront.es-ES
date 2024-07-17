---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: connections-annd-webhooks
title: Crear conexiones en  [!DNL Adobe Workfront Fusion]
description: Una conexión debe cumplir los requisitos establecidos por la API de la aplicación o del servicio web al que se conecta. Por este motivo, las instrucciones para configurar una conexión varían en función de la aplicación o el servicio web. Este artículo puede ayudarte a identificar y localizar las instrucciones para conectar [!DNL Adobe Workfront Fusion] a la aplicación o servicio web que hayas elegido.
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 1%

---

# Crear conexiones en [!DNL Adobe Workfront Fusion]

<!-- Audited: 3/2024-->

Una conexión debe cumplir los requisitos establecidos por la API de la aplicación o del servicio web al que se conecta. Por este motivo, las instrucciones para configurar una conexión varían en función de la aplicación o el servicio web. Este artículo puede ayudarle a identificar y localizar las instrucciones para conectar a [!DNL Adobe Workfront Fusion] con la aplicación o el servicio web que haya elegido.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>Cualquiera</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td>  
   <td> <p>Nuevo: [!UICONTROL Standard]</p><p>O</p><p>Actual: [!UICONTROL Work] o superior</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td>  
   <td> 
   <p>Actual: no se requiere licencia para [!DNL Workfront Fusion].</p> 
   <p>O</p> 
   <p>Heredado: cualquiera </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Product</td>  
   <td> 
   <p>Nuevo:</p> <ul><li>Plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront]: su organización debe adquirir [!DNL Adobe Workfront Fusion].</li><li>Se incluye el plan [!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion].</li></ul> 
   <p>O</p> 
   <p>Actual: su organización debe comprar [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conectarse a una aplicación o servicio web que no requiera configuración

En la mayoría de los casos, puede utilizar el módulo para crear una conexión con poca o ninguna información adicional. [!DNL Workfront Fusion] administra la autenticación automáticamente.

Para obtener instrucciones sobre cómo crear una conexión sin consideraciones especiales, vea [Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md).

## Conectar con una aplicación o servicio web [!DNL Microsoft]

La mayoría de las [!DNL Microsoft] aplicaciones de [!DNL Workfront Fusion] le permiten crear una conexión sin información adicional.

Las siguientes circunstancias no requieren pasos adicionales para crear una conexión:

* Usando módulos de [!DNL Microsoft Dynamics 365].

  Para obtener instrucciones, consulte [[!DNL Microsoft Dynamics 365] módulos](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* Conectando con [!DNL Microsoft Graph API] mediante un módulo [!UICONTROL HTTP]

  Para obtener instrucciones, consulte [Llamar a [!DNL MS Graph REST API] a través de [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud OAuth 2.0] módulo](../../workfront-fusion/connections/call-the-ms-graph-rest-api.md).

## Conectar con una aplicación o servicio web [!DNL Google]

El proceso de conexión a las aplicaciones de [!DNL Google] puede diferir según el tipo de cuenta de [!DNL Google] que esté usando. Además, las medidas de seguridad de [!DNL Google] pueden requerir una configuración adicional al conectarse a [!DNL Workfront Fusion].

Para obtener más información, consulte:

* [Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] mediante un cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] con medidas de seguridad actualizadas](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## Otras aplicaciones que requieren una configuración adicional

Las siguientes aplicaciones no siguen la configuración básica de [!DNL Workfront Fusion] conexiones. Puede encontrar instrucciones para conectar estas aplicaciones en el artículo para esa aplicación.

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Servicio web/aplicación</th> 
   <th>Información adicional sobre las conexiones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">Conectar [!DNL Adobe Workfront] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">Conectar [!DNL Allocadia] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">Conectar [!DNL Anaplan] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] módulos</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">Conectar [!DNL Azure DevOps] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> en <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] módulos</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">Conectar [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">Conectar [!DNL Datadog] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">Conectar [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Correo electrónico</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">Conecte su correo electrónico a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref"> módulos[!UICONTROL Email]</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">Conectar [!DNL Gmail] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">Conectar [!DNL Jira Cloud] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">Conectar [!DNL Jira Server] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">Conectar [!DNL MariaDB] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">Conectando [!DNL Qualtrics] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">Conectar [!DNL ServiceNow] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref"> módulos[!UICONTROL SFTP]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">Conectar [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">Conectar [!DNL Split.io] a [!DNL Workfront Fusion] </a> en <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ensanchado</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">Conectar [!DNL Widen] a [!DNL Workfront Fusion] </a> en <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] módulos</a></td> 
  </tr> 
 </tbody> 
</table>
