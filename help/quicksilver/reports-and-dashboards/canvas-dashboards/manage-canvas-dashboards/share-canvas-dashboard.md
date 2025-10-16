---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: Compartir un panel de lienzo
description: Puede compartir un panel de lienzo con otros usuarios de Adobe Workfront para que puedan verlo o editarlo.
author: Jenny
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
source-git-commit: 1059950dd3b20e0959c626e580f958bed5076541
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 10%

---

# Compartir un panel de lienzo

>[!IMPORTANT]
>
>Actualmente, la función Paneles de lienzo solo está disponible para los usuarios que participan en la fase beta. Es posible que algunas partes de la función no estén completas o que no funcionen según lo previsto durante esta fase. Envíe cualquier comentario sobre su experiencia siguiendo las instrucciones de la sección [Proporcionar comentarios](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) del artículo Información general sobre la versión beta de los paneles de lienzo.<br>
>&#x200B;>Si tiene comentarios acerca de un posible error o problema técnico, envíe un ticket al equipo de asistencia de Workfront. Para obtener más información, consulte [Póngase en contacto con Atención al cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>&#x200B;>Tenga en cuenta que esta versión beta no está disponible en los siguientes proveedores de la nube:
>
>* Traer su propia clave para Amazon Web Service
>* Azure
>* Google Cloud Platform

Puede compartir un panel de lienzo con otros usuarios de Adobe Workfront para que puedan verlo o editarlo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquiera </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td> 
<p>Estándar </p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td> 
   <td><p>Acceso de visualización a informes, paneles de control y calendarios</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td><p>Ver permisos del tablero para compartir el tablero</p>
   <p>Administre permisos para el tablero para asignar permisos de tablero</p>
  </td> 
  </tr>
</tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Consideraciones sobre el uso compartido de paneles

* Los paneles se pueden compartir con el usuario, el equipo, el grupo, la función del puesto o los recursos de la empresa.

* De forma predeterminada, el creador de un tablero tiene permisos de administración para el tablero.

* Los administradores del sistema y los usuarios con el permiso Administrar pueden conceder el acceso Ver o Administrar a un tablero.

* Los usuarios con permiso de visualización en un panel pueden conceder acceso de visualización a un panel.

* Al compartir un tablero, los recursos con los que se comparte heredarán los permisos de los informes que se muestran en el tablero.

* Cuando se distribuye un tablero mediante una plantilla de diseño, se concede un permiso de vista automático para el tablero (y sus informes) a todos los recursos asignados a la plantilla de diseño.


## Compartir un panel de lienzo


{{step1-to-dashboards}}

1. En el panel izquierdo, haga clic en **Paneles de control de lienzo**.

1. En la página **Paneles de lienzo**, seleccione el panel que desee compartir.

1. En la esquina superior derecha de la página, haga clic en el botón **Compartir**. Aparece el cuadro de diálogo **Uso compartido de paneles**.

1. En el campo **Dar acceso a**, empiece a escribir el nombre de un usuario, equipo, rol, grupo o compañía específico con el que desee compartir el panel de lienzo y, a continuación, selecciónelo cuando aparezca en la lista desplegable.

1. (Opcional) Para editar el acceso de un recurso al panel, haga clic en **Ver** junto a su nombre y, a continuación, seleccione **Administrar** en la lista desplegable que aparece.

   >[!NOTE]
   >
   > Cuando los usuarios no tienen los permisos de edición en un panel asignado a través de su nivel de acceso, no se les pueden asignar permisos de administración en un panel.

1. Repita los pasos del 5 al 6 con cada recurso con el que desee compartir el tablero.

1. Haga clic en el botón **Compartir**. Los destinatarios reciben una notificación por correo electrónico que les informa de que el tablero se ha compartido con ellos y a la que ahora pueden acceder en **Paneles** > **Paneles de lienzo** > **Paneles compartidos**.

   >[!NOTE]
   >
   > Pueden aplicarse preferencias de usuario individuales y exclusiones del sistema para las notificaciones por correo electrónico. <br>
   > Las notificaciones solo se envían cuando se comparten directamente con un usuario. El uso compartido en grupos, roles, compañías y equipos no genera notificaciones por correo electrónico.<br>
   > Los permisos heredados de una plantilla de diseño no generan una notificación por correo electrónico sobre el acceso al panel.
