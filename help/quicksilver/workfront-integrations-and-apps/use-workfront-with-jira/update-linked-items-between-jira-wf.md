---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Actualizar elementos vinculados entre  [!DNL Jira] y [!DNL Adobe Workfront]
description: Cuando vincula  [!DNL Jira] problemas a [!DNL Adobe Workfront] tareas o problemas, los usuarios pueden actualizar los elementos en una aplicación y la contraparte de ese elemento también se actualiza para los usuarios que trabajan en la segunda aplicación.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: e01f5eaf3133fa1bdaedf4dad56e9a8175b70667
workflow-type: tm+mt
source-wordcount: '1570'
ht-degree: 0%

---

# Actualizar elementos vinculados entre [!DNL Jira] y [!DNL Adobe Workfront]

Cuando vincula [!DNL Jira] problemas a [!DNL Adobe Workfront] tareas o problemas, los usuarios pueden actualizar los elementos en una aplicación y la contraparte de ese elemento también se actualiza para los usuarios que trabajan en la segunda aplicación.

Para obtener más información sobre cómo vincular elementos entre [!DNL Workfront] y [!DNL Jira], vea [Vincular elementos entre Adobe Workfront y Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Al configurar [!DNL Workfront] para [!DNL Jira], como administrador del sistema de [!DNL Jira], puede configurar ciertos campos de una aplicación para sincronizarlos con campos de elementos vinculados en la otra aplicación.

Para obtener más información sobre cómo sincronizar campos entre [!DNL Jira] y [!DNL Workfront] elementos vinculados, consulte [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td><p>Nuevo: Cualquiera</p>
       <p>o</p>
       <p>Actual: [!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Nuevo: [!UICONTROL Standard]</p>
       <p>o</p>
       <p>Actual: [!UICONTROL plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Se recomienda crear cuentas de administrador del sistema independientes en [!DNL Jira] y [!DNL Workfront] para dedicarlas a esta integración, en lugar de usar las existentes que podrían adjuntarse a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

Para poder vincular elementos entre [!DNL Workfront] y [!DNL Jira], debe:

* Instalar [!DNL Workfront for Jira].

  Para obtener instrucciones sobre la instalación de [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurar [!DNL Workfront for Jira].

  Para obtener instrucciones sobre cómo configurar [!DNL Workfront for Jira], consulte [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Vincular elementos entre [!DNL Workfront] y [!DNL Jira].

  Para obtener instrucciones, vea [Vincular elementos entre [!DNL Adobe Workfront] y [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Actualizar elementos vinculados en [!DNL Workfront]

Si trabaja principalmente en [!DNL Workfront], puede actualizar los elementos de trabajo en [!DNL Workfront] y sus equivalentes en [!DNL Jira] también. Esta actualización se produce mediante la integración de [!DNL Workfront] para [!DNL Jira], que no requiere que tenga una licencia de [!DNL Jira].

Siempre que el administrador de [!DNL Workfront] haya configurado [!DNL Workfront for Jira] para sincronizar los campos entre los elementos vinculados, ciertos campos que se actualizan en [!DNL Workfront] también se actualizan para el problema de [!DNL Jira] vinculado. Para obtener más información acerca de la actualización de elementos en [!DNL Workfront], vea [Editar problemas](../../manage-work/issues/manage-issues/edit-issues.md) y [Editar tareas](../../manage-work/tasks/manage-tasks/edit-tasks.md).

La siguiente lista muestra qué [!DNL Workfront] campos se sincronizan con [!DNL Jira] campos en elementos vinculados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Se ha actualizado el campo [!DNL Workfront]</strong> </th> 
   <th><strong>Campo/ actualización [!DNL Jira] sincronizados</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Problema o nombre de tarea]</td> 
   <td> <p>[!UICONTROL Nombre de problema]</p> <p>Se agrega un comentario sobre el cambio de nombre a la ficha <strong>[!DNL Workfront]</strong> del problema [!DNL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema o Descripción de tarea]</td> 
   <td> <p> [!UICONTROL Descripción del problema]</p> <p>Se agrega un comentario sobre la descripción actualizada a la ficha <strong>[!DNL Workfront]</strong> del problema [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Documentos cargados]</p> <p>Nota: Los documentos vinculados a [!DNL Workfront] elementos de un servidor externo no se transfieren a [!DNL Jira] problemas. Solo los documentos cargados directamente en [!DNL Workfront] elementos también se actualizan a los [!DNL Jira] problemas vinculados. </p> </td> 
   <td> <p>[!UICONTROL Archivos adjuntos]</p> <p>Se agrega un comentario sobre los archivos adjuntos cargados a la ficha <strong>[!DNL Workfront]</strong> del problema [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha planificada de finalización]</td> 
   <td> <p>[!UICONTROL Fecha de vencimiento]</p> <p>Se agrega un comentario acerca de que [!UICONTROL Fecha de vencimiento] ha cambiado a la ficha [!DNL Workfront] del problema [!DNL Jira]. </p> <p>Nota: Debe habilitar <strong>[!UICONTROL Fecha de vencimiento]</strong> para que sus [!DNL Jira] problemas puedan ver este campo actualizado en [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Forms personalizado y campos personalizados</td> 
   <td> <p> Mostrar en el panel derecho [!DNL Workfront] del problema [!DNL Jira]. <br>En el panel solo se muestran los campos personalizados que tienen un valor real.<br></p> <p>Nota: Las secciones de formularios personalizados se muestran con el nivel de acceso del administrador [!DNL Workfront]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema o prioridad de tarea]</td> 
   <td>Se muestra en el panel derecho [!DNL Workfront] del problema [!DNL Jira]. <br>No se actualiza el campo <strong>[!UICONTROL Priority]</strong> del problema en [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hora de registro] </td> 
   <td> <p>Se agrega un comentario sobre el tiempo registrado en la ficha <strong>[!DNL Workfront]</strong> del problema [!DNL Jira]. Esto incluye el nombre del usuario que registra la hora, así como el usuario para el que se registra la hora, en caso de que sea diferente. No se registró ninguna hora en la ficha <strong>[!UICONTROL Registro de trabajo]</strong> en [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comentarios]</td> 
   <td> <p>El comentario se agrega a la ficha <strong>[!DNL Workfront]</strong> del problema [!DNL Jira]. No se agregó a la ficha <strong>[!UICONTROL Comentarios]</strong> del problema [!DNL Jira]</p> <p>Nota: Cuando vincula dos elementos existentes manualmente, los comentarios que se agregaron al elemento [!DNL Workfront] antes de vincularlo a [!DNL Jira] no se sincronizan con el problema [!DNL Jira]. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Actualizar elementos vinculados en [!DNL Jira]

Si trabaja principalmente en [!DNL Jira], puede actualizar los elementos de trabajo en [!DNL Jira] y sus equivalentes en [!DNL Workfront] también. No necesita una licencia de [!DNL Workfront] para los [!DNL Workfront] elementos vinculados a sus [!DNL Jira] problemas para recibir las actualizaciones que está realizando en [!DNL Jira].

Con la condición de que el administrador de [!DNL Workfront] haya configurado [!DNL Workfront] para [!DNL Jira] con el fin de sincronizar los campos entre los elementos vinculados, ciertos campos que se actualizan en [!DNL Jira] también se actualizan para el elemento [!DNL Workfront] vinculado.

La siguiente lista muestra qué [!DNL Jira] campos se sincronizan con [!DNL Workfront] campos en elementos vinculados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Se ha actualizado el campo [!DNL Jira]</strong> </th> 
   <th><strong>Campo/ Actualización [!DNL Workfront] Sincronizado</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Estado del problema]</td> 
   <td> <p> [!UICONTROL Estado de tarea o problema]</p> <p>El estado del problema en [!DNL Jira] se sincroniza con los siguientes estados, o estados que se igualan con los siguientes estados, en Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL Nuevo] ([!UICONTROL NUEVO])</p> </li> 
     <li> <p>[!UICONTROL En curso] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Cerrado]/[!UICONTROL Completado] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Nota: El estado [!DNL Jira] se sincroniza con el primer estado [!DNL Workfront] que coincide con el estado apropiado.</p> <p>Para obtener más información sobre los estados de los elementos de [!DNL Workfront], vea <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Crear o editar un estado</a>.</p> </td> 
  </tr>
  <tr> 
   <td>Archivos adjuntos de [!UICONTROL Issue]</td> 
   <td> [!UICONTROL Problema o documentos de tarea]<br>Se agrega un comentario acerca de la carga de un nuevo documento en [!DNL Jira] a la ficha [!UICONTROL Actualizaciones] del problema o tarea [!DNL Workfront].  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de vencimiento]</td> 
   <td> <p> Se agrega un comentario acerca del cambio de [!UICONTROL Fecha de vencimiento] en [!DNL Jira] a la ficha [!UICONTROL Actualizaciones] del problema o tarea [!DNL Workfront]. </p> <p>Nota: No hay cambios de fechas en el problema o la tarea [!DNL Workfront]. </p> </td> 
  </tr> 
  <tr> 
   <td> Registrar tiempo en el panel derecho de [!DNL Workfront] o en el menú [!UICONTROL Más] del problema [!DNL Jira]<br></td> 
   <td> <p>Horas<br>Además de agregar las horas registradas en Jira al elemento [!DNL Workfront] vinculado, se agrega un comentario acerca del registro del tiempo a la ficha [!UICONTROL Actualizaciones] del elemento [!DNL Workfront].</p> <p>Para obtener más información sobre el registro de tiempo en los problemas vinculados de [!DNL Jira], incluida la actualización del usuario de [!DNL Jira] que está registrando el tiempo en [!DNL Workfront], vea <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Registrar tiempo para elementos vinculados de [!DNL Jira] y [!DNL Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Comentarios <br><br></td> 
   <td> <p>Los comentarios se agregan a la ficha [!UICONTROL Actualizaciones] del problema o tarea [!DNL Workfront] si la configuración <strong>[!UICONTROL Comentarios]</strong> de la sección [!UICONTROL SINCRONIZAR DE JIRA A WORKFRONT] de la ficha [!UICONTROL Configuración] es <strong>[!UICONTROL Siempre]</strong>.</p> <p>Para obtener información acerca de la configuración de Workfront en [!DNL Jira], vea <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configurar [!DNL Workfront for Jira]</a>.</p> <p>Para obtener información sobre cómo comentar elementos de problemas vinculados de [!DNL Jira], consulte <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Comentario de un problema vinculado de [!DNL Jira]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Registrar tiempo de [!DNL Jira] problemas vinculados

La hora que registre para un elemento de [!DNL Jira] en [!DNL Jira] también se transferirá al elemento de [!DNL Workfront] vinculado, independientemente de dónde registre la hora en [!DNL Jira].\
Cuando registra tiempo en Jira en el panel [!DNL Workfront], el tiempo solo se registra en [!DNL Workfront].\
El tiempo que registre en [!DNL Workfront] no afecta el tiempo del problema vinculado en [!DNL Jira].

>[!NOTE]
>
>Si la hora se agrega a un elemento [!DNL Jira] vinculado a una tarea [!DNL Workfront], el [!UICONTROL tipo de hora] para la hora en [!DNL Workfront] es [!UICONTROL tiempo de tarea]. Si la hora se agrega a un elemento de [!DNL Jira] vinculado a un problema de [!DNL Workfront], el [!UICONTROL tipo de hora] para el tiempo de [!DNL Workfront] es [!UICONTROL tiempo de problema].

Se agrega un comentario a la ficha **[!DNL Workfront]** en [!DNL Jira] y a la ficha **[!UICONTROL Actualizaciones]** del elemento en [!DNL Workfront] para registrar el registro de la hora.\
La hora también se muestra en la ficha **[!UICONTROL Horas]** del elemento [!DNL Workfront].

* [Registrar tiempo para elementos enlazados [!DNL Jira] y [!DNL Workfront] elementos](#log-time-for-linked-jira-and-workfront-items)
* [Registrar tiempo de  [!DNL Jira]  a  [!DNL Workfront] elemento](#log-time-from-jira-to-a-workfront-item)

### Registrar tiempo para elementos enlazados [!DNL Jira] y [!DNL Workfront]

Puede registrar el tiempo de un problema de [!DNL Jira] vinculado a un elemento de [!DNL Workfront], y el tiempo se registra tanto en el problema de [!DNL Jira] como en el elemento de [!DNL Workfront].

>[!IMPORTANT]
>
>Si el usuario que registra la hora en [!DNL Jira] no existe en [!DNL Workfront], la integración crea un nuevo usuario activo en Workfront si **[!UICONTROL Crea automáticamente un usuario en [!DNL Workfront] si el usuario [!DNL Jira] no tiene una *cuenta [!DNL Workfront]]** se establece en**[!UICONTROL  Siempre ]**. Este usuario no ocupa una licencia de [!DNL Workfront]. Puede asignar usuarios activos a elementos de trabajo en [!DNL Workfront], pero no puede incluirlos en las actualizaciones. Para obtener información acerca de cómo configurar la creación automática de [!DNL Workfront] usuarios de [!DNL Jira], vea [Configurar [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Para registrar el tiempo de un elemento en [!DNL Jira] y que se registre tanto en [!DNL Jira] como en [!DNL Workfront]:

1. Iniciar sesión en [!DNL Jira].
1. Vaya al problema [!DNL Jira] que está vinculado al elemento [!DNL Workfront].
1. Expanda el menú **[!UICONTROL Más]** y haga clic en **[!UICONTROL Registro del trabajo]**.

1. En el campo **[!UICONTROL Tiempo empleado]** especifique la cantidad de tiempo empleado trabajando en este problema. Debe especificar el tiempo utilizando los siguientes períodos de tiempo:

   * [!UICONTROL Semanas] (ancho)
   * [!UICONTROL Días] (d)
   * [!UICONTROL Horas] (h)

1. Continúe agregando información a su entrada de tiempo, incluida una **[!UICONTROL Descripción del trabajo]**, y después haga clic en **[!UICONTROL Registro]**.\
   La hora se agrega a la ficha **[!UICONTROL Registro de trabajo]** del elemento [!DNL Jira], así como al elemento [!DNL Workfront] vinculado a él.\
   La descripción de trabajo de la entrada de tiempo se registra como una nota en la entrada de horas de [!DNL Workfront].

### Registrar tiempo desde [!DNL Jira] hasta un elemento [!DNL Workfront]

Puede registrar tiempo solo en el elemento [!DNL Workfront] vinculado desde el problema [!DNL Jira] sin registrar este tiempo en el problema [!DNL Jira].

1. Iniciar sesión en [!DNL Jira].
1. Vaya a un problema [!DNL Jira] que está vinculado a un elemento [!DNL Workfront].

   Los detalles del elemento [!DNL Workfront] deben mostrarse en el panel derecho [!DNL Workfront] del problema.

1. Haga clic en el icono **[!UICONTROL Registrar tiempo]**.

1. Especifique la cantidad de **[!UICONTROL horas]** y **[!UICONTROL minutos]** que desea registrar para el problema.

1. Haga clic en **[!UICONTROL Registrar tiempo]**.

   La hora se agrega al elemento [!DNL Workfront].

   Esta vez no se agregó a la ficha [!UICONTROL Registro de trabajo] del problema [!DNL Jira].

## Comentario de un problema [!DNL Jira] vinculado {#comment-from-a-linked-jira-issue}

Cuando comenta un elemento de [!DNL Jira] desde el panel derecho de [!DNL Workfront] en [!DNL Jira], el comentario también se agrega a la pestaña [!UICONTROL Actualizaciones] del elemento vinculado en Workfront.

Para agregar un comentario de [!DNL Jira] a un elemento de [!DNL Workfront]:

1. Iniciar sesión en [!DNL Jira].
1. Vaya a un problema [!DNL Jira] que está vinculado a un elemento [!DNL Workfront].

   Los detalles del elemento [!DNL Workfront] deben mostrarse en el panel derecho [!DNL Workfront] del problema.

1. Haga clic en el icono **[!UICONTROL Comentarios]** en el panel [!DNL Workfront] o en la ficha **[!UICONTROL Comentarios]**.

1. Empiece a escribir un comentario y, a continuación, haga clic en **[!UICONTROL Enviar]**.

   El comentario se añade a lo siguiente:

   * La ficha **[!DNL Workfront]** del problema [!DNL Jira].
   * La ficha **[!UICONTROL Comentarios]** del problema [!DNL Jira].
   * La ficha **[!UICONTROL Actualizaciones]** del elemento vinculado en Workfront.
