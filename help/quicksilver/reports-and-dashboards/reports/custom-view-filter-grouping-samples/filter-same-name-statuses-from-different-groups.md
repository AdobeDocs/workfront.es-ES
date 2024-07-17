---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: mostrar elementos por estados del mismo nombre cuando los estados están asociados con grupos diferentes"
description: Puede tener un estado de tarea asignado al grupo A denominado Nuevo estado con la clave de 3 letras NST. Es posible que tenga otro estado de tarea asignado al Grupo B, también denominado Nuevo estado con la clave de 3 letras NES. Aunque los nombres de los dos estados pueden ser idénticos, el código de 3 letras siempre es único. Para obtener más información sobre los estados de grupo, consulte Crear o editar un estado de grupo.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Filtrar: muestra los elementos por estados del mismo nombre cuando los estados están asociados con grupos diferentes

Puede asignarse un estado de tarea al grupo A denominado *Nuevo estado* con la clave de 3 letras *NST*. Es posible que tenga otro estado de tarea asignado al Grupo B también denominado *Nuevo estado* con la clave de 3 letras *NES.* Aunque los nombres de los dos estados pueden ser idénticos, el código de 3 letras siempre es único.\
Para obtener más información acerca de los estados de grupo, vea [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Con el generador de filtros, no se puede identificar entre los 2 estados que tienen el mismo nombre. Debe utilizar el modo Texto para distinguir entre los 2 estados.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud para modificar un filtro </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar un filtro</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Mostrar elementos por estados del mismo nombre cuando los estados están asociados con grupos diferentes

1. Vaya al filtro que desee personalizar para ver una lista de tareas, por ejemplo.\
   Esto también funciona para proyectos y problemas.
1. Haga clic en **Agregar una regla de filtro** para el campo **Estado** del objeto de su lista.\
   Por ejemplo, en un informe de tareas, agregue **Estado igual a nuevo estado**, si desea mostrar solamente las tareas que tengan el estado **Nuevo estado**.

   >[!TIP]
   >
   >Tenga en cuenta que solo tiene una opción para un estado denominado Nuevo estado.

1. Haga clic en **Cambiar al modo de texto**.\
   Se debe mostrar el siguiente código:
   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >Aquí solo se muestra un estado. La línea de estado muestra una de las claves de 3 letras para uno de los estados.

1. Agregue las dos líneas de código siguientes para añadir el estado que falta en el filtro:
   <pre>OR:1:status=NES<br>OR:1:status_Mod=in</pre>

1. Haga clic en **Listo** y luego en **Guardar filtro**.

   La lista muestra ambas tareas con el estado &quot;Nuevo estado&quot; del Grupo A y con el estado &quot;Nuevo estado&quot; del Grupo B.
