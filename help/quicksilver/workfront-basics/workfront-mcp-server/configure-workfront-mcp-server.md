---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configuración del servidor MCP de Adobe Workfront
description: Configure su instancia de Workfront y su plataforma agéntica de IA para poder trabajar con Workfront a través de una conversación en lenguaje natural.
author: Courtney
feature: Get Started with Workfront
source-git-commit: dd1123c8803a7d3c8ef7b461fe0e01610e0dccc9
workflow-type: tm+mt
source-wordcount: '2007'
ht-degree: 1%

---


# Configuración del servidor MCP de Adobe Workfront

El servidor MCP [!DNL Adobe Workfront] le permite trabajar con sus datos de Workfront a través de una conversación en lenguaje natural en una plataforma independiente compatible.

Para poder conectar una plataforma independiente de IA a Workfront, un administrador de Workfront debe habilitar el acceso al servidor MCP en la instancia de Workfront. Los pasos exactos para conectar una plataforma agéntica de IA son diferentes para cada plataforma agéntica de IA admitida.

## Plataformas agénticas de IA compatibles

El servidor MCP de Workfront funciona con cualquier plataforma agéntica de IA que admita el protocolo de contexto de modelo (MCP).

Este artículo explica los pasos de conexión para:

* [!DNL Claude]
* [!DNL ChatGPT]

Si utiliza una plataforma agéntica de IA compatible con MCP diferente (por ejemplo, [!DNL Gemini] o [!DNL Microsoft Copilot]), siga los pasos de la documentación de dicha plataforma para agregar un servidor MCP personalizado. Cuando se le pida la URL del servidor MCP, introduzca:

```
https://mcp.workfront.adobe.com/mcp/v1/workfront
```

## Requisitos previos

Para poder conectar Workfront a una plataforma independiente de IA, debe:

* Tener una cuenta activa de [!DNL Adobe Workfront] con permiso para tener acceso a los datos con los que desea trabajar
* Tener acceso a una plataforma agéntica de IA como [!DNL Claude]
* La instancia de Workfront debe estar habilitada en Adobe Identity Management System (IMS).
* Para utilizar MCP con Workfront Planning, su organización debe estar en un paquete de Workfront que incluya Adobe Workfront Planning.


### Requisitos previos de administración

El acceso al servidor MCP está cerrado por dos administradores independientes.

* El administrador de Workfront controla el acceso al servidor MCP de la instancia de Workfront mediante dos conmutadores en Preferencias del sistema: **Herramientas de MCP de solo lectura** (habilitadas de forma predeterminada) y **Escribir herramientas MCP** (deshabilitadas de forma predeterminada). Si puede encontrar elementos de Workfront a través de la plataforma agéntica de IA pero no puede crearlos, actualizarlos o eliminarlos, pídale al administrador de Workfront que habilite las acciones de escritura.

  Para obtener más información, consulte [Configurar las preferencias del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* Si utiliza una versión empresarial de una plataforma independiente de IA, su administrador de dicha plataforma debe habilitar el conector [!DNL Adobe Workfront] para su organización o proporcionarle acceso de URL personalizado para conectarse al servidor MCP de Workfront.


## Conectar Workfront a Claude

Se conecta a Workfront una vez por cuenta de [!DNL Claude]. La conexión le autentica en una instancia de Workfront específica y permanecerá conectado hasta que decida desconectarse.

* [Conéctese al escritorio Claude desde el directorio de conectores](#connect-to-claude-desktop-from-the-connectors-directory)
* [Conectarse a Claude con una URL](#connect-to-claude-with-a-url)
* [Personalizar el comportamiento de Claude con habilidades](#customize-claude-behavior-with-skills)

### Conéctese al escritorio Claude desde el directorio de conectores

+++ Amplíe para ver instrucciones paso a paso para conectar Workfront a [!DNL Claude].

Para conectar Workfront a [!DNL Claude]:

1. Abra [!DNL Claude].
1. Haga clic en **Personalizar**.
1. En el panel de navegación izquierdo, haga clic en **Conectores**.
1. Busque **[!DNL Adobe Workfront]** en la lista de conectores.

   Si no lo ve, vea [Requisitos previos de administración](#admin-prerequisites) en este artículo.
1. Haga clic en **Conectar**.
1. Cuando se le solicite, inicie sesión en la instancia de Workfront. Es posible que tenga que seleccionar un perfil y una instancia de Workfront. El perfil que seleccione determina qué espacio de trabajo está conectado.

   Una vez finalizada la autenticación, el servidor MCP de Workfront está conectado.



+++

### Conectarse a Claude con una URL

+++ Amplíe para ver instrucciones paso a paso para conectar Workfront a [!DNL Claude] con una dirección URL.

>[!NOTE]
>
>Debe ser el propietario de un entorno de Claude empresarial para realizar este procedimiento.
>
>Para obtener la declaración de Claude sobre el requisito de propietario, consulte [Agregar un conector personalizado](https://support.claude.com/en/articles/11175166-get-started-with-custom-connectors-using-remote-mcp#:~:text=Note%3A%20While,has%20access%20to) en la documentación de Claude.

Para conectar Workfront a [!DNL Claude] con una dirección URL:

1. Inicie sesión en [Claude](https://claude.ai) con sus credenciales.
1. En el menú de la izquierda, seleccione el icono **Personalizar**.
1. En el panel de navegación izquierdo, seleccione **Conectores**.
1. Seleccione el icono **+** y luego seleccione **Agregar conector personalizado**.
1. Asigne al conector el nombre deseado (como &quot;Workfront&quot;) e introduzca la URL del servidor MCP:

   ```
   https://mcp.workfront.adobe.com/mcp/v1/workfront
   ```

1. Haga clic en **Conectar**.
Aparece una ventana de inicio de sesión de Workfront.
1. Autentique con sus credenciales de Adobe ID.
Es posible que tenga que seleccionar un perfil y una instancia de Workfront. El perfil que seleccione determina qué espacio de trabajo está conectado.

+++

### Personalizar el comportamiento de Claude con habilidades

[!DNL Claude] admite conjuntos de instrucciones creados por el usuario llamados aptitudes. Puede utilizar una habilidad para personalizar el comportamiento de [!DNL Claude] con Workfront. Por ejemplo, puede crear una aptitud que indique a [!DNL Claude] que siempre recupere datos nuevos de Workfront en lugar de depender de resultados anteriores.

Para obtener más información acerca de las habilidades de [!DNL Claude], consulte la [documentación del usuario Claude](https://code.claude.com/docs/en/skills) o pídale ayuda con las habilidades.

## Conectar con ChatGPT

El procedimiento para conectar el servidor MCP de Workfront con ChatGPT difiere según si está usando ChatGPT Desktop o Codex, o ChatGPT en la web.

* [Conectar con el escritorio ChatGPT o el códice ChatGPT](#connect-to-chatgpt-desktop-or-chatgpt-codex)
* [Conectarse a ChatGPT en la web](#connect-to-chatgpt-on-the-web)
* [Personalización del comportamiento de ChatGPT con GPT personalizados](#customize-chatgpt-behavior-with-custom-gpts)

### Conectar con el escritorio ChatGPT o el códice ChatGPT

+++ Amplíe para ver instrucciones paso a paso para conectar Workfront a ChatGPT Desktop o ChatGPT Codex.

1. En ChatGPT, abra **Configuración**.
1. Haga clic en **Complementos** en el panel de navegación izquierdo.
1. Haga clic en **Agregar servidor** cerca de la esquina superior derecha de la ventana.
1. Escriba un nombre para el servidor.
1. Para el tipo, seleccione **HTTP transmisible**.
1. Establezca la URL del servidor MCP:

   ```
   https://mcp.workfront.adobe.com/mcp/v1/workfront
   ```

1. Haga clic en **Guardar**.
1. En la lista que aparece, haga clic en **Autenticar** para el servidor MCP que está agregando.
1. Inicie sesión en Workfront.
Es posible que tenga que seleccionar un perfil y una instancia de Workfront. El perfil que seleccione determina qué espacio de trabajo está conectado.
1. En ChatGPT, en la lista de servidores MCP, asegúrese de que la opción a la derecha del nuevo servidor MCP permanezca activada.

+++

### Conectarse a ChatGPT en la web

+++ Amplíe para ver instrucciones paso a paso para conectar Workfront a ChatGPT en la web.

1. Inicie sesión en [ChatGPT](https://chatgpt.com) con sus credenciales.
1. En la esquina inferior izquierda, selecciona tu nombre y, a continuación, selecciona **Configuración**.
1. En el panel de navegación izquierdo, seleccione **Seguridad e inicio de sesión**.
1. Vaya a la página de complementos de ChatGPT en https://chatgpt.com/plugins.
1. Haga clic en el icono Más cerca de la parte superior derecha de la página Plugins.
1. En el campo **Nombre**, escriba un nombre para el servidor MCP.
1. En el campo **Conexión**, seleccione **URL del servidor** e introduzca la URL del servidor MCP:

   ```
   https://mcp.workfront.adobe.com/mcp/v1/workfront
   ```

1. Asegúrese de que Autenticación esté configurada en **OAuth** (de forma predeterminada).
1. Lea el mensaje de riesgo y marque la casilla para mostrar que lo ha leído.
1. Haga clic en **Crear**.
1. Una vez creada la aplicación, aparece una ventana de inicio de sesión de Workfront. Autentique con sus credenciales de Adobe ID. Es posible que tenga que seleccionar un perfil y una instancia de Workfront. El perfil que seleccione determina qué espacio de trabajo está conectado.

+++

### Personalización del comportamiento de ChatGPT con GPT personalizados

ChatGPT admite asistentes creados por el usuario llamados GPT personalizados. Puede utilizar un GPT personalizado para personalizar el comportamiento de ChatGPT con su conector. Por ejemplo, puede crear un GPT personalizado que indique a ChatGPT que siempre obtenga datos nuevos del servicio conectado en lugar de depender de resultados anteriores.

Para obtener más información acerca de los GPT personalizados, consulte la [documentación del usuario de ChatGPT](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts) o pida ayuda a ChatGPT con los GPT personalizados.

## Conectar Workfront a Copilot

+++ Amplíe para ver instrucciones paso a paso para conectar Workfront a Copilot.

Para crear un agente de Copilot personalizado al que se pueda conectar el MCP de Workfront, utilice Copilot Studio.

1. En Copilot Studio, haga clic en **Crear agente en blanco**.
1. Asigne un nombre al agente y haga clic en **Crear**.
Se abre la ventana del agente.

1. En el campo **Instrucciones**, describa lo que desea que haga el agente. Incluya información como sus procesos y cómo utiliza Workfront. Recomendamos proporcionar una gran cantidad de detalles.
1. En la barra de navegación superior, haz clic en **Herramientas** y luego haz clic en **Agregar una herramienta**.
1. Seleccione el mosaico **Protocolo de contexto del modelo**.
1. En el panel que aparece, escriba un nombre y una descripción para esta conexión.
1. En el campo URL del servidor, introduzca la URL:

   ```
   https://mcp.workfront.adobe.com/mcp/v1/workfront`
   ```

1. Para la autenticación, selecciona **OAuth 2.0** y, a continuación, selecciona **Detección dinámica**.
1. Haga clic en **Crear** en la parte inferior del panel.

   La aplicación está registrada.

1. Una vez registrada la aplicación, en el panel que aparece, haz clic en **No conectado**, luego haz clic en **Crear una nueva conexión** y, a continuación, haz clic en **Crear**.
1. Para configurar una conexión, haz clic en **No conectado**, luego en **Crear nueva conexión** y después en **Crear**.
1. En el panel de inicio de sesión que aparece, inicie sesión en Workfront, seleccione la instancia que desee usar (si tiene acceso a más de una instancia) y, a continuación, haga clic en **Continuar**.
1. En el panel que muestra su servidor, haga clic en **Agregar y configurar**.

   Ahora puede empezar a utilizar y configurar herramientas para su servidor MCP.
1. Cuando haya configurado y probado una herramienta, haga clic en **Publicar**.

   Es posible que no tenga permisos para publicar. Si este es el caso, póngase en contacto con el administrador de Copilot.

+++

## Conectar Workfront a una solución MCP personalizada

Si está creando su propia aplicación o agente personalizado, puede conectarse directamente al servidor MCP de Workfront.

Hay dos formas de conectarse:

* [Conectar con un token de servicio a servicio](#connect-with-a-service-to-service-token)
* [Conexión con OAuth](#connect-with-oauth)

### Conectar con un token de servicio a servicio

1. Cree una credencial de servicio con Adobe Developer Console. Para obtener más información, consulte [Autenticación de servidor a servidor](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/).
1. Conéctese al servidor MCP de Workfront con la siguiente información:

   * **URL**: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
   * **Encabezados**:

     * `Authorization: Bearer <access_token>`
     * `wf-url: <your_subdomain>.my.workfront.com` (obligatorio si sus credenciales tienen acceso a más de una instancia de Workfront, como Previsualización y Producción).

### Conexión con OAuth

La compatibilidad de autoservicio para integraciones de OAuth personalizadas aún no está disponible para Workfront.

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
>* Cerrar sesión por sí solo no cambia la instancia de Workfront. Debe desconectar y volver a conectar el conector.


<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server:  
   ```
   https://mcp.workfront.adobe.com/mcp/v1/workfront|
   
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
| --- | --- | --- |
| No se encuentra el conector [!DNL Adobe Workfront] en [!DNL Claude]. | El administrador de [!DNL Claude] no lo ha habilitado. | Póngase en contacto con el administrador de [!DNL Claude] (no con el administrador de Workfront) y pídale que habilite el conector [!DNL Adobe Workfront]. |
| Se ha conectado, pero no puede ver los datos. | Se ha autenticado en la instancia incorrecta de Workfront. | Desconecte el conector, vuelva a conectarse y autentique en la instancia correcta. |
| Error de autenticación o la conexión dejó de funcionar. | La sesión de autenticación ha caducado o hay un error de conexión. | Desconecte y vuelva a conectar el conector. |
| Desea cambiar a una instancia de Workfront diferente. | Una sola conexión lo vincula a una instancia. | Desconectar, volver a conectar y autenticar en la nueva instancia. |
| No puede conectarse a Workfront o verá un mensaje que indica que el acceso al servidor MCP está deshabilitado. | El administrador de Workfront ha desactivado el acceso al servidor MCP para su instancia. | Póngase en contacto con el administrador de Workfront y pídale que habilite el acceso al servidor MCP en Preferencias del sistema. |
| La plataforma agéntica de IA puede encontrar sus elementos de Workfront, pero no puede crearlos, actualizarlos o eliminarlos. | El administrador de Workfront ha deshabilitado las acciones de escritura para el servidor MCP de Workfront. | Póngase en contacto con el administrador de Workfront y pídale que habilite acciones de escritura en Preferencias del sistema. |

Para obtener información sobre la solución de problemas diaria después de conectarse (por ejemplo, si se trata de resultados antiguos o de un comportamiento inesperado), consulte [Usar el servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).


+++

## Preguntas frecuentes sobre la configuración

+++ Amplíe para ver las preguntas más frecuentes sobre la configuración del servidor MCP de Workfront.

* [¿Puedo conectarme a varias instancias de Workfront al mismo tiempo?](#can-i-connect-to-multiple-workfront-instances-at-the-same-time)
* [¿Qué administrador habilita esto?](#which-administrator-enables-this)
* [¿Puedo usar el servidor MCP de Workfront si mi instancia de Workfront no está habilitada en Adobe Identity Management System (IMS)?](#can-i-use-the-workfront-mcp-server-if-my-workfront-instance-isnt-enabled-on-adobe-identity-management-system-ims)

### ¿Puedo conectarme a varias instancias de Workfront al mismo tiempo?

No. Cada conexión vincula una plataforma auténtica de IA a una sola instancia de Workfront. Para cambiar, desconectar y volver a conectar, autenticándose en la nueva instancia.

### ¿Qué administrador habilita esto?

Tanto el administrador de Workfront como el administrador de la plataforma agéntica de IA. El administrador de Workfront habilita el acceso al servidor MCP en el lado de Workfront. El administrador de la plataforma agéntica de IA habilita el acceso de Workfront del lado de la plataforma. Para [!DNL Claude], el administrador empresarial de [!DNL Claude] habilita el conector [!DNL Adobe Workfront].

### ¿Puedo usar el servidor MCP de Workfront si mi instancia de Workfront no está habilitada en Adobe Identity Management System (IMS)?

No. La instancia de Workfront debe estar habilitada en Adobe Identity Management System (IMS) para utilizar el servidor MCP de Workfront. Si no está seguro de si la instancia está habilitada en IMS, póngase en contacto con el administrador de Workfront.

+++ 

