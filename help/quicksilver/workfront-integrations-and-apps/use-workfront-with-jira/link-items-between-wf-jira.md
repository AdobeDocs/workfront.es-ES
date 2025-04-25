---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Vincular elementos entre  [!DNL Adobe Workfront]  y  [!DNL Jira]
description: Puede vincular problemas de  [!DNL Jira]  a tareas o problemas de  [!DNL Adobe Workfront]  de forma automática o manual.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 96%

---

# Vincular elementos entre [!DNL Adobe Workfront] y [!DNL Jira]

Puede vincular [!DNL Jira] problemas a [!DNL Adobe Workfront] tareas o problemas de forma automática o manual.

Solo se puede vincular un elemento de [!DNL Workfront] a un elemento de [!DNL Jira]. Nunca puede vincular un elemento de [!DNL Workfront] a varios problemas de [!DNL Jira], ni un problema de [!DNL Jira] a varios elementos de [!DNL Workfront].

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general de las licencias de Adobe[!DNL Workfront]</a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acceso a Jira</td> 
   <td> <p>Acceso de administrador del sistema</p> <p><b>IMPORTANTE</b>

Recomendamos que cree cuentas de administrador del sistema separadas en [!DNL Jira] y [!DNL Workfront] para dedicar a esta integración, en lugar de usar cuentas existentes que puedan estar asociadas a usuarios.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de [!DNL Workfront]. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>.</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un [!DNL Workfront] administrador puede modificar tu nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Requisitos previos

Para poder vincular elementos entre [!DNL Workfront] y [!DNL Jira], debe

* Instalar [!DNL Workfront] para [!DNL Jira]

  Para obtener instrucciones sobre la instalación de Workfront para Jira, consulte [Instalar Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurar [!DNL Workfront] para Jira

  Para obtener instrucciones sobre cómo configurar Workfront para Jira, consulte [Configurar Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Vincular automáticamente [!DNL Workfront] elementos a [!DNL Jira] problemas

Como [!DNL Workfront] administrador, puedes definir activadores que automáticamente creen un problema en [!DNL Jira] cada vez que se cumplan ciertas condiciones en una tarea o un problema en [!DNL Workfront]. Los elementos Workfront y [!DNL Jira] se vinculan.

Una vez que haya completado la configuración de [!DNL Workfront] para Jira, cuando un elemento se cree o se actualice en [!DNL Workfront] para coincidir con tus activadores, se creará automáticamente un nuevo elemento en [!DNL Jira].\
Los usuarios de Workfront que crean y actualizan elementos en Workfront no necesitan una licencia de [!DNL Jira] para activar la creación de elementos en [!DNL Jira].

Para obtener más información sobre cómo definir activadores para crear problemas en Jira automáticamente, consulte [Configurar [!DNL Adobe Workfront] para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Puede crear [!DNL Jira] elementos automáticamente adjuntando una plantilla a un proyecto. Si la plantilla contiene tareas con asignaciones que cumplan con los activadores de [!DNL Jira], las nuevas tareas generarán nuevos problemas de [!DNL Jira].

Vincular automáticamente un problema de [!DNL Workfront] a un problema de [!DNL Jira] es idéntico a vincular automáticamente una tarea de [!DNL Workfront] a un problema de [!DNL Jira].

Para vincular automáticamente una tarea de [!DNL Workfront] a un problema de [!DNL Jira]:

1. Asegúrate de que su [!DNL Jira] administrador del sistema haya configurado activadores para crear automáticamente problemas de [!DNL Jira] cuando se asignen elementos de [!DNL Workfront], luego inicia sesión en [!DNL Workfront] con un nivel de acceso que permita crear una tarea.

   Para obtener más información acerca del acceso a las tareas, consulte [Conceder acceso a las tareas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. Vaya a un proyecto y seleccione **[!UICONTROL Tareas]** ![Icono de tareas](assets/tasks-icon-in-left-panel-14x14.png) en el panel izquierdo.

1. Haga clic en **[!UICONTROL Nueva tarea]**

   O

   Seleccione una tarea existente y luego haga clic en **Editar**.

1. Especifique o actualice cualquiera de los campos disponibles para la tarea.
1. Haga clic en **[!UICONTROL Asignaciones]** y asigne la tarea a un usuario, rol o equipo que esté especificado como déclencheur en la integración de [!DNL Jira].

1. Haga clic en **Guardar cambios**.

   Se crea una nueva tarea en Workfront.

   En el área **[!UICONTROL Actualizaciones]** de la nueva tarea, hay un comentario que indica que también se ha creado un nuevo problema en [!DNL Jira].

1. (Opcional) Haga clic en el vínculo del problema de Jira para abrirlo en Jira.

   O

   Haga clic en el enlace **[!UICONTROL Ir a Jira]** en el área de **[!UICONTROL Integraciones]** de la sección **[!UICONTROL Detalles]** o en el encabezado de la tarea o problema, para abrir el problema [!DNL Jira].

   Su administrador de sistema o de grupo debe añadir el campo [!UICONTROL Integraciones] a su plantilla de diseño para que se muestre en el encabezado de la tarea o problema. Para obtener más información, consulte [Personalización de áreas de objeto con una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Cualquier [!DNL Jira] usuario puede empezar a trabajar inmediatamente en los elementos creados automáticamente desde [!DNL Workfront] y sus actualizaciones se transferirán a [!DNL Workfront] sin necesidad de una licencia de [!DNL Workfront] para hacerlo.

   Solo se actualizan los campos que usted como administrador de [!DNL Workfront] configuró durante la configuración del complemento [!DNL Workfront].

   Para obtener más información sobre la sincronización de campos entre Workfront y Jira, consulte la sección [Configurar Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) en [Configurar Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >El problema [!DNL Jira] no se ha asignado a nadie en [!DNL Jira] cuando se crea automáticamente a partir de Workfront.

## Vincular manualmente [!DNL Jira] problemas a [!DNL Workfront] elementos

Una vez creados los elementos en [!DNL Jira] y [!DNL Workfront], independientemente unos de otros, puede vincular manualmente un problema de [!DNL Jira] a una tarea o problema de [!DNL Workfront] existente.\
No puede vincular manualmente un elemento [!DNL Workfront] de [!DNL Workfront] a un elemento [!DNL Jira] existente.

>[!NOTE]
>
>Si el problema de [!DNL Jira] no está en un proyecto que no está identificado como un activador en la [!DNL Workfront] Integración, no puedes vincularlo manualmente a un elemento de Workfront cuando uses la integración con [!DNL Jira] On-Premise .\
>Para obtener más información sobre cómo configurar activadores para el flujo de trabajo de Workfront a Jira, consulte [Vincular automáticamente elementos de Workfront a problemas de Jira](#automatically-link-workfront-items-to-jira-issues).

Cuando los elementos [!DNL Workfront] y [!DNL Jira] están vinculados, ciertos campos de un elemento se pueden actualizar automáticamente en el otro.\
Para obtener más información sobre cómo actualizar los elementos vinculados, consulte [Actualizar elementos vinculados entre Jira y Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Para vincular manualmente problemas de [!DNL Jira] los elementos de [!DNL Workfront]:

1. (Condicional) Inicie sesión en [!DNL Workfront] y busque un problema o una tarea que desee vincular a [!DNL Jira] problema.
1. (Condicional) En el área [!UICONTROL Detalles], copie el **[!UICONTROL Número de referencia]** del elemento en Workfront.

   O

   En la barra de direcciones del elemento, copie la **URL** del elemento en Workfront.

   >[!IMPORTANT]
   >
   >Si su organización ha sido incorporada a la Experiencia unificada de Adobe, debe usar el **Número de referencia** para vincular elementos de Workfront a Jira. (La opción URL está disponible, pero devolverá un error si la utiliza). Para obtener información sobre la experiencia unificada, consulte [Experiencia unificada de Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
   >
   >Para organizaciones que no están en la experiencia unificada de Adobe, no se recomienda utilizar la opción URL porque las direcciones URL pueden cambiar.

   >[!NOTE]
   >
   >Debe tener una licencia de [!DNL Workfront] para iniciar sesión en [!DNL Workfront]. De lo contrario, un usuario de [!DNL Workfront] debe proporcionarle esta información.

1. En [!DNL Jira], vaya a un problema que desee vincular manualmente al elemento [!DNL Workfront].
1. En el panel derecho de [!DNL Workfront], pega el **[!UICONTROL Número de Referencia]** o la **URL** del [!DNL Workfront] elemento que deseas vincular a este.

1. Haz clic en **[!UICONTROL Vincular]**.

   Los dos elementos se vinculan y el [!DNL Workfront] panel derecho se completa con información del elemento [!DNL Workfront].

   Los siguientes [!DNL Workfront] campos están visibles en [!DNL Jira], de forma predeterminada, en el panel derecho de [!DNL Workfront]:

   * El **[!UICONTROL Nombre]** del elemento: puede tener acceso al elemento [!DNL Workfront] haciendo clic en el nombre en el panel.
   * **[!UICONTROL Nombre del proyecto]**
   * El **[!UICONTROL estado]** del elemento
   * La **[!UICONTROL Prioridad]** del elemento
   * La fecha en la que se creó en [!DNL Workfront]
   * Las **[!UICONTROL horas planificadas]** del elemento
   * El **[!UICONTROL número de referencia]**: Para tener acceso al elemento [!DNL Workfront], haga clic en el [!UICONTROL número de referencia] en el panel.

Para obtener más información sobre cómo habilitar campos adicionales para que se muestren en el panel derecho, consulte la sección [Configurar la sincronización de campos entre [!DNL Jira]  y  [!DNL Workfront] Elementos](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) en [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Se publica un comentario del administrador de [!DNL Workfront] asociado con la integración en la ficha **[!DNL Workfront]** del problema [!DNL Jira] para confirmar que se ha creado un nuevo elemento de [!DNL Jira]. El comentario contiene un vínculo al problema [!DNL Jira].

## Desvincular elementos entre [!DNL Jira] y [!DNL Workfront]

Los elementos vinculados entre [!DNL Jira] y [!DNL Workfront] se pueden desvincular manualmente de [!DNL Jira].\
No se puede desvincular un [!DNL Workfront] elemento de su [!DNL Jira] equivalente en [!DNL Workfront].

Necesita el siguiente acceso para desvincular el elemento vinculado manualmente:

* Usted es el usuario que vinculó manualmente los elementos
* Usted es el administrador del sistema [!DNL Jira]

Solamente un administrador de [!DNL Workfront] puede desenlazar elementos que se vincularon automáticamente.

Para desvincular un problema de [!DNL Jira] de un elemento de [!DNL Workfront]:

1. En [!DNL Jira], navegue hasta un problema que esté vinculado a una tarea o problema de [!DNL Workfront].
1. Vaya al [!DNL Workfront] panel derecho, y haga clic en el icono **[!UICONTROL Desvincular]**, luego haz clic en **[!UICONTROL Desvincular]**.

   Los elementos enlazados anteriormente [!DNL Jira] y [!DNL Workfront] ahora están desenlazados. Cualquier campo, comentario o documento que se actualice individualmente en ellos en el futuro no se actualizará en su equivalente anterior en la otra aplicación.
