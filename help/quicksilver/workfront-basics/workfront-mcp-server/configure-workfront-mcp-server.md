---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configuración del servidor MCP de Adobe Workfront
description: Configure su instancia de Workfront y su plataforma agéntica de IA para poder trabajar con Workfront a través de una conversación en lenguaje natural.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 98d5b93bcb99c468de2ad107a2aca3a9a1995429
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 0%

---


# Configuración del servidor MCP de Adobe Workfront

El servidor MCP [!DNL Adobe Workfront] le permite trabajar con sus datos de Workfront a través de una conversación en lenguaje natural en una plataforma independiente de IA compatible como Claude o ChatGPT.

Para poder conectar una plataforma independiente de IA a Workfront, un administrador de Workfront debe habilitar el acceso al servidor MCP en la instancia de Workfront. Los pasos exactos para conectar una plataforma agéntica de IA son diferentes para cada plataforma agéntica de IA admitida.

Para obtener más información sobre el servidor MCP de Workfront, consulte [Descripción general del servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Plataformas agénticas de IA compatibles

Actualmente, el servidor MCP de Workfront admite las siguientes plataformas agénticas de IA:

* [!DNL Claude]
* [!DNL ChatGPT]

## Requisitos previos

Para poder conectar Workfront a una plataforma independiente de IA, debe:

* Tener una cuenta activa de [!DNL Adobe Workfront] con permiso para tener acceso a los datos con los que desea trabajar.
* Tener acceso a una plataforma agéntica de IA como [!DNL Claude].

### Requisitos previos de administración

El acceso al servidor MCP está cerrado por dos administradores independientes.

* **Su administrador de Workfront** controla el acceso al servidor MCP para su instancia de Workfront. El acceso está habilitado de forma predeterminada en Preferencias del sistema, por lo que no se requiere ninguna acción a menos que el administrador haya elegido deshabilitarlo. <!-- TODO: link to the System Preferences AI preferences article once the Enable MCP toggle is documented there. -->

* Si utiliza una versión empresarial de una plataforma agéntica de IA, su administrador de dicha plataforma debe habilitar el conector [!DNL Adobe Workfront] para su organización.


## Conectar Workfront a Claude

Se conecta a Workfront una vez por cuenta de [!DNL Claude]. La conexión le autentica en una instancia de Workfront específica y permanecerá conectado hasta que decida desconectarse.

### Conectar desde el directorio de conectores

+++ Amplíe para ver instrucciones paso a paso para conectar Workfront a [!DNL Claude].

Para conectar Workfront a [!DNL Claude]:

1. Abra [!DNL Claude].

1. Vaya al área de conectores.

   <!-- NEEDS DETAIL: Exact menu path (for example, "Click Settings, then click Connectors"). -->

1. Busque **[!DNL Adobe Workfront]** en la lista de conectores.

   Si no lo ve, vea [Requisitos previos de administración](#admin-prerequisites) en este artículo.

1. Haga clic en **Conectar**.

   <!-- NEEDS DETAIL: Confirm the exact button label. -->

1. Cuando se le solicite, inicie sesión en la instancia de Workfront.

   <!-- NEEDS DETAIL: Describe the auth flow — does it open a new browser tab, an in-app window, prompt for a Workfront domain? -->

1. Una vez finalizada la autenticación, estará conectado.

   <!-- NEEDS DETAIL: Add a screenshot of the connected state in Claude. -->

+++

### Conexión con una dirección URL

+++ Amplíe para ver instrucciones paso a paso para conectar Workfront a [!DNL Claude] con una dirección URL.

Para conectar Workfront a [!DNL Claude] con una dirección URL:

1. Inicie sesión en [Claude](https://claude.ai) con sus credenciales.
1. En el menú de la izquierda, seleccione el icono **Personalizar**.
1. Seleccione **Conectores** y, a continuación, seleccione el icono **+** para agregar un conector.
1. Seleccione el botón **Crear aplicación**.
1. Asigne al conector un nombre deseado (como &quot;Workfront&quot;) e introduzca la URL del servidor MCP deseada: `https://mcp.workfront.adobe.com/mcp/v1/workfront`

1. Una vez creado el conector, aparece una ventana de inicio de sesión. Autentique con sus credenciales de Adobe ID. Asegúrese de seleccionar la instancia de Workfront que desee si pertenece a más de una.

+++

### Personalizar el comportamiento de Claude con habilidades

[!DNL Claude] admite conjuntos de instrucciones creados por el usuario llamados aptitudes. Puede utilizar una habilidad para personalizar el comportamiento de [!DNL Claude] con Workfront. Por ejemplo, puede crear una aptitud que indique a [!DNL Claude] que siempre recupere datos nuevos de Workfront en lugar de depender de resultados anteriores.

Para obtener más información acerca de las habilidades de [!DNL Claude], consulte la [documentación del usuario Claude](https://code.claude.com/docs/en/skills) o pídale ayuda con las habilidades.

## Conectar con ChatGPT

1. Inicie sesión en [ChatGPT](https://chatgpt.com) con sus credenciales.
1. En la esquina inferior izquierda, seleccione **su nombre** → **Configuración**.
1. Seleccione **Aplicaciones** y, a continuación, habilite **Modo de desarrollador**.
1. Seleccione el botón **Crear aplicación**.
1. Asigne a la aplicación un nombre (como &quot;Workfront&quot;) e introduzca la URL del servidor MCP que desee: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
1. Asegúrese de que Autenticación está establecida en **OAuth** (establecida de forma predeterminada) y active la casilla de verificación de aceptación para continuar.
1. Una vez creada la aplicación, aparece una ventana de inicio de sesión. Autentique con sus credenciales de Adobe ID. Asegúrese de seleccionar la instancia de Workfront que desee si pertenece a más de una.

### Personalización del comportamiento de ChatGPT con GPT personalizados

ChatGPT admite asistentes creados por el usuario llamados GPT personalizados. Puede utilizar un GPT personalizado para personalizar el comportamiento de ChatGPT con su conector. Por ejemplo, puede crear un GPT personalizado que indique a ChatGPT que siempre obtenga datos nuevos del servicio conectado en lugar de depender de resultados anteriores.

Para obtener más información acerca de los GPT personalizados, consulte la [documentación del usuario de ChatGPT](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts) o pida ayuda a ChatGPT con los GPT personalizados.

## Compruebe la conexión

Para confirmar que la plataforma agéntica de IA está conectada a Workfront, pídale que enumere las acciones que el servidor MCP de Workfront pone a disposición. Por ejemplo:

* *¿Qué acciones de Workfront puede realizar?*
* *Enumerar las herramientas de Workfront a las que tiene acceso.*

También puede ver la lista completa de herramientas en [Adobe Workfront MCP server tools](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

## Herramientas disponibles

El servidor MCP de Workfront expone un conjunto de herramientas que la plataforma agéntica de IA conectada llama en su nombre, por ejemplo, herramientas para buscar Workfront, crear elementos, actualizar campos y administrar aprobaciones. Para obtener la lista de referencia completa, agrupada por área de Workfront, consulte [Herramientas de servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

## Cambiar a otra instancia de Workfront

Cada conexión autentica la plataforma agéntica de IA en una sola instancia de Workfront. Para utilizar una instancia diferente, desconecte y vuelva a conectar.

Para conectarse a una instancia de Workfront diferente:

1. En la plataforma agéntica de IA, desconecte el servidor MCP de Workfront.
1. Vuelva a conectar el conector.
1. Autenticar en la nueva instancia de Workfront.

>[!NOTE]
>
>Cerrar sesión por sí solo no cambia la instancia de Workfront. Debe desconectar y volver a conectar el conector.

<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
-->

<!--
## Connect to Microsoft Copilot

✅ 1) Copilot Studio (most common for agents / enterprise use)
This is the cleanest "paste a URL" flow.
Steps
1. Open your Copilot Studio agent
2. Go to Tools
3. Click:
    * Add a tool → New tool → Model Context Protocol
4. In the wizard, fill in:
    * Server name (anything)
    * Server description
    * ✅ Server URL (your MCP endpoint)
5. Choose auth (if needed):
    * None / API key / OAuth
6. Click Create
👉 That's it—your MCP server is now attached to the agent.
This flow is explicitly documented:
* You add MCP via Tools → Add tool → Model Context Protocol
* Then provide Server name, description, and URL ￼
￼
What happens next
* Copilot discovers tools automatically from the MCP server
* You can enable/disable tools per agent
* The agent calls them when relevant

-->

## Solucionar problemas de configuración y autenticación

+++ Amplíe para ver sugerencias de solución de problemas para la configuración y autenticación del servidor MCP de Workfront.

| Problema | Causa probable | Corregir |
|---|---|---|
| No se encuentra el conector [!DNL Adobe Workfront] en [!DNL Claude]. | El administrador de [!DNL Claude] no lo ha habilitado. | Póngase en contacto con el administrador de [!DNL Claude] (no con el administrador de Workfront) y pídale que habilite el conector [!DNL Adobe Workfront]. |
| Se ha conectado, pero no puede ver los datos. | Se ha autenticado en la instancia incorrecta de Workfront. | Desconecte el conector, vuelva a conectarse y autentique en la instancia correcta. |
| Error de autenticación o la conexión dejó de funcionar. | La sesión de autenticación ha caducado o hay un error de conexión. | Desconecte y vuelva a conectar el conector. |
| Desea cambiar a una instancia de Workfront diferente. | Una sola conexión lo vincula a una instancia. | Desconectar, volver a conectar y autenticar en la nueva instancia. |
| No puede conectarse a Workfront o verá un mensaje que indica que el acceso al servidor MCP está deshabilitado. | El administrador de Workfront ha desactivado el acceso al servidor MCP para su instancia. | Póngase en contacto con el administrador de Workfront y pídale que habilite el acceso al servidor MCP en Preferencias del sistema. |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

Para obtener información sobre la solución de problemas diaria después de conectarse (por ejemplo, si se trata de resultados antiguos o de un comportamiento inesperado), consulte [Usar el servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).


+++


<!--
+++

## Frequently asked questions about setup

+++ Expand to view frequently asked questions about setting up the Workfront MCP server.

### Can I connect to multiple Workfront instances at once?

No. Each connection ties an AI agentic platform to a single Workfront instance. To switch, disconnect and reconnect, authenticating to the new instance.

### Which administrator enables this?

Both your Workfront administrator and the administrator for your AI agentic platform. Your Workfront administrator enables MCP server access on the Workfront side. The administrator for your AI agentic platform enables Workfront access on that platform's side. For [!DNL Claude], the [!DNL Claude] Enterprise administrator enables the [!DNL Adobe Workfront] connector.

+++

-->