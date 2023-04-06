---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Usar diagnósticos para déclencheur de procesos automatizados
description: Puede utilizar Diagnósticos para almacenar en déclencheur manualmente los procesos automatizados, como secuencias de comandos basadas en el tiempo, nuevos cálculos o notificaciones por correo electrónico.
feature: System Setup and Administration
role: Admin
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 6%

---

# Usar diagnósticos para déclencheur de procesos automatizados

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Puede utilizar Diagnósticos para almacenar en déclencheur manualmente los procesos automatizados, como secuencias de comandos basadas en el tiempo, nuevos cálculos o notificaciones por correo electrónico.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plan de Adobe Workfront</a> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre licencias heredadas</a> </td> 
   <td> <p>Plan </p>Debe ser administrador de Workfront. Para obtener información sobre los administradores de Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</td> 
  </tr> 
 </tbody> 
</table>

## Utilice diagnósticos para déclencheur de procesos automatizados

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Expandir **Sistema** y haga clic en **Diagnóstico**.
1. Seleccione una de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Enviar notificaciones vencidas</td> 
      <td> <p>Envía manualmente las notificaciones de recordatorio automáticas para tareas y problemas vencidos. </p> <p>Para obtener más información sobre la configuración de recordatorios automáticos, consulte <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurar recordatorios automáticos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviar notificaciones tempranas</td> 
      <td> <p>Envía manualmente las notificaciones de recordatorio automáticas para las tareas y los problemas que se acercan a sus fechas de vencimiento.</p> <p>Para obtener más información sobre la configuración de recordatorios automáticos, consulte <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurar recordatorios automáticos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviar notificaciones de recordatorio</td> 
      <td> <p>Envía manualmente notificaciones de recordatorio. </p> <p>Para obtener más información sobre la configuración de notificaciones de recordatorio, consulte <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configuración de notificaciones de recordatorio</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comprobar todas las cuentas POP</td> 
      <td> <p>Comprueba si hay nuevos correos electrónicos que se hayan enviado a cuentas POP vinculadas a Workfront. </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Volver a calcular las escalas de tiempo</td> 
      <td> <p>Vuelve a calcular la cronología de todos los proyectos de Workfront que estén en estado Actual. </p> <p>Para obtener más información sobre el cálculo automático o manual de la cronología de los proyectos, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Volver a calcular las líneas de tiempo del proyecto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Restablecer informes de cliente personalizados</td> 
      <td>Restaura los informes predeterminados que se entregaron originalmente con Workfront, de modo que sean visibles en la variable <strong>Informes</strong> para todos los usuarios.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Generar hojas de horas</td> 
      <td>Genera hojas de horas para los usuarios en función de sus perfiles recurrentes de hojas de horas. Esta opción solo debe ejecutarse si el perfil del parte de horas se ha modificado significativamente después de haberse asignado a usuarios y solo después de que se hayan eliminado cualquier hoja de horas actual y futura.</td> 
     </tr> 
    </tbody> 
   </table>
