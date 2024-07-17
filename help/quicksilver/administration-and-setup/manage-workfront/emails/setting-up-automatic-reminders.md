---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Configurar recordatorios automáticos
description: Configurar recordatorios automáticos
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 4%

---

# Configurar recordatorios automáticos

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como administrador de Adobe Workfront, puede configurar recordatorios automáticos para almacenar en déclencheur las notificaciones por correo electrónico cuando todas las tareas o problemas venzan, se retrasen o estén cerca de la fecha planificada de finalización. Después de establecer esta configuración, los usuarios no pueden deshabilitar los avisos automáticos.

Para las notificaciones tardías, el correo electrónico se envía todas las noches hasta que se complete la tarea o el problema.

Se puede enviar un recordatorio automático a una o varias de las siguientes direcciones:

* Los usuarios asignados a una tarea o un problema
* El responsable inmediato del usuario
* El gerente del gerente inmediato

>[!NOTE]
>
>No puede cambiar el contenido ni la línea de asunto del correo electrónico activado por un recordatorio automático.

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

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Haga clic en **Correo electrónico** >**Recordatorios automáticos**.

1. En el área **Enviar una notificación tardía a**, seleccione cualquiera de las siguientes opciones:

   <table>
    <tr>
        <td>El usuario "Asignado a"</td>
        <td>Seleccione esta opción si desea que el usuario asignado a una tarea o problema reciba una notificación tardía sobre el retraso de su elemento de trabajo.</td>
        <td></td>
    </tr>
    <tr>
        <td>El gerente de ese usuario</td>
        <td>Seleccione esta opción si desea que el administrador del usuario reciba una notificación tardía sobre el retraso de un elemento de trabajo del informe directo.</td>
        <td></td>
    </tr>
    <tr>
        <td>El gerente de ese gerente</td>
        <td>Seleccione esta opción si desea que el administrador del administrador inmediato reciba una notificación tardía sobre un elemento de trabajo de uno de los usuarios de su informe directo que está atrasado.</td>
        <td></td>
    </tr>
    <tr>
        <td>El usuario "Asignado a"</td>
        <td>(En el área <b>Enviar recordatorio de fecha límite al área </b>). Seleccione esta opción si desea que el usuario asignado a una tarea o un problema reciba una notificación sobre su elemento de trabajo cuando se aproxime la fecha de vencimiento.</td>
        <td></td>
    </tr>
</table>

1. Seleccione la hora de envío del recordatorio automático seleccionando la cantidad de tiempo antes o después de la fecha de vencimiento del elemento de trabajo.

   El tiempo se calcula a partir de la fecha planificada de finalización de la tarea o problema.

   Especifique el número de minutos, horas, días, semanas o meses para agregar tiempo a la Fecha planificada de finalización de las tareas o problemas. Seleccione **Minutos transcurridos**, **Horas transcurridas**, **Días transcurridos** o **Semanas transcurridas** para agregar tiempo que incluya cualquier fin de semana, festivos y horas no laborables como se indica en su programación.

   Por ejemplo, si una tarea se asigna el viernes y tiene una duración de 3 días transcurridos, la fecha de finalización de la tarea se establece en lunes (suponiendo que sábado y domingo sea fin de semana). Si la tarea tiene una duración de 3 días (no transcurridos), la fecha de finalización de la tarea se establece en miércoles.

   ![](assets/time-increments-for-automatic-reminder.png)

1. Haga clic en **Guardar**.

## Recibir recordatorios automáticos

Si usted es la entidad designada en una notificación de recordatorio automático, recibirá un correo electrónico cuando se cumpla la fecha límite especificada. Para las notificaciones tardías, el correo electrónico se envía todas las noches hasta que se complete la tarea o el problema.

Las tareas con ciertos tipos de dependencias pueden entregarse después de la fecha de inicio especificada, aunque hayan vencido. Por ejemplo, si una tarea tiene una tarea predecesora con una dependencia Fin-Comienzo (fs), no se incluirá en el mensaje de correo electrónico, aunque se haya pasado la fecha de comienzo especificada, porque no se puede iniciar la tarea hasta que se complete la predecesora.

Para obtener más información sobre cómo recibir correos electrónicos de recordatorios automáticos, consulte la sección [Recordatorios automáticos](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) en [notificaciones de Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Envío de recordatorios automáticos

Los recordatorios automáticos se envían en cuanto se cumple la hora seleccionada por el administrador de Workfront.

Si desea almacenar en déclencheur el envío manual de los correos electrónicos de recordatorio automático, puede hacerlo mediante Diagnóstico. Para obtener más información acerca del acceso y uso de los diagnósticos en Workfront, vea [Usar diagnósticos para almacenar en déclencheur procesos automatizados](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
