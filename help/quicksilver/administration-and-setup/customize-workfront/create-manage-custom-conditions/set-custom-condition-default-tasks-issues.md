---
title: Establecer una condición personalizada como predeterminada para tareas y problemas
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Cuando un usuario hace clic en Trabajar en ello o agrega un comentario de actualización a una nueva tarea a la que se les ha asignado (sin configurar manualmente una condición para la tarea), Adobe Workfront muestra la condición predeterminada para las tareas, que se configura en Configuración. Lo mismo ocurre con los problemas.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Establecer una condición personalizada como predeterminada para tareas y problemas

Cuando un usuario hace clic en Trabajar en ello o agrega un comentario de actualización a una nueva tarea a la que se les ha asignado (sin configurar manualmente una condición para la tarea), Adobe Workfront muestra la condición predeterminada para las tareas, que se configura en Configuración. Lo mismo ocurre con los problemas.

Workfront utiliza la condición integrada Ir sin problemas como condición predeterminada para las tareas y, por separado, para los problemas. Como administrador de Workfront, puede cambiar la condición predeterminada para ambos tipos de objetos a una condición personalizada que haya creado.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Establezca una condición personalizada como condición predeterminada para las tareas o para los problemas:

{{step-1-to-setup}}

1. Haga clic en **Preferencias del proyecto** > **Condiciones**.

1. Haga clic en la ficha **Tareas** o **Problemas**.

1. Haga clic en **Establecer condiciones predeterminadas**.
1. En el menú desplegable, haga clic en la condición personalizada que desee como condición predeterminada para las tareas (o problemas).
1. Haga clic en **Guardar**.

>[!NOTE]
>
>* Un usuario asignado a una tarea o un problema, o que tenga permisos de administración en ellos, puede cambiar su condición manualmente. Para obtener más información, consulte [Actualizar condición para tareas y problemas](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* Las tres condiciones predeterminadas para las tareas y los problemas que se incluyen en Workfront son Continuar sin problemas, Algunas preocupaciones y Obstáculos principales. No puede ocultar ni eliminar estas condiciones, pero puede cambiar sus nombres y colores. O puede crear otras nuevas para usarlas en su lugar, tal como se describe en [Crear o editar una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
>

Para obtener información acerca de cómo configurar una condición personalizada como condición predeterminada para los proyectos, vea [Establecer una condición personalizada como predeterminada para los proyectos](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Para obtener información acerca de las condiciones personalizadas, vea [Condiciones personalizadas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
