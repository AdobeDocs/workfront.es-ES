---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Compartir un tablero
description: El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar paneles cuando asignan niveles de acceso. Junto con el nivel de acceso que se concede a los usuarios, también puede concederles permisos para Ver o Administrar paneles específicos que tiene acceso para compartir.
author: Nolan
feature: Reports and Dashboards
exl-id: 21bd531f-8732-4d6c-b91f-990887285447
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Compartir un tablero

El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar paneles cuando asignan niveles de acceso. Para obtener más información sobre la concesión de acceso a los problemas, consulte [Conceder acceso a informes, paneles y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Junto con el nivel de acceso que se concede a los usuarios, también puede concederles permisos para Ver o Administrar paneles específicos que tiene acceso para compartir. Para obtener más información sobre los niveles de acceso y los permisos, vea [Cómo funcionan juntos los niveles de acceso y los permisos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Los permisos son específicos de un elemento en Workfront y definen qué acciones se pueden realizar sobre ese elemento.

>[!NOTE]
>
>Un administrador de Workfront puede agregar o quitar permisos a cualquier elemento del sistema, para todos los usuarios, sin ser el propietario de esos elementos.

## Requisitos de acceso

Debe tener lo siguiente para compartir objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Ver el acceso o superior a Informes, Paneles, Calendarios</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver permisos o superior en el tablero</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe crearse el tablero para poder compartirlo.

Para obtener información sobre cómo crear paneles, consulte [Crear un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Consideraciones sobre el uso compartido de paneles

Además de las consideraciones siguientes, vea [Compartir informes, tableros y calendarios](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* El creador de un tablero tiene permisos de administración de forma predeterminada.

* Puede compartir los paneles que cree con otras personas, equipos, grupos, funciones del puesto o empresas. También puede compartir tableros que otros hayan creado y que se hayan compartido con usted.
* También puede compartirlos con toda la organización haciéndolos visibles en todo el sistema.
* Puede compartir un tablero individual o puede compartir varios tableros de una lista.
* Al compartir un tablero, los usuarios heredan los permisos de Vista en todos los objetos de informes del tablero de forma predeterminada.

  Para obtener más información acerca de la jerarquía de objetos en Workfront, vea [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Para obtener información acerca de cómo ver los permisos heredados, vea [Ver permisos heredados en objetos](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Compartir un tablero

Compartir uno o varios tableros de una lista es idéntico.

1. Vaya a una lista de paneles y seleccione uno o varios, luego haga clic en **Compartir** ![](assets/share-icon.png).

   O

   Haga clic en el nombre de un tablero y, a continuación, haga clic en **Acciones de tablero >****Compartir**.

   ![](assets/qs-dashboard-actions-menu-350x318.png)

1. En el campo **Agregar personas, equipos, roles, grupos o empresas ...**, empiece a escribir el nombre del usuario, equipo, rol, grupo o compañía con el que desea compartir el panel y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. (Opcional) Para que todos los usuarios del sistema tengan acceso al tablero, haga clic en el icono **Configuración** en la esquina superior derecha del cuadro de diálogo de uso compartido y, a continuación, seleccione **Hacer esto visible en todo el sistema**.

1. Haga clic en **Guardar**.
