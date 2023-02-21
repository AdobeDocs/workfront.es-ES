---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Vincular elementos entre [!DNL Adobe Workfront] y [!DNL Jira]
description: Puede vincular [!DNL Jira] problemas con [!DNL Adobe Workfront] tareas o problemas de forma automática o manual.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 0%

---

# Vincular elementos entre [!DNL Adobe Workfront] y [!DNL Jira]

Puede vincular [!DNL Jira] problemas con [!DNL Adobe Workfront] tareas o problemas de forma automática o manual.

Solo un elemento de [!DNL Workfront] se puede vincular a un elemento de [!DNL Jira]. Nunca se puede vincular una [!DNL Workfront] elemento a varios [!DNL Jira] problemas, ni uno [!DNL Jira] problema con varios [!DNL Workfront] elementos.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] información general sobre licencias</a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acceso a Jira</td> 
   <td> <p>Acceso de administrador del sistema</p> <p><b>IMPORTANTE</b>

Se recomienda crear cuentas de administrador del sistema independientes en [!DNL Jira] y [!DNL Workfront] para dedicarse a esta integración, en lugar de usar las existentes que se podrían adjuntar a los usuarios.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Antes de poder vincular elementos entre [!DNL Workfront] y [!DNL Jira], debe

* Instalar [!DNL Workfront] para [!DNL Jira]

   Para obtener instrucciones sobre la instalación de Workfront para Jira, consulte [Instalación de Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurar [!DNL Workfront] para Jira

   Para obtener instrucciones sobre la configuración de Workfront para Jira, consulte [Configuración de Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Vincular automáticamente [!DNL Workfront] elementos a [!DNL Jira] problemas

Como [!DNL Workfront] administrador, puede definir déclencheur que puedan crear automáticamente un problema en [!DNL Jira] cada vez que se cumplen determinadas condiciones en una tarea o un problema en [!DNL Workfront]. Workfront y [!DNL Jira] los elementos se vinculan.

Una vez completada la configuración de [!DNL Workfront] para Jira, cuando se crea o actualiza un elemento en [!DNL Workfront] para que coincida con sus déclencheur, se crea automáticamente un nuevo artículo en [!DNL Jira].\
Los usuarios de Workfront que crean y actualizan elementos de Workfront no necesitan una [!DNL Jira] licencia para déclencheur de la creación de elementos en [!DNL Jira].

Para obtener más información sobre la definición de déclencheur para crear problemas de Jira automáticamente, consulte  [Configurar [!DNL Adobe Workfront] para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Puede crear [!DNL Jira] elementos automáticamente adjuntando una plantilla a un proyecto. Si la plantilla contiene tareas con asignaciones que cumplen la función [!DNL Jira] déclencheur, las nuevas tareas generan nuevas [!DNL Jira] problemas.

Vinculación automática de una [!DNL Workfront] enviar a un [!DNL Jira] el problema es idéntico al de la vinculación automática de [!DNL Workfront] tarea a [!DNL Jira] problema.

Para vincular automáticamente un [!DNL Workfront] tarea a [!DNL Jira] problema:

1. Asegúrese de que su [!DNL Jira] el administrador del sistema ha configurado déclencheur para crear automáticamente [!DNL Jira] problemas cuando [!DNL Workfront] elementos asignados y luego iniciar sesión en [!DNL Workfront] con un nivel de acceso que le permite crear una tarea.

   Para obtener más información sobre el acceso a las tareas, consulte [Concesión de acceso a tareas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. Vaya a un proyecto y seleccione **[!UICONTROL Tareas]** ![](assets/tasks-icon-in-left-panel-14x14.png) en el panel izquierdo.

1. Haga clic en **[!UICONTROL Nueva tarea]**

   O

   Seleccione una tarea existente y haga clic en **Editar**.

1. Especifique o actualice cualquiera de los campos disponibles para la tarea.
1. Haga clic en **[!UICONTROL Asignaciones]** y asigne la tarea a un usuario, función o equipo que esté especificado como déclencheur en la variable [!DNL Jira] integración.

1. Haga clic en **Guardar cambios**.

   Se crea una nueva tarea en Workfront.

   En el **[!UICONTROL Actualizaciones]** del área de la nueva tarea, hay un comentario que indica que también se ha creado un nuevo problema en [!DNL Jira].

1. (Opcional) Haga clic en el enlace al problema de Jira para abrirlo en Jira.

   O

   Haga clic en el **[!UICONTROL Ir a Jira]** en el **[!UICONTROL Integraciones]** del **[!UICONTROL Detalles]** para abrir la sección [!DNL Jira] problema.

   El administrador del sistema o del grupo debe agregar la variable [!UICONTROL Integraciones] a la plantilla de diseño para mostrarla en el encabezado de la tarea o del problema. Para obtener más información, consulte [Personalización de encabezados de objeto mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Cualquiera [!DNL Jira] el usuario puede empezar a trabajar inmediatamente en elementos creados automáticamente a partir de [!DNL Workfront] y sus actualizaciones se transferirán a [!DNL Workfront] sin necesidad de una licencia para [!DNL Workfront] para ello.

   Solo los campos que se muestran como [!DNL Workfront] el administrador configurado durante la configuración del [!DNL Workfront] se actualizan los complementos.

   Para obtener más información sobre la sincronización de campos entre Workfront y Jira, consulte la [Configuración de Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) en  [Configuración de Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >La variable [!DNL Jira] no está asignado a nadie en [!DNL Jira] cuando se crea automáticamente desde Workfront.

## Vínculo manual [!DNL Jira] problemas con [!DNL Workfront] items

Una vez creados los elementos en [!DNL Jira] y [!DNL Workfront], independientemente de los demás, puede vincular manualmente un [!DNL Jira] problema con una [!DNL Workfront] tarea o problema.\
No se puede vincular manualmente un [!DNL Workfront] elemento de [!DNL Workfront] a una [!DNL Jira] elemento.

>[!NOTE]
>
>Si la variable [!DNL Jira] El problema no está en un proyecto que no esté identificado como déclencheur en la variable [!DNL Workfront] Integración no puede vincularla manualmente a un elemento de Workfront al utilizar la integración con [!DNL Jira] On-Premise.\
>Para obtener más información sobre la configuración de déclencheur para el flujo de trabajo de Workfront to Jira , consulte [Vincular automáticamente elementos de Workfront a problemas de Jira](#automatically-link-workfront-items-to-jira-issues).

When [!DNL Workfront] y [!DNL Jira] Los elementos están vinculados, ciertos campos de un elemento se pueden actualizar automáticamente en el otro.\
Para obtener más información sobre la actualización de elementos vinculados, consulte [Actualización de elementos vinculados entre Jira y Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Para vincular manualmente [!DNL Jira] problemas con [!DNL Workfront] elementos:

1. (Condicional) Inicie sesión en [!DNL Workfront] y busque un problema o una tarea a la que desee vincular [!DNL Jira] problema.
1. (Condicional) En la barra de direcciones del elemento, copie el **URL** del elemento en Workfront.

   O

   En el [!UICONTROL Detalles] , copie el **[!UICONTROL Número de referencia]** del elemento en Workfront.

   >[!NOTE]
   >
   >Debe tener un [!DNL Workfront] licencia para iniciar sesión en [!DNL Workfront]. De lo contrario, un [!DNL Workfront] El usuario debe proporcionarle esta información.

1. En [!DNL Jira], vaya a un problema que desee vincular manualmente al [!DNL Workfront] elemento.
1. En el [!DNL Workfront] panel derecho, pegue el **URL** o **[!UICONTROL Número de referencia]** del [!DNL Workfront] elemento que desea vincular a él.

1. Haga clic en **[!UICONTROL Vínculo]**.

   Los dos elementos se vinculan y la variable [!DNL Workfront] el panel derecho se rellena con información del [!DNL Workfront] elemento.

   Lo siguiente [!DNL Workfront] los campos están visibles en [!DNL Jira], de forma predeterminada, en la variable [!DNL Workfront] panel derecho:

   * La variable **[!UICONTROL Nombre]** del elemento: Puede acceder al [!DNL Workfront] haciendo clic en el nombre del panel.
   * **[!UICONTROL Nombre del proyecto]**
   * La variable **[!UICONTROL Estado]** del elemento
   * La variable **[!UICONTROL Prioridad]** del elemento
   * La fecha en la que se creó [!DNL Workfront]
   * La variable **[!UICONTROL Horas planificadas]** del elemento
   * La variable **[!UICONTROL Número de referencia]**: Puede acceder al [!DNL Workfront] haciendo clic en el botón [!UICONTROL Número de referencia] en el panel .

Para obtener más información sobre cómo activar campos adicionales para que se muestren en el panel derecho, consulte [Configuración de la sincronización de campos entre [!DNL Jira] y [!DNL Workfront] Elementos](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) en [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Un comentario del [!DNL Workfront] el administrador asociado a la integración se publica en la **[!DNL Workfront]** de la pestaña [!DNL Jira] problema para confirmar que [!DNL Jira] se ha creado el elemento. El comentario contiene un vínculo al [!DNL Jira] problema.

## Desvincular elementos entre [!DNL Jira] y [!DNL Workfront]

Elementos vinculados entre [!DNL Jira] y [!DNL Workfront] se puede desvincular manualmente de [!DNL Jira].\
No se puede desvincular un [!DNL Workfront] elemento de su [!DNL Jira] homólogo en [!DNL Workfront].

Necesita el siguiente acceso para desvincular un elemento vinculado manualmente:

* Usted es el usuario que vinculó manualmente los elementos
* Usted es el [!DNL Jira] administrador del sistema

Solo un [!DNL Workfront] el administrador puede desvincular elementos que se vincularon automáticamente.

Para desvincular un [!DNL Jira] desde un [!DNL Workfront] elemento:

1. En [!DNL Jira], vaya a un problema vinculado a un [!DNL Workfront] tarea o problema.
1. Vaya a la [!DNL Workfront] panel derecho y haga clic en el botón **[!UICONTROL Desvincular]** y, a continuación, haga clic en **[!UICONTROL Desvincular]**.

   El vínculo anterior [!DNL Jira] y [!DNL Workfront] los elementos ahora están desvinculados. Los campos, comentarios o documentos que puedan actualizarse sobre ellos individualmente en el futuro no se actualizan en su contraparte anterior en la otra aplicación.
