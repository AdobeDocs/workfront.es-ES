---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Configurar recordatorios automáticos
description: Configurar recordatorios automáticos
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 1%

---

# Configurar recordatorios automáticos

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como administrador de Adobe Workfront, puede configurar recordatorios automáticos para enviar notificaciones por correo electrónico cuando todas las tareas o problemas venzan, se retrasan o se acercan a la fecha de finalización planificada. Después de configurar estos ajustes, los usuarios no pueden deshabilitar los recordatorios automáticos.

Para las notificaciones atrasadas, el correo electrónico se envía todas las noches hasta que se complete la tarea o el problema.

Se puede enviar un recordatorio automático a una o varias de las siguientes opciones:

* Los usuarios asignados a una tarea o problema
* El administrador inmediato del usuario
* El administrador del administrador inmediato

>[!NOTE]
>
>No se puede cambiar el contenido ni la línea de asunto del correo electrónico activado por un recordatorio automático.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Administrador del sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar recordatorios automáticos

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Correo electrónico** >**Recordatorios automáticos**.

1. En el **Enviar una notificación tarde a** seleccione cualquiera de las siguientes opciones:

   <table>
    <tr>
        <td>El usuario "Asignado a"</td>
        <td>Seleccione esta opción si desea que el usuario asignado a una tarea o un problema reciba una notificación tardía acerca de que su elemento de trabajo está atrasado.</td>
        <td></td>
    </tr>
    <tr>
        <td>El gerente de ese usuario</td>
        <td>Seleccione esta opción si desea que el administrador del usuario reciba una notificación tardía acerca de que el elemento de trabajo de su informe directo está retrasado.</td>
        <td></td>
    </tr>
    <tr>
        <td>El gerente de ese gerente</td>
        <td>Seleccione esta opción si desea que el administrador del administrador inmediato reciba una notificación tardía acerca de un elemento de trabajo de uno de los usuarios de su informe directo que está retrasado.</td>
        <td></td>
    </tr>
    <tr>
        <td>El usuario "Asignado a"</td>
        <td>(En el <b>Enviar recordatorio de fecha límite a</b> ). Seleccione esta opción si desea que el usuario asignado a una tarea o a un problema reciba una notificación sobre su elemento de trabajo que se acerca a la fecha de vencimiento.</td>
        <td></td>
    </tr>
</table>

1. Seleccione la hora para enviar el recordatorio automático seleccionando la cantidad de tiempo antes o después de la fecha de vencimiento del elemento de trabajo.

   La hora se calcula a partir de la fecha de finalización prevista de la tarea o el problema.

   Especifique el número de minutos, horas, días, semanas o meses para agregar la hora a la Fecha de Finalización Planificada de las tareas o problemas. Select **Minutos transcurridos**, **Horas transcurridas**, **Días transcurridos** o **Semanas transcurridas** para agregar tiempo que incluya fines de semana, días festivos y horas no laborables, como se indica en la programación.

   Por ejemplo, si una tarea está asignada el viernes y tiene una duración de 3 días transcurridos, la fecha de finalización de la tarea se establece para el lunes (suponiendo que sábado y domingo sean un fin de semana). Si la tarea tiene una duración de 3 días (no transcurrido), la fecha de finalización de la tarea se establece para el miércoles.

   ![](assets/time-increments-for-automatic-reminder.png)

1. Haga clic en **Guardar**.

## Recibir recordatorios automáticos

Si es la entidad designada en una notificación de recordatorio automático, recibirá un correo electrónico cuando se cumpla la fecha límite especificada. Para las notificaciones atrasadas, el correo electrónico se envía todas las noches hasta que se complete la tarea o el problema.

Las tareas con ciertos tipos de dependencia pueden entregarse después de la fecha de inicio especificada, aunque hayan vencido. Por ejemplo, si una tarea tiene un predecesor con una dependencia Finish-Start (fs), no se incluirá en el correo electrónico, aunque haya pasado la fecha de inicio especificada, porque no se puede iniciar la tarea hasta que el predecesor esté completo.

Para obtener más información sobre la recepción de correos electrónicos de recordatorios automáticos, consulte la [Avisos automáticos](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) en [Notificaciones de Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Enviar recordatorios automáticos

Los recordatorios automáticos se envían en cuanto se cumple la hora seleccionada por el administrador de Workfront.

Si desea almacenar en déclencheur el envío manual de correos electrónicos de recordatorio automáticos, puede hacerlo mediante Diagnósticos. Para obtener más información sobre el acceso y el uso de los diagnósticos en Workfront, consulte [Usar diagnósticos para déclencheur de procesos automatizados](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
