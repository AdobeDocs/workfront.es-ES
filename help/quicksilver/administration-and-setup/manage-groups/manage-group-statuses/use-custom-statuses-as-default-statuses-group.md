---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Usar un estado personalizado como estado predeterminado para un grupo
description: Como administrador de grupos, puede configurar un estado personalizado como estado predeterminado para un grupo o subgrupo que administra. Esto resulta útil cuando el sistema necesita asignar automáticamente un estado de Workfront a un proyecto, tarea o problema. Un proyecto, tarea o problema siempre muestra el estado personalizado que ha establecido como estado predeterminado en lugar de mostrar el estado de Workfront al que se equipara.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Usar un estado personalizado como estado predeterminado para un grupo

Como administrador de grupos, puede configurar un estado personalizado como estado predeterminado para un grupo o subgrupo que administra. Esto resulta útil cuando el sistema necesita asignar automáticamente un estado de Workfront a un proyecto, tarea o problema. Un proyecto, tarea o problema siempre muestra el estado personalizado que ha establecido como estado predeterminado en lugar de mostrar el estado de Workfront al que se equipara.

El estado que configure puede ser cualquier estado personalizado creado para el grupo, heredado de un grupo por encima del grupo o heredado del nivel del sistema.

Si hay algún grupo por encima del grupo que administra, sus administradores también pueden hacerlo por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!INFO]
>
>**Ejemplo:** Puede crear un estado personalizado llamado Finished y establecerlo como un estado predeterminado equivalente al estado de Workfront Complete.
>
>A continuación, para las tareas configuradas para cambiar al estado Completado cuando alcanzan el 100 %, el estado se muestra como Finalizado en lugar de Completado.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o administrador de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Estados de problemas

Si el estado personalizado es un estado de problema, los cuatro tipos de problema deben estar habilitados para él (informe de errores, orden de cambio, problema y solicitud). Por ejemplo, en el estado del problema que se muestra a continuación, el estado Reabierto no se puede usar como estado predeterminado porque el tipo de problema Cambiar orden no está seleccionado:

![](assets/all-4-issue-types-enabled.png)

## Establecer un estado personalizado como estado predeterminado para un grupo

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).
1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png)y, a continuación, haga clic en el nombre del grupo en el que desea crear o personalizar estados.
1. En el panel izquierdo, haga clic en **Estados** ![](assets/gear-icon-settings.png).
1. Abra el **Proyecto**, **Tareas** o **Problemas** , según el tipo de estado que desee establecer como estado predeterminado.
1. Haga clic en **Definir estados predeterminados** cerca de la esquina superior derecha.
1. En el área desplegable que se muestra, junto al estado en el que desea definir el estado predeterminado, seleccione el estado predeterminado que desee establecer.
1. Haga clic en **Guardar**.

   El estado ahora está disponible como estado predeterminado para su uso con proyectos asociados al grupo.

1. Asocie el estado personalizado al proyecto en el que desea utilizarlo.

   El estado se asocia al proyecto asociándolo al grupo donde reside el estado. Los usuarios pueden utilizar el estado personalizado solo si el grupo en el que reside el estado está asociado al proyecto.

   >[!NOTE]
   >
   >Si asigna el proyecto a un grupo diferente, el estado del proyecto se volverá a cargar y podría cambiar.

   1. Vaya al proyecto en el que desea utilizar el estado personalizado.
   1. Haga clic en el menú Más ![](assets/more-icon.png)y haga clic en **Editar**.
   1. En el **Editar proyecto** que se muestra en la **Grupo** campo bajo **Asociación de proyectos**, seleccione el grupo al que está asociado el estado personalizado.

   1. Haga clic en **Guardar cambios**.

## Los grupos heredan las configuraciones de estado predeterminadas

Una vez que un administrador de Workfront configura un estado personalizado como predeterminado, los nuevos grupos que se crean heredan esa configuración.

Del mismo modo, después de que un administrador de grupo establezca un estado personalizado como predeterminado, los nuevos subgrupos creados directamente debajo del grupo heredarán esa configuración.

Para obtener más información, consulte [Cómo heredan los estados los grupos](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## Cuando el estado predeterminado está oculto

Si oculta un estado predeterminado (habilitando la opción Ocultar estado para él), el sistema intenta establecer otro estado del tipo equivalente como predeterminado en su lugar.

Si no hay ningún estado disponible del tipo equivalente, el tipo de estado se muestra como **Oculto** y no está disponible para elementos de trabajo.

![](assets/when-hide-default-status-no-equivalent.png)
