---
title: Agregar una aprobación a un formulario de solicitud en Adobe Workfront Planning
description: Puede agregar un proceso de aprobación a un formulario de solicitud de Adobe Workfront Planning para iniciar una aprobación para cada solicitud enviada antes de crear un registro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 18%

---

# Agregar una aprobación a un formulario de solicitud en Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Puede agregar un proceso de aprobación a un formulario de solicitud de Adobe Workfront Planning para iniciar una aprobación para cada solicitud enviada antes de crear un registro.

Este artículo describe cómo un administrador del espacio de trabajo puede agregar una aprobación a un formulario de solicitud asociado a un tipo de registro.

Para obtener información acerca de cómo crear un formulario de solicitud en Workfront Planning, vea [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Para obtener información sobre cómo enviar una solicitud a un tipo de registro para crear un registro, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Productos</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Planificación de Adobe Workfront<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td>
   <td>
<p>Cualquiera de los siguientes planes de Workfront:</p>
<ul><li>Seleccionar</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning no está disponible para planes Workfront heredados</p>
   </td>

<tr>
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td>
   <td>
<p>Cualquiera </p>  
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </td>

<tr>
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td>
   <td>
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a todas las funcionalidades de Workfront Planning.</p>
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Estándar</p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos de objeto</p></td>
   <td>
   <ul>
   <li><p>Administración de permisos en un espacio de trabajo <!--<span class="preview">and record type</span>--></p></li>
    <li><p>Los administradores del sistema pueden administrar los espacios de trabajo que no hayan creado. </p></li>
    </ul>
   <p>Para obtener información acerca de los permisos de uso compartido para objetos de Workfront Planning, consulte 
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Información general sobre los permisos de uso compartido en Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p>  
</td>
  </tr>
 </tbody>
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre la adición de aprobaciones a un formulario de solicitud

* Puede agregar uno o varios aprobadores a un formulario de solicitud. Solo puede agregar usuarios como aprobadores.
* Cuando se agregan varios aprobadores a un formulario de solicitud, todos los aprobadores deben aceptar la solicitud antes de crear un registro en Workfront Planning.
* Si todos los aprobadores aprueban la solicitud, se crea un registro para el tipo de registro asociado al formulario de solicitud.
* Si al menos un aprobador rechaza la solicitud y todos los demás la aprueban, se crea una solicitud para el área de Solicitudes en Workfront, pero no se crea ningún registro para el tipo de registro asociado al formulario de solicitud.
* Añadir aprobaciones a un formulario de solicitud es opcional. Workfront Planning crea inmediatamente un registro cuando se envía una solicitud, si el formulario de solicitud no está asociado a una aprobación.

## Añadir una aprobación a un formulario de solicitud

1. Comience a crear un formulario de solicitud para un tipo de registro, como se describe en [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Haga clic en **Configuración**.

   Se muestra el área **Configuración**.

   ![Ficha de configuración](assets/configuration-tab.png)
1. En el campo **Aprobadores**, haga clic en el icono desplegable y seleccione uno o varios nombres en la lista

   O

   Empiece a escribir el nombre de un aprobador y selecciónelo cuando aparezca en la lista.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* Puede agregar uno o varios aprobadores a un formulario de solicitud.
   >
   >* Si agrega más de un aprobador, todos los aprobadores deben aprobar la solicitud antes de que Workfront Planning cree un registro.
   >
   >* Si al menos un aprobador rechaza la solicitud, esta se rechaza y no se crea el registro. La solicitud permanece en la pestaña Planificación de la sección Enviados del área Solicitudes de Workfront.
   >
   >* Todos los aprobadores deben tomar una decisión antes de aprobar o rechazar una solicitud.


1. (Opcional) Haga clic en **Publicar** si nunca antes había compartido el formulario de solicitud

   O

   Haga clic en **Compartir** para compartir el formulario y luego en **Copiar vínculo**.
1. (Opcional) Una vez que un usuario utiliza el vínculo que comparte y envía una solicitud, Workfront Planning envía una notificación de aprobación en la aplicación y un correo electrónico a los aprobadores.

   >[!NOTE]
   >
   >   La instancia de Workfront de su organización debe incorporarse a la experiencia unificada de Adobe para que los usuarios puedan recibir notificaciones por correo electrónico y en la aplicación.


   Para obtener información acerca de cómo aprobar solicitudes, vea [Aprobar una solicitud](/help/quicksilver/planning/requests/approve-request.md).
