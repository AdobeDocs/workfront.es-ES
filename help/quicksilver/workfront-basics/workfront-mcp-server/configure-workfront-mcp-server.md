---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configuración del servidor MCP de Adobe Workfront
description: Configure la instancia de Workfront y el asistente de IA para poder trabajar con Workfront a través de una conversación en lenguaje natural.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 5%

---


# Configuración del servidor MCP de Adobe Workfront

El servidor MCP de [!DNL Adobe Workfront] le permite trabajar con los datos de Workfront a través de una conversación en lenguaje natural en un asistente de IA compatible como Claude o ChatGPT.

Para poder conectar un asistente de IA a Workfront, un administrador de Workfront debe habilitar el acceso al servidor MCP en la instancia de Workfront. Los pasos exactos para conectar un asistente de IA son diferentes para cada asistente de IA admitido.

Para obtener más información sobre el servidor MCP de Workfront, consulte [Descripción general del servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Asistentes de IA admitidos

En la actualidad, el servidor MCP de Workfront admite los siguientes asistentes de IA:

* [!DNL Claude]

<!-- NEEDS DETAIL: Update this list as Adobe adds support for additional AI assistants (for example, [!DNL Gemini], or [!DNL Microsoft Copilot]). -->

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront package requirement (Select, Prime, Ultimate, Any?) --></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront license requirement (Standard, Work, etc.) --></p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para poder conectar Workfront a un asistente de IA, debe:

* Tener una cuenta activa de [!DNL Adobe Workfront] con permiso para tener acceso a los datos con los que desea trabajar.
* Tener acceso a un asistente de IA como [!DNL Claude].

  <!-- NEEDS DETAIL: Confirm which Claude tiers are supported. Claude Enterprise is confirmed; Claude Pro and Claude Team support is unconfirmed. -->

### Requisitos previos de administración

El acceso al servidor MCP está cerrado por dos administradores independientes. Ambos deben habilitar el acceso para poder conectarse.

* **El administrador de Workfront** debe habilitar el acceso al servidor MCP en su instancia de Workfront.

* Si utiliza una versión empresarial de un asistente de IA, su administrador del asistente de IA debe habilitar el conector [!DNL Adobe Workfront] para su organización.


## Conectar Workfront a Claude

Se conecta a Workfront una vez por cuenta de [!DNL Claude]. La conexión le autentica en una instancia de Workfront específica y permanecerá conectado hasta que decida desconectarse.


>[!IMPORTANT]
>
>Si usa [!DNL Claude] Enterprise, **su administrador de [!DNL Claude] Enterprise** debe habilitar el conector [!DNL Adobe Workfront] para su organización. Hasta que lo hagan, el conector [!DNL Adobe Workfront] no aparecerá cuando lo busque en [!DNL Claude]. Póngase en contacto primero con el administrador de [!DNL Claude].


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

### Compruebe la conexión

Para confirmar que [!DNL Claude] está conectado a Workfront, pida a [!DNL Claude] que enumere las acciones que el servidor MCP de Workfront pone a disposición. Por ejemplo:

* *¿Qué acciones de Workfront puede realizar?*
* *Enumerar las herramientas de Workfront a las que tiene acceso.*

[!DNL Claude] devuelve la lista de acciones disponibles.

<!-- NEEDS DETAIL: Add a screenshot of the tool-list response. -->

### Cambiar a otra instancia de Workfront

Cada conexión autentica [!DNL Claude] en una sola instancia de Workfront. Para utilizar una instancia diferente, desconecte y vuelva a conectar.

Para conectarse a una instancia de Workfront diferente:

1. En [!DNL Claude], desconecte el conector [!DNL Adobe Workfront].
1. Vuelva a conectar el conector.
1. Autenticar en la nueva instancia de Workfront.

>[!NOTE]
>
>El cierre de sesión de [!DNL Claude] por sí solo no cambia la instancia de Workfront. Debe desconectar y volver a conectar el conector.

## Personalizar el comportamiento de Claude con habilidades

<!-- NEEDS DETAIL: Confirm whether Adobe is shipping any pre-built Claude skills alongside the MCP server. If yes, list them and link to download or installation guidance. If no, decide whether to mention skills as a user-driven workaround at all, or remove this section. -->

[!DNL Claude] admite conjuntos de instrucciones creados por el usuario llamados aptitudes. Puede utilizar una habilidad para personalizar el comportamiento de [!DNL Claude] con Workfront. Por ejemplo, puede crear una aptitud que indique a [!DNL Claude] que siempre recupere datos nuevos de Workfront en lugar de depender de resultados anteriores.

## Solucionar problemas de configuración y autenticación

| Problema | Causa probable | Corregir |
|---|---|---|
| No se encuentra el conector [!DNL Adobe Workfront] en [!DNL Claude]. | El administrador de [!DNL Claude] no lo ha habilitado. | Póngase en contacto con el administrador de [!DNL Claude] (no con el administrador de Workfront) y pídale que habilite el conector [!DNL Adobe Workfront]. |
| Se ha conectado, pero no puede ver los datos. | Se ha autenticado en la instancia incorrecta de Workfront. | Desconecte el conector, vuelva a conectarse y autentique en la instancia correcta. |
| Error de autenticación o la conexión dejó de funcionar. | La sesión de autenticación ha caducado o hay un error de conexión. | Desconecte y vuelva a conectar el conector. |
| Desea cambiar a una instancia de Workfront diferente. | Una sola conexión lo vincula a una instancia. | Desconectar, volver a conectar y autenticar en la nueva instancia. |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

Para obtener información sobre la solución de problemas diaria después de conectarse (por ejemplo, si se trata de resultados antiguos o de un comportamiento inesperado), consulte [Usar el servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).

## Preguntas frecuentes sobre la configuración

### ¿Puedo conectarme a varias instancias de Workfront a la vez?

No. Cada conexión vincula un asistente de IA a una sola instancia de Workfront. Para cambiar, desconectar y volver a conectar, autenticándose en la nueva instancia.

### ¿Funciona esto con Claude Pro o Claude Team, o solo con Claude Enterprise?

<!-- NEEDS DETAIL: Confirm Claude tier support and answer this directly. -->

### ¿Qué administrador habilita esto?

Tanto el administrador de Workfront como el administrador del asistente de IA. El administrador de Workfront habilita el acceso al servidor MCP en el lado de Workfront. El administrador del asistente de IA habilita el acceso de Workfront en el lado del asistente de IA. Para [!DNL Claude], el administrador empresarial de [!DNL Claude] habilita el conector [!DNL Adobe Workfront].
