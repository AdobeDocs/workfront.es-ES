---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restaurar elementos eliminados
description: Si es administrador de Workfront, puede restaurar proyectos, tareas, problemas, documentos y plantillas en Adobe Workfront si se han eliminado en los últimos 30 días. Después de 30 días, estos elementos se eliminan de forma permanente y no se pueden restaurar. Al restaurar un objeto, también se restauran todos sus objetos secundarios y campos. Por ejemplo, si restaura un proyecto, también se restaurarán todas las tareas, problemas, documentos, horas, notas, asignaciones y datos personalizados del proyecto.elementos
feature: System Setup and Administration
author: Lisa
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '1082'
ht-degree: 2%

---

# Restaurar elementos eliminados

<!--Audited: 12/2023-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Si es administrador de Workfront, puede restaurar proyectos, tareas, problemas, documentos y plantillas en Adobe Workfront si se han eliminado en los últimos 30 días. Después de 30 días, estos elementos se eliminan de forma permanente y no se pueden restaurar.

Al restaurar un objeto, también se restauran todos sus objetos secundarios y campos. Por ejemplo, si restaura un proyecto, también se restaurarán todas las tareas, problemas, documentos, horas, notas, asignaciones y datos personalizados del proyecto.

Un administrador de grupo también puede restaurar estos objetos para un grupo que administre.

>[!IMPORTANT]
>
>* Si elimina un informe, tablero, usuario, grupo, equipo o iteración, no se podrá restaurar.
>* En un grupo, cuando alguien que no sea el administrador del grupo carga un documento directamente en el área de Documentos de un objeto, sólo un administrador de Workfront puede restaurar el documento.
>
>* Si mueve una tarea o un problema y decide no mover también los documentos adjuntos a la tarea o al problema, los documentos se eliminan y se colocan en la papelera de reciclaje durante 30 días. Un administrador puede restaurarlos y se vuelven a adjuntar a la tarea o al problema movido. Si la tarea o el problema se han eliminado desde que se movió, los documentos se restauran en el área Documentos de la página del usuario del administrador que los restaura.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td><p>Nuevo: estándar</p>
   o
   <p>Actual: plan</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

+++

## Información que se recupera al restaurar un proyecto, tarea o problema

Al restaurar un proyecto, una tarea o un problema, se recupera junto con ella la siguiente información asociada:

* Comentarios y respuestas en el área de Actualizaciones
* Rutas de aprobación
* Asignaciones
* Formularios personalizados
* Configuración de cola
* Casos comerciales, incluidos cuadros de resultados, objetivos y riesgos
* Equipos de proyecto
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
   * Las restricciones de tareas
   * Tipo de duración

* Líneas base

  Las líneas de base de tareas se recuperan al restaurar su proyecto o tarea principal, pero no al restaurar tareas eliminadas individualmente.

* Horas (e ID de hora)

  La restauración de las horas en el elemento eliminado depende de la configuración que elija al configurar las preferencias para las plantillas de horas y las horas. Para obtener más información, vea [Configurar el efecto en horas cuando se elimina y restaura un objeto](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* La dirección URL del elemento

  Cuando se restaura, la dirección URL del elemento sigue siendo la misma. Si las personas han creado marcadores de explorador para el elemento, siguen siendo válidos.

* Acceso y permisos

  Los usuarios que tenían acceso al elemento antes de eliminarlo recuperan el acceso después de restaurarlo.

* Documentos (incluidos los documentos revisados)

  Tenga en cuenta lo siguiente al restaurar documentos y versiones de documentos:

   * Los documentos que se eliminaron individualmente se pueden restaurar individualmente.

     Los documentos que se eliminaron junto con su proyecto, tarea o problema principal se recuperan al restaurar el elemento principal, pero no se pueden restaurar de forma individual.

   * Todas las versiones de un documento o de una revisión de documento se restauran cuando se restaura el documento.\
     Las versiones individuales de un documento o una prueba de documento que se eliminaron individualmente no se pueden recuperar.

## Información que no se recupera al restaurar un proyecto, tarea o problema

Al restaurar un proyecto, una tarea o un problema, la siguiente información asociada no se recupera junto con ella:

* Me gusta
* Endosos
* Dirección de correo electrónico de admisión en una cola de solicitudes
* Favoritos

  Un proyecto, tarea o problema que agregó al menú Favoritos antes de eliminarlo no vuelve a aparecer en el menú Favoritos después de restaurarlo.

* Resolver objetos

  Un objeto de resolución es un problema convertido configurado con la opción **Mantener el problema original y enlazar su solución a este** &lt;**proyecto** o **tarea)**>. Si elimina el proyecto o la tarea principal, el problema ya no se identifica como objeto de resolución porque ya no hay un vínculo que lo conecte al proyecto o la tarea. Si restaura el elemento principal, el vínculo no se restaura.

  Para obtener más información sobre cómo un administrador de Workfront o de grupo configura problemas para que coincidan con el objeto de resolución cuando se convierte, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) y [Configurar las preferencias de tareas y problemas para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

  Para obtener más información sobre la conversión de problemas, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Restaurar elementos

{{step-1-to-setup}}

1. Haga clic en **Papelera de reciclaje** > **Eliminada recientemente**.
1. Haga clic en la ficha **Proyectos**, **Tareas**, **Problemas**, **Plantillas** o **Documentos**, según el tipo de elemento que desee restaurar.

   Los elementos se ordenan por la columna **Fecha de eliminación** de manera predeterminada.

1. Seleccione hasta 10 elementos que desee restaurar.

   Si elimina una tarea secundaria, esta se muestra en la lista.

   Si elimina una tarea principal, solo se muestra la tarea principal en la lista. Sin embargo, todas las tareas secundarias se restauran al restaurar una tarea principal.

1. Haga clic en **Restaurar** para restaurar los elementos seleccionados a su ubicación original.
1. (Opcional) Para ver rápidamente el elemento restaurado, siga los pasos de [Ver elemento restaurado](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   Para obtener más información acerca de lo que sucede después de restaurar un elemento, vea la sección [Qué sucede después de restaurar los elementos](#what-happens-after-you-restore-items) en este artículo.

## Qué sucede después de restaurar los elementos {#what-happens-after-you-restore-items}

* Al restaurar tareas y subtareas, se muestran en el orden en que se encontraban antes de eliminarse.

  Sin embargo, si el orden de las demás tareas cambia mientras se elimina la tarea, ésta puede restaurarse al final de la lista de tareas o subtareas.

* Después de restaurar un elemento:

   * Aparece un mensaje para que sepa si se ha realizado correctamente.

     También recibe una notificación por correo electrónico. Si ha restaurado varios elementos, el correo electrónico los enumera.

   * Un comentario se muestra en el área de Actualizaciones del proyecto, tarea o problema y en la del objeto principal.

     Esto no sucede cuando se restaura un documento o una plantilla.

## Pruebas restauradas

Cuando alguien restaura un documento que tiene una prueba, la página Actividades de prueba para la prueba puede mostrar el nombre del primer administrador de Workfront activo que aparezca en la lista de la instancia de su organización (en orden de ID de perfil) en lugar de la persona real que la restauró.
