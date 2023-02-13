---
content-type: api
navigation-topic: api-navigation-topic
title: Finalización de la compatibilidad con JSONP
description: Finalización de la compatibilidad con JSONP
author: John
feature: Workfront API
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Finalización de la compatibilidad con JSONP

Como JSONP (Javascript con margen) es un estándar antiguo con vulnerabilidades de seguridad conocidas, Adobe Workfront dejará de ser compatible con JSONP a partir de noviembre de 2018. Esta decisión apoya nuestra iniciativa más amplia de modernizar la plataforma Workfront.

JSONP es un estándar mediante el cual se pueden realizar solicitudes entre orígenes o sitios. Muchos clientes y socios de Workfront utilizan JSONP para acceder a Workfront desde un sistema en su propio dominio como parte de una integración. JSONP permite que la aplicación Workfront procese solicitudes de dominios que no sean de Workfront.

Si utiliza JSONP como parte de cualquiera de las integraciones de Workfront, debe actualizar la integración para que utilice el estándar CORS (Uso compartido de recursos de origen cruzado). Esta actualización requiere que haga lo siguiente:

1. Envíe una solicitud al equipo de asistencia de Workfront para que tenga cualquier dominio que se esté utilizando para realizar solicitudes de origen cruzado a nuestra lista de permitidos.

   Para que sus dominios se añadan a la lista de permitidos de CORS, póngase en contacto con el servicio de asistencia al cliente de Workfront al 844-306-HELP(4357) o envíe un ticket de asistencia en línea.

   >[!NOTE]
   >
   >Añadir dominios a la lista de permitidos para CORS solo es compatible con los clientes que utilizaban JSONP antes del 1 de agosto de 2018.


1. Realice cambios en el código de integración para utilizar CORS.
