---
content-type: reference
navigation-topic: announcements
title: Los clientes de los clústeres 1, 2 y 3 deben actualizar cualquier bloque de IP de lista de permitidos para evitar el bloqueo de los servicios de Adobe Workfront
description: Para mejorar nuestra infraestructura principal, pronto migraremos los clientes de Adobe Workfront de los clústeres 01, 02 y 03 a la nube pública de AWS.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Los clientes de los clústeres 1, 2 y 3 deben actualizar cualquier bloque de IP de lista de permitidos para evitar el bloqueo de los servicios de Adobe Workfront

Para mejorar nuestra infraestructura principal, pronto migraremos los clientes de Adobe Workfront de los clústeres 01, 02 y 03 a la nube pública de AWS.

Como parte de este cambio, debe agregar las siguientes IP a los bloques de IP de lista de permitidos para evitar el bloqueo de los servicios de Workfront:

Para SSO y POP:

* 34 215 145 168
* 54.69.155.48
* 35.160.44.226
* 34 213 96 218
* 3.16.210.22
* 3.16.229.153
* 18 224 117 99
* 18.123.153
* 3 211 159 196
* 3.85.255.45
* 3.210.78.197
* 3 211 23 183

Para correo electrónico:

* 54 240 60 174
* 54 240 60 175

Asegúrese de que los bloques de IP de lista de permitidos estén actualizados antes del 13 de mayo de 2019. Para obtener más información, consulte [Configuración de la lista de permitidos del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Gracias por su continuo apoyo a Workfront, ya que trabajamos para crear una experiencia más fiable y sólida para nuestros clientes.

Si tiene alguna pregunta adicional, póngase en contacto con nuestro equipo de asistencia visitando experience.workfront.com o llamando al 844.306.4357 (EE. UU.) o al +44.1256.274200 (EMEA).

## FAQ

### ¿Por qué Workfront está realizando este cambio?

En un esfuerzo por proporcionar a nuestros clientes el mejor servicio posible de forma consistente, Workfront busca constantemente formas de mejorar la experiencia del usuario. Este cambio hace uso de nuevas tecnologías que nos permiten ofrecer la mejor experiencia posible y mejorar nuestro ya robusto modelo de seguridad.

### ¿Qué acciones debo realizar como administrador de Workfront?

Póngase en contacto con su departamento interno de TI o de seguridad para obtener ayuda con la revisión de los bloques de IP de lista de permitidos y la adición de las IP enumeradas anteriormente.

### ¿Qué puede esperar mi organización si no realizamos este cambio?

No podrá acceder a los servicios de Workfront a medida que migremos los servicios a las nuevas IP.
