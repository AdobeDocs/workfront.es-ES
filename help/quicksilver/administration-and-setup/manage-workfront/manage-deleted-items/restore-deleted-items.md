---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restaurar elementos eliminados
description: 'Si es administrador de Workfront, puede restaurar los proyectos, tareas, problemas, documentos y plantillas en Adobe Workfront que se hayan eliminado en los últimos 30 días. Pasados esos 30 días, estos elementos se eliminan de forma permanente y no se pueden restaurar. '
feature: System Setup and Administration
author: Lisa
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 97%

---

# Restaurar elementos eliminados

<!--Audited: 12/2023-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Si es administrador de Workfront, puede restaurar los proyectos, tareas, problemas, documentos y plantillas en Adobe Workfront que se hayan eliminado en los últimos 30 días. Pasados esos 30 días, estos elementos se eliminan de forma permanente y no se pueden restaurar. 

Al restaurar un objeto, también se restauran todos sus objetos secundarios y campos. Por ejemplo, si restaura un proyecto, también se restaurarán todas las tareas, problemas, documentos, horas, notas, asignaciones y datos personalizados del proyecto.

Un administrador de grupos también puede restaurar estos objetos para un grupo que administre.

>[!IMPORTANT]
>
>* Si elimina un informe, tablero, usuario, grupo, equipo o iteración, no se podrá restaurar.
>* En un grupo, cuando alguien que no sea el administrador de grupos carga un documento directamente en el área Documentos de un objeto, solo un administrador de Workfront puede restaurar el documento.
>
>* Si mueve una tarea o un problema y decide no mover también los documentos adjuntos a la tarea o al problema, los documentos se eliminan y se colocan en la papelera de reciclaje durante 30 días. Un administrador puede restaurarlos y se vuelven a adjuntar a la tarea o al problema movido. Si la tarea o el problema se han eliminado desde que se movieron, los documentos se restauran en el área Documentos de la página de usuario del administrador que los restaura.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Información que se recupera al restaurar un proyecto, tarea o problema

Al restaurar un proyecto, una tarea o un problema, junto con ellos se recupera la siguiente información asociada:

* Comentarios y respuestas en el área Actualizaciones
* Rutas de aprobación
* Asignaciones
* Formularios personalizados
* Configuración de cola
* Casos empresariales, incluidos cuadros de resultados, metas y riesgos
* Equipos del proyecto
* Fechas
* Problemas
* Tareas
* Subtareas
* Estados
* Información financiera:

   * Registros de facturación
   * Tarifas de facturación
   * Gastos

* Información de cronología:

   * Predecesoras
   * Restricciones de tareas
   * Tipo de duración

* Líneas base

  Las líneas de base de las tareas se recuperan al restaurar su proyecto o tarea principal, pero no al restaurar las tareas eliminadas individualmente.

* Horas (e ID de hora)

  La restauración de las horas en el elemento eliminado depende de la configuración que elija al configurar las preferencias de las plantillas de horas y las horas. Para obtener más información, consulte [Configurar el efecto sobre las horas cuando se elimina y restaura un objeto](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* La dirección URL del elemento

  Cuando se restaura, la dirección URL del elemento sigue siendo la misma. Si las personas han creado marcadores de explorador para el elemento, dichos marcadores seguirán siendo válidos.

* Acceso y permisos

  Los usuarios que tenían acceso al elemento antes de que se eliminara recuperarán el acceso después de restaurarlo.

* Documentos (incluidos los documentos revisados)

  Tenga en cuenta lo siguiente a la hora de restaurar documentos y versiones de documentos:

   * Los documentos que se eliminaron individualmente se pueden restaurar individualmente.

     Los documentos que se eliminaron junto con su proyecto, tarea o problema principal se recuperarán al restaurar el elemento principal, pero no se podrán restaurar de forma individual.

   * Todas las versiones de un documento o de una prueba de documento se restaurarán cuando se restaure el documento.\
     Las versiones individuales de un documento o una prueba de documento que se eliminaron individualmente no se pueden recuperar.

## Información que no se recupera al restaurar un proyecto, tarea o problema

Al restaurar un proyecto, una tarea o un problema, la siguiente información asociada no se recupera junto con ella:

* Me gusta
* Endosos
* Dirección del correo electrónico de admisión en una cola de solicitudes
* Favoritos

  Un proyecto, tarea o problema que añadió al menú Favoritos antes de eliminarlo o eliminarla no vuelve a aparecer en el menú Favoritos después de restaurarlo.

* Objetos de resolución

  Un objeto de resolución es un problema convertido configurado con la opción **Mantener el problema original y enlazar su solución a este** &lt;**(proyecto** o **tarea)**>. Si elimina el proyecto o la tarea principal, el problema ya no se identificará como objeto de resolución porque ya no habrá un vínculo que lo conecte al proyecto o la tarea. Si restaura el elemento principal, el vínculo no se restaura.

  Para obtener más información sobre cómo un administrador de Workfront o de grupos configura problemas para que coincidan con el objeto de resolución al convertirlo, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) y [Configurar las preferencias de tareas y problemas para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

  Para obtener más información sobre la conversión de problemas, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Restaurar elementos

{{step-1-to-setup}}

1. Haga clic en **Papelera de reciclaje** > **Eliminado recientemente**.
1. Haga clic en la pestaña **Proyectos**, **Tareas**, **Problemas**, **Plantillas** o **Documentos**, según el tipo de elemento que desee restaurar.

   Los elementos se ordenan por la columna **Fecha de eliminación** de manera predeterminada.

1. Seleccione hasta 10 elementos que desee restaurar.

   Si elimina una tarea secundaria, se mostrará en la lista.

   Si elimina una tarea principal, solo se mostrará la tarea principal en la lista. Sin embargo, todas las tareas secundarias se restaurarán al restaurar una tarea principal.

1. Haga clic en **Restaurar** para restaurar los elementos seleccionados a su ubicación original.
1. (Opcional) Para ver rápidamente el elemento restaurado, siga los pasos indicados en [Ver elemento restaurado](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   Para obtener más información sobre lo que sucede después de restaurar un elemento, consulte la sección [Qué sucede después de restaurar los elementos](#what-happens-after-you-restore-items) en este artículo.

## Qué sucede después de restaurar los elementos {#what-happens-after-you-restore-items}

* Al restaurar tareas y subtareas, se muestran en el orden en que se encontraban antes de eliminarse.

  Sin embargo, si el orden de las demás tareas cambia mientras se elimina la tarea, ésta podrá restaurarse al final de la lista de tareas o subtareas.

* Después de restaurar un elemento:

   * Aparece un mensaje para que sepa si se ha realizado correctamente.

     También recibirá una notificación por correo electrónico. Si ha restaurado varios elementos, el correo electrónico los enumera.

   * Aparece un comentario en el área de Actualizaciones del proyecto, tarea o problema y en la del objeto principal.

     Esto no sucede cuando se restaura un documento o una plantilla.

## Pruebas restauradas

Cuando una persona restaura un documento que tiene una prueba, la página Actividades de revisión de la prueba puede mostrar el nombre del primer administrador de Workfront activo que aparece en la lista de la instancia de su organización (en orden de ID de perfil) en lugar de la persona real que restauró la prueba.
