---
content-type: reference
navigation-topic: notifications
title: 'Notificaciones: Aprobaciones unificadas'
description: Las siguientes notificaciones le avisan sobre las actividades de aprobación para la experiencia de aprobaciones unificadas. Para obtener información sobre cómo configurar las notificaciones que recibe, consulte Modificación de sus propias notificaciones por correo electrónico.
author: Courtney
feature: Get Started with Workfront
exl-id: 6e60a9ec-4fe0-4f3d-a4dd-8dc09d11b834
last-update: 2026-10-20T00:00:00.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 7957c410d4a0e39b23b4f5a3d29a794e5deec72a
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 3%
---
# Notificaciones: Aprobaciones unificadas

{{highlighted-preview}}

Utilice las siguientes notificaciones para mantenerse informado sobre la actividad de para la revisión unificada y las aprobaciones. Para obtener información sobre cómo configurar las notificaciones por correo electrónico que recibes, consulta [Modificar tus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Estas notificaciones solo están disponibles como notificaciones instantáneas y no están disponibles en un resumen diario.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificación</th> 
   <th>Campos incluidos</th> 
   <th>Estado predeterminado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Aprobación finalizada - Aprobada</strong> </p> <p>La aprobación de un documento finaliza con una decisión final de Aprobado.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Decisión final: (Documento) aprobada</em></p> </td> 
   <td> <p>Decisión final<br>Documento<br>Fecha solicitada de aprobación<br>Fecha de vencimiento<br> Botón "Ir a revisión"<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Mensaje personalizado<br>Fase<br>Proyecto</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Aprobación finalizada - Aprobada con cambios</strong> </p> <p>La aprobación de un documento finaliza con una decisión final de Aprobado con cambios.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Decisión final: (Documento) se aprueba con cambios</em></p> </td> 
   <td> <p>Decisión final<br>Documento<br>Fecha solicitada de aprobación<br>Fecha de vencimiento<br> Botón "Ir a revisión"<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Mensaje personalizado<br>Fase<br>Proyecto</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Aprobación finalizada - Necesita trabajo</strong> </p> <p>La aprobación de un documento finaliza con una decisión final de Necesidades de trabajo.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Decisión final: (Documento) necesita trabajo</em></p> </td> 
   <td> <p>Decisión final<br>Documento<br>Fecha solicitada de aprobación<br>Fecha de vencimiento<br> Botón "Ir a revisión"<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Mensaje personalizado<br>Fase<br>Proyecto</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se acerca el plazo</strong> </p> <p>La aprobación de documento de la que forma parte se acerca a su fecha límite.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Se acerca el plazo de aprobación para (documento)</em></p> </td> 
   <td> <p>Solicitante<br>Su función<br>Equipo<br>Fecha solicitada de aprobación<br>Fecha de vencimiento<br>"Ir a la revisión" botón<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Vista previa del documento<br>Mensaje personalizado<br>Fase<br>Proyecto</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se superó el plazo</strong> </p> <p>Una aprobación de documento de la que forma parte pasa su fecha límite sin una decisión final.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Se superó el plazo de aprobación de (documento)</em></p> </td> 
   <td> <p>Titular fijo<br>Fecha solicitada de aprobación<br>Fecha de vencimiento<br> Botón "Ir a revisión"<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Fase</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Revisión completada</strong> </p> <p>Un revisor finaliza la revisión de una aprobación de documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>(documento) se ha revisado</em></p> </td> 
   <td> <p>Revisor<br>Documento<br>"Ir a revisión" botón<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Vista previa del documento<br>Fase<br>Proyecto</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se acerca el límite de aprobación de vídeo (80 %)</strong> </p> <p>Una aprobación de vídeo alcanza el 80 % del límite de aprobación de vídeo de su plan.</p> <p>El asunto del mensaje de correo electrónico de notificación instantánea es: <em>Estás cerca del límite anual de solicitudes de aprobación de vídeo en Workfront</em></p> </td> 
   <td> Titular y texto del cuerpo<br>Se solicitan aprobaciones de vídeo (uso actual)<br>Límite total (el límite)<br>Otros destinatarios<br> Botón "Ver en Workfront"<br> Botón "Actualizar a FIO enterprise" </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se ha alcanzado el límite de aprobación de vídeo</strong> </p> <p>Una aprobación de vídeo alcanza el límite de aprobación de vídeo de su plan.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Ha alcanzado el límite anual de solicitudes de aprobación de vídeo en Workfront</em></p> </td> 
   <td> Titular y texto del cuerpo<br>Se solicitan aprobaciones de vídeo (uso actual)<br>Límite total (el límite)<br>Otros destinatarios<br> Botón "Ver en Workfront"<br> Botón "Actualizar a FIO enterprise" </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Decisión tomada - Aprobada</strong> </p> <p>Un aprobador toma una decisión de Aprobado al aprobar un documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>(documento) aprobado por (nombre)</em></p> </td> 
   <td> <p>Responsable de la toma de decisiones<br>Decisión<br>Documento y versión<br>"Ir a revisión" botón<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Vista previa del documento<br>Mensaje personalizado<br>Fase<br>Proyecto</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Decisión tomada - Aprobada con cambios</strong> </p> <p>Un aprobador toma una decisión de Aprobado con cambios en una aprobación de documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>(documento) aprobado con cambios por (nombre)</em></p> </td> 
   <td> <p>Responsable de la toma de decisiones<br>Decisión<br>Documento y versión<br>"Ir a revisión" botón<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Vista previa del documento<br>Mensaje personalizado<br>Fase<br>Proyecto</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Decisión tomada - Necesita trabajo</strong> </p> <p>Un aprobador toma una decisión de Necesita trabajar en una aprobación de documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>(documento) necesita trabajar por (nombre)</em></p> </td> 
   <td> <p>Responsable de la toma de decisiones<br>Decisión<br>Documento y versión<br>"Ir a revisión" botón<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Vista previa del documento<br>Mensaje personalizado<br>Fase<br>Proyecto</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Documentos agregados o eliminados de una aprobación agrupada</strong> </p> <p>Los documentos se agregan o eliminan de una aprobación de documento agrupada de la que forma parte.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Se agregó o eliminó un documento de una aprobación de la que es parte</em></p> </td> 
   <td> <p><strong>Añadido:</strong><br>Solicitante<br>Nombre del grupo<br>Vista previa en miniatura<br>Fechas<br>"Ir a revisión" botón<br>Bloque de detalles: Nombre del grupo, Número de recursos, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Mensaje personalizado<br>Proyecto</p> <p><strong>Eliminado:</strong><br>Solicitante<br>Nombre del grupo<br>Vista previa en miniatura (sin botón ni bloque de detalles)</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Todas las revisiones completadas</strong> </p> <p>Todos los revisores completan su revisión cuando aprueban un documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Todas las revisiones se completaron el (Documento)</em></p> </td> 
   <td> <p>Documento<br>Fecha solicitada de aprobación<br>Fecha de vencimiento<br> Botón "Ir a revisión"<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Mensaje personalizado<br>Fase<br>Proyecto</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Recordatorio - 24 horas</strong> </p> <p>Le quedan 24 horas para revisar y aprobar el documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Recordatorio: se necesita su aprobación el (documento)</em></p> </td> 
   <td> <p>Solicitante<br>Su función<br>Equipo<br>Fecha solicitada de aprobación<br>Fecha de vencimiento<br>"Ir a la revisión" botón<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Vista previa del documento<br>Mensaje personalizado<br>Fase<br>Proyecto</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Recordatorio - 72 horas</strong> </p> <p>Le quedan 72 horas para revisar y aprobar el documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Recordatorio: se necesita su aprobación el (documento)</em></p> </td> 
   <td> <p>Solicitante<br>Su función<br>Equipo<br>Fecha solicitada de aprobación<br>Fecha de vencimiento<br>"Ir a la revisión" botón<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Vista previa del documento<br>Mensaje personalizado<br>Fase<br>Proyecto</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se agregó como aprobador o revisor</strong> </p> <p>Se le agregará como aprobador o revisor al aprobar un documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Se necesita su aprobación el (Documento)</em></p> </td> 
   <td> <p>Solicitante<br>Su función<br>Equipo<br>Fecha solicitada de aprobación<br>Fecha de vencimiento<br>"Ir a la revisión" botón<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Vista previa del documento<br>Mensaje personalizado<br>Fase<br>Proyecto</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eliminado como aprobador o revisor</strong> </p> <p>Se le eliminará como aprobador o revisor de una aprobación de documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Ya no se necesita su aprobación el (Documento)</em></p> </td> 
   <td> <p>Solicitante<br>Documento y versión<br>Rol<br>Equipo (sin botón ni bloque de detalles)</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Vista previa del documento<br>Mensaje personalizado</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Se cambió la función</strong> </p> <p>Su función de aprobador o revisor cambia al aprobar un documento.</p> <p>El asunto del correo electrónico de notificación instantánea es: <em>Su rol en (Documento) ha cambiado</em></p> </td> 
   <td> <p>Solicitante<br>Documento y versión<br>Cambio de dirección de la función<br> Botón "Ir a revisión"<br>Bloque de detalles: Nombre del documento, Detalles del documento, Todos los destinatarios</p> <p><em>Incluido cuando forma parte de la aprobación:</em><br>Vista previa del documento<br>Fase<br>Proyecto</p> </td> 
   <td><strong>Instantáneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
