---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Explicación de la migración de Workfront a Adobe Admin Console
description: Este artículo describe en términos generales el proceso de mover una organización a Adobe Admin Console para que usted como administrador de Workfront sepa qué debe esperar.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 98%

---

# Explicación de la migración de Workfront a Adobe Admin Console

<!--DELETE ME MARCH 2026-->

>[!IMPORTANT]
>
>Todas las organizaciones de Workfront se han incorporado a Adobe Admin Console.
>
>Este artículo se eliminará en un futuro próximo.

Adobe está cambiando la forma de administrar los usuarios de Adobe Workfront, lo que le permite aumentar la productividad tanto a usted como a su organización. Como parte de este cambio, Adobe está migrando su instancia de Workfront y usuarios a Adobe Admin Console. Se trata de una migración necesaria y no afectará a ningún informe, ruta de aprobación, contenido ni recursos. Afectará a cómo administra el acceso de los usuarios y cómo estos inician sesión.

Este artículo describe en términos generales el proceso de mover una organización a Adobe Admin Console para que usted como administrador de Workfront sepa qué debe esperar.

Para obtener más información sobre cómo usar Adobe Admin Console para administrar los derechos de Adobe en toda la organización, consulte [Administrar usuarios en Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## ¿Qué está cambiando?

Como parte de la migración, la administración de usuarios se va a mover desde la aplicación de Workfront a Adobe Admin Console con las siguientes funciones administrativas:

* **Los administradores del sistema** son superusuarios con privilegios de todos los administradores. Asignan todas las funciones administrativas y administran los usuarios de toda la organización para todos los productos.

* **Los administradores con perfil de producto (administradores del sistema de Workfront)** administran qué usuarios de la organización obtienen acceso a Workfront.

* **Los usuarios iniciarán sesión con una identidad de Adobe.** Después de que Adobe migre los usuarios existentes a Adobe Admin Console, los usuarios iniciarán sesión en sus instancias de Workfront con su nueva identidad de Adobe, ya sea con Adobe ID o con Federated ID de Adobe (SSO).

* **No hay cambios en la forma de administrar todas las demás funcionalidades** de la propia aplicación de Workfront, incluida la administración de características, funciones de usuario, espacios de trabajo, funcionalidad y comportamiento.

## Cronología del recorrido de migración

Adobe migrará primero la instancia de Workfront a Adobe Admin Console y, a continuación, todos los usuarios existentes con direcciones de correo electrónico comprobadas. Si usted es administrador del sistema o de perfiles de producto de Workfront (administrador del sistema de Workfront), recibirá correos electrónicos que le guiarán por el recorrido de la migración. Esta es una cronología de lo que puede esperar:

### Migración de Workfront a Adobe Admin Console completada

Los administradores del sistema recibirán un correo electrónico cuando se complete la migración de Workfront a Adobe Admin Console. En este momento, es posible que los administradores del sistema tengan que completar algunos pasos necesarios **antes de que comience la migración de usuarios**, para minimizar el impacto a los usuarios de Workfront.

* **Si los usuarios de Workfront inician sesión con SSO**, debe configurar el SSO en Adobe Admin Console para que los usuarios puedan continuar iniciando sesión con SSO. Si los usuarios de Workfront actualmente no utilizan SSO, pero desea configurarlo en Adobe Admin Console, puede hacerlo en este punto del recorrido de la migración.
* **Si ya administra otros productos de Adobe en su Adobe Admin Console**, es posible que Adobe solicite su consentimiento para migrar automáticamente los usuarios a su consola existente. Haga clic en el botón **Empezar** del correo electrónico para ir a la página de consentimiento.
* **Si ha eliminado anteriormente el tipo de licencia de solicitante**, se añadirá a su sistema. No se asignará ningún usuario a este tipo de licencia, pero es necesaria para la sincronización entre Workfront y Adobe Admin Console. No es necesario que realice ninguna acción en relación con el tipo de licencia del solicitante.

No hay cambios en la administración de usuarios en este momento. Los administradores de Workfront seguirán administrando usuarios en Workfront y los usuarios seguirán iniciando sesión con su ID de Workfront o SSO hasta que se complete la migración de usuarios.

### Programación de la migración de usuarios

Una vez que el administrador del sistema complete los requisitos previos descritos en la sección anterior, Adobe programará automáticamente la migración de usuarios durante 30 días después de que se completen estos requisitos previos y se comunicará con los administradores del perfiles de producto de Workfront (administradores del sistema de Workfront) para administrar la migración de usuarios.

Los administradores de perfiles de producto de Workfront (administradores de sistema de Workfront):

* Reciben un correo electrónico con la fecha de inicio de la migración de usuarios programada (unos 30 días después de que se cumplan estos requisitos previos)
* Obtienen acceso a la consola de administrador de Workfront designada, en donde tienen la opción de cambiar la fecha de la migración

  >[!NOTE]
  >
  >Debido a la complejidad de la migración, los cambios de fecha están restringidos a no más de 30 días después de la fecha programada. Póngase en contacto con el servicio de soporte si necesita una fecha posterior.

* Reciben un correo electrónico recordatorio un día antes de la fecha de inicio de la migración de usuarios

### Preparar usuarios para el día de la migración

Como administrador de perfiles de producto de Workfront (administrador del sistema de Workfront), son responsables de garantizar que todos los usuarios estén preparados para el día de la migración.

* Preparan a todos los usuarios para la próxima migración a Adobe Identity notificándoles lo siguiente:

   * A medida que los usuarios migren, recibirán un correo electrónico de Adobe de notificándoles el cambio en la forma en que inician sesión en Workfront. Se invitará a los usuarios a aceptar una invitación para iniciar sesión con Adobe Identity por primera vez, ya sea iniciando sesión con un Adobe ID existente o configurando uno nuevo con la misma dirección de correo electrónico.

### Qué esperar el día de la migración

* **La migración de usuarios comenzará a la medianoche del centro de datos de Workfront que aloja al cliente.**

* **Adobe migrará automáticamente primero a los administradores de Workfront.** Cuando los administradores de Workfront se migren a Adobe Identity, se les asignará la función de administrador de perfiles de producto de Adobe (administrador del sistema de Workfront). Las funciones existentes antes de la migración no se verán afectadas.

  >[!NOTE]
  >
  >El acceso al producto se mantendrá durante la migración de usuarios. Si la sesión está iniciada durante la migración de usuario, no habrá ningún impacto. Sin embargo, la próxima vez que el usuario inicie sesión, se le pedirá que utilice su identidad de Adobe.



* **Una vez realizada la migración, el usuario recibirá un correo electrónico de Adobe notificándole el cambio en la forma de inicio de sesión en Workfront.** Los usuarios recibirán una invitación para iniciar sesión con la identidad de Adobe por primera vez, ya sea con una Adobe ID existente o configurando una nueva con la misma dirección de correo electrónico.

  Para obtener más información sobre cómo iniciar sesión en Workfront con una Adobe ID, consulte [Iniciar sesión en Adobe Experience Cloud](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### Migración de usuarios completada

Una vez migrados todos los administradores y usuarios, Adobe notificará por correo electrónico a los administradores del sistema y del perfil de producto (administradores del sistema de Workfront). Entonces, todos los usuarios de Workfront para esa instancia iniciarán sesión en Workfront con la identidad de Adobe. Los administradores del sistema de Workfront y del perfil de producto (administradores del sistema de Workfront) pueden gestionar el acceso de los usuarios en Adobe Admin Console. Si los clientes no utilizan una forma de sincronización de directorios en la consola de administración, pueden seguir gestionando el acceso a Workfront en la aplicación de Workfront.

## Soporte

Para cualquier pregunta o inquietud, siga los pasos descritos en el artículo [Póngase en contacto con el servicio de Atención al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).




