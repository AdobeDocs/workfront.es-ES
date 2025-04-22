---
title: Compartir un portafolio
description: Puede compartir un portafolio con otros usuarios si tiene permisos para acceder a él.
author: Courtney
draft: Probably
feature: Get Started with Workfront
exl-id: 79643202-2d91-4028-b673-c3443b50d898
source-git-commit: fcf6165c9c641316c701d92af2e39294a9fe0123
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 47%

---

# Compartir un portafolio

El administrador de Adobe Workfront puede concederle acceso para ver o editar portafolios cuando le asigna su nivel de acceso. Debe tener una licencia de Plan para poder acceder y editar un portafolio. Para obtener más información, consulte [Conceder acceso a portafolios](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md).

Junto con el nivel de acceso que se le ha concedido, también puede recibir permisos para ver o administrar portafolios específicos de usuarios que pueden compartirlos con usted. Para obtener más información sobre los niveles de acceso y los permisos, consulte [Cómo funcionan juntos los niveles de acceso y los permisos](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Los permisos son específicos de un elemento en Workfront y definen qué acciones pueden realizar los usuarios sobre ese elemento.


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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: estándar</p> 
   O
   <p>Actual: Trabajo o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior sobre los objetos que desea compartir</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización o superiores sobre los objetos que desea compartir</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre el uso compartido de portafolios

Además de las consideraciones siguientes, consulte [Información general sobre los permisos de uso compartido en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Un administrador de Workfront puede añadir o quitar permisos a cualquier elemento del sistema, para todos los usuarios, sin que tengan que ser el propietario de esos elementos.

* El creador de un portafolio tiene permisos de administración de forma predeterminada.
* Puede compartir un portafolio individualmente o puede compartir varios portafolios al mismo tiempo. El uso compartido de un portafolio es idéntico al uso compartido de otros objetos en Workfront. Para obtener más información, consulte [Compartir un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Solo puede conceder permisos para Ver o Administrar los portafolios.
</span>
* Cuando comparte un portafolio, los usuarios heredan los mismos permisos en todos los objetos secundarios asociados con el portafolio de forma predeterminada.

Para obtener más información sobre la jerarquía de objetos en Workfront, consulte [Comprender los objetos en Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Puede quitar los permisos heredados del portafolio. Para obtener más información sobre cómo quitar permisos de los objetos, consulte [Quitar permisos de los objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Compartir un portafolio

{{step1-to-portfolios}}

1. En la página **Portafolios**, seleccione el portafolio que desee compartir. Se abre la página del portafolio.

1. A la derecha del nombre del portafolio, haga clic en **Compartir**. Se abre el cuadro de diálogo **Compartir [Portfolio Name]**.

   ![Botón Compartir portafolio](assets/share-portfolio-button.png)

1. En el campo **Conceder acceso al portafolio a**, empiece a escribir el nombre del usuario, equipo, rol, grupo o compañía con el que desea compartir el portafolio y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   >[!TIP]
   >
   >Solo puede compartir un portafolio con usuarios, equipos, funciones o empresas activos.


1. (Opcional) Seleccione la lista desplegable **Quién tiene acceso** y seleccione el nivel de acceso del portafolio:

   * **Solo las personas invitadas pueden acceder a:** Solo los usuarios invitados al portafolio pueden acceder a él (Predeterminado).
   * **Todos los usuarios del sistema pueden ver**: todos los usuarios del sistema pueden ver el portafolio sin invitación.

1. Haga clic en la lista desplegable a la derecha del nombre del usuario y seleccione su nivel de permisos para este portafolio:

   * **Ver**: el usuario puede revisar y compartir el portafolio.
   * **Administrar**: el usuario tiene acceso completo al portafolio sin derechos administrativos, que se conceden en el nivel de acceso (también incluye todos los permisos de Vista).

1. (Opcional) Haga clic en el icono de opciones avanzadas junto al nivel de permisos que ha concedido para configurar permisos específicos en el portafolio.

   ![Opciones de permiso avanzadas configuradas](assets/advanced-options-icon.png)

1. (Opcional) Para compartir rápidamente el portafolio mediante un vínculo, haga clic en **Copiar vínculo** y reenvíelo al destinatario.

1. Haga clic en **Guardar**.

## Compartir portafolios de forma masiva

{{step1-to-portfolios}}

1. En la página **Portafolios**, seleccione el cuadro de la izquierda de cada portafolio que desee compartir y, a continuación, haga clic en el icono **Compartir** ![Compartir icono](assets/share-icon.png) en la parte superior de la página. Se abre el modal de uso compartido.

   ![Portafolios de uso compartido en lotes](assets/bulk-share-portfolios.png)

1. En el campo **Conceder acceso al portafolio a**, empiece a escribir el nombre del usuario, equipo, rol, grupo o compañía con el que desea compartir los portafolios y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   >[!TIP]
   >
   >Solo puede compartir portafolios con usuarios, equipos, funciones o empresas activos.


1. (Opcional) Seleccione la lista desplegable **Quién tiene acceso** y el nivel de acceso de los portafolios:

   * **Solo las personas invitadas pueden acceder a:** Solo los usuarios invitados a los portafolios pueden acceder a ellos (predeterminado).
   * **Todos los usuarios del sistema pueden ver**: todos los usuarios del sistema pueden ver los portafolios sin invitación.


1. Haga clic en la lista desplegable a la derecha del nombre del usuario y seleccione su nivel de permisos para los portafolios:

   * **Ver**: el usuario puede revisar y compartir los portafolios.
   * **Administrar**: el usuario tiene acceso completo a los portafolios sin derechos administrativos, que se conceden en el nivel de acceso (también incluye todos los permisos de Vista).

1. (Opcional) Haga clic en el icono de opciones avanzadas junto al nivel de permisos que ha concedido para configurar permisos específicos en los portafolios.

   ![Opciones de permiso avanzadas configuradas](assets/advanced-options-icon.png)

1. Haga clic en **Guardar**.


## Permisos de portafolio

La siguiente tabla muestra qué permisos puede conceder a los usuarios cuando les permite ver o administrar un portafolio:

| **Acciones** | **Administrar** | **Vista** |
|---|---|---|
| Editar detalles del portafolio | ✓ |   |
| Ver un portafolio | ✓ | ✓ |
| Eliminar un calendario | ✓ |   |
| Adjuntar un formulario personalizado | ✓ |   |
| Editar un formulario personalizado | ✓ |   |
| Añadir o quitar un programa&#42; | ✓ |   |
| Añadir o quitar un proyecto&#42; | ✓ |   |
| Aprobar un proyecto | ✓ |   |
| Optimización del portafolio&#42; | ✓ |   |
| Añadir una carpeta de documentos&#42; | ✓ | ✓ |
| Añadir un documento | ✓ | ✓ |
| Actualizaciones/comentarios | ✓ | ✓ |
| Compartir | ✓ | ✓ |
| Compartir en todo el sistema |   | ✓ |

*Estos permisos están controlados por el nivel de acceso y los permisos de otros objetos, como proyectos, programas o documentos.
