---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restaurar elementos eliminados
description: Si es administrador de Workfront, puede restaurar proyectos, tareas, problemas, documentos y plantillas en Adobe Workfront si estos se han eliminado en los últimos 30 días. Después de 30 días, estos elementos se eliminan de forma permanente y no se pueden restaurar. Al restaurar un objeto, también se restauran todos sus objetos y campos secundarios. Por ejemplo, si restaura un proyecto, también se restaurarán todas las tareas, problemas, documentos, horas, notas, asignaciones y datos personalizados del proyecto.
feature: System Setup and Administration
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 1fb283df7090173d8f4dd36b9474ced10c8d30d1
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 1%

---

# Restaurar elementos eliminados

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Si es administrador de Workfront, puede restaurar proyectos, tareas, problemas, documentos y plantillas en Adobe Workfront si estos se han eliminado en los últimos 30 días. Después de 30 días, estos elementos se eliminan de forma permanente y no se pueden restaurar.

Al restaurar un objeto, también se restauran todos sus objetos y campos secundarios. Por ejemplo, si restaura un proyecto, también se restaurarán todas las tareas, problemas, documentos, horas, notas, asignaciones y datos personalizados del proyecto.

Un administrador de grupos también puede restaurar estos objetos para un grupo que administra.

>[!IMPORTANT]
>
>* Si elimina un informe, tablero, usuario, grupo, equipo o iteración, no se puede restaurar.
>* En un grupo, cuando alguien que no sea el administrador del grupo carga un documento directamente en el área Documentos de un objeto, solo un administrador de Workfront puede restaurar el documento.
>
>* Si mueve una tarea o un problema y decide no mover también los documentos adjuntos a la tarea o al problema, los documentos se eliminan y se colocan en la Papelera de reciclaje durante 30 días. Un administrador puede restaurarlos y se adjuntarán de nuevo a la tarea o problema que se haya movido. Si la tarea o el problema se han eliminado desde que se movieron, los documentos se restaurarán en el área Documentos de la página de usuario del administrador que los restaura.


## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Información que se recupera al restaurar un proyecto, una tarea o un problema

Al restaurar un proyecto, tarea o problema, se recupera la siguiente información asociada junto con él:

* Comentarios y respuestas en el área Actualizaciones
* Rutas de aprobación
* Asignaciones
* Formularios personalizados
* Configuración de cola
* Casos de negocio, incluidos informes de valoración, objetivos y riesgos
* Equipos de proyecto
* Fechas
* Problemas
* Tareas
* Subtareas
* Estados
* Información financiera:

   * Registros de facturación
   * Tasas de facturación
   * Gastos

* Información de línea de tiempo:

   * Predecesoras
   * Restricciones de tareas
   * Tipo de duración

* Líneas base

   Las líneas de base de tareas se recuperan cuando restaura su proyecto o tarea principal, pero no cuando restaura tareas eliminadas individualmente.

* Horas (ID de hora)

   El hecho de que las horas se restauren al elemento eliminado depende de la configuración que haya elegido al configurar las preferencias de hojas de horas y horas. Para obtener más información, consulte [Configurar el efecto en horas en las que se elimina y se restaura un objeto](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* La dirección URL del elemento

   Cuando se restaura, la dirección URL del elemento sigue siendo la misma. Si las personas han creado marcadores del explorador para el elemento, estos siguen siendo válidos.

* Acceso y permisos

   Los usuarios que tenían acceso al elemento antes de eliminarlo recuperan el acceso después de restaurarlo.

* Documentos (incluidos documentos probados)

   Tenga en cuenta lo siguiente al restaurar documentos y versiones de documentos:

   * Los documentos que se eliminaron individualmente se pueden restaurar individualmente.

      Los documentos que se eliminaron junto con su proyecto principal, tarea o problema se recuperan al restaurar el principal, pero no se pueden restaurar individualmente.

   * Todas las versiones de un documento o de una prueba de documento se restauran cuando se restaura el documento.\
      Las versiones individuales de un documento o prueba de documento que se eliminaron individualmente no se pueden recuperar.

## Información que no se recupera al restaurar un proyecto, una tarea o un problema

Cuando restaura un proyecto, tarea o problema, la siguiente información asociada no se recupera junto con él:

* Cantidad de &quot;Me gusta&quot;
* Endosos
* Admitir dirección de correo electrónico en una cola de solicitudes
* Favoritos

   Un proyecto, tarea o problema que agregó al menú Favoritos antes de eliminarlo no vuelve a aparecer en el menú Favoritos después de restaurarlo.

* Resolución de objetos

   Un objeto de resolución es un problema convertido configurado con la opción **Mantener el problema original y enlazar su resolución a esto** &lt;**proyecto** o **task)**>. Si elimina el proyecto o la tarea principal, el problema ya no se identifica como un objeto de resolución porque ya no hay un vínculo que lo conecte al proyecto o la tarea. Si restaura el vínculo principal, este no se restaura.

   Para obtener más información sobre cómo un administrador de Workfront o un administrador de grupos configura los problemas para que coincidan con el objeto de resolución al convertirse, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) y [Configuración de las preferencias de tarea y problema para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   Para obtener más información sobre la conversión de problemas, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Restaurar elementos

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Papelera de reciclaje** > **Eliminado recientemente**.
1. Haga clic en el **Proyectos**, **Tareas**, **Problemas** o **Documentos** , en función del tipo de elemento que desee restaurar.

   Los elementos se ordenan por **Fecha de eliminación** de forma predeterminada.

1. Seleccione hasta 10 elementos que desee restaurar.

   Si elimina una tarea secundaria, esta se muestra en la lista.

   Si elimina una tarea principal, solo se mostrará en la lista la tarea principal. Pero todas las tareas secundarias se restauran cuando restaura una tarea principal.

1. Haga clic en **Restaurar** para restaurar los elementos seleccionados a su ubicación original.
1. (Opcional) Para ver rápidamente el elemento restaurado, siga los pasos indicados en [Ver elemento restaurado](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   Para obtener más información sobre lo que sucede después de restaurar un elemento, consulte [Qué sucede después de restaurar elementos](#what-happens-after-you-restore-items) en este artículo.

## Qué sucede después de restaurar elementos {#what-happens-after-you-restore-items}

* Al restaurar tareas y subtareas, aparecen en el orden en que estaban antes de ser eliminadas.

   Sin embargo, si el orden de otras tareas cambia mientras se elimina la tarea, esta se puede restaurar a la parte inferior de la lista de tareas o subtareas.

* Después de restaurar un elemento:

   * Aparece un mensaje que le informa de si se ha realizado correctamente.

      También recibirá una notificación por correo electrónico. Si ha restaurado varios elementos, el correo electrónico los enumera.

   * Se muestra un comentario en el área Actualizaciones del proyecto, la tarea o el problema y en el del objeto principal.

      Esto no ocurre cuando se restaura un documento.

## Pruebas restauradas

En este momento, cuando alguien restaura un documento que tiene una prueba, la página Actividades de prueba para la prueba podría mostrar el nombre del primer administrador de Workfront activo enumerado para la instancia de su organización (en orden de ID de perfil) en lugar de la persona real que restauró la prueba.
