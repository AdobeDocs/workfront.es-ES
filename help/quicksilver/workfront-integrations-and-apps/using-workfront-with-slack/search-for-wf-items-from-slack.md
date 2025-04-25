---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Buscar  [!DNL Adobe Workfront] elementos de [!DNL Slack]
description: Puede buscar elementos de  [!DNL Adobe Workfront]  desde  [!DNL Slack], if your instance of Slack has had the [!DNL Workfront]  aplicación instalada.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 99%

---

# Buscar elementos de [!DNL Adobe Workfront] desde [!DNL Slack]

Puede buscar elementos de [!DNL Adobe Workfront] desde [!DNL Slack], si su instancia de [!DNL Slack] tiene instalada la aplicación [!DNL Workfront].

Para obtener más información sobre la configuración de [!DNL Workfront] con [!DNL Slack], consulte [Configurar [!DNL Adobe Workfront] para [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].\

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
