---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: connections-annd-webhooks
title: Crear conexiones en [!DNL Adobe Workfront Fusion]
description: Una conexión debe cumplir los requisitos establecidos por la API de la aplicación o el servicio web al que se conecta. Por este motivo, las instrucciones para configurar una conexión varían según la aplicación o el servicio web. Este artículo puede ayudarle a identificar y localizar las instrucciones de conexión [!DNL Adobe Workfront Fusion] a la aplicación o servicio web que haya elegido.
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# Crear conexiones en [!DNL Adobe Workfront Fusion]

Una conexión debe cumplir los requisitos establecidos por la API de la aplicación o el servicio web al que se conecta. Por este motivo, las instrucciones para configurar una conexión varían según la aplicación o el servicio web. Este artículo puede ayudarle a identificar y localizar las instrucciones de conexión [!DNL Adobe Workfront Fusion] a la aplicación o servicio web que haya elegido.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td>

</tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connect [!DNL Adobe Workfront] a [!DNL Workfront Fusion]

Workfront y [!DNL Workfront Fusion] están diseñadas para trabajar juntos. La conexión que cree determinará la cuenta que [!DNL Workfront Fusion] utiliza para realizar acciones en Workfront.

Para obtener instrucciones, consulte [Connect [!DNL Workfront] a [!DNL Workfront Fusion]](../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect) in [[!DNL Adobe Workfront] módulos](../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

## Conectarse a una aplicación o servicio web que no requiera configuración

En la mayoría de los casos, puede utilizar el módulo para crear una conexión con poca o ninguna información adicional. [!DNL Workfront Fusion] gestiona la autenticación automáticamente.

Para obtener instrucciones sobre la creación de una conexión sin consideraciones especiales, consulte [Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md).

## Conectarse a un [!DNL Microsoft] aplicación o servicio web

La mayoría de los [!DNL Microsoft] aplicaciones en [!DNL Workfront Fusion] permite crear una conexión sin información adicional.

Las siguientes circunstancias requieren pasos adicionales para crear una conexión:

* Uso [!DNL Microsoft Dynamics 365] módulos.

   Para obtener instrucciones, consulte [[!DNL Microsoft Dynamics 365] módulos](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* Conexión a [!DNL Microsoft Graph API] usando un [!UICONTROL HTTP] módulo

   Para obtener instrucciones, consulte [Llame a la función [!DNL MS Graph REST API] a través de la variable [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud de OAuth 2.0] módulo](../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## Conectarse a un [!DNL Google] aplicación o servicio web

Proceso para conectarse a [!DNL Google] las aplicaciones pueden variar en función del tipo de [!DNL Google] cuenta que está utilizando. Además, [!DNL Google] las medidas de seguridad pueden requerir una configuración adicional al conectarse a [!DNL Workfront Fusion].

Para obtener más información, consulte:

* [Connect [!DNL Adobe Workfront Fusion] a [!DNL Google Services] uso de un cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [Connect [!DNL Adobe Workfront Fusion] a [!DNL Google Services] con medidas de seguridad actualizadas](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## Otras aplicaciones que requieren configuración adicional

Las siguientes aplicaciones no siguen la configuración básica de [!DNL Workfront Fusion] conexiones. Puede encontrar instrucciones para conectar estas aplicaciones en el artículo correspondiente a esa aplicación.

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Aplicación/Servicio web</th> 
   <th>Información adicional sobre conexiones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">Connect [!DNL Adobe Workfront] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">Connect [!DNL Allocadia] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">Connect [!DNL Anaplan] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] módulos</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">Connect [!DNL AWS] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">Connect [!DNL Azure DevOps] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">Connect [!DNL Bynder] a [!DNL Workfront Fusion] </a> en <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">Connect [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] módulos</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">Connect [!DNL Cvent] a [!DNL Adobe Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">Connect [!DNL Datadog] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">Connect [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Correo electrónico</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">Conecte el correo electrónico a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">Módulos de [!UICONTROL Email]</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">Connect [!DNL Gmail] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Intacct]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/intacct-modules.md#connecti" class="MCXref xref">Connect [!DNL Intacct] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/intacct-modules.md" class="MCXref xref">[!DNL Intacct] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">Connect [!DNL Jira Cloud] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">Connect [!DNL Jira Server] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">Connect [!DNL MariaDB] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">Conexión [!DNL Qualtrics] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">Connect [!DNL ServiceNow] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">Conectar SFTP a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">Módulos [!UICONTROL SFTP]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">Connect [!DNL SharePoint] a [!DNL Workfront Fusion]</a> en <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">Connect [!DNL Split.io] a [!DNL Workfront Fusion] </a> en <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] módulos</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ensanchado</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">Connect [!DNL Widen] a [!DNL Workfront Fusion] </a> en <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] módulos</a></td> 
  </tr> 
 </tbody> 
</table>
