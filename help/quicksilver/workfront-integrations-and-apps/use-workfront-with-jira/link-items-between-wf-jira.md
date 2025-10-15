---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Vincular elementos entre  [!DNL Adobe Workfront]  y  [!DNL Jira]
description: Puede vincular problemas de  [!DNL Jira]  a tareas o problemas de  [!DNL Adobe Workfront]  de forma automática o manual.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: 064418302767ad20e176080ba9a12db548750f3c
workflow-type: tm+mt
source-wordcount: '1324'
ht-degree: 53%

---

# Vincular elementos entre [!DNL Adobe Workfront] y [!DNL Jira]

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>Para ofrecer integraciones más estables y escalables, estamos adoptando un enfoque de integración moderno y flexible mediante la automatización e integración (Fusion) de Workfront. Como parte de este proceso de transición, la integración de Workfront para Jira no estará disponible después del **28 de febrero de 2026**.
>
>Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Jira.
>
>Para obtener una descripción general de la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obtener información sobre las capacidades específicas de los módulos de integración y automatización de Workfront para Jira, consulte [Módulos de software de Jira](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Puede vincular [!DNL Jira] problemas a [!DNL Adobe Workfront] tareas o problemas de forma automática o manual.

Solo se puede vincular un elemento de [!DNL Workfront] a un elemento de [!DNL Jira]. Nunca puede vincular un elemento de [!DNL Workfront] a varios problemas de [!DNL Jira], ni un problema de [!DNL Jira] a varios elementos de [!DNL Workfront].

## Requisitos de acceso

Debe tener lo siguiente:

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/es/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a></td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre las licencias de [!DNL Workfront]</a></td> 
   <td> 
   <p>Nuevo: estándar<p>
   <p>O</p>
   <p>Actual: plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acceso a Jira</td> 
   <td> <p>Acceso de administrador del sistema</p> <p><b>IMPORTANTE</b>

Recomendamos que cree cuentas de administrador del sistema separadas en [!DNL Jira] y [!DNL Workfront] para dedicar a esta integración, en lugar de usar cuentas existentes que puedan estar asociadas a usuarios.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de [!DNL Workfront]. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>.</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creación o modificación de niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para poder vincular elementos entre [!DNL Workfront] y [!DNL Jira], debe hacer lo siguiente:

* Instalar [!DNL Workfront] para [!DNL Jira].

  Para obtener instrucciones, consulte [Instalar Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configure [!DNL Workfront] para Jira.

  Para obtener instrucciones, consulte [Configuración de Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Vincular automáticamente [!DNL Workfront] elementos a [!DNL Jira] problemas

Como administrador de [!DNL Workfront], puede definir déclencheur que crearán automáticamente un problema en [!DNL Jira] cada vez que se cumplan ciertas condiciones en una tarea o un problema en [!DNL Workfront]. Los elementos Workfront y [!DNL Jira] se vinculan.

Una vez que haya completado la configuración de [!DNL Workfront] para Jira, cuando un elemento se cree o se actualice en [!DNL Workfront] para coincidir con tus activadores, se creará automáticamente un nuevo elemento en [!DNL Jira].

Los usuarios de Workfront que crean y actualizan elementos en Workfront no necesitan una licencia de [!DNL Jira] para activar la creación de elementos en [!DNL Jira].

Para obtener más información, consulta [Configurar [!DNL Adobe Workfront] para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Puede crear [!DNL Jira] elementos automáticamente adjuntando una plantilla a un proyecto. Si la plantilla contiene tareas con asignaciones que cumplan con los activadores de [!DNL Jira], las nuevas tareas generarán nuevos problemas de [!DNL Jira].

Vincular automáticamente un problema de [!DNL Workfront] a un problema de [!DNL Jira] es idéntico a vincular automáticamente una tarea de [!DNL Workfront] a un problema de [!DNL Jira].

Para vincular automáticamente una tarea de [!DNL Workfront] a un problema de [!DNL Jira]:

1. Asegúrate de que su [!DNL Jira] administrador del sistema haya configurado activadores para crear automáticamente problemas de [!DNL Jira] cuando se asignen elementos de [!DNL Workfront], luego inicia sesión en [!DNL Workfront] con un nivel de acceso que permita crear una tarea.

   Para obtener más información acerca del acceso a las tareas, consulte [Conceder acceso a las tareas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

{{step1-to-projects}}

1. En la página **Proyectos**, seleccione un proyecto.

1. En el panel izquierdo del proyecto, seleccione **[!UICONTROL Tareas]**.

1. Haga clic en **+ Nueva tarea**.

   >[!NOTE]
   >
   >Para vincular un elemento existente de Workfront a un problema con Jira, selecciona **Editar** en el menú **Más** ![Icono de más](assets/more-icon.png) del elemento.

1. Especifique o actualice cualquiera de los campos disponibles para la tarea.
1. En el campo **[!UICONTROL Asignaciones]**, busque y seleccione el usuario, rol o equipo especificado como déclencheur en la integración de [!DNL Jira].

1. Haga clic en **Crear tarea**. La tarea se crea en Workfront y aparece un nuevo comentario en la ficha **Actualizaciones** de la tarea para indicar que también se ha creado un nuevo problema en [!DNL Jira].

1. (Opcional) En el área **[!UICONTROL Integraciones]** de la sección **[!UICONTROL Detalles]** del encabezado de la tarea o del problema, haga clic en el vínculo **[!UICONTROL Ir a Jira]** para abrir el problema en Jira.

   Su administrador de sistema o de grupo debe añadir el campo [!UICONTROL Integraciones] a su plantilla de diseño para que se muestre en el encabezado de la tarea o problema. Para obtener más información, consulte [Personalización de áreas de objeto con una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Cualquier [!DNL Jira] usuario puede empezar a trabajar inmediatamente en los elementos creados automáticamente desde [!DNL Workfront] y sus actualizaciones se transferirán a [!DNL Workfront] sin necesidad de una licencia de [!DNL Workfront] para hacerlo.

   Solo se actualizan los campos que usted como administrador de [!DNL Workfront] configuró durante la configuración del complemento [!DNL Workfront].

   Para obtener más información sobre cómo sincronizar campos entre Workfront y Jira, consulte la sección Configuración de Workfront para Jira en [Configuración de Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >El problema [!DNL Jira] no se ha asignado a nadie en [!DNL Jira] cuando se crea automáticamente a partir de Workfront.

## Vincular manualmente [!DNL Jira] problemas a [!DNL Workfront] elementos

Una vez creados los elementos en [!DNL Jira] y [!DNL Workfront] de forma independiente entre sí, puede vincular manualmente un problema de [!DNL Jira] a una tarea o problema de [!DNL Workfront] existente.

No puede vincular manualmente un elemento [!DNL Workfront] de [!DNL Workfront] a un elemento [!DNL Jira] existente.

>[!NOTE]
>
>Si el problema de [!DNL Jira] no está en un proyecto que no está identificado como un activador en la [!DNL Workfront] Integración, no puedes vincularlo manualmente a un elemento de Workfront cuando uses la integración con [!DNL Jira] On-Premise .\
>Para obtener más información sobre cómo configurar activadores para el flujo de trabajo de Workfront a Jira, consulte [Vincular automáticamente elementos de Workfront a problemas de Jira](#automatically-link-workfront-items-to-jira-issues).

Cuando los elementos [!DNL Workfront] y [!DNL Jira] están vinculados, ciertos campos de un elemento se pueden actualizar automáticamente en el otro.\
Para obtener más información sobre cómo actualizar los elementos vinculados, consulte [Actualizar elementos vinculados entre Jira y Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Para vincular manualmente problemas de [!DNL Jira] los elementos de [!DNL Workfront]:

1. (Condicional) Inicie sesión en [!DNL Workfront] y busque un problema o una tarea que desee vincular a un problema de [!DNL Jira].
1. (Condicional) En la sección **Información básica** de las pestañas **Detalles de la tarea** o **Detalles del problema**, copie el **[!UICONTROL Número de referencia]** del elemento en Workfront.

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
1. En el panel derecho de [!DNL Workfront], pegue el **[!UICONTROL número de referencia]** o la **URL** del elemento [!DNL Workfront] al que desea vincularlo.

1. Haga clic en **[!UICONTROL Vínculo]**. Los dos elementos se vinculan y el [!DNL Workfront] panel derecho se completa con información del elemento [!DNL Workfront].

   De manera predeterminada, los siguientes [!DNL Workfront] campos están visibles en [!DNL Jira] en el panel derecho de [!DNL Workfront]:

   * El **[!UICONTROL nombre]** del elemento. Puede acceder al elemento [!DNL Workfront] si hace clic en el nombre en el panel.
   * El **[!UICONTROL Nombre De Proyecto]**.
   * El **[!UICONTROL estado]** del elemento.
   * La **[!UICONTROL prioridad]** del elemento.
   * La fecha en la que se creó en [!DNL Workfront].
   * Las **[!UICONTROL horas planificadas]** del elemento.
   * El **[!UICONTROL Número De Referencia]**. Puede obtener acceso al elemento [!DNL Workfront] haciendo clic en el **Número de referencia** en el panel.

   Para obtener más información acerca de cómo habilitar campos adicionales para que se muestren en el panel derecho, vea la sección Configurar la sincronización de campos entre [!DNL Jira] y [!DNL Workfront] elementos en [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Se publica un comentario del administrador de [!DNL Workfront] asociado con la integración en la ficha **[!DNL Workfront]** del problema [!DNL Jira] para confirmar que se ha creado un nuevo elemento de [!DNL Jira]. El comentario contiene un vínculo al problema [!DNL Jira].

## Desvincular elementos entre [!DNL Jira] y [!DNL Workfront]

Los elementos vinculados entre [!DNL Jira] y [!DNL Workfront] se pueden desvincular manualmente en [!DNL Jira]. No se puede desvincular un [!DNL Workfront] elemento de su [!DNL Jira] equivalente en [!DNL Workfront].

Necesita el siguiente acceso para desvincular el elemento vinculado manualmente:

* Usted es el usuario que vinculó manualmente los elementos.
* Usted es el administrador del sistema [!DNL Jira].

>[!NOTE]
>
>Solamente un administrador de [!DNL Workfront] puede desenlazar elementos que se vincularon automáticamente.

Para desvincular un problema de [!DNL Jira] de un elemento de [!DNL Workfront]:

1. Inicie sesión en Jira.
1. Vaya al problema que está vinculado a una tarea o problema de [!DNL Workfront].
1. Vaya al panel derecho de **Workfront**.
1. Haz clic en el icono **[!UICONTROL Desvincular]** y luego haz clic en **[!UICONTROL Desvincular]**. Los elementos enlazados anteriormente [!DNL Jira] y [!DNL Workfront] se desenlazan.

   Cualquiera de sus campos, comentarios o documentos que se actualicen en el futuro no se actualiza en su homólogo anterior de la otra aplicación.
