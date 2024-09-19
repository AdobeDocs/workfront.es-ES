---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Uso de archivos grandes en Adobe Workfront Fusion
description: Actualmente, se admite archivos grandes para los conectores Workfront y HTTP.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: d380f495c098e45897ca58627571dfc7dfdcb0f7
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 0%

---

# Uso de archivos grandes en Adobe Workfront Fusion

Actualmente, se admite archivos grandes para los conectores Workfront y HTTP.

## Efecto del tamaño de archivo grande en el tiempo de ejecución del escenario

Los archivos grandes pueden tardar algún tiempo en cargarse, descargarse o procesarse en su escenario de Fusion. Aunque no hay límite en el tamaño del archivo, hay un límite de 40 minutos en el tiempo de ejecución del escenario. Por lo tanto, si los archivos grandes hacen que la ejecución tarde más de 40 minutos, el escenario falla.

El tiempo de ejecución de un escenario también puede verse afectado por el tamaño del escenario, la complejidad del módulo y la velocidad de la red. Por lo tanto, le recomendamos que tenga en cuenta estos aspectos de los escenarios al utilizar archivos grandes.


<!--
## Connectors that do not support large files

Some Fusion connectors do not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

The following connectors do **not** support large files. 

* Archive
* Box
* Convert
* CSV
* Datastores
* Flow control
* FTP
* JSON
* JWT
* Markdown
* Math
* Microsoft Word templates
* MIME
* Microsoft SQL
* SFTP
* Adobe Acrobat Sign
* SOAP
* Tools
* XML

If a connector is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.-->






<!--## Connectors that support large files

The following connectors support large files.

Workfront
HTTP
Webhooks
Salesforce
Microsoft Email
Workfront Proof
AEM Assets
Email
Slack
Jira
Microsoft Excel
SharePoint
Frame.io
Adobe PDF Services
Marketo
Azure Devops 
Google Email
Jira Server
Google Sheets
Microsoft OneDrive
ServiceNow 
AWS S3
Bynder
OneDrive Business
Adobe Authenticator
Google Drive
Microsoft Dynamics
Google Docs
NetSuite
Airtable
Azure AD
QuickBase 
Adobe Target
Adobe Campaign Classic
Microsoft Calendar
Workfront Planning
HubSpot CRM  
DropBox
Cloud Convert
Egnyte
Adobe Firefly
OpenAI / Chat GPT
Allocadia
Cvent
GitLab 
Google Team Drive
Google Calendar
Workfront SDL Managed Translation
Widen
Workfront Boards
Google Slides
Qualtrics
Microsoft Power BI
Adobe Photoshop
Anaplan
DocuSign 
MariaDB
Adobe Creative Cloud Libraries
Figma
AEM Forms
Datadog
GitHub 
Google Forms
Adobe I/O Events
Trello
Workday
Adobe Journey Optimizer
Adobe Lightroom









If a file is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

-->