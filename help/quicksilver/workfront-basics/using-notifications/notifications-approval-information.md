---
content-type: reference
navigation-topic: notifications
title: "Notificaciones: Información de aprobación"
description: Las siguientes notificaciones le avisan sobre las actividades de aprobación que se producen en un elemento de trabajo con el que está involucrado. Para obtener información sobre cómo configurar las notificaciones que recibe, consulte Modificación de sus propias notificaciones por correo electrónico.
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# Notificaciones: Información de aprobación

Las siguientes notificaciones le avisan sobre las actividades de aprobación que se producen en un elemento de trabajo con el que está involucrado. Para obtener información sobre cómo configurar las notificaciones que recibe, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte también [Notificaciones de eventos](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificación</th> 
   <th> <p>Campos incluidos </p> <p> *Solo campos de resumen diario</p> </th> 
   <th>Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Se completó una solicitud de aprobación delegada de problema</strong> </p> <p>Ese usuario aprobó o rechazó una aprobación de problema que delegó en otro usuario.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Aprobación/rechazo del problema hecho a nombre suyo por] &lt;Nombre de usuario&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de la información de aprobación] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> <p>Nombre del problema<br>Nombre del proyecto<br>Número de referencia del problema<br>Nombre del usuario que aprobó o rechazó el problema en su nombre<br>Decisión de aprobación<br>Estado del problema<br>Nombre del usuario que solicitó la aprobación<br><strong>[!UICONTROL Ver más detalles]</strong> button<br>*Número de referencia del proyecto<br>*Nombre del proyecto<br>*Número total de aprobaciones delegadas del problema<br>*Nombre del problema<br>*Nombre del aprobador<br>*Fecha del resumen diario<br><br></p> </td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó una solicitud de aprobación delegada de proyecto</strong> </p> <p>Ese usuario aprobó o rechazó una aprobación de proyecto que delegó en otro usuario.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Aprobación/rechazo del proyecto hecho a nombre suyo por] &lt;Nombre de usuario&gt;</em></p> <p><em>El asunto de la notificación de resumen diario es: [!UICONTROL Resumen de la información de aprobación] &lt;Fecha del resumen diario&gt;</em> </p> </td> 
   <td> Nombre del proyecto<br>[!UICONTROL Nombre del Portfolio]<br>[!UICONTROL Número de referencia del proyecto]<br>Nombre del usuario que aprobó o rechazó el proyecto en su nombre<br>[!UICONTROL Decisión de aprobación de]<br>[!UICONTROL Estado del proyecto]<br>Nombre del usuario que solicitó la aprobación<br><strong>[!UICONTROL Ver más detalles]</strong> botón<br>*Número de referencia del proyecto<br>*Nombre del proyecto<br>*Nombre del aprobador<br>[!UICONTROL *Fecha del resumen diario]<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se completó una solicitud de aprobación delegada de tarea</strong> </p> <p>Ese usuario aprobó o rechazó una aprobación de tarea que delegó en otro usuario.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Aprobación/rechazo de tarea hecho a nombre suyo por] &lt;Nombre de usuario&gt;</em></p> <p>El asunto de la notificación de resumen diario es:<em> [!UICONTROL Resumen de la información de aprobación] &lt;Fecha del resumen diario&gt;</em></p> </td> 
   <td> Nombre de tarea<br>Nombre de proyecto<br>Número de referencia de tarea<br>Nombre del usuario que aprobó o rechazó la tarea en su nombre<br>Decisión de aprobación<br>Estado de la tarea<br>Nombre del usuario que solicitó la aprobación<br><strong>Ver más detalles</strong> botón<br>*Número de referencia del proyecto<br>*Nombre del proyecto<br>*Número total de aprobaciones delegadas de tareas<br>*Nombre de tarea<br>*Nombre del aprobador<br>*Fecha del resumen diario<br></td> 
   <td><strong>Diariamente</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se canceló una solicitud de aprobación de documento</strong> </p> <p>El aprobador del documento recibe una notificación por correo electrónico cuando se cancela la solicitud de aprobación del documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>&lt;Nombre de usuario&gt; [!UICONTROL canceló la solicitud de aprobación de documento]</em></p> <p> <p>Nota: No puede configurar esta notificación para un correo electrónico de resumen diario.</p> </p> </td> 
   <td> Nombre del usuario que canceló la solicitud de aprobación <br>[!UICONTROL Document Name] </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se me ha delegado como aprobador</strong> </p> <p>Si alguien le delegó una aprobación, recibe una notificación por correo electrónico. </p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Delegado] &lt;Tipo de objeto&gt; [!UICONTROL Aprobación - Favor de revisar] &lt;Nombre de objeto&gt;</em></p> <p> <p>Nota: No puede configurar esta notificación para un correo electrónico de resumen diario.</p> </p> </td> 
   <td> <p>[!UICONTROL Nombre del objeto]<br>[!UICONTROL Nombre del objeto principal]<br>[!UICONTROL Número de referencia del objeto]<br>Nombre del usuario que envió el objeto para su aprobación<br>Nombre del usuario en nombre del cual está aprobando el objeto<br>Estado del objeto<br>Fecha y hora en que se solicitó la aprobación<br>Prioridad del objeto<br>Nombre del paso de aprobación<br>[!UICONTROL Fecha planificada de finalización] del objeto<br><strong>[!UICONTROL Tomar decisión de aprobación]</strong> botón</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se aprobó mi hoja de horas</strong> </p> <p>Cuando se apruebe la plantilla de horas, recibirá una notificación por correo electrónico.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>[!UICONTROL Hoja de horas aprobada]: &lt;Fecha de inicio de la hoja de horas&gt; - &lt;Fecha de finalización de la hoja de horas&gt;</em></p> <p> <p>Nota: No puede configurar esta notificación para un correo electrónico de resumen diario.</p> </p> </td> 
   <td> Nombre del usuario que aprobó su hoja de horas<br>Fecha y hora en que se aprobó la hoja de horas<br>Estado de la hoja de horas ([!UICONTROL Aprobado])<br>Fecha de inicio y fecha de finalización de la hoja de horas<br>Total de horas registradas en la hoja de horas<br>Horas extra registradas en la hoja de horas </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
