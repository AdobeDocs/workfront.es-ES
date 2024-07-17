---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Utilice Diagnóstico para almacenar en déclencheur los procesos automatizados
description: Puede utilizar Diagnósticos para almacenar en déclencheur manualmente procesos automatizados, como scripts basados en tiempo, nuevos cálculos o notificaciones por correo electrónico.
feature: System Setup and Administration
role: Admin
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 6%

---

# Utilice Diagnóstico para almacenar en déclencheur los procesos automatizados

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Puede utilizar Diagnósticos para almacenar en déclencheur manualmente procesos automatizados, como scripts basados en tiempo, nuevos cálculos o notificaciones por correo electrónico.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plan Adobe Workfront</a> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Resumen de licencias</a> </td> 
   <td> <p>Plan </p>Debe ser administrador de Workfront. Para obtener información sobre los administradores de Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo total a un usuario</a>.</td> 
  </tr> 
 </tbody> 
</table>

## Usar diagnósticos para almacenar en déclencheur procesos automatizados

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Expanda **Sistema** y, a continuación, haga clic en **Diagnóstico**.
1. Seleccione una de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Enviar notificaciones vencidas</td> 
      <td> <p>Envía manualmente las notificaciones automáticas de recordatorio de las tareas y problemas vencidos. </p> <p>Para obtener más información sobre la configuración de avisos automáticos, vea <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurar avisos automáticos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviar notificaciones tempranas</td> 
      <td> <p>Envía manualmente las notificaciones automáticas de recordatorio para las tareas y los problemas que se están acercando a la fecha de vencimiento.</p> <p>Para obtener más información sobre la configuración de avisos automáticos, vea <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurar avisos automáticos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviar notificaciones de recordatorio</td> 
      <td> <p>Envía manualmente notificaciones de recordatorio. </p> <p>Para obtener más información sobre cómo configurar notificaciones de recordatorio, consulte <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurar notificaciones de recordatorio</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comprobar todas las cuentas POP</td> 
      <td> <p>Comprueba nuevos correos electrónicos que se han enviado a cuentas POP vinculadas a Workfront. </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Volver a calcular las escalas de tiempo</td> 
      <td> <p>Vuelve a calcular la cronología de todos los proyectos de Workfront que están en estado Actual. </p> <p>Para obtener más información sobre cómo calcular la escala de tiempo de los proyectos automática o manualmente, proyecto por proyecto, vea <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Volver a calcular las escalas de tiempo de los proyectos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Restablecer informes de cliente personalizados</td> 
      <td>Restaura los informes predeterminados que se entregaron originalmente con Workfront, de modo que estén visibles en la sección <strong>Informes</strong> para todos los usuarios.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Generar hojas de horas</td> 
      <td>Genera hojas de horas para los usuarios en función de sus perfiles de hojas de horas recurrentes. Esta opción solo debe ejecutarse si el perfil de la plantilla de horas se ha modificado significativamente después de asignarse a los usuarios y solo después de eliminar cualquier plantilla de horas actual y futura.</td> 
     </tr> 
    </tbody> 
   </table>
