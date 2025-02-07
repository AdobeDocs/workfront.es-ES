---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Usar Diagnósticos para activar procesos automatizados
description: Puede utilizar Diagnósticos para activar manualmente procesos automatizados, como scripts basados en tiempo, nuevos cálculos o notificaciones por correo electrónico.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 94%

---

# Usar Diagnósticos para activar procesos automatizados

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Puede utilizar Diagnósticos para activar manualmente procesos automatizados, como scripts basados en tiempo, nuevos cálculos o notificaciones por correo electrónico.

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

## Usar diagnósticos para activar procesos automatizados

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![Icono de configuración de engranajes](assets/gear-icon-settings.png).

1. Expanda **Sistema** y, a continuación, haga clic en **Diagnósticos**.
1. Seleccione una de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Enviar notificaciones vencidas</td> 
      <td> <p>Envía manualmente las notificaciones automáticas de recordatorio de las tareas y problemas vencidos. </p> <p>Para obtener más información sobre la configuración de recordatorios automáticos, consulte <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurar recordatorios automáticos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviar notificaciones tempranas</td> 
      <td> <p>Envía manualmente las notificaciones automáticas de recordatorio para las tareas y problemas que se están acercando a la fecha de vencimiento.</p> <p>Para obtener más información sobre la configuración de recordatorios automáticos, consulte <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurar recordatorios automáticos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviar notificaciones de recordatorio</td> 
      <td> <p>Envía manualmente notificaciones de recordatorio. </p> <p>Para obtener información sobre cómo configurar las notificaciones de recordatorio, consulte <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurar las notificaciones de recordatorio</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comprobar todas las cuentas POP</td> 
      <td> <p>Comprueba nuevos mensajes de correo electrónico que se enviaron a cuentas POP vinculadas a Workfront. </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Volver a calcular las escalas de tiempo</td> 
      <td> <p>Vuelve a calcular la línea de tiempo de todos los proyectos de Workfront que están en estado Actual. </p> <p>Para obtener más información sobre cómo calcular la línea de tiempo de los proyectos de forma automática o manual, proyecto por proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalcular líneas de tiempo del proyecto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Restablecer informes de cliente personalizados</td> 
      <td>Restaura los informes predeterminados que se entregaron originalmente con Workfront, de modo que estén visibles en la sección <strong>Informes</strong> para todos los usuarios.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Generar hojas de horas</td> 
      <td>Generar hojas de horas para usuarios de acuerdo con su configuración de perfil de plantilla de horas. Esta opción solo debe ejecutarse si el perfil de la plantilla de horas se ha modificado significativamente después de haber sido asignado a los usuarios y solo después de eliminar cualquier plantilla de horas actual y futura.</td> 
     </tr> 
    </tbody> 
   </table>
