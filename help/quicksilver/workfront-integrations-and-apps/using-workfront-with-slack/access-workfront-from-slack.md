---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Acceso [!DNL Adobe Workfront] from [!DNL Slack]
description: Integración [!DNL Adobe Workfront] con [!DNL Slack] le permite acceder a [!DNL Workfront] del Slack o realice determinadas acciones en [!DNL Workfront] usando un comando barra oblicua. La integración se puede utilizar desde cualquier [!DNL Slack] entorno, incluido el [!DNL Slack] aplicación móvil.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1075'
ht-degree: 1%

---

# Acceso [!DNL Adobe Workfront] from [!DNL Slack]

Integración [!DNL Adobe Workfront] con [!DNL Slack] le permite acceder a [!DNL Workfront] from [!DNL Slack]o realizar determinadas acciones en [!DNL Workfront] usando un comando barra oblicua. La integración se puede utilizar desde cualquier [!DNL Slack] entorno, incluido el [!DNL Slack] aplicación móvil.

Usted o su [!DNL Slack] El administrador debe instalar [!DNL Workfront] en su [!DNL Slack] instancia antes de poder usar [!DNL Workfront] from [!DNL Slack]. Para obtener más información, consulte [Configuración de Adobe Workfront para Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Acerca de los comandos de barra oblicua {#about-slash-commands}

Al usar [!DNL Slack], los mensajes se escriben dentro de un campo de mensaje. Cuando inicia el mensaje con una barra diagonal, se convierte en un comando y se comporta de forma diferente que un mensaje simple. El comando indica [!DNL Slack] para realizar una acción.

Puede acceder a su [!DNL Workfront] instancia de [!DNL Slack] escribiendo un comando de barra diagonal en cualquier [!DNL Slack] canal.

Recuerde lo siguiente cuando utilice un comando de barra oblicua en [!DNL Slack] para acceder a [!DNL Workfront]:

* Los comandos de barra diagonal distinguen entre mayúsculas y minúsculas.
* Los comandos para [!DNL Workfront] solo son visibles para usted, independientemente del canal en el que los escriba.
* El comando siempre debe comenzar con `/workfront` o `/wf`, seguido de un espacio y el nombre de una acción en la que desea realizar [!DNL Workfront].

   Esto indica que el comando está diseñado para la variable [!DNL Workfront] aplicación. Los comandos para [!DNL Workfront] solo funciona cuando ya ha configurado la variable [!DNL Workfront] la aplicación con su [!DNL Slack] instancia.

Para obtener una lista de todos los comandos que puede ejecutar desde el Slack para [!DNL Workfront], consulte [Acceso [!DNL Workfront] desde un comando barra oblicua en [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Iniciar sesión en [!DNL Workfront] from [!DNL Slack] {#log-in-to-workfront-from-slack}

Cuando escriba cualquier comando en el campo de mensaje en el Slack, se le pedirá que inicie sesión en [!DNL Workfront] primero.\
Para obtener una lista completa de [!DNL Workfront] comandos de [!DNL Slack], consulte la [Acceso [!DNL Workfront] desde un comando barra oblicua en [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) en este artículo.

Para iniciar sesión en [!DNL Workfront] from [!DNL Slack]:

1. Inicie sesión en su [!DNL Slack] instancia.
1. Desde cualquier canal, escriba uno de los siguientes comandos:\
   `/workfront log in`

   O

   `/wf log in`

1. Haga clic en el [!DNL Workfront] **[!UICONTROL Iniciar sesión]** vínculo mostrado en la respuesta.\
   Una nueva pestaña se abre con campos para [!DNL Workfront] credenciales.

1. Siga las indicaciones para iniciar sesión en [!DNL Workfront] mediante la autenticación mejorada, OAuth 2.0 o la URL del lenguaje de marcado de aserción de seguridad (SAML).

   >[!NOTE]
   >
   >* Cuando se le pida que introduzca el host de su [!DNL Workfront] cuenta, escríbala con este formato: *yourCompany&#39;sDomain.my.workfront.com*. El dominio de la empresa suele ser el nombre de la empresa.
   >* La autenticación mejorada no está disponible hasta que se [!DNL Workfront] el administrador lo habilita para esta integración.



   La página de configuración de [!DNL Workfront] notificaciones en [!DNL Slack] se abre.

1. (Opcional) Desactive cualquier [!DNL Workfront] notificaciones que no desea recibir en [!DNL Slack].

   Para obtener información sobre cómo configurar [!DNL Workfront] configuración para [!DNL Slack], consulte la [Configuración](#configure-settings-configure-settings) sección de este artículo

1. Vuelva a la [!DNL Slack] canal.

   Ha iniciado sesión en [!DNL Workfront] de su [!DNL Slack] instancia.

## Acceso [!DNL Workfront] from [!DNL Slack]

* [Acerca de los comandos de barra oblicua](#about-slash-commands-about-slash-commands)
* [Acceso [!DNL Workfront] desde un vínculo compartido en [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Acceso [!DNL Workfront] desde un comando barra oblicua en [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Inicie sesión en su [!DNL Slack] instancia e inicie sesión en [!DNL Workfront] from [!DNL Slack].\
   Para obtener más información sobre cómo iniciar sesión en [!DNL Workfront] from [!DNL Slack], consulte [Iniciar sesión en [!DNL Workfront] from [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. Desde cualquier canal, empiece a escribir el siguiente comando en el campo del mensaje:

   `/workfront help`

   O

   `/wf help`

1. Seleccione entre los siguientes comandos:

   * `/wf home`

      Muestra los botones desde los que puede acceder a las listas de tareas, problemas y aprobaciones. Al hacer clic en uno de los botones, se muestran los 20 primeros elementos de cada lista de [!DNL Slack].

      Para obtener más información sobre la administración [!DNL Workfront] elementos de trabajo de [!DNL Slack], consulte [Administre su trabajo y aprobaciones desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

      Incluya el nombre de la tarea tal como aparecerá en el [!DNL Workfront] interfaz.

      Agrega una tarea a [!DNL Workfront].

      Para obtener más información sobre cómo agregar tareas a [!DNL Workfront] del Slack, consulte &quot;Creación de tareas a partir de [!DNL Slack]&quot; en [Crear tareas y problemas desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

      Incluya el nombre del problema tal como aparecerá en el [!DNL Workfront] interfaz.

      Agrega un problema a [!DNL Workfront]

      Para obtener más información sobre cómo agregar problemas a [!DNL Workfront] from [!DNL Slack], consulte &quot;Creación de problemas desde [!DNL Slack]&quot; en [Crear tareas y problemas desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

      Muestra la lista de [!DNL Workfront] Favoritos.

      Para obtener más información sobre el acceso a sus favoritos desde [!DNL Slack], consulte la [Acceder a su [!UICONTROL Favoritos] Lista de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) en la sección [Acceder a sus favoritos y elementos recientes desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) artículo.

   * `/wf recent`

      Muestra la lista de los elementos a los que accedió más recientemente en [!DNL Workfront].

      Para obtener más información sobre el acceso a los elementos recientes desde [!DNL Slack], consulte la [Acceder a su [!UICONTROL Artículos recientes] Lista de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] y [!UICONTROL artículos recientes de [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) artículo.

   * `wf tasks`

      Muestra una lista de las tareas realizadas.

      Para obtener más información sobre la administración de tareas de [!DNL Slack], consulte &quot;Administración de tareas desde [!DNL Slack]&quot; en [Administración del trabajo y las aprobaciones desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

      Muestra una lista de los problemas.

      Para obtener más información sobre la administración de problemas de [!DNL Slack], consulte &quot;Gestionar sus problemas desde [!DNL Slack]&quot; en [Administración del trabajo y las aprobaciones desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Muestra el [!DNL Workfront] aprobaciones.\

      Para obtener más información sobre la administración de aprobaciones de [!DNL Slack], consulte &quot;Administración de aprobaciones de [!DNL Slack]&quot; en [Administre su trabajo y aprobaciones desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

      Incluir palabra clave.

      Busque una palabra clave específica. Puede buscar los siguientes objetos de tipo :

      * Proyecto
      * Tarea
      * Problema
      * Informe
      * Personas
      * Plantilla
      * Documento
      * Portafolio
      * Programar
      * Panel
      * Compañía
      * Nota  \

         Para obtener más información sobre la búsqueda en [!DNL Slack], consulte [Buscar [!DNL Adobe Workfront] elementos del Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

      Inicie sesión en [!DNL Workfront] from [!DNL Slack].

   * `/wf log out `

      Le cierra la sesión [!DNL Workfront] from [!DNL Slack]. Ha iniciado sesión en [!DNL Workfront] si tiene una [!DNL Workfront] la instancia se abre en otra pestaña del explorador en otra aplicación.
   * `/wf settings`

      Le da acceso para configurar su [!DNL Workfront] configuración de [!DNL Slack].

      Para obtener información sobre cómo configurar [!DNL Workfront] configuración en Slack, consulte [Configuración](#configure-settings-configure-settings).

   * `/wf help`
Muestra una lista completa de comandos para [!DNL Workfront].


   * `Visit Workfront Help`: Abre el [!UICONTROL Slack] en la sección [!DNL Workfront] Sitio de ayuda en una nueva ficha del explorador.


1. (Opcional) Para eliminar el mensaje de cualquier comando, pase el ratón sobre la esquina superior derecha del mensaje del Slack que contiene el comando y haga clic en &#x200B;**[!UICONTROL Mostrar acciones de mensaje]** y haga clic en **[!UICONTROL Eliminar mensaje]**.

1. (Opcional y condicional) Haga clic en **[!UICONTROL Eliminar]** para confirmar que desea eliminar este mensaje.

### Acceso [!DNL Workfront] desde un vínculo compartido en [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

Puede acceder a [!DNL Workfront] objetos de un vínculo a los objetos que se comparten con usted en [!DNL Slack].

Para obtener más información sobre el acceso a [!DNL Workfront] desde un vínculo compartido, consulte [Acceso [!DNL Adobe Workfront] objetos de un vínculo compartido en [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Configuración {#configure-settings}

1. Dentro de un [!DNL Slack] campo de mensaje, escriba el siguiente comando:

   `/workfront settings`

   O

   `/wf settings`

   Todos los ajustes están habilitados de forma predeterminada.

1. Anule la selección de las siguientes opciones para deshabilitar la configuración de Workfront:

   * En el **[!UICONTROL Configuración general]** , desactive la **[!UICONTROL Al pegar un [!DNL Workfront] URL en un [!DNL Slack] canal, mostrar descripción adicional, fecha de vencimiento o nombre del solicitante]**&#x200B; de configuración si no desea [!DNL Slack] para agregar información adicional sobre [!DNL Workfront] objetos al compartir una dirección URL con el objeto [!UICONTROL Slack].

   * En el **[!UICONTROL Configuración de notificaciones]** , desactive las notificaciones que desee dejar de recibir de Workfront.\

      Para obtener información sobre la recepción [!DNL Workfront] notificaciones en [!DNL Slack], consulte [Recibir [!DNL Adobe Workfront] notificaciones en [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Cerrar sesión [!DNL Workfront] from [!DNL Slack]

1. Dentro de un [!DNL Slack] campo de mensaje, escriba el siguiente comando:\
   `/workfront log out` O\
   `/wf log out`\
   Recibe la confirmación de que se ha cerrado la sesión de [!DNL Workfront].\
   Ha iniciado sesión en [!DNL Workfront] si tiene una [!DNL Workfront] la instancia se abre en otra pestaña del explorador en otra aplicación.
