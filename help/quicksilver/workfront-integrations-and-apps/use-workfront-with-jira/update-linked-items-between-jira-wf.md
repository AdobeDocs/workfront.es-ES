---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Actualizar elementos vinculados entre [!DNL Jira] y [!DNL Adobe Workfront]
description: Al vincular [!DNL Jira] problemas para [!DNL Adobe Workfront] tareas o problemas, los usuarios pueden actualizar los elementos en una aplicación y la contraparte de ese elemento también se actualiza para los usuarios que trabajan en la segunda aplicación.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: e01f5eaf3133fa1bdaedf4dad56e9a8175b70667
workflow-type: tm+mt
source-wordcount: '1570'
ht-degree: 0%

---

# Actualizar elementos vinculados entre [!DNL Jira] y [!DNL Adobe Workfront]

Al vincular [!DNL Jira] problemas para [!DNL Adobe Workfront] tareas o problemas, los usuarios pueden actualizar los elementos en una aplicación y la contraparte de ese elemento también se actualiza para los usuarios que trabajan en la segunda aplicación.

Para obtener más información sobre cómo vincular elementos entre [!DNL Workfront] y [!DNL Jira], consulte [Vincular elementos entre Adobe Workfront y Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Al configurar el [!DNL Workfront] para [!DNL Jira], como [!DNL Jira] administrador del sistema, puede configurar ciertos campos de una aplicación para sincronizarlos con campos de elementos vinculados en la otra aplicación.

Para obtener más información sobre la sincronización de campos entre campos vinculados [!DNL Jira] y [!DNL Workfront] elementos, consulte [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

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
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Le recomendamos que cree cuentas de administrador del sistema independientes en [!DNL Jira] y [!DNL Workfront] para dedicarse a esta integración, en lugar de utilizar las existentes que podrían adjuntarse a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser un [!DNL Workfront] administrador.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

Antes de poder vincular elementos entre [!DNL Workfront] y [!DNL Jira], debe:

* Instalar [!DNL Workfront for Jira].

  Para obtener instrucciones sobre la instalación [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurar [!DNL Workfront for Jira].

  Para obtener instrucciones sobre la configuración [!DNL Workfront for Jira], consulte [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Vincular elementos entre [!DNL Workfront] y [!DNL Jira].

  Para obtener instrucciones, consulte [Vincular elementos entre [!DNL Adobe Workfront] y [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Actualización de elementos vinculados en [!DNL Workfront]

Si trabaja principalmente en [!DNL Workfront], puede actualizar los elementos de trabajo en [!DNL Workfront] y sus contrapartes en [!DNL Jira] también actualizar. Esta actualización se produce mediante la integración de [!DNL Workfront] para [!DNL Jira] que no requiere que tenga un [!DNL Jira] licencia.

Mientras su [!DNL Workfront] el administrador ha configurado [!DNL Workfront for Jira] para sincronizar los campos entre elementos vinculados, seleccione ciertos campos que debe actualizar en [!DNL Workfront] también actualizar para el vinculado [!DNL Jira] problema. Para obtener más información sobre la actualización de elementos en [!DNL Workfront], consulte [Editar problemas](../../manage-work/issues/manage-issues/edit-issues.md) y [Editar tareas](../../manage-work/tasks/manage-tasks/edit-tasks.md).

La siguiente lista muestra qué [!DNL Workfront] campos sincronizados con [!DNL Jira] campos en elementos vinculados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Actualizado [!DNL Workfront] campo</strong> </th> 
   <th><strong>Sincronizado [!DNL Jira] field/ update</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Problema o nombre de tarea]</td> 
   <td> <p>[!UICONTROL Nombre de problema]</p> <p>Se agrega un comentario sobre el cambio de nombre al <strong>[!DNL Workfront]</strong> de la pestaña [!DNL Jira] problema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema o Descripción de tarea]</td> 
   <td> <p> [!UICONTROL Descripción del problema]</p> <p>Se agrega un comentario sobre la descripción actualizada a la <strong>[!DNL Workfront]</strong> de la pestaña [!DNL Jira] problema.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Documentos cargados]</p> <p>Nota: Documentos que están vinculados a [!DNL Workfront] los elementos de un servidor externo no se transfieren a [!DNL Jira] problemas. Solo los documentos cargados directamente en [!DNL Workfront] los elementos también se actualizan al vínculo [!DNL Jira] problemas. </p> </td> 
   <td> <p>[!UICONTROL Archivos adjuntos]</p> <p>Se agrega un comentario sobre los archivos adjuntos cargados a <strong>[!DNL Workfront]</strong> de la pestaña [!DNL Jira] problema.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha planificada de finalización]</td> 
   <td> <p>[!UICONTROL Fecha de vencimiento]</p> <p>Se agrega a un comentario acerca de que [!UICONTROL Fecha de vencimiento] ha cambiado [!DNL Workfront] de la pestaña [!DNL Jira] problema. </p> <p>Nota: Debe activar <strong>[!UICONTROL Fecha de vencimiento]</strong> para su [!DNL Jira] problemas para poder ver este campo actualizado en [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Forms personalizado y campos personalizados</td> 
   <td> <p> Mostrar en la [!DNL Workfront] panel derecho del [!DNL Jira] problema. <br>En el panel solo se muestran los campos personalizados que tienen un valor real.<br></p> <p>Nota: Las secciones de formulario personalizado se muestran con el nivel de acceso del [!DNL Workfront] administrador. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema o prioridad de tarea]</td> 
   <td>Se muestra en la [!DNL Workfront] panel derecho del [!DNL Jira] problema. <br>No actualiza el problema <strong>[!UICONTROL Prioridad]</strong> field en [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hora de registro] </td> 
   <td> <p>Se agrega un comentario sobre el tiempo registrado en la variable <strong>[!DNL Workfront]</strong> de la pestaña [!DNL Jira] problema. Esto incluye el nombre del usuario que registra la hora, así como el usuario para el que se registra la hora, en caso de que sea diferente. No se ha registrado tiempo en <strong>[!UICONTROL Registro de trabajo]</strong> pestaña en [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comentarios]</td> 
   <td> <p>El comentario se añade a <strong>[!DNL Workfront]</strong> de la pestaña [!DNL Jira] problema. No se añade a <strong>[!UICONTROL Comentarios]</strong> de la pestaña [!DNL Jira] problema</p> <p>Nota: Cuando vincula dos elementos existentes manualmente, los comentarios que se agregaron a la [!DNL Workfront] antes de vincularlo a [!DNL Jira] no sincronizar con el [!DNL Jira] problema. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Actualización de elementos vinculados en [!DNL Jira]

Si trabaja principalmente en [!DNL Jira], puede actualizar los elementos de trabajo en [!DNL Jira] y sus contrapartes en [!DNL Workfront] también actualizar. No tiene que tener un [!DNL Workfront] licencia para el [!DNL Workfront] elementos vinculados a su [!DNL Jira] problemas para recibir las actualizaciones que está realizando en [!DNL Jira].

A condición de que su [!DNL Workfront] el administrador ha configurado [!DNL Workfront] para [!DNL Jira] para sincronizar los campos entre los elementos vinculados, seleccione ciertos campos que debe actualizar en [!DNL Jira] también actualizar para el vinculado [!DNL Workfront] elemento.

La siguiente lista muestra qué [!DNL Jira] campos sincronizados con [!DNL Workfront] campos en elementos vinculados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Actualizado [!DNL Jira] Campo</strong> </th> 
   <th><strong>Sincronizado [!DNL Workfront] Campo/ Actualización</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Estado del problema]</td> 
   <td> <p> [!UICONTROL Estado de tarea o problema]</p> <p>Estado del problema en [!DNL Jira] se sincroniza con los siguientes estados, o estados que se igualan con los siguientes estados, en Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL Nuevo] ([!UICONTROL NUEVO])</p> </li> 
     <li> <p>[!UICONTROL En curso] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Cerrado]/[!UICONTROL Completado] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Nota: La [!DNL Jira] el estado se sincroniza con el primero [!DNL Workfront] estado que equivale al estado adecuado.</p> <p>Para obtener más información sobre los estados de los elementos en [!DNL Workfront], consulte <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Creación o edición de un estado</a>.</p> </td> 
  </tr>
  <tr> 
   <td>Archivos adjuntos de [!UICONTROL Issue]</td> 
   <td> [!UICONTROL Problema o documentos de tarea]<br>Un comentario sobre cómo cargar un nuevo documento en [!DNL Jira] se agrega a la ficha [!UICONTROL Updates] de [!DNL Workfront] problema o tarea.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de vencimiento]</td> 
   <td> <p> Un comentario acerca del cambio de [!UICONTROL Fecha de vencimiento] en [!DNL Jira] se agrega a la ficha [!UICONTROL Updates] de [!DNL Workfront] problema o tarea. </p> <p>Nota: No se han cambiado fechas en la [!DNL Workfront] problema o tarea. </p> </td> 
  </tr> 
  <tr> 
   <td> Registrar tiempo en [!DNL Workfront] en el panel derecho o en el menú [!UICONTROL Más] del [!DNL Jira] problema<br></td> 
   <td> <p>Horas<br>Además de agregar las horas registradas en Jira a los vínculos [!DNL Workfront] , se agrega un comentario sobre el registro del tiempo a la ficha [!UICONTROL Updates] del [!DNL Workfront] elemento.</p> <p>Para obtener más información sobre cómo registrar la hora en los vínculos [!DNL Jira] problemas, incluida la actualización de [!DNL Jira] usuario que está iniciando sesión [!DNL Workfront], consulte <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Registrar tiempo para elementos vinculados [!DNL Jira] y [!DNL Workfront] items</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Comentarios <br><br></td> 
   <td> <p>Los comentarios se agregan a la ficha [!UICONTROL Updates] del [!DNL Workfront] problema o tarea si la variable <strong>[!UICONTROL Comentarios]</strong> estableciendo en la sección [!UICONTROL SYNCHRONIZE FROM JIRA to WORKFRONT] de la ficha [!UICONTROL Setup] como <strong>[!UICONTROL Siempre]</strong>.</p> <p>Para obtener información sobre la configuración de Workfront en [!DNL Jira], consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuración [!DNL Workfront for Jira]</a>.</p> <p>Para obtener información sobre cómo comentar elementos de elementos vinculados [!DNL Jira] problemas, consulte <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Comentario de un vínculo [!DNL Jira] problema</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Registrar tiempo desde vínculos [!DNL Jira] problemas

La hora que se registra para un [!DNL Jira] elemento en [!DNL Jira] también se transferirá al asociado [!DNL Workfront] elemento, independientemente de en qué punto de [!DNL Jira] registras el tiempo.\
Cuando ingresa tiempo en Jira en el [!DNL Workfront] panel, el tiempo se registra solo en [!DNL Workfront].\
La hora en que graba [!DNL Workfront] no afecta al tiempo del problema vinculado en [!DNL Jira].

>[!NOTE]
>
>Si la hora se añade a un [!DNL Jira] elemento vinculado a [!DNL Workfront] la tarea, el [!UICONTROL Tipo de hora] por la hora en [!DNL Workfront] es [!UICONTROL Hora de tarea]. Si la hora se añade a un [!DNL Jira] elemento vinculado a [!DNL Workfront] problema, el [!UICONTROL Tipo de hora] por la hora en [!DNL Workfront] es [!UICONTROL Hora del problema].

Se agrega un comentario a **[!DNL Workfront]** pestaña en [!DNL Jira] y a la **[!UICONTROL Actualizaciones]** pestaña del elemento en [!DNL Workfront] para registrar el registro de la hora.\
La hora también se muestra en la **[!UICONTROL Horas]** de la pestaña [!DNL Workfront] elemento.

* [Registrar tiempo para elementos vinculados [!DNL Jira] y [!DNL Workfront] items](#log-time-for-linked-jira-and-workfront-items)
* [Registrar tiempo desde [!DNL Jira] a un [!DNL Workfront] artículo](#log-time-from-jira-to-a-workfront-item)

### Registrar tiempo para elementos vinculados [!DNL Jira] y [!DNL Workfront] items

Puede registrar tiempo desde un [!DNL Jira] problema vinculado a [!DNL Workfront] y la hora se registra tanto en el [!DNL Jira] problema, así como el [!DNL Workfront] elemento.

>[!IMPORTANT]
>
>Si el usuario inicia la sesión [!DNL Jira] no existe en [!DNL Workfront], la integración crea un nuevo usuario activo en Workfront si **[!UICONTROL Crear automáticamente un usuario en [!DNL Workfront]&#x200B;si la variable [!DNL Jira] el usuario no tiene un *[!DNL Workfront]&#x200B;account]** se ha definido en**[!UICONTROL  Siempre ]**. Este usuario no ocupa un [!DNL Workfront] licencia. Puede asignar usuarios activos a elementos de trabajo en [!DNL Workfront], pero no se pueden incluir en las actualizaciones. Para obtener información sobre cómo configurar la creación automática de [!DNL Workfront] usuarios de [!DNL Jira], consulte [Configuración [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Para registrar el tiempo de un elemento en [!DNL Jira] y grabarlo tanto en [!DNL Jira] y [!DNL Workfront]:

1. Iniciar sesión en [!DNL Jira].
1. Vaya a la [!DNL Jira] problema que está vinculado al [!DNL Workfront] elemento.
1. Expanda el **[!UICONTROL Más]** y haga clic en **[!UICONTROL Registrar trabajo]**.

1. En el **[!UICONTROL Tiempo empleado]** , especifique la cantidad de tiempo empleado trabajando en este problema. Debe especificar el tiempo utilizando los siguientes períodos de tiempo:

   * [!UICONTROL Semanas] (w)
   * [!UICONTROL Días] (d)
   * [!UICONTROL Horas] (h)

1. Siga agregando información a la entrada de tiempo, incluido un **[!UICONTROL Descripción del trabajo]**, luego haga clic en **[!UICONTROL Registro]**.\
   La hora se añade a **[!UICONTROL Registro de trabajo]** de la pestaña [!DNL Jira] elemento, así como al [!DNL Workfront] elemento vinculado a él.\
   La descripción de trabajo de la entrada de tiempo se registra como una nota en la entrada de horas en [!DNL Workfront].

### Registrar tiempo desde [!DNL Jira] a un [!DNL Workfront] artículo

Puede registrar tiempo solo en el elemento vinculado [!DNL Workfront] elemento de la [!DNL Jira] problema sin registrar este tiempo en [!DNL Jira] problema.

1. Iniciar sesión en [!DNL Jira].
1. Vaya a [!DNL Jira] problema que está vinculado a [!DNL Workfront] elemento.

   Los detalles de la [!DNL Workfront] elemento debe mostrarse en la [!DNL Workfront] panel derecho de la incidencia.

1. Haga clic en **[!UICONTROL Hora de registro]** icono.

1. Especifique la cantidad de **[!UICONTROL Horas]** y **[!UICONTROL Minutes]** desea registrar el problema.

1. Clic **[!UICONTROL Hora de registro]**.

   La hora se añade a [!DNL Workfront] elemento.

   Esta vez no se añade a [!UICONTROL Registro de trabajo] de la pestaña [!DNL Jira] problema.

## Comentario de un vínculo [!DNL Jira] problema {#comment-from-a-linked-jira-issue}

Cuando comenta sobre un [!DNL Jira] elemento de la [!DNL Workfront] panel derecho en [!DNL Jira], el comentario también se agrega al [!UICONTROL Actualizaciones] del elemento vinculado en Workfront.

Para realizar comentarios desde [!DNL Jira] a un [!DNL Workfront] elemento:

1. Iniciar sesión en [!DNL Jira].
1. Vaya a [!DNL Jira] problema que está vinculado a [!DNL Workfront] elemento.

   Los detalles de la [!DNL Workfront] elemento debe mostrarse en la [!DNL Workfront] panel derecho de la incidencia.

1. Haga clic en **[!UICONTROL Comentarios]** en el menú [!DNL Workfront] o en el **[!UICONTROL Comentarios]** pestaña.

1. Empiece a escribir un comentario y haga clic en **[!UICONTROL Enviar]**.

   El comentario se añade a lo siguiente:

   * El **[!DNL Workfront]** de la pestaña [!DNL Jira] problema.
   * El **[!UICONTROL Comentarios]** de la pestaña [!DNL Jira] problema.
   * El **[!UICONTROL Actualizaciones]** del elemento vinculado en Workfront.
