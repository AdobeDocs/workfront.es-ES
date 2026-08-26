---
title: Cree aplicaciones de App Builder con habilidades con Claude Code
description: Use un conjunto de habilidades de Claude Code para crear aplicaciones de Adobe Workfront App Builder personalizadas describiendo lo que desea, en lugar de ejecutar los pasos de configuración e implementación usted mismo.
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: e5a288dcac20be9176d1541d531edaf0d8c99a8c
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 5%

---


# Cree aplicaciones de App Builder con habilidades con Claude Code

Un conjunto de [!DNL Claude Code] aptitudes permite que [!DNL Claude] cree aplicaciones [!DNL Adobe App Builder] personalizadas para [!DNL Workfront]. Esto significa que puede crear uno describiendo lo que desea en inglés sin formato, sin ser desarrollador ni escribir los pasos de configuración usted mismo.

Las extensiones de la interfaz de usuario de Workfront, con tecnología de Adobe App Builder, permiten a los clientes y partners crear experiencias de usuario personalizadas. Las extensiones de IU le permiten modificar la experiencia de Workfront de su organización para satisfacer mejor las necesidades de la organización, lo que puede mejorar la eficacia, ofrecer experiencias conectadas sin problemas y mejorar significativamente la satisfacción del usuario, así como ayudar a su organización a materializar su visión única.

Para obtener más información acerca de las extensiones de la interfaz de usuario de Workfront, consulte [Crear aplicaciones personalizadas para Workfront con Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Habilidades de extensibilidad de IU para Claude

Generar en [!DNL Adobe App Builder] puede ser muy técnico, lo que puede crear barreras si un usuario no está familiarizado con el procedimiento o las técnicas. Las habilidades de extensibilidad de la interfaz de usuario simplifican este proceso al usar [!DNL Claude]. Usted describe la característica que desea y [!DNL Claude] hace el trabajo práctico, como configurar las herramientas, crear el proyecto en [!DNL Adobe App Builder], crear la aplicación, implementarla en la nube de Adobe y ejecutarla dentro de Workfront. Solo participa en el proceso cuando hay una decisión o un inicio de sesión que requiere que realice alguna acción.

## Requisitos previos

Antes de empezar, asegúrese de que dispone de lo siguiente:

* **[!DNL Claude Code]** instalado.
* **Acceso a las habilidades**.

  * Puede encontrar las habilidades en [https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md).

    Si este vínculo no se abre, pídale al administrador que le conceda acceso.
  * Después de descargar las aptitudes, ejecute los siguientes comandos para configurarlas.

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
