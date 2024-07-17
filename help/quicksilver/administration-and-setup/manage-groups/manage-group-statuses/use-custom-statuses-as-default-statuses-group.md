---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Usar un estado personalizado como estado predeterminado para un grupo
description: Como administrador de grupo, puede configurar un estado personalizado como estado predeterminado para un grupo o subgrupo que administre. Esto resulta útil cuando el sistema necesita asignar automáticamente un estado de Workfront a un proyecto, tarea o problema. Un proyecto, tarea o problema siempre muestra el estado personalizado que ha establecido como estado predeterminado en lugar de mostrar el estado de Workfront al que equivale.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---

# Usar un estado personalizado como estado predeterminado para un grupo

Como administrador de grupo, puede configurar un estado personalizado como estado predeterminado para un grupo o subgrupo que administre. Esto resulta útil cuando el sistema necesita asignar automáticamente un estado de Workfront a un proyecto, tarea o problema. Un proyecto, tarea o problema siempre muestra el estado personalizado que ha establecido como estado predeterminado en lugar de mostrar el estado de Workfront al que equivale.

El estado que configure puede ser cualquier estado personalizado creado para el grupo, heredado de un grupo por encima del grupo o heredado del nivel del sistema.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!INFO]
>
>**Ejemplo:** Puede crear un estado personalizado llamado Finalizado y establecerlo como un estado predeterminado equiparado con el estado de Workfront Finalizado.
>
>A continuación, para las tareas configuradas para cambiar al estado Completado cuando alcanzan el 100%, el estado se muestra como Finalizado en lugar de Completado.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

## Estados de problemas

Si el estado personalizado es un estado de problema, deben habilitarse los cuatro tipos de problemas (informe de errores, orden de cambio, problema y solicitud). Por ejemplo, en el estado de problema que se muestra a continuación, el estado Reabierto no se puede utilizar como estado por defecto porque el tipo de problema Orden de cambio no está seleccionado:

![](assets/all-4-issue-types-enabled.png)

## Definir un estado personalizado como estado predeterminado para un grupo

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).
1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png) y, a continuación, haga clic en el nombre del grupo en el que desea crear o personalizar estados.
1. En el panel izquierdo, haga clic en **Estados** ![](assets/gear-icon-settings.png).
1. Abra la ficha **Proyecto**, **Tareas** o **Problemas**, según el tipo de estado que desee establecer como estado predeterminado.
1. Haga clic en **Establecer estados predeterminados** cerca de la esquina superior derecha.
1. En el área desplegable que se muestra, junto al estado en el que desea establecer el estado predeterminado, seleccione el estado predeterminado que desee establecer.
1. Haga clic en **Guardar**.

   El estado ya está disponible como estado predeterminado para su uso con proyectos asociados al grupo.

1. Asocie el estado personalizado al proyecto en el que desea utilizarlo.

   Para asociar el estado al proyecto, asocie el grupo en el que reside el estado con el proyecto. Los usuarios solo pueden utilizar el estado personalizado si el grupo en el que reside el estado está asociado al proyecto.

   >[!NOTE]
   >
   >Si asigna el proyecto a un grupo diferente, el estado del proyecto se volverá a cargar y podría cambiar.

   1. Vaya al proyecto en el que desea utilizar el estado personalizado.
   1. Haga clic en el menú Más ![](assets/more-icon.png) y luego haga clic en **Editar**.
   1. En el cuadro **Editar proyecto** que se muestra, en el campo **Grupo** bajo **Asociación de proyecto**, seleccione el grupo al que está asociado el estado personalizado.

   1. Haga clic en **Guardar cambios**.

## Los grupos heredan las configuraciones de estado predeterminadas

Después de que un administrador de Workfront configure un estado personalizado como estado predeterminado, los nuevos grupos que se creen heredarán esa configuración.

Del mismo modo, después de que un administrador de grupo establezca un estado personalizado como estado predeterminado, los nuevos subgrupos creados directamente debajo del grupo heredan esa configuración.

Para obtener más información, vea [Cómo heredan los grupos los estados](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## Cuando un estado predeterminado está oculto

Si oculta un estado predeterminado (activando la opción Ocultar estado ), el sistema intenta establecer otro estado del tipo equivalente como predeterminado en su lugar.

Si no hay ningún estado disponible del tipo equivalente, el tipo de estado se mostrará como **Oculto** y no estará disponible para los elementos de trabajo.

![](assets/when-hide-default-status-no-equivalent.png)
