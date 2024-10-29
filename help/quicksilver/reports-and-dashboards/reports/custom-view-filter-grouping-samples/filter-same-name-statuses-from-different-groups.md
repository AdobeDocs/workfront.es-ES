---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtrar: mostrar elementos por estados del mismo nombre cuando los estados están asociados a grupos diferentes"
description: Puede tener un estado de tarea asignado al grupo A denominado Nuevo estado con la clave de 3 letras NST. Es posible que tenga otro estado de tarea asignado al Grupo B, también denominado Nuevo estado con la clave de 3 letras NES. Aunque los nombres de los dos estados pueden ser idénticos, el código de 3 letras siempre es único. Para obtener más información sobre los estados de grupo, consulte Crear o editar un estado de grupo.
author: Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Filtrar: muestra los elementos por estados del mismo nombre cuando los estados están asociados con grupos diferentes

<!--Audited: 10/2024-->

Puede asignarse un estado de tarea al grupo A denominado *Nuevo estado* con la clave de 3 letras *NST*. Es posible que tenga otro estado de tarea asignado al Grupo B también denominado *Nuevo estado* con la clave de 3 letras *NES.* Aunque los nombres de los dos estados pueden ser idénticos, el código de 3 letras siempre es único.

Para obtener más información acerca de los estados de grupo, vea [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Con el generador de filtros, no se puede identificar entre los 2 estados que tienen el mismo nombre. Debe utilizar el modo Texto en un filtro personalizado para distinguir entre los 2 estados.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
    <p>Nuevo:</p>
   <ul><li><p>Colaborador para modificar un filtro </p></li>
   <li><p>Estándar para modificar un informe</p></li> </ul>

<p>Actual:</p>
   <ul><li><p>Solicitud para modificar un filtro </p></li>
   <li><p>Plan para modificar un informe</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mostrar elementos por estados del mismo nombre cuando los estados están asociados con grupos diferentes

1. Vaya al menú desplegable **Filtro** para el filtro que desea personalizar para una lista de tareas, por ejemplo.\
   Esto también funciona para proyectos y problemas.
1. Haga clic en **Nuevo filtro**.
1. En la primera lista desplegable de la esquina superior izquierda, seleccione Tarea > Estado.
1. Seleccione **Es igual a** para el modificador y, a continuación, seleccione uno de los estados sobre el que desee generar el informe.

   Por ejemplo, en un informe de tareas, agregue **Estado es igual a nuevo estado**, si desea mostrar solamente las tareas que están en un estado de **Nuevo estado**.

   >[!TIP]
   >
   >Tenga en cuenta que solo tiene una opción para un estado denominado Nuevo estado.

1. Haga clic en **Modo de texto**.\
   El siguiente código debe mostrarse en el espacio proporcionado:

   <pre>OR:1:status=NST<br>OR:1:status_Mod=in </pre>

   >[!NOTE]
   >
   >Aquí solo se muestra un estado. La línea de estado muestra una de las claves de 3 letras para uno de los estados.

1. Agregue las dos líneas de código siguientes para añadir el estado que falta en el filtro:

   <pre>OR:2:status=NES<br>OR:2:status_Mod=in</pre>

1. Haga clic en **Aplicar** y luego en **Guardar como nuevo**.

   La lista muestra ambas tareas con el estado &quot;Nuevo estado&quot; del Grupo A y con el estado &quot;Nuevo estado&quot; del Grupo B.
