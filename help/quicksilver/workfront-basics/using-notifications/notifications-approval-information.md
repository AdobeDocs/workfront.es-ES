---
content-type: reference
navigation-topic: notifications
title: 'Notificaciones: Información de aprobación'
description: Las siguientes notificaciones le avisan de las actividades de aprobación que se producen en un elemento de trabajo con el que esté involucrado. Para obtener información sobre la configuración de las notificaciones que recibe, consulte Activación o desactivación de sus propias notificaciones de evento.
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 6%

---

# Notificaciones: Información de aprobación

Las siguientes notificaciones le avisan de las actividades de aprobación que se producen en un elemento de trabajo con el que esté involucrado. Para obtener información sobre la configuración de las notificaciones que recibe, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte también [Notificaciones de eventos](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificación</th> 
   <th> <p>Campos incluidos </p> <p> *Solo campos de resumen diarios</p> </th> 
   <th>Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Se completó una solicitud de aprobación delegada de problema</strong> </p> <p>Ese usuario aprobó o rechazó una aprobación de problemas que delegó en otro usuario.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Aprobación/Rechazo hecho en su nombre por] &lt;user name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de información de aprobación] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que aprobó/rechazó el problema en su nombre<br>Decisión de aprobación<br>Estado del problema<br>Nombre del usuario que solicitó la aprobación<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Número de referencia del proyecto<br>*Nombre del proyecto<br>*Número total de aprobaciones de emisión delegadas<br>*Nombre del problema<br>*Nombre del aprobador<br>*Fecha del compendio diario<br><br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó una solicitud de aprobación delegada de proyecto</strong> </p> <p>El usuario aprobó o rechazó una aprobación de proyecto delegada a otro usuario.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Aprobación/Rechazo del proyecto realizado en su nombre por] &lt;user name=""&gt;</em></p> <p><em>El tema de la notificación diaria de compendio es: [!UICONTROL Resumen de información de aprobación] &lt;date of="" daily="" digest=""&gt;</em> </p> </td> 
   <td> Nombre del proyecto<br>[!UICONTROL Portfolio Name]<br>[!UICONTROL Project Reference Number]<br>Nombre del usuario que aprobó/rechazó el proyecto en su nombre<br>[!UICONTROL Decisión de aprobación]<br>[!UICONTROL Estado del proyecto]<br>Nombre del usuario que solicitó la aprobación<br><strong>[!UICONTROL Ver Más Detalles]</strong> botón<br>*Número de referencia del proyecto<br>*Nombre del proyecto<br>*Nombre del aprobador<br>[!UICONTROL *Fecha del compendio diario]<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó una solicitud de aprobación delegada de tarea</strong> </p> <p>Ese usuario aprobó o rechazó una aprobación de tareas delegada a otro usuario.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Aprobación/Rechazo de tarea en su nombre por] &lt;user name=""&gt;</em></p> <p>El tema de la notificación diaria de compendio es:<em> [!UICONTROL Resumen de información de aprobación] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nombre de la tarea<br>Nombre del proyecto<br>Número de referencia de tarea<br>Nombre del usuario que aprobó/rechazó la tarea en su nombre<br>Decisión de aprobación<br>Estado de la tarea<br>Nombre del usuario que solicitó la aprobación<br><strong>Ver más detalles</strong> botón<br>*Número de referencia del proyecto<br>*Nombre del proyecto<br>*Número total de aprobaciones de tareas delegadas<br>*Nombre de la tarea<br>*Nombre del aprobador<br>*Fecha del compendio diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se canceló una solicitud de aprobación de documento</strong> </p> <p>El Aprobador de documento recibe una notificación por correo electrónico cuando se cancela la solicitud de aprobación del documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;user name=""&gt; [!UICONTROL ha cancelado la solicitud de aprobación del documento]</em></p> <p> <p>Nota: No puede configurar esta notificación para un correo electrónico de compendio diario.</p> </p> </td> 
   <td> Nombre del usuario que ha cancelado la solicitud de aprobación<br>[!UICONTROL Document Name] </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se me ha delegado como aprobador</strong> </p> <p>Si alguien le ha delegado una aprobación, recibirá una notificación por correo electrónico. </p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Delegado] &lt;object type=""&gt; [!UICONTROL Aprobación - Revise] &lt;object name=""&gt;</em></p> <p> <p>Nota: No puede configurar esta notificación para un correo electrónico de compendio diario.</p> </p> </td> 
   <td> <p>[!UICONTROL Nombre de objeto]<br>[!UICONTROL Nombre de objeto principal]<br>[!UICONTROL Número de referencia del objeto]<br>Nombre del usuario que envió el objeto para su aprobación<br>Nombre del usuario en nombre del que está aprobando el objeto<br>Estado del objeto<br>Fecha y hora en que se solicitó la aprobación<br>Prioridad del objeto<br>Nombre del paso de aprobación<br>[!UICONTROL Fecha de finalización prevista] del objeto<br><strong>[!UICONTROL Toma Decisión de Aprobación]</strong> botón</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se aprueba mi hoja de horas</strong> </p> <p>Cuando se aprueba el parte de horas, recibe una notificación por correo electrónico.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Hoja de horas aprobada]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> <p>Nota: No puede configurar esta notificación para un correo electrónico de compendio diario.</p> </p> </td> 
   <td> Nombre del usuario que aprobó el parte de horas<br>Fecha y hora en que se aprobó el parte de horas<br>Estado del parte de horas ([!UICONTROL Aprobado])<br>Fecha de inicio y fecha de finalización del parte de horas<br>Horas totales registradas en el parte de horas<br>Horas extra registradas en el parte de horas </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
