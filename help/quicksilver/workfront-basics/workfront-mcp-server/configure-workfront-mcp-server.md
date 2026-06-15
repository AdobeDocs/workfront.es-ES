---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configuración del servidor MCP de Adobe Workfront
description: Configure su instancia de Workfront y su plataforma agéntica de IA para poder trabajar con Workfront a través de una conversación en lenguaje natural.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 0445376ea187b589040c8fdc56ea0d11f44b0b37
workflow-type: tm+mt
source-wordcount: '1748'
ht-degree: 1%

---


# Configuración del servidor MCP de Adobe Workfront

El servidor MCP [!DNL Adobe Workfront] le permite trabajar con sus datos de Workfront a través de una conversación en lenguaje natural en una plataforma independiente compatible.

Para poder conectar una plataforma independiente de IA a Workfront, un administrador de Workfront debe habilitar el acceso al servidor MCP en la instancia de Workfront. Los pasos exactos para conectar una plataforma agéntica de IA son diferentes para cada plataforma agéntica de IA admitida.

>[!IMPORTANT]
>
>Actualmente, el servidor MCP de Workfront solo está disponible para los clientes que utilizan AWS. Los clientes que utilicen GCP o Azure podrán utilizar esta funcionalidad en un futuro próximo.

## Plataformas agénticas de IA compatibles

El servidor MCP de Workfront funciona con cualquier plataforma agéntica de IA que admita el protocolo de contexto de modelo (MCP).

Este artículo explica los pasos de conexión para:

* [!DNL Claude]
* [!DNL ChatGPT]

Si utiliza una plataforma agéntica de IA compatible con MCP diferente (por ejemplo, [!DNL Gemini] o [!DNL Microsoft Copilot]), siga los pasos de la documentación de dicha plataforma para agregar un servidor MCP personalizado. Cuando se le pida la URL del servidor MCP, introduzca la URL de su región:

| Región | URL |
| --- | --- |
| EE. UU. | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
| UE | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |

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



### Conéctese al escritorio Claude desde el directorio de conectores

>[!IMPORTANT]
>
>Actualmente, Claude Connector solo admite la conexión al servidor MCP de Workfront en la región de Estados Unidos.  Para conectarse a una instancia de Workfront en la región de la UE, consulte [Conectarse al escritorio de Claude con una URL](#connect-to-claude-desktop-with-a-url) en este artículo.

+++ Amplíe para ver instrucciones paso a paso para conectar Workfront a [!DNL Claude].

Para conectar Workfront a [!DNL Claude]:

1. Abra [!DNL Claude].

1. Vaya al área de conectores.



1. Busque **[!DNL Adobe Workfront]** en la lista de conectores.

   Si no lo ve, vea [Requisitos previos de administración](#admin-prerequisites) en este artículo.

1. Haga clic en **Conectar**.



1. Cuando se le solicite, inicie sesión en la instancia de Workfront.


1. Una vez finalizada la autenticación, estará conectado.



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
1. Seleccione **Conectores** y, a continuación, seleccione el icono **+** para agregar un conector.
1. Seleccione el botón **Crear aplicación**.
1. Asigne al conector el nombre deseado (como &quot;Workfront&quot;) e introduzca la URL del servidor MCP deseada:

   | Región | URL |
   | --- | --- |
   | EE. UU. | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | UE | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |

1. Una vez creado el conector, aparece una ventana de inicio de sesión. Autentique con sus credenciales de Adobe ID. Asegúrese de seleccionar la instancia de Workfront que desee si pertenece a más de una.

   >[!NOTE]
   >
   >La instancia de Workfront debe conectarse con el servidor MCP de la región de dicha instancia. Por ejemplo, una instancia de la UE debe conectarse al servidor MCP de la UE.
   >
   >Al seleccionar una instancia, las instancias que no son compatibles con la región del servidor MCP aparecen atenuadas y no se puede conectar a ellas.
   >
   >Para conectarse a una instancia que no sea compatible con la región del servidor MCP, configure una nueva conexión MCP con la dirección URL correcta para esa región.

+++

### Personalizar el comportamiento de Claude con habilidades

[!DNL Claude] admite conjuntos de instrucciones creados por el usuario llamados aptitudes. Puede utilizar una habilidad para personalizar el comportamiento de [!DNL Claude] con Workfront. Por ejemplo, puede crear una aptitud que indique a [!DNL Claude] que siempre recupere datos nuevos de Workfront en lugar de depender de resultados anteriores.

Para obtener más información acerca de las habilidades de [!DNL Claude], consulte la [documentación del usuario Claude](https://code.claude.com/docs/en/skills) o pídale ayuda con las habilidades.

## Conectar con ChatGPT

1. Inicie sesión en [ChatGPT](https://chatgpt.com) con sus credenciales.
1. En la esquina inferior izquierda, seleccione **su nombre** → **Configuración**.
1. Seleccione **Aplicaciones** y, a continuación, habilite **Modo de desarrollador**.
1. Seleccione el botón **Crear aplicación**.
1. Asigne a la aplicación un nombre (como &quot;Workfront&quot;) e introduzca la URL del servidor MCP que desee:

   | Región | URL |
   | --- | --- |
   | EE. UU. | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | UE | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |

1. Asegúrese de que Autenticación está establecida en **OAuth** (establecida de forma predeterminada) y active la casilla de verificación de aceptación para continuar.
1. Una vez creada la aplicación, aparece una ventana de inicio de sesión. Autentique con sus credenciales de Adobe ID. Asegúrese de seleccionar la instancia de Workfront que desee si pertenece a más de una.

   >[!NOTE]
   >
   >La instancia de Workfront debe conectarse con el servidor MCP de la región de dicha instancia. Por ejemplo, una instancia de la UE debe conectarse al servidor MCP de la UE.
   >
   >Al seleccionar una instancia, las instancias que no son compatibles con la región del servidor MCP aparecen atenuadas y no se puede conectar a ellas.
   >
   >Para conectarse a una instancia que no sea compatible con la región del servidor MCP, configure una nueva conexión MCP con la dirección URL correcta para esa región.


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
>* Cerrar sesión por sí solo no cambia la instancia de Workfront. Debe desconectar y volver a conectar el conector.
>
>* La instancia de Workfront debe conectarse con el servidor MCP de la región de dicha instancia. Por ejemplo, una instancia de la UE debe conectarse al servidor MCP de la UE.
>
>   Al seleccionar una instancia, las instancias que no son compatibles con la región del servidor MCP aparecen atenuadas y no se puede conectar a ellas.
>
>   Para conectarse a una instancia que no sea compatible con la región del servidor MCP, configure una nueva conexión MCP con la dirección URL correcta para esa región.


<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server:  

   | Region | URL |
   | --- | --- |
   | US | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | EU | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |
   
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
| La instancia de Workfront a la que desea conectarse aparece atenuada y aparece un mensaje que indica que no está disponible para conectarse en su región | El servidor MCP está configurado para una región (UE o EE. UU.) diferente a la de su instancia. | Configure el servidor MCP con la dirección URL de la región a la que está asignada la instancia de Workfront. |
| La plataforma agéntica de IA puede encontrar sus elementos de Workfront, pero no puede crearlos, actualizarlos o eliminarlos. | El administrador de Workfront ha deshabilitado las acciones de escritura para el servidor MCP de Workfront. | Póngase en contacto con el administrador de Workfront y pídale que habilite acciones de escritura en Preferencias del sistema. |

Para obtener información sobre la solución de problemas diaria después de conectarse (por ejemplo, si se trata de resultados antiguos o de un comportamiento inesperado), consulte [Usar el servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).


+++

## Preguntas frecuentes sobre la configuración

+++ Amplíe para ver las preguntas más frecuentes sobre la configuración del servidor MCP de Workfront.

### ¿Puedo conectarme a varias instancias de Workfront al mismo tiempo?

No. Cada conexión vincula una plataforma auténtica de IA a una sola instancia de Workfront. Para cambiar, desconectar y volver a conectar, autenticándose en la nueva instancia.

### ¿Qué administrador habilita esto?

Tanto el administrador de Workfront como el administrador de la plataforma agéntica de IA. El administrador de Workfront habilita el acceso al servidor MCP en el lado de Workfront. El administrador de la plataforma agéntica de IA habilita el acceso de Workfront del lado de la plataforma. Para [!DNL Claude], el administrador empresarial de [!DNL Claude] habilita el conector [!DNL Adobe Workfront].

### ¿Puedo usar el servidor MCP de Workfront si mi instancia de Workfront no está habilitada en Adobe Identity Management System (IMS)?

No. La instancia de Workfront debe estar habilitada en Adobe Identity Management System (IMS) para utilizar el servidor MCP de Workfront. Si no está seguro de si la instancia está habilitada en IMS, póngase en contacto con el administrador de Workfront.

+++ 
