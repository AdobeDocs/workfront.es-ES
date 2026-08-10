---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Aptitudes disponibles para la instalación directa
description: Workfront ofrece algunas habilidades que puede instalar directamente en su LLM.
author: Becky
feature: Get Started with Workfront
source-git-commit: 20f5a513d8d33ecf8770f35bc73ee799a7de939e
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---


# Aptitudes disponibles para la instalación directa

Workfront ofrece algunas habilidades que puede instalar directamente en su LLM. Las habilidades guían cómo se utilizan esas herramientas para tareas específicas, con los pasos correctos ya integrados.

Puede encontrar estas habilidades en el repositorio de GitHub de Adobe Skills.

>[!NOTE]
>
>Actualmente, estas habilidades solo están disponibles para Claude.
>Para obtener instrucciones sobre cómo configurar Claude con Adobe, consulte [Introducción](https://developer.adobe.com/adobe-for-creativity/getting-started/) en la documentación de Adobe Developer.

## Instale una aptitud del repositorio de GitHub de Workfront en Claude.

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
