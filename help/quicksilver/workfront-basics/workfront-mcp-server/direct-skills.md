---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Aptitudes disponibles para la instalación directa
description: Workfront ofrece algunas habilidades que puede instalar directamente en su LLM.
author: Becky
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
source-git-commit: 7fd4c07f2ea1e47e7abb7d3dd78638a6a01d0f47
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Aptitudes disponibles para la instalación directa

Adobe Workfront ofrece algunas habilidades que puede instalar directamente en su LLM. Las habilidades guían cómo se utilizan esas herramientas para tareas específicas, con los pasos correctos ya integrados.

Puede encontrar estas habilidades como archivos en el repositorio de GitHub de Adobe Skills. Este repositorio contiene archivos para una variedad de productos de Adobe. Al descargar estos archivos y copiarlos en Claude, Claude puede utilizar las habilidades descritas en los archivos.

Por ejemplo, las habilidades de arquitecto de soluciones de Planning permiten a Claude responder preguntas sobre Workfront Planning y realizar algunas acciones en él.

No es necesario que llame a estas aptitudes ni las almacene en déclencheur después de copiarlas en la LLM. En su lugar, puede interactuar con su LLM como de costumbre, haciendo preguntas en lenguaje natural, y el LLM utiliza la información y las acciones descritas en la habilidad que son apropiadas para la conversación.

>[!NOTE]
>
>Actualmente, estas habilidades solo están disponibles para Claude.
>Para obtener instrucciones sobre cómo configurar Claude con Adobe, consulte [Introducción](https://developer.adobe.com/adobe-for-creativity/getting-started/) en la documentación de Adobe Developer.

## Instalar una aptitud del repositorio de GitHub de Workfront en Claude

1. Vaya al [repositorio de habilidades de Adobe Workfront](https://github.com/adobe/skills/tree/main/plugins/workfront) en GitHub.
1. Descargue la carpeta de aptitudes que desee utilizar.
1. Copie la carpeta en la biblioteca de aptitudes de Claude.

   * Claude Desktop: `~/Library/Application Support/Claude/skills/` (macOS) o equivalente.
   * Código de Claude: `~/.claude/skills/`.

<!--

1. Go to the [Adobe Workfront skills repository](https://github.com/adobe/skills/tree/main/plugins/workfront) on GitHub.
1. Download the skill file you want to use.
1. In Claude, click **Customize**.
1. Select **Skills**.
1. Click **Create skill** -> **Upload a skill**.
1. Upload the zipped skill file to Claude, then click **Confirm** to install.

-->

## Aptitudes disponibles actualmente

| Aptitud/vínculo a la carpeta | Descripción de aptitud | Disponible para |
|---|---|---|
| [Arquitecto de soluciones de Planning](https://github.com/adobe/skills/tree/main/plugins/workfront/skills/wf-planning-solution-architect) | Configure un espacio de trabajo de Workfront Planning para satisfacer sus necesidades y responder preguntas sobre Workfront Planning. | Claude |
