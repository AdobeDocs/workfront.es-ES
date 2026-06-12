---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Información general del servidor MCP de Adobe Workfront
description: Descubra qué hace el servidor MCP de Adobe Workfront y cómo le permite trabajar con Workfront a través de una conversación en lenguaje natural en una plataforma independiente de IA.
author: Courtney
feature: Get Started with Workfront
source-git-commit: b63c45eaf380137f2ebfc5cb99e503085f878389
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# Información general del servidor MCP de Adobe Workfront

El servidor MCP de [!DNL Adobe Workfront] conecta su instancia de Workfront con una plataforma independiente de IA, como [!DNL Claude] o [!DNL ChatGPT]. Desde la plataforma agéntica de IA, puede encontrar, crear, actualizar y administrar elementos de Workfront realizando solicitudes en lenguaje natural.

Por ejemplo, puede preguntar:

* *Mostrarme todos los proyectos activos del equipo de marketing de marca.*
* *Actualice la tarea &quot;Revisión de diseño&quot; para que finalice el 18 de abril.*
* *Envíe un recordatorio a los aprobadores del recurso &quot;Vídeo de campaña de primavera&quot; que no hayan respondido.*

No necesita saber la API de Workfront ni cómo funcionan los servidores MCP para utilizar el servidor MCP de Workfront.

>[!IMPORTANT]
>
>Actualmente, el servidor MCP de Workfront solo está disponible para clientes de la región de EE. UU. que utilizan AWS.

## Qué es un servidor MCP

Un servidor MCP es un punto de conexión que permite que una plataforma auténtica de IA funcione con otro sistema. El servidor MCP de Workfront es a lo que se conecta su plataforma agéntica de IA para que pueda leer y actuar en sus datos de Workfront en su nombre.

MCP significa Protocolo de contexto de modelo. Este es el estándar que define cómo las plataformas agénticas de IA y los sistemas externos se comunican entre sí.

## Configuración de la conexión

El servidor MCP de Workfront funciona con cualquier plataforma independiente de IA compatible con MCP, como [!DNL Claude] o [!DNL ChatGPT]. Antes de poder usarlo, debe ocurrir lo siguiente:

* Un administrador de Workfront debe habilitar el acceso al servidor MCP en la instancia de Workfront.
* Usted (o su administrador) debe conectar su plataforma agéntica de IA a Workfront.

Para obtener más información, consulte [Configuración del servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

## Empezar a utilizar el servidor MCP de Workfront

Después de la configuración, puede pedir a su plataforma agéntica de IA que busque, cree, actualice y administre elementos de Workfront en lenguaje natural.

Para obtener más información, incluidas solicitudes de ejemplo, aspectos que se deben tener en cuenta e información sobre datos y seguridad, vea [Usar el servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).
