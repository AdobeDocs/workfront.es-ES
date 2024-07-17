---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Vincular elementos entre  [!DNL Adobe Workfront] y [!DNL Jira]
description: Puede vincular  [!DNL Jira] problemas a [!DNL Adobe Workfront] tareas o problemas de forma automática o manual.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1158'
ht-degree: 0%

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
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Resumen de licencias de Adobe [!DNL Workfront]</a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acceso a Jira</td> 
   <td> <p>Acceso de administrador del sistema</p> <p><b>IMPORTANTE</b>

Se recomienda crear cuentas de administrador del sistema independientes en [!DNL Jira] y [!DNL Workfront] para dedicarlas a esta integración, en lugar de usar las existentes que podrían adjuntarse a los usuarios.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de [!DNL Workfront]. Para obtener información sobre los administradores de [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
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

Como administrador de [!DNL Workfront], puede definir déclencheur que puedan crear automáticamente un problema en [!DNL Jira] cada vez que se cumplan ciertas condiciones en una tarea o un problema en [!DNL Workfront]. Los elementos Workfront y [!DNL Jira] se vinculan.

Después de completar la configuración de [!DNL Workfront] para Jira, cuando se crea o actualiza un elemento en [!DNL Workfront] para que coincida con sus déclencheur, se crea automáticamente un nuevo elemento en [!DNL Jira].\
Los usuarios de Workfront que creen y actualicen elementos de Workfront no necesitan una licencia de [!DNL Jira] para almacenar en déclencheur la creación de elementos en [!DNL Jira].

Para obtener más información sobre la definición de déclencheur para crear problemas de Jira automáticamente, consulte [Configurar [!DNL Adobe Workfront] para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Puede crear [!DNL Jira] elementos automáticamente adjuntando una plantilla a un proyecto. Si la plantilla contiene tareas con asignaciones que cumplen los [!DNL Jira] déclencheur, las nuevas tareas generarán nuevos [!DNL Jira] problemas.

Vincular automáticamente un problema de [!DNL Workfront] a un problema de [!DNL Jira] es idéntico a vincular automáticamente una tarea de [!DNL Workfront] a un problema de [!DNL Jira].

Para vincular automáticamente una tarea de [!DNL Workfront] a un problema de [!DNL Jira]:

1. Asegúrese de que el administrador del sistema de [!DNL Jira] haya configurado déclencheur para crear automáticamente [!DNL Jira] problemas cuando se asignen [!DNL Workfront] elementos y, a continuación, inicie sesión en [!DNL Workfront] con un nivel de acceso que le permita crear una tarea.

   Para obtener más información acerca del acceso a las tareas, vea [Conceder acceso a las tareas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. Vaya a un proyecto y seleccione **[!UICONTROL Tareas]** ![](assets/tasks-icon-in-left-panel-14x14.png) en el panel izquierdo.

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

   Haga clic en el vínculo **[!UICONTROL Ir a Jira]** en el área de **[!UICONTROL Integraciones]** de la sección **[!UICONTROL Detalles]** o en el encabezado de la tarea o del problema para abrir el problema [!DNL Jira].

   El administrador del sistema o del grupo debe agregar el campo [!UICONTROL Integraciones] a la plantilla de diseño para mostrarlo en el encabezado de la tarea o del problema. Para obtener más información, vea [Personalizar encabezados de objeto mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Cualquier usuario de [!DNL Jira] puede empezar a trabajar inmediatamente en los elementos creados automáticamente a partir de [!DNL Workfront] y sus actualizaciones se transferirán a [!DNL Workfront] sin necesidad de una licencia para que [!DNL Workfront] lo haga.

   Solo se actualizan los campos que usted como administrador de [!DNL Workfront] configuró durante la configuración del complemento [!DNL Workfront].

   Para obtener más información sobre cómo sincronizar campos entre Workfront y Jira, consulte la sección [Configurar Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) en [Configurar Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >El problema [!DNL Jira] no se ha asignado a nadie en [!DNL Jira] cuando se crea automáticamente a partir de Workfront.

## Vincular manualmente [!DNL Jira] problemas a [!DNL Workfront] elementos

Una vez creados los elementos en [!DNL Jira] y [!DNL Workfront], independientemente unos de otros, puede vincular manualmente un problema de [!DNL Jira] a una tarea o problema de [!DNL Workfront] existente.\
No puede vincular manualmente un elemento [!DNL Workfront] de [!DNL Workfront] a un elemento [!DNL Jira] existente.

>[!NOTE]
>
>Si el problema [!DNL Jira] no se encuentra en un proyecto que no está identificado como un déclencheur en la integración de [!DNL Workfront], no podrá vincularlo manualmente a un elemento de Workfront al usar la integración con [!DNL Jira] local.\
>Para obtener más información sobre la configuración de déclencheur para el flujo de trabajo de Workfront a Jira, consulte [Vincular automáticamente elementos de Workfront a problemas de Jira](#automatically-link-workfront-items-to-jira-issues).

Cuando los elementos [!DNL Workfront] y [!DNL Jira] están vinculados, ciertos campos de un elemento se pueden actualizar automáticamente en el otro.\
Para obtener más información sobre cómo actualizar los elementos vinculados, vea [Actualizar elementos vinculados entre Jira y Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Para vincular manualmente [!DNL Jira] problemas a [!DNL Workfront] elementos:

1. (Condicional) Inicie sesión en [!DNL Workfront] y busque un problema o una tarea que desee vincular a [!DNL Jira] problema.
1. (Condicional) En la barra de direcciones del elemento, copie la **URL** del elemento en Workfront.

   O

   Desde el área [!UICONTROL Detalles], copie el **[!UICONTROL Número de referencia]** del elemento en Workfront.

   >[!NOTE]
   >
   >Debe tener una licencia de [!DNL Workfront] para iniciar sesión en [!DNL Workfront]. De lo contrario, un usuario de [!DNL Workfront] debe proporcionarle esta información.

1. En [!DNL Jira], vaya a un problema que desee vincular manualmente al elemento [!DNL Workfront].
1. En el panel derecho de [!DNL Workfront], pegue la **URL** o el **[!UICONTROL Número de referencia]** del elemento [!DNL Workfront] al que desea vincular.

1. Haga clic en **[!UICONTROL Vínculo]**.

   Los dos elementos se vinculan y el panel derecho [!DNL Workfront] se rellena con información del elemento [!DNL Workfront].

   Los siguientes [!DNL Workfront] campos están visibles en [!DNL Jira], de forma predeterminada, en el panel derecho de [!DNL Workfront]:

   * El **[!UICONTROL Nombre]** del elemento: puede tener acceso al elemento [!DNL Workfront] haciendo clic en el nombre en el panel.
   * **[!UICONTROL Nombre de proyecto]**
   * El **[!UICONTROL estado]** del elemento
   * La **[!UICONTROL prioridad]** del elemento
   * La fecha en la que se creó en [!DNL Workfront]
   * Las **[!UICONTROL horas planificadas]** del elemento
   * El **[!UICONTROL número de referencia]**: Para tener acceso al elemento [!DNL Workfront], haga clic en el [!UICONTROL número de referencia] en el panel.

Para obtener más información acerca de cómo habilitar campos adicionales para que se muestren en el panel derecho, vea la sección [Configurar la sincronización de campos entre [!DNL Jira] y [!DNL Workfront] Elementos](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) en [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Se publica un comentario del administrador de [!DNL Workfront] asociado con la integración en la ficha **[!DNL Workfront]** del problema [!DNL Jira] para confirmar que se ha creado un nuevo elemento de [!DNL Jira]. El comentario contiene un vínculo al problema [!DNL Jira].

## Desvincular elementos entre [!DNL Jira] y [!DNL Workfront]

Los elementos vinculados entre [!DNL Jira] y [!DNL Workfront] se pueden desvincular manualmente de [!DNL Jira].\
No puede desvincular un elemento [!DNL Workfront] de su homólogo [!DNL Jira] en [!DNL Workfront].

Necesita el siguiente acceso para desvincular el elemento vinculado manualmente:

* Usted es el usuario que vinculó manualmente los elementos
* Usted es el administrador del sistema [!DNL Jira]

Solamente un administrador de [!DNL Workfront] puede desenlazar elementos que se vincularon automáticamente.

Para desvincular un problema de [!DNL Jira] de un elemento de [!DNL Workfront]:

1. En [!DNL Jira], navegue hasta un problema que esté vinculado a una tarea o problema de [!DNL Workfront].
1. Vaya al panel derecho de [!DNL Workfront], haga clic en el icono **[!UICONTROL Desvincular]** y, a continuación, haga clic en **[!UICONTROL Desvincular]**.

   Los elementos enlazados anteriormente [!DNL Jira] y [!DNL Workfront] ahora están desenlazados. Los campos, comentarios o documentos que puedan actualizarse individualmente en el futuro no se actualizan con respecto a su homólogo anterior en la otra aplicación.
