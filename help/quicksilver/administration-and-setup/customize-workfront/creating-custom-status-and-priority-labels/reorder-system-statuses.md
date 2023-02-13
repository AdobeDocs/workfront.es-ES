---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Reordenar los estados del sistema y del grupo
description: Como administrador de Workfront, puede cambiar el orden de los estados de proyecto, tarea y problema para todos los miembros del sistema o de un solo grupo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 6%

---

# Reordenar los estados del sistema y del grupo

Como administrador de Workfront, puede cambiar el orden de los estados de proyecto, tarea y problema para todos los miembros del sistema o de un solo grupo.

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![](assets/statuses.png)

>[!NOTE]
>
>* La reordenación de los estados a nivel del sistema no afecta al orden de los estados dentro de los grupos.
>
>  Sin embargo, los estados de un grupo de nivel superior creado recientemente heredan el orden de los estados de nivel del sistema. (Un nuevo subgrupo hereda el orden de los estados del grupo un nivel superior).
>
>* Puede reordenar los estados bloqueados. Para obtener información sobre los estados bloqueados, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* Los administradores de grupos también pueden reordenar los estados que se usan en sus grupos. Para obtener más información, consulte [Reordenar estados de grupos](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md).
>


## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront* </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de Workfront. Para obtener información sobre los administradores de Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Orden predeterminado de los estados

De forma predeterminada, los estados se muestran en el siguiente orden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">Proyecto</th> 
   <th width="33.33%">Tarea</th> 
   <th width="33.33%">Problema</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Al día</li> 
     <li>Inactivo</li> 
     <li> En espera </li> 
     <li> Planificación </li> 
     <li> Finalizado </li> 
     <li> Solicitado </li> 
     <li> Aprobado </li> 
     <li> Rechazado </li> 
     <li> Idea </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Nuevo</li> 
     <li>En curso</li> 
     <li>Finalizado</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Nuevo</li> 
     <li>En curso</li> 
     <li>Vuelto a abrir</li> 
     <li>Esperando comentarios</li> 
     <li>En espera</li> 
     <li>No se puede duplicar</li> 
     <li>Cerrado</li> 
     <li>Resuelto</li> 
     <li>Verificación completa</li> 
     <li>No se puede resolver</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Reordenar estados para tareas y proyectos de todo el sistema o para un grupo

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Preferencias del proyecto > Estados**.
1. (Condicional) Si está reordenando los estados de un grupo, empiece a escribir el nombre del grupo en el cuadro de la esquina superior derecha y, a continuación, haga clic en el nombre cuando aparezca.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Sobre la lista Estados que se muestra, haga clic en el botón **Proyectos** o **Tareas** pestaña .

1. Arrastre y suelte los estados en el orden que desee.

   El nuevo orden de estado se guarda automáticamente.

1. Para probar el nuevo orden de estado, vaya a una tarea o proyecto, haga clic en el estado en la esquina superior derecha y asegúrese de que los estados que se muestran estén en el orden configurado.

## Reordenar estados por problemas

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Preferencias del proyecto > Estados.**
1. (Condicional) Si está reordenando los estados de un grupo, empiece a escribir el nombre del grupo en el cuadro de la esquina superior derecha y, a continuación, haga clic en el nombre cuando aparezca.

   ![](assets/issue-statuses-group-name.png)

1. Haga clic en el **Problemas** pestaña .
1. (Opcional) Seleccione un tipo de problema (**Informe de errores**, **Cambiar orden**, **Problema** o **Solicitud**).

   >[!NOTE]
   >
   >* No se puede personalizar el orden de los estados de la lista maestra.
   >* Le recomendamos que ordene los estados de cada tipo de problema del mismo modo. Para obtener más información sobre los tipos de problemas, consulte [Configurar tipos de solicitud](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).


1. Arrastre y suelte los estados en el orden que desee.

   El nuevo orden de estado se guarda automáticamente.

1. Para probar el nuevo orden de estado, vaya a un problema, haga clic en el estado en la esquina superior derecha y asegúrese de que los estados que se muestran estén en el orden configurado.
