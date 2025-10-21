---
content-type: reference
navigation-topic: get-started-with-workfront
title: Preparación para HIPAA para Workfront
description: Un cliente de Workfront que, tal como se define en HIPAA, es un Asociado Comercial y/o la Entidad Cubierta en cuyo nombre el Asociado Comercial proporciona Adobe Workfront debe utilizar las siguientes directrices para configurar Workfront para el uso compatible con HIPAA.
feature: Get Started with Workfront
author: Courtney
exl-id: e3cdaa03-d523-46a4-954b-8456d5f190e4
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Preparación para HIPAA para Workfront

Un cliente de Workfront que, tal como se define en la HIPAA, es un socio comercial y/o la entidad cubierta en cuyo nombre el socio comercial proporciona Adobe Workfront debe utilizar las siguientes directrices para configurar Workfront para el uso compatible con HIPAA:


## Requisitos de contraseña

| **Configuración de seguridad** | **¿Qué Es?** | **Requisito** |
|----------------------|------------------|------------------|
| Seguridad mínima de contraseña para acuerdos | ¿Cuál es la seguridad mínima de las contraseñas de acuerdo? | No menos de 8 caracteres |
| Seguridad mínima de las contraseñas de usuario | ¿Cuál es la seguridad mínima de las contraseñas de los usuarios? | Caracteres de tres de las siguientes categorías:<br> Letras mayúsculas (alfabeto latino)<br> Letras minúsculas (alfabeto latino)<br> Base 10 dígitos<br> Caracteres no alfanuméricos |
| Duración de contraseña | ¿Durante cuánto tiempo se debe permitir que las contraseñas permanezcan sin cambios? | Las contraseñas deben cambiarse al menos cada 90 días |
| Historial de contraseñas | ¿Cuántas contraseñas pasadas deben recordarse y no permitirse? | No menos de 5 |


## Requisitos de inicio de sesión

| **Configuración de seguridad** | **¿Qué Es?** | **Requisito** |
|----------------------|------------------|------------------|
| Máximo de errores de inicio de sesión | ¿Cuántos intentos de inicio de sesión erróneos hacen que el usuario esté bloqueado? | No más de 5 intentos dentro de un período de 5 minutos; se permiten reintentos pasados 30 minutos |
| Máximo de errores de verificación de SSO | ¿Cuántos intentos de verificación de SSO fallidos causan un bloqueo? | No más de 5 (se aplica solo a los clientes que utilizan SSO) |


## Requisitos de sesión

| **Configuración de seguridad** | **¿Qué Es?** | **Requisito** |
|----------------------|------------------|------------------|
| Tiempo de espera de sesión | ¿Cuántos minutos de inactividad provocan un cierre de sesión? | No más de 15 minutos |

## Responsabilidades del cliente

Asegúrese de que todos los empleados, representantes o agentes conozcan y comprendan los términos de las licencias o los acuerdos de servicio firmados entre las partes, según corresponda, relevantes para el uso de los datos con Workfront.

En particular, deben revisarse y comunicarse las siguientes responsabilidades y obligaciones: 

* El cliente es responsable del uso del Servicio de Workfront por parte de todos sus usuarios. 

* El cliente debe cumplir todos los términos de su acuerdo con Adobe que incluyen la carga de elementos de datos prohibidos en Workfront. 

* Cualquier dato sensible, incluyendo, pero no limitado a ePHI, se carga bajo el propio riesgo del cliente.  El cliente es en todo momento responsable de todos los datos del cliente. 


## Protección de datos y cumplimiento normativo

>[!IMPORTANT]
>
>Workfront no está diseñado para ser un repositorio de registros médicos electrónicos (EHR). La información protegida sobre su salud sólo puede ser procesada si Adobe la autoriza expresamente por escrito. 

* Para cualquier base de datos de Workfront donde se pueda tener acceso a ePHI, asegúrese de que **Encryption at Rest (EAR)** esté habilitado.
   * Póngase en contacto con su ejecutivo de cuentas (AEM) para verificar que el EAR esté incluido en su compra de Workfront.
   * Configurar sistemas/bases de datos accesibles a través de Workfront para cumplir con las obligaciones de cumplimiento.
* Asegúrese de que ePHI no se transfiera, vincule o comparta con otras soluciones de Adobe no preparadas para HIPAA.
* Asegúrese de que las fotografías de los pacientes procesadas mediante Workfront se almacenen de forma segura y no sean de acceso público.
