---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Cómo compartir objetos sin generar notificaciones
description: Descubra cómo puede compartir objetos y evitar que se envíen notificaciones sobre este cambio. Esto resulta especialmente útil cuando se comparten objetos de forma masiva.
author: Alina
feature: Get Started with Workfront
source-git-commit: b14dd633edec3e9746f7f1412445b74bcd37a676
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 22%

---


# Cómo compartir objetos sin generar notificaciones

<!--Audited: 12/2024-->

Cuando comparte un objeto en Adobe Workfront, las personas con las que comparte el objeto reciben una notificación por correo electrónico sobre el uso compartido.

Es importante que tenga en cuenta este cambio cuando reciba una notificación por correo electrónico cuando alguien comparta un objeto con usted. Sin embargo, demasiadas notificaciones pueden resultar demasiado confusas para los usuarios. Si desea compartir un gran número de objetos con los usuarios al mismo tiempo, desactivar temporalmente las notificaciones ayudará a evitar la confusión.

Las personas reciben notificaciones por correo electrónico cuando se habilita la siguiente configuración al mismo tiempo:

* Una o ambas de las siguientes Notificaciones de eventos están habilitadas en el sistema o en el nivel de grupo:

   * Objeto compartido con usuario
   * Objeto compartido con equipo está habilitado en el sistema o en el nivel de grupo.
* Una o ambas de las siguientes notificaciones por correo electrónico están habilitadas en el perfil del usuario:

   * Alguien comparte un objeto conmigo
   * Alguien comparte un objeto con mi equipo

Si necesita compartir varios objetos con varias personas (de forma masiva), pero no desea que reciban notificaciones por correo electrónico sobre este cambio, haga lo siguiente:

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Se necesita tener lo siguiente para compartir objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nueva licencia: estándar</p> 
   O
   <p>Licencia actual: plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior sobre los objetos que desea compartir</p>
   <p>Editar el acceso de los usuarios</p>
   <p><b>NOTA</b></p>
   <p> Debe ser administrador de sistemas o de grupos para comprobar el estado de las notificaciones de eventos del sistema o del grupo</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización o superiores sobre los objetos que desea compartir</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Compartir objetos sin generar notificaciones

1. Asegúrese de que las siguientes **Notificaciones de eventos** estén habilitadas en el nivel de sistema o grupo:

   * **Objeto compartido con el usuario**
   * **El uso compartido de objetos en el equipo está habilitado en el nivel de sistema o grupo**.

   Para obtener más información, consulte [Configurar notificaciones de los eventos para todos los usuarios del sistema](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Si estas notificaciones de eventos no están habilitadas, las notificaciones sobre cómo compartir un objeto no se enviarán a los usuarios. Si una o ambas están habilitadas, continúe con los siguientes pasos.

{{step-1-to-users}}

1. Seleccione varios usuarios en la lista y luego haga clic en **Notificaciones** > **Varios**.
1. Deshabilite una o ambas de las siguientes notificaciones (en función de las que estén habilitadas desde el nivel de sistema o grupo):

   * **Alguien comparte un objeto conmigo**
   * **Alguien comparte un objeto con mi equipo**

   Asegúrese de que todos los usuarios seleccionados tengan estas notificaciones seleccionadas antes de desactivarlas. De este modo, puede volver a activarlos de forma masiva para todos ellos después de compartir los objetos.

1. Haga clic en **Guardar cambios**.
1. Vaya a una lista de los objetos que desea compartir y selecciónelos. Luego, haga clic en el icono **Compartir** que se encuentra en la parte superior de la lista.

   Para obtener información sobre cómo compartir objetos de forma masiva, vea [Compartir un objeto](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

1. Vuelva a la lista de usuarios para los que desactivó las notificaciones y seleccione los mismos usuarios.
1. Seleccione los mismos usuarios en la lista y luego haga clic en **Notificaciones** > **Varios**.
1. Habilite una o ambas de las siguientes notificaciones (en función de las que estén habilitadas desde el nivel de sistema o grupo):

   * **Alguien comparte un objeto conmigo**
   * **Alguien comparte un objeto con mi equipo**

1. Haga clic en **Guardar cambios**.

   Los objetos se compartieron con los usuarios seleccionados y ninguno de ellos recibió notificaciones por correo electrónico sobre este cambio.






