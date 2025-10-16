---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Actualización de elementos vinculados entre  [!DNL Jira]  y  [!DNL Adobe Workfront]
description: Cuando vincula problemas de  [!DNL Jira]  a tareas o problemas de  [!DNL Adobe Workfront] , los usuarios pueden actualizar los elementos en una aplicación y el equivalente de ese elemento también se actualiza para los usuarios que trabajan en la segunda aplicación.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: b1b55b8046aa771abb2cceda333940ccf827356a
workflow-type: tm+mt
source-wordcount: '1657'
ht-degree: 92%

---

# Actualización de elementos vinculados entre [!DNL Jira] y [!DNL Adobe Workfront]

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

Cuando vincula problemas de [!DNL Jira] a tareas o problemas de [!DNL Adobe Workfront], los usuarios pueden actualizar los elementos en una aplicación y el equivalente de ese elemento también se actualiza para los usuarios que trabajan en la segunda aplicación.

Para obtener más información sobre la vinculación de elementos entre [!DNL Workfront] y [!DNL Jira], consulte [Vinculación de elementos entre Adobe Workfront y Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Al configurar [!DNL Workfront] para [!DNL Jira], como administrador del sistema de [!DNL Jira], puede configurar determinados campos de una aplicación para sincronizarlos con los campos de elementos vinculados en la otra aplicación.

Para obtener más información sobre la sincronización de campos entre los elementos de [!DNL Jira] y [!DNL Workfront] vinculados, consulte [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Acceso a Jira</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Se recomienda crear cuentas de administrador del sistema independientes en Jira y Workfront para dedicarlas a esta integración, en lugar de utilizar las existentes que podrían adjuntarse a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para poder vincular elementos entre [!DNL Workfront] y [!DNL Jira], debe:

* Instalar [!DNL Workfront for Jira]

  Para obtener instrucciones sobre la instalación de [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurar [!DNL Workfront for Jira].

  Para obtener instrucciones sobre la configuración de [!DNL Workfront for Jira], consulte [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Vincular elementos entre [!DNL Workfront] y [!DNL Jira].

  Para obtener instrucciones, consulte [Vinculación de elementos entre  [!DNL Adobe Workfront]  y  [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Actualización de elementos vinculados en [!DNL Workfront]

Si trabaja principalmente en [!DNL Workfront], puede actualizar los elementos de trabajo en [!DNL Workfront] y sus equivalentes en [!DNL Jira] también se actualizan. Esta actualización se produce mediante la integración de [!DNL Workfront] para [!DNL Jira], que no requiere que tenga una licencia de [!DNL Jira].

Siempre que el administrador de [!DNL Workfront] haya configurado [!DNL Workfront for Jira] para sincronizar los campos entre los elementos vinculados, determinados campos que se actualizan en [!DNL Workfront] también se actualizan para el problema de [!DNL Jira] vinculado. Para obtener más información sobre la actualización de elementos en [!DNL Workfront], consulte [Editar problemas](../../manage-work/issues/manage-issues/edit-issues.md) y [Editar tareas](../../manage-work/tasks/manage-tasks/edit-tasks.md).

En la siguiente lista se muestra qué campos de [!DNL Workfront] se sincronizan con los campos de [!DNL Jira] en los elementos vinculados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Campo de [!DNL Workfront] actualizado</strong> </th> 
   <th><strong>Campo sincronizado/actualización de [!DNL Jira]</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue or Task name]</td> 
   <td> <p>[!UICONTROL Issue name]</p> <p>Se añade un comentario sobre el cambio de nombre a la pestaña de <strong>[!DNL Workfront]</strong> del problema de [!DNL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Description]</td> 
   <td> <p> [!UICONTROL Issue Description]</p> <p>Se añade un comentario sobre la descripción actualizada a la pestaña de <strong>[!DNL Workfront]</strong> del problema de [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Uploaded Documents]</p> <p>Nota: Los documentos que se vinculan a los elementos de [!DNL Workfront] desde un servidor externo no se transfieren a los problemas de [!DNL Jira]. Solo los documentos cargados directamente en los elementos de [!DNL Workfront] se actualizan también en los problemas de [!DNL Jira] vinculados. </p> </td> 
   <td> <p>[!UICONTROL Attachments]</p> <p>Se añade un comentario sobre los archivos adjuntos cargados a la pestaña de <strong>[!DNL Workfront]</strong> del problema de [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>[!UICONTROL Due Date]</p> <p>Se añade un comentario sobre el hecho de que [!UICONTROL Due Date] ha cambiado en la pestaña [!DNL Workfront] del problema de [!DNL Jira]. </p> <p>Nota: Debe habilitar <strong>[!UICONTROL Due Date]</strong> para sus problemas de [!DNL Jira] para poder ver este campo actualizado en [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Formularios personalizados y campos personalizados</td> 
   <td> <p> Se muestran en el panel derecho de [!DNL Workfront] del problema de [!DNL Jira]. <br>Solo los campos personalizados que tienen un valor real se muestran en el panel.<br></p> <p>Nota: Las secciones de formularios personalizados se muestran con el nivel de acceso del administrador de [!DNL Workfront]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Priority]</td> 
   <td>Se muestran en el panel derecho de [!DNL Workfront] del problema de [!DNL Jira]. <br>No actualiza el campo <strong>[!UICONTROL Priority]</strong> del problema en [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Log time] </td> 
   <td> <p>Se añade un comentario sobre el tiempo registrado a la pestaña <strong>[!DNL Workfront]</strong> del problema de [!DNL Jira]. Esto incluye el nombre del usuario que registra la hora, así como el usuario para el que se registra la hora, en caso de que sea varíe. No se ha registrado ninguna hora en la pestaña <strong>[!UICONTROL Work log]</strong> en [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comments]</td> 
   <td> <p>El comentario se añade a la pestaña <strong>[!DNL Workfront]</strong> del problema de [!DNL Jira]. No se añade a la pestaña <strong>[!UICONTROL Comments]</strong> del problema de [!DNL Jira].</p> <p>Nota: Cuando vincula dos elementos existentes manualmente, los comentarios que se han añadido al elemento de [!DNL Workfront] antes de vincularlo a [!DNL Jira] no se sincronizan con el problema [!DNL Jira]. </p> <p>Los comentarios de Jira no se sincronizan con Workfront.</td> 
  </tr> 
 </tbody> 
</table>

## Actualización de elementos vinculados en [!DNL Jira]

Si trabaja principalmente en [!DNL Jira], puede actualizar los elementos de trabajo en [!DNL Jira] y sus equivalentes en [!DNL Workfront] también. No necesita una licencia de [!DNL Workfront] para que los elementos de [!DNL Workfront] vinculados a sus problemas de [!DNL Jira] reciban las actualizaciones que está realizando en [!DNL Jira].

Con la condición de que el administrador de [!DNL Workfront] haya configurado [!DNL Workfront] para [!DNL Jira] con el fin de sincronizar los campos entre los elementos vinculados, determinados campos que se actualizan en [!DNL Jira] también se actualizan para el elemento de [!DNL Workfront] vinculado.

La siguiente lista muestra qué campos de [!DNL Jira] se sincronizan con campos de [!DNL Workfront] en elementos vinculados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Campo de [!DNL Jira] actualizado</strong> </th> 
   <th><strong>Campo/Actualización de [!DNL Workfront] sincronizados</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue Status]</td> 
   <td> <p> [!UICONTROL Issue or Task Status]</p> <p>El estado del problema en [!DNL Jira] se sincroniza con los siguientes estados, o estados que equivalen a los siguientes estados, en Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL New] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL In Progress] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Nota: El estado [!DNL Jira] se sincroniza con el primer estado [!DNL Workfront] que equivale al estado apropiado.</p> <p>Para obtener más información sobre los estados de los elementos de [!DNL Workfront], consulte <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Crear o editar un estado</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Issue Attachments]</td> 
   <td> [!UICONTROL Issue or Task Documents]<br>Se añade un comentario sobre la carga de un nuevo documento en [!DNL Jira] a la pestaña [!UICONTROL Updates] del problema o de la tarea de [!DNL Workfront].  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Due Date]</td> 
   <td> <p> Se añade un comentario sobre el cambio de [!UICONTROL Due Date] en [!DNL Jira] a la pestaña [!UICONTROL Updates] del problema o de la tarea de [!DNL Workfront]. </p> <p>Nota: No hay cambios de fechas en el problema o la tarea de [!DNL Workfront]. </p> </td> 
  </tr> 
  <tr> 
   <td> Registro de tiempo en el panel derecho de [!DNL Workfront] o en el menú [!UICONTROL More] del problema de [!DNL Jira]<br></td> 
   <td> <p>Horas<br>Además de añadir las horas registradas en Jira al elemento de [!DNL Workfront] vinculado, se añade un comentario acerca del registro del tiempo a la pestaña [!UICONTROL Updates] del elemento de [!DNL Workfront].</p> <p>Para obtener más información sobre cómo registrar tiempo en los problemas vinculados de [!DNL Jira], incluida la actualización del usuario de [!DNL Jira] que está registrando el tiempo en [!DNL Workfront], consulte <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Registro de tiempo para elementos de [!DNL Jira] y [!DNL Workfront]</a> vinculados.</p> </td> 
  </tr> 
  <tr> 
   <td> Comentarios <br><br></td> 
   <td> <p>Los comentarios se añaden a la pestaña [!UICONTROL Updates] del problema o tarea de [!DNL Workfront] si la configuración de <strong>[!UICONTROL Comments]</strong> de la sección [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] de la pestaña [!UICONTROL Setup] es <strong>[!UICONTROL Always]</strong>.</p> <p>Para obtener información acerca de la configuración de Workfront en [!DNL Jira], consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuración de [!DNL Workfront for Jira]</a>.</p> <p>Para obtener información sobre cómo comentar elementos de problemas vinculados de [!DNL Jira], consulte <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Comentario de un problema vinculado de [!DNL Jira]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Registro de tiempo de problemas de [!DNL Jira] vinculados

El tiempo que registre para un elemento de [!DNL Jira] en [!DNL Jira] también se transferirá al elemento de [!DNL Workfront] vinculado, independientemente de dónde registre el tiempo en [!DNL Jira].\
Cuando registra tiempo en Jira en el panel de [!DNL Workfront], el tiempo solo se registra en [!DNL Workfront].\
El tiempo que registre en [!DNL Workfront] no afecta al tiempo del problema vinculado en [!DNL Jira].

>[!NOTE]
>
>Si la hora se añade a un elemento [!DNL Jira] vinculado a una tarea [!DNL Workfront], el [!UICONTROL Tipo de hora] para la hora en [!DNL Workfront] es [!UICONTROL Tiempo de tarea]. Si la hora se añade a un elemento de [!DNL Jira] vinculado a un problema de [!DNL Workfront], el [!UICONTROL Tipo de hora] para el tiempo de [!DNL Workfront] es [!UICONTROL Tiempo de problema].

Se añade un comentario a la **[!DNL Workfront]** pestaña en [!DNL Jira] y a la pestaña **[!UICONTROL Actualizaciones]** del elemento en [!DNL Workfront] para registrar el registro de la hora.\
La hora también se muestra en la pestaña **[!UICONTROL Horas]** del elemento [!DNL Workfront].

* [Registrar tiempo para  [!DNL Jira] vinculados y [!DNL Workfront] elementos](#log-time-for-linked-jira-and-workfront-items)
* [Registrar tiempo desde [!DNL Jira] hasta un elemento [!DNL Workfront] &#x200B;](#log-time-from-jira-to-a-workfront-item)

### Registrar tiempo para [!DNL Jira] vinculados y elementos [!DNL Workfront]

Puede registrar el tiempo desde un problema de [!DNL Jira] vinculado hasta un elemento de [!DNL Workfront], mientras que el tiempo se registra tanto en el problema de [!DNL Jira] como en el elemento de [!DNL Workfront].

>[!IMPORTANT]
>
>Si el usuario que registra la hora en [!DNL Jira] no existe en [!DNL Workfront], la integración crea un nuevo usuario activo en Workfront si **[!UICONTROL Cree automáticamente un usuario en [!DNL Workfront]si el [!DNL Jira] usuario no tiene una *[!DNL Workfront]cuenta]** se establece en&#x200B;**[!UICONTROL &#x200B; Siempre &#x200B;]**. Este usuario no ocupa una licencia de [!DNL Workfront]. Puede asignar usuarios activos a elementos de trabajo en [!DNL Workfront], pero no puede incluirlos en las actualizaciones. Para obtener información acerca de cómo configurar la creación automática de [!DNL Workfront] usuarios de [!DNL Jira], consulte [Configurar [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Para registrar el tiempo de un elemento en [!DNL Jira] y que se registre tanto en [!DNL Jira] como en [!DNL Workfront]:

1. Inicie sesión en [!DNL Jira].
1. Vaya al problema [!DNL Jira] que está vinculado al elemento [!DNL Workfront].
1. Expanda el menú **[!UICONTROL Más]** y haga clic en **[!UICONTROL Registro del trabajo]**.

1. En el campo **[!UICONTROL Tiempo empleado]** especifique la cantidad de tiempo empleado trabajando en este problema. Debe especificar el tiempo utilizando los siguientes períodos de tiempo:

   * [!UICONTROL Semanas] (s)
   * [!UICONTROL Días] (d)
   * [!UICONTROL Horas] (h)

1. Continúe añadiendo información a su entrada de tiempo, incluida una **[!UICONTROL Descripción del trabajo]**, y después haga clic en **[!UICONTROL Registro]**.\
   La hora se añade a la pestaña **[!UICONTROL Registro de trabajo]** del elemento [!DNL Jira], así como al elemento [!DNL Workfront] vinculado a él.\
   La descripción de trabajo de la entrada de tiempo se registra como una nota en la entrada de horas en [!DNL Workfront].

### Registrar tiempo desde [!DNL Jira] hasta un elemento [!DNL Workfront]

Puede registrar tiempo solo en el elemento [!DNL Workfront] vinculado desde el problema [!DNL Jira] sin registrar este tiempo en el problema [!DNL Jira].

1. Iniciar sesión en [!DNL Jira].
1. Navegue hasta un problema [!DNL Jira] que esté vinculado a un elemento [!DNL Workfront].

   Los detalles del elemento [!DNL Workfront] deben mostrarse en el panel derecho [!DNL Workfront] del problema.

1. Haga clic en el icono **[!UICONTROL Registrar tiempo]**.

1. Especifique la cantidad de **[!UICONTROL horas]** y **[!UICONTROL minutos]** que desea registrar para el problema.

1. Haga clic en **[!UICONTROL Registrar tiempo]**.

   La hora se añade al elemento [!DNL Workfront].

   Esta vez no se agregó a la pestaña [!UICONTROL Registro de trabajo] del problema [!DNL Jira].

## Comentar desde un problema [!DNL Jira] vinculado {#comment-from-a-linked-jira-issue}

Cuando comenta un elemento de [!DNL Jira] desde el panel derecho de [!DNL Workfront] en [!DNL Jira], el comentario también se añade a la pestaña [!UICONTROL Actualizaciones] del elemento vinculado en Workfront.

Para comentar desde [!DNL Jira] hasta un elemento de [!DNL Workfront]:

1. Inicie sesión en [!DNL Jira].
1. Navegue hasta un problema [!DNL Jira] que esté vinculado a un elemento [!DNL Workfront].

   Los detalles del elemento [!DNL Workfront] deben mostrarse en el panel derecho [!DNL Workfront] del problema.

1. Haga clic en el icono **[!UICONTROL Comentarios]** en el panel [!DNL Workfront] o en la pestaña **[!UICONTROL Comentarios]**.

1. Empiece a escribir un comentario y, a continuación, haga clic en **[!UICONTROL Enviar]**.

   El comentario se añade a lo siguiente:

   * La pestaña **[!DNL Workfront]** del problema [!DNL Jira].
   * La pestaña **[!UICONTROL Comentarios]** del problema [!DNL Jira].
   * La pestaña **[!UICONTROL Actualizaciones]** del elemento vinculado en Workfront.
