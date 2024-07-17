---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Acceder [!DNL Adobe Workfront] desde [!DNL Slack]
description: Integrar [!DNL Adobe Workfront] con [!DNL Slack] te permite acceder a [!DNL Workfront] desde el Slack o realizar ciertas acciones en [!DNL Workfront] usando un comando de barra diagonal. La integración se puede usar desde cualquier  [!DNL Slack] entorno, incluida la [!DNL Slack] aplicación móvil.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 1%

---

# Acceder a [!DNL Adobe Workfront] desde [!DNL Slack]

La integración de [!DNL Adobe Workfront] con [!DNL Slack] le permite obtener acceso a [!DNL Workfront] desde [!DNL Slack] o realizar determinadas acciones en [!DNL Workfront] mediante un comando de barra diagonal. La integración se puede usar desde cualquier entorno de [!DNL Slack], incluida la aplicación móvil [!DNL Slack].

Usted o su administrador de [!DNL Slack] deben instalar la aplicación [!DNL Workfront] en su instancia de [!DNL Slack] para poder usar [!DNL Workfront] desde [!DNL Slack]. Para obtener más información, consulte [Configuración de Adobe Workfront para el Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Comandos de barra diagonal {#about-slash-commands}

Al usar [!DNL Slack], se escriben mensajes dentro de un campo de mensaje. Al iniciar el mensaje con una barra oblicua, se convierte en un comando y se comporta de forma diferente que un mensaje simple. El comando indica a [!DNL Slack] que realice una acción.

Puede obtener acceso a la instancia de [!DNL Workfront] desde [!DNL Slack] escribiendo un comando de barra diagonal en cualquier canal de [!DNL Slack].

Recuerde lo siguiente cuando use un comando de barra oblicua en [!DNL Slack] para tener acceso a [!DNL Workfront]:

* Los comandos de barra diagonal distinguen entre mayúsculas y minúsculas.
* Los comandos de [!DNL Workfront] sólo son visibles para usted, independientemente del canal en el que los esté escribiendo.
* El comando siempre debe comenzar con `/workfront` o `/wf`, seguido de un espacio y el nombre de una acción que desee realizar en [!DNL Workfront].

  Esto indica que el comando está diseñado para la aplicación [!DNL Workfront]. Los comandos de [!DNL Workfront] solo funcionan si ya ha configurado la aplicación [!DNL Workfront] con la instancia [!DNL Slack].

Para obtener una lista de todos los comandos que puede ejecutar desde el Slack para [!DNL Workfront], vea [Acceso [!DNL Workfront] desde un comando de barra diagonal en [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Iniciar sesión en [!DNL Workfront] desde [!DNL Slack] {#log-in-to-workfront-from-slack}

Cuando escriba cualquier comando en el campo de mensaje del Slack, se le pedirá que inicie sesión primero en [!DNL Workfront].\
Para obtener una lista completa de [!DNL Workfront] comandos de [!DNL Slack], consulte la sección [Acceder [!DNL Workfront] desde un comando de barra diagonal en [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) en este artículo.

Para iniciar sesión en [!DNL Workfront] desde [!DNL Slack]:

1. Inicie sesión en su instancia de [!DNL Slack].
1. Desde cualquier canal, escriba uno de los siguientes comandos:\
   `/workfront log in`

   O

   `/wf log in`

1. Haga clic en el vínculo [!DNL Workfront] **[!UICONTROL Iniciar sesión]** que se muestra en la respuesta.\
   Se abre una nueva pestaña con campos para las credenciales de [!DNL Workfront].

1. Siga las indicaciones para iniciar sesión en [!DNL Workfront] mediante la autenticación mejorada, OAuth 2.0 o su URL de lenguaje de marcado de aserción de seguridad (SAML).

   >[!NOTE]
   >
   >* Cuando se le pida que introduzca el host de su cuenta de [!DNL Workfront], escríbalo con este formato: *yourCompany&#39;sDomain.my.workfront.com*. El dominio de su empresa suele ser el nombre de su empresa.
   >* La autenticación mejorada no está disponible hasta que un administrador de [!DNL Workfront] la habilite para esta integración.


   Se abre la página de configuración de [!DNL Workfront] notificaciones en [!DNL Slack].

1. (Opcional) Deshabilite las [!DNL Workfront] notificaciones que no desee recibir en [!DNL Slack].

   Para obtener información acerca de la configuración de [!DNL Workfront] para [!DNL Slack], vea la sección [Configurar opciones](#configure-settings-configure-settings) en este artículo

1. Vuelva al canal [!DNL Slack].

   Ha iniciado sesión en [!DNL Workfront] desde su instancia de [!DNL Slack].

## Acceder a [!DNL Workfront] desde [!DNL Slack]

* [Comandos de barra diagonal](#about-slash-commands-about-slash-commands)
* [Tener acceso a  [!DNL Workfront] desde un vínculo compartido en [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Obtener acceso a [!DNL Workfront] desde un comando de barra diagonal en [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Inicie sesión en la instancia de [!DNL Slack] e inicie sesión en [!DNL Workfront] desde [!DNL Slack].\
   Para obtener más información sobre cómo iniciar sesión en [!DNL Workfront] desde [!DNL Slack], consulte [Iniciar sesión en [!DNL Workfront] desde [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. Desde cualquier canal, empiece a escribir el siguiente comando en el campo de mensaje:

   `/workfront help`

   O

   `/wf help`

1. Seleccione entre los siguientes comandos:

   * `/wf home`

     Muestra botones desde los cuales puede acceder a listas de sus tareas, problemas y aprobaciones. Al hacer clic en uno de los botones, se muestran los primeros 20 elementos de cada lista en [!DNL Slack].

     Para obtener más información sobre la administración de [!DNL Workfront] elementos de trabajo de [!DNL Slack], consulte [Administrar su trabajo y las aprobaciones de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

     Incluya el nombre de la tarea tal como aparecerá en la interfaz [!DNL Workfront].

     Agrega una tarea a [!DNL Workfront].

     Para obtener más información acerca de cómo agregar tareas a [!DNL Workfront] desde el Slack, vea la sección &quot;Creando tareas a partir de [!DNL Slack]&quot; en [Crear tareas y problemas a partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

     Incluya el nombre del problema tal como aparecerá en la interfaz [!DNL Workfront].

     Agrega un problema a [!DNL Workfront]

     Para obtener más información sobre cómo agregar problemas a [!DNL Workfront] desde [!DNL Slack], consulte la sección &quot;Creando problemas a partir de [!DNL Slack]&quot; en [Crear tareas y problemas a partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

     Muestra la lista de favoritos de [!DNL Workfront].

     Para obtener más información sobre cómo obtener acceso a tus favoritos desde [!DNL Slack], consulta la sección [Obtener acceso a tu lista de [!UICONTROL favoritos] desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) en el artículo [Obtener acceso a tus favoritos y a los elementos recientes desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md).

   * `/wf recent`

     Muestra la lista de los elementos a los que se ha tenido acceso más recientemente en [!DNL Workfront].

     Para obtener más información sobre el acceso a los elementos recientes de [!DNL Slack], consulte el artículo [Acceso a la lista de [!UICONTROL elementos recientes] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] y [!UICONTROL elementos recientes de [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md).

   * `wf tasks`

     Muestra una lista de las tareas.

     Para obtener más información sobre la administración de tareas de [!DNL Slack], consulte la sección &quot;Administración de tareas de [!DNL Slack]&quot; en [Administración del trabajo y las aprobaciones de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

     Muestra una lista de sus problemas.

     Para obtener más información sobre la administración de los problemas de [!DNL Slack], consulte la sección &quot;Administrar los problemas de [!DNL Slack]&quot; en [Administrar el trabajo y las aprobaciones de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` muestra sus [!DNL Workfront] aprobaciones.\

     Para obtener más información sobre la administración de las aprobaciones de [!DNL Slack], consulte la sección &quot;Administrar las aprobaciones de [!DNL Slack]&quot; en [Administrar el trabajo y las aprobaciones de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

     Palabra clave Include.

     Busque una palabra clave específica. Puede buscar los siguientes tipos de objetos:

      * Proyecto
      * Tarea
      * Problema
      * Informe
      * Personas
      * Plantilla
      * Documento
      * Portafolio
      * Programar
      * Panel de control
      * Compañía
      * Nota \

        Para obtener más información sobre la búsqueda en [!DNL Slack], consulte [Buscar  [!DNL Adobe Workfront] elementos del Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

     Inicia sesión en [!DNL Workfront] desde [!DNL Slack].

   * `/wf log out `

     Cierra la sesión de [!DNL Workfront] desde [!DNL Slack]. Permanece conectado a [!DNL Workfront] si tiene una instancia de [!DNL Workfront] independiente abierta en otra ficha del explorador en otra aplicación.
   * `/wf settings`

     Le permite configurar su configuración de [!DNL Workfront] en [!DNL Slack].

     Para obtener información acerca de la configuración de [!DNL Workfront] en el Slack, vea [Configurar opciones](#configure-settings-configure-settings).

   * `/wf help`
Muestra una lista completa de comandos para [!DNL Workfront].


   * `Visit Workfront Help`: abre la sección [!UICONTROL Slack] en el sitio de ayuda de [!DNL Workfront] en una nueva pestaña del explorador.


1. (Opcional) Para eliminar el mensaje de cualquier comando, pase el ratón sobre la esquina superior derecha del mensaje del Slack que contiene el comando y haga clic en&#x200B;**[!UICONTROL Mostrar acciones del mensaje]** y, a continuación, haga clic en **[!UICONTROL Eliminar mensaje]**.

1. (Opcional y condicional) Haga clic en **[!UICONTROL Eliminar]** para confirmar que desea eliminar este mensaje.

### Obtener acceso a [!DNL Workfront] desde un vínculo compartido en [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

Puede tener acceso a [!DNL Workfront] objetos desde un vínculo a esos objetos que se compartió con usted en [!DNL Slack].

Para obtener más información sobre cómo tener acceso a [!DNL Workfront] desde un vínculo compartido, vea [Tener acceso a [!DNL Adobe Workfront] objetos desde un vínculo compartido en [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Configurar opciones {#configure-settings}

1. Dentro de un campo de mensaje [!DNL Slack], escriba el siguiente comando:

   `/workfront settings`

   O

   `/wf settings`

   Todos los ajustes están activados de forma predeterminada.

1. Anule la selección de las siguientes opciones para deshabilitar la configuración de Workfront:

   * En el área de **[!UICONTROL Configuración general]**, deshabilite **[!UICONTROL Al pegar una URL de [!DNL Workfront] en un canal de [!DNL Slack], muestre una descripción adicional, una fecha de vencimiento o un nombre de solicitante]** si no desea que [!DNL Slack] agregue información adicional sobre los objetos de [!DNL Workfront] cuando comparta una URL con el objeto en [!UICONTROL Slack].

   * En el área **[!UICONTROL Configuración de notificaciones]**, deshabilite las notificaciones que desee que dejen de recibirse de Workfront.\

     Para obtener información acerca de cómo recibir [!DNL Workfront] notificaciones en [!DNL Slack], vea [Recibir [!DNL Adobe Workfront] notificaciones en [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Cerrar sesión de [!DNL Workfront] desde [!DNL Slack]

1. Dentro de un campo de mensaje [!DNL Slack], escriba el siguiente comando:\
   `/workfront log out` O\
   `/wf log out`\
   Recibirá una confirmación de que ha cerrado la sesión de [!DNL Workfront].\
   Permanece conectado a [!DNL Workfront] si tiene una instancia de [!DNL Workfront] independiente abierta en otra ficha del explorador en otra aplicación.
