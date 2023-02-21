---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Actualizar elementos vinculados entre [!DNL Jira] y [!DNL Adobe Workfront]
description: Al vincular [!DNL Jira] problemas con [!DNL Adobe Workfront] tareas o problemas, los usuarios pueden actualizar elementos en una aplicación y la contrapartida de ese elemento también se actualiza para los usuarios que trabajan en la segunda aplicación.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 0%

---

# Actualizar elementos vinculados entre [!DNL Jira] y [!DNL Adobe Workfront]

Al vincular [!DNL Jira] problemas con [!DNL Adobe Workfront] tareas o problemas, los usuarios pueden actualizar elementos en una aplicación y la contrapartida de ese elemento también se actualiza para los usuarios que trabajan en la segunda aplicación.

Para obtener más información sobre la vinculación de elementos entre [!DNL Workfront] y [!DNL Jira], consulte [Vincular elementos entre Adobe Workfront y Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

A medida que va configurando [!DNL Workfront] para [!DNL Jira], como [!DNL Jira] administrador del sistema, puede configurar ciertos campos de una aplicación para que se sincronicen con los campos de elementos vinculados de la otra aplicación.

Para obtener más información sobre la sincronización de campos entre vínculos [!DNL Jira] y [!DNL Workfront] elementos, consulte [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] información general sobre licencias</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Se recomienda crear cuentas de administrador del sistema independientes en [!DNL Jira] y [!DNL Workfront] para dedicarse a esta integración, en lugar de usar las existentes que se podrían adjuntar a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Antes de poder vincular elementos entre [!DNL Workfront] y [!DNL Jira], debe

* Instalar [!DNL Workfront for Jira].

   Para obtener instrucciones sobre la instalación [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurar [!DNL Workfront for Jira].

   Para obtener instrucciones sobre la configuración [!DNL Workfront for Jira], consulte [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Vincular elementos entre [!DNL Workfront] y [!DNL Jira].

   Para obtener instrucciones, consulte [Vincular elementos entre [!DNL Adobe Workfront] y [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Actualizar elementos vinculados en [!DNL Workfront]

Si trabaja principalmente en [!DNL Workfront], puede actualizar los elementos de trabajo en [!DNL Workfront] y sus homólogos de [!DNL Jira] actualizar también. Esta actualización se produce mediante la integración de [!DNL Workfront] para [!DNL Jira] que no requiere que tenga un [!DNL Jira] licencia.

Mientras su [!DNL Workfront] administrador configurado [!DNL Workfront for Jira] para sincronizar los campos entre elementos vinculados, ciertos campos que se actualizan en [!DNL Workfront] actualizar también para el [!DNL Jira] problema. Para obtener más información sobre la actualización de elementos en [!DNL Workfront], consulte [Editar problemas](../../manage-work/issues/manage-issues/edit-issues.md) y [Editar tareas](../../manage-work/tasks/manage-tasks/edit-tasks.md).

La siguiente lista muestra cuál [!DNL Workfront] campos sincronizar [!DNL Jira] campos en elementos vinculados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Actualizado [!DNL Workfront] field</strong> </th> 
   <th><strong>Sincronizado [!DNL Jira] field/ update</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Problema o nombre de tarea]</td> 
   <td> <p>[!UICONTROL Nombre del problema]</p> <p>Se agrega un comentario sobre el cambio de nombre al <strong>[!DNL Workfront]</strong> de la pestaña [!DNL Jira] problema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema o Descripción de tarea]</td> 
   <td> <p> [!UICONTROL Problema Descripción]</p> <p>Se agrega un comentario sobre la Descripción actualizada al <strong>[!DNL Workfront]</strong> de la pestaña [!DNL Jira] problema.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Documentos cargados]</p> <p>Nota: Documentos vinculados a [!DNL Workfront] los elementos de un servidor externo no se transfieren a [!DNL Jira] problemas. Solo los documentos cargados directamente en [!DNL Workfront] los elementos también se actualizan al [!DNL Jira] problemas. </p> </td> 
   <td> <p>[!UICONTROL Attachments]</p> <p>Se agrega un comentario sobre los archivos adjuntos cargados a la variable <strong>[!DNL Workfront]</strong> de la pestaña [!DNL Jira] problema.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de finalización prevista]</td> 
   <td> <p>[!UICONTROL Fecha de vencimiento]</p> <p>Se agrega un comentario sobre el [!UICONTROL Fecha de vencimiento] que ha cambiado a la variable [!DNL Workfront] de la pestaña [!DNL Jira] problema. </p> <p>Nota: Debe habilitar <strong>[!UICONTROL Fecha de vencimiento]</strong> para su [!DNL Jira] problemas para poder ver este campo actualizado en [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Forms personalizado y campos personalizados</td> 
   <td> <p> Mostrar en la [!DNL Workfront] panel derecho del [!DNL Jira] problema. <br>En el panel solo se muestran los campos personalizados que tienen un valor real.<br></p> <p>Nota: Las secciones Formulario personalizado se muestran con el nivel de acceso de la variable [!DNL Workfront] administrador. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema o prioridad de tareas]</td> 
   <td>Se muestra en la [!DNL Workfront] panel derecho del [!DNL Jira] problema. <br>No actualiza el problema <strong>[!UICONTROL Priority]</strong> en [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Log time] </td> 
   <td> <p>Se agrega un comentario sobre la hora registrada en la variable <strong>[!DNL Workfront]</strong> de la pestaña [!DNL Jira] problema. Esto incluye el nombre del usuario que registra la hora, así como el usuario para el que se registra la hora, en caso de que sean diferentes. No hay tiempo de que se inicie sesión en el <strong>[!UICONTROL Work log]</strong> en [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comentarios]</td> 
   <td> <p>El comentario se agrega al <strong>[!DNL Workfront]</strong> de la pestaña [!DNL Jira] problema. No se agrega al <strong>[!UICONTROL Comentarios]</strong> de la pestaña [!DNL Jira] problema</p> <p>Nota: Cuando vincula dos elementos existentes manualmente, los comentarios que se agregaron al informe [!DNL Workfront] elemento antes de vincularlo a [!DNL Jira] no sincronizar con [!DNL Jira] problema. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Actualizar elementos vinculados en [!DNL Jira]

Si trabaja principalmente en [!DNL Jira], puede actualizar los elementos de trabajo en [!DNL Jira] y sus homólogos de [!DNL Workfront] actualizar también. No tiene que tener un [!DNL Workfront] licencia para [!DNL Workfront] elementos vinculados a su [!DNL Jira] problemas para recibir las actualizaciones que está realizando en [!DNL Jira].

Con la condición de que [!DNL Workfront] administrador configurado [!DNL Workfront] para [!DNL Jira] para sincronizar los campos entre elementos vinculados, ciertos campos que se actualizan en [!DNL Jira] actualizar también para el [!DNL Workfront] elemento.

La siguiente lista muestra cuál [!DNL Jira] campos sincronizar [!DNL Workfront] campos en elementos vinculados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Actualizado [!DNL Jira] Campo</strong> </th> 
   <th><strong>Sincronizado [!DNL Workfront] Campo/Actualización</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Estado del problema]</td> 
   <td> <p> [!UICONTROL Problema o estado de tarea]</p> <p>Estado del problema en [!DNL Jira] se sincroniza con los siguientes estados o estados que se equiparan con los siguientes estados en Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL Nuevo] ([!UICONTROL NUEVO])</p> </li> 
     <li> <p>[!UICONTROL In Progress] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Cerrado]/[!UICONTROL Completado] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Nota: La variable [!DNL Jira] se sincroniza el estado con la primera [!DNL Workfront] estado que equivale al estado adecuado.</p> <p>Para obtener más información sobre los estados de los elementos de [!DNL Workfront], consulte <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Crear o editar un estado</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema asignado]</td> 
   <td> <p> [!UICONTROL Problema o asignador de tareas]</p> <p>Importante: Al asignar un artículo en [!DNL Jira] a un usuario que no tiene un [!DNL Workfront] cuenta, la integración crea un nuevo usuario activo en [!DNL Workfront] solo cuando la opción "[!UICONTROL Crear automáticamente un usuario en [!DNL Workfront] si la variable [!DNL Jira] el usuario no tiene un [!DNL Workfront] account]" se establece en [!UICONTROL Always]. Este usuario no ocupa un [!DNL Workfront] licencia. Los usuarios activos pueden asignarse a elementos de trabajo en [!DNL Workfront], pero no se puede incluir en las actualizaciones. Para obtener más información sobre la configuración de la creación automática de [!DNL Workfront] usuarios de [!DNL Jira], consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuración [!DNL Workfront for Jira]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema con los archivos adjuntos]</td> 
   <td> [!UICONTROL Problema o documentos de tarea]<br>Un comentario sobre la carga de un nuevo documento en [!DNL Jira] se añade a la pestaña [!UICONTROL Actualizaciones] de la variable [!DNL Workfront] problema o tarea.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de vencimiento]</td> 
   <td> <p> Un comentario sobre el cambio de la [!UICONTROL Fecha de vencimiento] en [!DNL Jira] se añade a la pestaña [!UICONTROL Actualizaciones] de la variable [!DNL Workfront] problema o tarea. </p> <p>Nota: Ninguna fecha cambia en la variable [!DNL Workfront] problema o tarea. </p> </td> 
  </tr> 
  <tr> 
   <td> Tiempo de inicio de sesión en la variable [!DNL Workfront] panel derecho o desde el menú [!UICONTROL Más] en el [!DNL Jira] problema<br></td> 
   <td> <p>Horas<br>Además de añadir las horas registradas en Jira al [!DNL Workfront] , se agrega un comentario sobre el tiempo de registro a la pestaña [!UICONTROL Actualizaciones] del [!DNL Workfront] elemento.</p> <p>Para obtener más información sobre el tiempo de inicio de sesión en los vínculos [!DNL Jira] problemas, incluida la actualización de [!DNL Jira] usuario que está iniciando sesión [!DNL Workfront], consulte <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Hora de registro de Linked [!DNL Jira] y [!DNL Workfront] items</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Comentarios <br><br></td> 
   <td> <p>Los comentarios se añaden a la pestaña [!UICONTROL Actualizaciones] del [!DNL Workfront] problema o tarea si la variable <strong>[!UICONTROL Comentarios]</strong> en la sección [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] de la pestaña [!UICONTROL Setup] para <strong>[!UICONTROL Siempre]</strong>.</p> <p>Para obtener información sobre la configuración de Workfront en [!DNL Jira], consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuración [!DNL Workfront for Jira]</a>.</p> <p>Para obtener información sobre los comentarios de elementos vinculados [!DNL Jira] problemas, consulte <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Comentario desde un vínculo [!DNL Jira] problema</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tiempo de registro vinculado [!DNL Jira] problemas

La hora que se registra para un [!DNL Jira] elemento en [!DNL Jira] también se transferirá al [!DNL Workfront] elemento, independientemente de donde [!DNL Jira] registra la hora.\
Cuando inicia sesión en Jira, en la [!DNL Workfront] , la hora solo se registra en [!DNL Workfront].\
La hora en la que se registra [!DNL Workfront] no afecta al tiempo del problema relacionado en [!DNL Jira].

>[!NOTE]
>
>Si la hora se agrega a un [!DNL Jira] elemento vinculado a un [!DNL Workfront] tarea, la variable [!UICONTROL Tipo de hora] para el tiempo en [!DNL Workfront] es [!UICONTROL Hora de la tarea]. Si la hora se agrega a un [!DNL Jira] elemento vinculado a un [!DNL Workfront] el problema, [!UICONTROL Tipo de hora] para el tiempo en [!DNL Workfront] es [!UICONTROL Hora del problema].

Se agrega un comentario al **[!DNL Workfront]** en [!DNL Jira] y **[!UICONTROL Actualizaciones]** del elemento en [!DNL Workfront] para registrar la hora.\
La hora también se muestra en la variable **[!UICONTROL Horas]** de la pestaña [!DNL Workfront] elemento.

* [Hora de registro de Linked [!DNL Jira] y [!DNL Workfront] items](#log-time-for-linked-jira-and-workfront-items)
* [Hora de registro desde [!DNL Jira] a [!DNL Workfront] item](#log-time-from-jira-to-a-workfront-item)

### Hora de registro de Linked [!DNL Jira] y [!DNL Workfront] items

Puede registrar la hora desde un [!DNL Jira] problema vinculado a un [!DNL Workfront] y la hora se registra en la variable [!DNL Jira] así como el [!DNL Workfront] elemento.

>[!IMPORTANT]
>
>Si el usuario inicia sesión [!DNL Jira] no existe en [!DNL Workfront], la integración crea un nuevo usuario activo en Workfront si la variable **[!UICONTROL Crear automáticamente un usuario en [!DNL Workfront]&#x200B; si la variable [!DNL Jira] el usuario no tiene un *[!DNL Workfront]&#x200B; cuenta]** está configurado como**[!UICONTROL  Siempre ]**. Este usuario no ocupa un [!DNL Workfront] licencia. Puede asignar usuarios activos a elementos de trabajo en [!DNL Workfront], pero no puede incluirlos en las actualizaciones. Para obtener información sobre cómo configurar la creación automática de [!DNL Workfront] usuarios de [!DNL Jira], consulte [Configuración [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Para registrar la hora de un elemento en [!DNL Jira] y hacer que se registre tanto en [!DNL Jira] y [!DNL Workfront]:

1. Iniciar sesión [!DNL Jira].
1. Vaya a la [!DNL Jira] problema vinculado al [!DNL Workfront] elemento.
1. Expanda el **[!UICONTROL Más]** y haga clic en **[!UICONTROL Trabajo de registro]**.

1. En el **[!UICONTROL Tiempo empleado]** especifique la cantidad de tiempo empleado en este problema. Debe especificar el tiempo mediante los siguientes períodos de tiempo:

   * [!UICONTROL Semanas] w)
   * [!UICONTROL Días] d)
   * [!UICONTROL Horas] h)

1. Continúe agregando información a su entrada horaria, incluido un **[!UICONTROL Descripción del trabajo]** y haga clic en **[!UICONTROL Registro]**.\
   La hora se agrega a la variable **[!UICONTROL Registro de trabajo]** de la pestaña [!DNL Jira] , así como al [!DNL Workfront] elemento vinculado a él.\
   La descripción de trabajo de la entrada de tiempo se registra como una nota en la entrada de hora en [!DNL Workfront].

### Hora de registro desde [!DNL Jira] a [!DNL Workfront] item

Puede registrar la hora solo en el vínculo [!DNL Workfront] del [!DNL Jira] sin registrar esta vez en el [!DNL Jira] problema.

1. Iniciar sesión [!DNL Jira].
1. Vaya a un [!DNL Jira] problema vinculado a un [!DNL Workfront] elemento.

   Los detalles del [!DNL Workfront] el elemento debe mostrarse en la [!DNL Workfront] panel derecho del problema.

1. Haga clic en el **[!UICONTROL Tiempo de registro]** icono.

1. Especifique la cantidad de **[!UICONTROL Horas]** y **[!UICONTROL Minutos]** desea registrar el problema.

1. Haga clic en **[!UICONTROL Tiempo de registro]**.

   La hora se agrega a la variable [!DNL Workfront] elemento.

   Esta vez no se agrega al [!UICONTROL Registro de trabajo] de la pestaña [!DNL Jira] problema.

## Comentario desde un vínculo [!DNL Jira] problema {#comment-from-a-linked-jira-issue}

Cuando realiza comentarios en un [!DNL Jira] del [!DNL Workfront] panel derecho en [!DNL Jira], el comentario también se agrega al [!UICONTROL Actualizaciones] del elemento vinculado en Workfront.

Para comentar desde [!DNL Jira] a [!DNL Workfront] elemento:

1. Iniciar sesión [!DNL Jira].
1. Vaya a un [!DNL Jira] problema vinculado a un [!DNL Workfront] elemento.

   Los detalles del [!DNL Workfront] el elemento debe mostrarse en la [!DNL Workfront] panel derecho del problema.

1. Haga clic en el **[!UICONTROL Comentarios]** en el [!DNL Workfront] o en el **[!UICONTROL Comentarios]** pestaña .

1. Comience a escribir un comentario y haga clic en **[!UICONTROL Enviar]**.

   El comentario se agrega a lo siguiente:

   * La variable **[!DNL Workfront]** de la pestaña [!DNL Jira] problema.
   * La variable **[!UICONTROL Comentarios]** de la pestaña [!DNL Jira] problema.
   * La variable **[!UICONTROL Actualizaciones]** del elemento vinculado en Workfront.
