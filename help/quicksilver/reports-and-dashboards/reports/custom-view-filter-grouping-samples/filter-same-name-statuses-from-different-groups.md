---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filtro: mostrar elementos por estados del mismo nombre cuando los estados están asociados a grupos diferentes'
description: Puede tener asignado un estado de tarea al grupo A denominado Nuevo estado con la clave de 3 letras NST. Es posible que tenga asignado otro estado de tarea al Grupo B que también se denomina Nuevo estado con la clave de 3 letras NES. Aunque los nombres de los 2 estados pueden ser idénticos, el código de 3 letras siempre es único. Para obtener más información sobre los estados de grupo, consulte Crear o editar un estado de grupo.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Filtro: mostrar elementos por estados del mismo nombre cuando los estados están asociados a diferentes grupos

Puede tener un estado de tarea asignado al Grupo A con el nombre *Nuevo estado* con la clave de 3 letras *NST*. Es posible que tenga asignado otro estado de tarea al grupo B también denominado *Nuevo estado* con la clave de 3 letras *NES.* Aunque los nombres de los 2 estados pueden ser idénticos, el código de 3 letras siempre es único.\
Para obtener más información sobre los estados de grupo, consulte [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Con el generador de filtros, no se puede identificar entre los 2 estados que tienen el mismo nombre. Debe utilizar el modo Texto para distinguir entre los dos estados.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Mostrar elementos por estados del mismo nombre cuando los estados están asociados a diferentes grupos

1. Vaya al filtro que desea personalizar para una lista de tareas, por ejemplo.\
   Esto funciona igual para proyectos y problemas también.
1. Haga clic en **Agregar una regla de filtro** para el **Estado** del objeto de la lista.\
   Por ejemplo, en un informe de tareas, agregue **Estado igual a nuevo estado**, si desea mostrar solo las tareas que están en estado de **Nuevo estado**.

   >[!TIP]
   >
   >Tenga en cuenta que solo tiene una opción para un estado denominado Nuevo estado.

1. Haga clic en **Cambiar al modo de texto**.\
   Se debe mostrar el siguiente código:

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >Aquí solo se muestra un estado. La línea de estado muestra una de las claves de 3 letras de uno de los estados.

1. Agregue las dos líneas de código siguientes para agregar el estado que falta en el filtro:

   <pre>O:1:status=NES<br>O:1:status_Mod=in</pre>

1. Haga clic en **Listo**, luego **Guardar filtro**.

   La lista muestra ambas tareas con el estado &quot;Nuevo estado&quot; del Grupo A y el estado &quot;Nuevo estado&quot; del Grupo B.
