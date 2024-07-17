---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Explicación de la migración de Workfront a Adobe Admin Console
description: Este artículo describe en términos generales el proceso de mover una organización a Adobe Admin Console, para que usted como administrador de Workfront pueda saber qué esperar.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: 633c41eeb570402254125f92f3624cad7befd609
workflow-type: tm+mt
source-wordcount: '1114'
ht-degree: 0%

---

# Explicación de la migración de Workfront a Adobe Admin Console

El Adobe está cambiando la forma de administrar los usuarios de Adobe Workfront, lo que aumenta la productividad para usted y su organización. Como parte de este cambio, el Adobe de está migrando la instancia de Workfront y los usuarios a Adobe Admin Console. Se trata de una migración necesaria que no afecta a los informes, rutas de aprobación, contenido ni recursos. Afectará a cómo administra el acceso de los usuarios y cómo inician sesión.

Este artículo describe en términos generales el proceso de mover una organización a Adobe Admin Console, para que usted como administrador de Workfront pueda saber qué esperar.

Para obtener información sobre cómo usar Adobe Admin Console para administrar los derechos de Adobe en toda la organización, consulte [Administrar usuarios en Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## ¿Qué está cambiando?

Como parte de la migración, la administración de usuarios se moverá desde la aplicación de Workfront a Adobe Admin Console con las siguientes funciones administrativas:

* **Los administradores del sistema** son superusuarios con privilegios de todos los administradores. Asignan todas las funciones administrativas y administran los usuarios de toda la organización para todos los productos.

* **Administradores de perfil de producto (administradores del sistema de Workfront)** administran qué usuarios de la organización obtienen acceso a Workfront.

* **Los usuarios iniciarán sesión con la identidad de Adobe.** Después de que el Adobe migre a los usuarios existentes a Adobe Admin Console, los usuarios iniciarán sesión en sus instancias de Workfront con su nueva identidad de Adobe: un Adobe ID o un Federated ID de Adobe (SSO).

* **No hay cambios en la forma de administrar todas las demás funciones** de la propia aplicación de Workfront, incluida la administración de características, funciones de usuario, espacios de trabajo, funcionalidad y comportamiento.

## Cronología del Recorrido de migración

El Adobe migrará primero la instancia de Workfront a Adobe Admin Console y, a continuación, todos los usuarios existentes con direcciones de correo electrónico comprobadas. Si es administrador del sistema o del perfil de producto de Workfront (administrador del sistema de Workfront), recibirá correos electrónicos que le guiarán a través del recorrido de migración. Esta es una cronología de lo que puede esperar:

### Migración de Workfront a Adobe Admin Console completada

Los administradores del sistema recibirán un correo electrónico cuando se complete la migración de Workfront a Adobe Admin Console. En este momento, es posible que los administradores del sistema tengan que completar algunos pasos necesarios **antes de que comience la migración de usuarios**, para minimizar el impacto a los usuarios de Workfront.

* **Si los usuarios de Workfront inician sesión con SSO**, debe configurar el SSO en Adobe Admin Console para que los usuarios puedan continuar iniciando sesión con SSO. Si los usuarios de Workfront no utilizan actualmente el SSO, pero desea configurarlo en Adobe Admin Console, puede hacerlo en este punto del recorrido de migración.
* **Si ya administra otros productos de Adobe en su Adobe Admin Console**, es posible que Adobe solicite su consentimiento para migrar automáticamente a los usuarios a su consola existente. Haga clic en el botón **Comenzar** del correo electrónico para ir a la página de consentimiento.
* **Si ha eliminado anteriormente el tipo de licencia de solicitante**, se agregará a su sistema. No se asignará ningún usuario a este tipo de licencia, pero es necesario para la sincronización entre Workfront y Adobe Admin Console. No es necesario que realice ninguna acción en relación con el tipo de licencia de solicitante.

No hay cambios en la administración de usuarios en este momento. Los administradores de Workfront seguirán administrando usuarios en Workfront y los usuarios seguirán iniciando sesión con su Workfront ID o SSO hasta que se complete la migración de usuarios.

### Programar migración de usuarios

Una vez que el administrador del sistema complete los requisitos previos descritos en la sección anterior, el Adobe programará automáticamente la migración de usuario durante 30 días después de que se completen estos requisitos previos y se comunicará con los administradores del perfil de producto de Workfront (administradores del sistema de Workfront) para administrar la migración de usuario.

Los administradores de perfil de producto de Workfront (administradores de sistema de Workfront):

* Reciba un correo electrónico con la fecha de inicio de la migración de usuarios programada (unos 30 días después de que se cumplan estos requisitos previos)
* Obtenga acceso a la consola de administrador de Workfront designada, donde tiene la opción de cambiar la fecha de migración

  >[!NOTE]
  >
  >Debido a la complejidad de la migración, los cambios de fecha están restringidos a no más de 30 días después de la fecha programada. Póngase en contacto con el servicio de asistencia si necesita una fecha posterior.

* Reciba un correo electrónico recordatorio 1 día antes de la fecha de inicio de la migración de usuarios

### Preparar usuarios para el día de la migración

Como administrador de Perfil de producto de Workfront (administrador del sistema de Workfront), es responsable de garantizar que todos los usuarios estén preparados para el día de la migración.

* Prepare a todos los usuarios para la próxima migración a la identidad de Adobe notificándoles lo siguiente:

   * A medida que los usuarios migren, recibirán un correo electrónico del Adobe de notificándoles el cambio en la forma en que inician sesión en Workfront. Se invitará a los usuarios a aceptar una invitación para iniciar sesión con ID de Adobe por primera vez, ya sea iniciando sesión con un Adobe ID existente o configurando uno nuevo con la misma dirección de correo electrónico.

### Qué esperar el día de la migración

* **La migración de usuarios comenzará a medianoche del centro de datos de Workfront que aloja al cliente.**

* **El Adobe migrará automáticamente primero a los administradores de Workfront.** Cuando los administradores de Workfront se migren a la identidad de Adobe, se les asignará la función de administrador del perfil de producto de Adobe (administrador del sistema de Workfront). Las funciones existentes que un usuario pueda tener antes de la migración no se verán afectadas.

  >[!NOTE]
  >
  >No se perderá el acceso al producto durante la migración de usuarios. Si un usuario ha iniciado sesión durante el tiempo en el que se está migrando su usuario, no habrá ningún impacto. Sin embargo, en el siguiente inicio de sesión se les pedirá que utilicen su identidad de Adobe.



* **A medida que los usuarios se migren, recibirán un mensaje de correo electrónico del Adobe notificándoles el cambio en la forma en que inician sesión en Workfront.Se invitará a** usuarios a aceptar una invitación para iniciar sesión con la identidad de Adobe por primera vez, ya sea iniciando sesión con una Adobe ID existente o configurando una Adobe ID nueva con la misma dirección de correo electrónico.

  Para obtener información sobre cómo iniciar sesión en Workfront con un Adobe ID, consulte [Iniciar sesión en Adobe Experience Cloud](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### Migración de usuarios completada

El Adobe de notificará por correo electrónico a todos los administradores del sistema y a los administradores del perfil de producto (administradores del sistema de Workfront) una vez migrados todos los administradores y usuarios. En este momento, todos los usuarios de Workfront para esa instancia iniciarán sesión en Workfront mediante Identidad de Adobe. Los administradores de sistemas de Workfront y de perfiles de producto (administradores de sistemas de Workfront) pueden administrar el acceso de los usuarios dentro de Adobe Admin Console. Si los clientes no utilizan una forma de sincronización de directorios en la consola de administración, pueden seguir gestionando el acceso a Workfront en la aplicación de Workfront.

## Obtener asistencia

Si tiene alguna pregunta o inquietud, siga los pasos descritos en el artículo [Comuníquese con la atención al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).




