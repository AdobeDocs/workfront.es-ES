---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Buscar  [!DNL Adobe Workfront] elementos de [!DNL Slack]
description: Puede buscar elementos de  [!DNL Adobe Workfront]  desde  [!DNL Slack], if your instance of Slack has had the [!DNL Workfront]  aplicación instalada.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
TQID: https://experienceleague.adobe.com/JulYq173XQa6mG93qzUwfBDn4TPVEafD2OVpcIAXxi8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 209
ht-degree: 100%

---

# Buscar elementos de [!DNL Adobe Workfront] desde [!DNL Slack]

Puede buscar elementos de [!DNL Adobe Workfront] desde [!DNL Slack], si su instancia de [!DNL Slack] tiene instalada la aplicación [!DNL Workfront].

Para obtener más información sobre la configuración de [!DNL Workfront] con [!DNL Slack], consulte [Configurar [!DNL Adobe Workfront] para [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Cualquiera</p>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para poder buscar elementos de [!DNL Workfront] desde [!DNL Slack], debe

* Configurar [!DNL Workfront] para [!DNL Slack]\
   Para obtener instrucciones sobre cómo configurar [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Buscar elementos de [!DNL Workfront] desde [!DNL Slack]:

1. Inicie sesión en la instancia de [!DNL Slack] e inicie sesión en [!DNL Workfront] desde [!DNL Slack].\
   Para obtener más información sobre el inicio de sesión en [!DNL Workfront] desde [!DNL Slack], consulte la sección “Inicio de sesión en [!DNL Workfront] desde [!DNL Slack]” en [Acceder a [!DNL Adobe Workfront] desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Desde cualquier canal, empiece a escribir cualquiera de los siguientes comandos en el campo de mensaje:

   `/workfront search <keyword>`

   O

   `/wf search <keyword>`

   >[!NOTE]
   >
   >Los comandos distinguen entre mayúsculas y minúsculas. La palabra clave no distingue entre mayúsculas y minúsculas y debe escribirse sin corchetes ni comillas.

1. En el campo que aparece, seleccione un tipo de objeto entre los siguientes:

   * Proyecto
   * Tarea
   * Problema
   * Informe
   * Personas
   * Plantilla
   * Documento
   * Portafolio
   * Programa
   * Panel de control
   * Compañía
   * Nota

     Solo se puede seleccionar un tipo de objeto a la vez.\
      Se muestra una lista de elementos que coinciden con los criterios de búsqueda.

1. Haga clic en el nombre de un elemento para abrirlo en [!DNL Workfront] en una nueva pestaña del explorador.
