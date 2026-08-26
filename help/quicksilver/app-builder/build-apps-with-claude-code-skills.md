---
title: Cree aplicaciones de App Builder con habilidades con Claude Code
description: Use un conjunto de habilidades de Claude Code para crear aplicaciones de Adobe Workfront App Builder personalizadas describiendo lo que desea, en lugar de ejecutar los pasos de configuración e implementación usted mismo.
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: 366cc4ffea48295b00389b5ee36f2df42b2c8a07
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 4%

---


# Cree aplicaciones de App Builder con habilidades con Claude Code

Un paquete de aptitudes permite que [!DNL Claude] (o cualquier mazo de codificación de IA que admita aptitudes con formato Claude, como [!DNL Claude Code] o [!DNL OpenAI Codex]) cree aplicaciones [!DNL Adobe App Builder] personalizadas para [!DNL Workfront]. Si tiene acceso a una de estas herramientas, puede crear una extensión de la interfaz de usuario describiendo lo que desea en inglés sin formato, sin requerir la experiencia del desarrollador ni pasos manuales de configuración.

Las extensiones de la interfaz de usuario de Workfront, con tecnología de Adobe App Builder, permiten a los clientes y partners crear experiencias de usuario personalizadas. Las extensiones de IU le permiten modificar la experiencia de Workfront de su organización para satisfacer mejor las necesidades de la organización, lo que puede mejorar la eficacia, ofrecer experiencias conectadas sin problemas y mejorar significativamente la satisfacción del usuario, así como ayudar a su organización a materializar su visión única.

Para obtener más información acerca de las extensiones de la interfaz de usuario de Workfront, consulte [Crear aplicaciones personalizadas para Workfront con Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Habilidades de extensibilidad de IU

Las habilidades de extensibilidad de la IU permiten que un mazo de codificación de IA administre la creación de extensiones de IU en Workfront. Usted describe la característica que desea y realiza el trabajo práctico, como configurar las herramientas, crear su proyecto en [!DNL Adobe App Builder], crear la aplicación, implementarla en la nube de Adobe y ejecutarla dentro de Workfront. Solo participa en el proceso cuando hay una decisión o un inicio de sesión que requiere que realice alguna acción. Este artículo usa [!DNL Claude] como ejemplo, pero las instrucciones se aplican a cualquier mazo de codificación de IA compatible con Claude Skills.

## Requisitos previos

Antes de empezar, asegúrese de que dispone de lo siguiente:

* **Arnés de codificación de IA que admite Claude Skills**, como [!DNL Claude Code].

  Para obtener más información sobre las aptitudes de Claude, consulte [¿Qué son las aptitudes?](https://support.claude.com/en/articles/12512176-what-are-skills) en la documentación de Claude.

* **Acceso a las habilidades**.

  * Puede encontrar las habilidades en [https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md).

    Si este vínculo no se abre, pídale al administrador que le conceda acceso.
  * Las aptitudes se publican en el mercado de aptitudes públicas de Adobe ([adobe/skills](https://github.com/adobe/skills)). En [!DNL Claude Code], ejecute:

    ```
    /plugin marketplace add adobe/skills
    ```

    ```
    /plugin install app-builder@adobe-skills
    ```

* Acceso de **[!DNL Adobe App Builder], con el rol de Desarrollador**. Su organización de Adobe necesita una licencia de App Builder y se le debe añadir como Desarrollador en ella. Esto es lo que permite que [!DNL Claude] abra Adobe Developer Console y cree su proyecto.

  Para comprobar que se cumple este requisito previo:

  1. Abra [Adobe Developer Console](https://developer.adobe.com/console).
  1. Confirme que la organización que se muestra en la esquina superior derecha es correcta.
  1. Haga clic en **Crear nuevo proyecto** > **Crear proyecto a partir de la plantilla**.
  1. Comprueba si **App Builder** aparece en la lista.

     * Si ve **App Builder** en la lista, tiene acceso.
     * Si no hay la opción **Crear proyecto a partir de plantilla** o no hay la opción **App Builder**, aún no tiene acceso. Solicite a su administrador de Workfront o Adobe que le añada como desarrollador (en Adobe Admin Console > Usuarios > Desarrolladores) y confirme que su organización tiene una licencia de App Builder.
* **El servidor MCP de Workfront se conectó**, por lo que [!DNL Claude] usa la API real de Workfront en lugar de adivinar los tipos de datos, los campos y los comandos.

  Para comprobar si el servidor MCP de Workfront ya está conectado, pregunte [!DNL Claude]: *&quot;¿Puede ver los recursos MCP de Workfront?&quot;*

  Para obtener más información e instrucciones, consulte [Conectar Workfront a Claude](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#connect-workfront-to-claude)en el artículo Configuración del servidor MCP de Adobe Workfront.
