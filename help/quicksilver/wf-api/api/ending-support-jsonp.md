---
content-type: api
navigation-topic: api-navigation-topic
title: Finalización de la compatibilidad con JSONP
description: Finalización de la compatibilidad con JSONP
author: Becky
feature: Workfront API
role: Developer
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Finalización de la compatibilidad con JSONP

Como JSONP (Javascript con relleno) es un estándar antiguo con vulnerabilidades de seguridad conocidas, Adobe Workfront dejará de ser compatible con JSONP a partir de noviembre de 2018. Esta decisión respalda nuestra iniciativa más amplia de modernización de la plataforma Workfront.

JSONP es un estándar mediante el cual se pueden realizar solicitudes de origen cruzado o entre sitios. Muchos clientes y socios de Workfront utilizan JSONP para acceder a Workfront desde un sistema en su propio dominio como parte de una integración. JSONP permite que la aplicación de Workfront procese las solicitudes de dominios que no son de Workfront.

Si utiliza JSONP como parte de cualquiera de las integraciones de Workfront, debe actualizar la integración para utilizar el estándar CORS (Intercambio de Recursos de Origen Cruzado). Esta actualización requiere que haga lo siguiente:

1. Envíe una solicitud al equipo de asistencia de Workfront para tener cualquier dominio que se esté utilizando para realizar solicitudes de origen cruzado a nuestra lista de permitidos.

   Para que sus dominios se añadan a la lista de permitidos de CORS, póngase en contacto con el servicio de atención al cliente de Workfront en el 844-306-HELP(4357) o envíe un ticket de asistencia en línea.

   >[!NOTE]
   >
   >La adición de dominios a la lista de permitidos para CORS solo es compatible con clientes que utilizaban JSONP antes del 1 de agosto de 2018.


1. Realice cambios en el código de integración para utilizar CORS.
