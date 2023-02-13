---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Compartir un tablero
description: El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar tableros cuando asignen niveles de acceso. Junto con el nivel de acceso que se concede a los usuarios, también puede concederles permisos para ver o administrar tableros específicos a los que tenga acceso para compartir.
author: Nolan
feature: Reports and Dashboards
exl-id: 21bd531f-8732-4d6c-b91f-990887285447
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Compartir un tablero

El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar tableros cuando asignen niveles de acceso. Para obtener más información sobre la concesión de acceso a problemas, consulte [Conceder acceso a informes, tableros y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Junto con el nivel de acceso que se concede a los usuarios, también puede concederles permisos para ver o administrar tableros específicos a los que tenga acceso para compartir. Para obtener más información sobre los niveles de acceso y los permisos, consulte [Cómo funcionan juntos los niveles de acceso y los permisos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Los permisos son específicos para un elemento de Workfront y definen qué acciones se pueden realizar en ese elemento.

>[!NOTE]
>
>Un administrador de Workfront puede agregar o quitar permisos para cualquier elemento del sistema, para todos los usuarios, sin ser el propietario de esos elementos.

## Requisitos de acceso

Debe tener lo siguiente para compartir objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Ver acceso o superior a informes, tableros y calendarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver permisos o superiores en el tablero</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

El tablero debe crearse para poder compartirlo.

Para obtener información sobre la creación de tableros, consulte [Crear un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Consideraciones sobre cómo compartir tableros

Además de las consideraciones siguientes, consulte [Compartir informes, tableros y calendarios](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* De forma predeterminada, el creador de un tablero tiene permisos de administración.

* Puede compartir los tableros que cree con otras personas, equipos, grupos, funciones de trabajo o empresas. También puede compartir los tableros que otros crearon y que se compartieron con usted.
* También puede compartirlas con toda la organización haciéndola visible en todo el sistema.
* Puede compartir un tablero individual o varios tableros de una lista.
* De forma predeterminada, cuando comparte un tablero, los usuarios heredan los permisos de visualización de todos los objetos de informes del tablero.

   Para obtener más información sobre la jerarquía de objetos en Workfront, consulte [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   Para obtener información sobre la visualización de permisos heredados, consulte [Ver permisos heredados en objetos](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Compartir un tablero

Compartir uno o varios tableros de una lista es idéntico.

1. Vaya a una lista de tableros, seleccione uno o varios tableros y haga clic en **Compartir** ![](assets/share-icon.png).

   O

   Haga clic en el nombre de un tablero y, a continuación, haga clic en **Acciones del tablero >****Uso compartido**.

   ![](assets/qs-dashboard-actions-menu-350x318.png)

1. En el **Agregar personas, equipos, funciones, grupos o empresas...** , empiece a escribir el nombre del usuario, equipo, función, grupo o empresa con el que desee compartir el tablero y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.
1. (Opcional) Para que el tablero sea accesible para todos los usuarios del sistema, haga clic en el **Configuración** en la esquina superior derecha del cuadro de diálogo de uso compartido y, a continuación, seleccione **Hacer que esto sea visible en todo el sistema**.

1. Haga clic en **Guardar**.
