---
title: Establecer una condición personalizada como predeterminada para tareas y problemas
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Cuando un usuario hace clic en Trabajar en ello o añada un comentario de actualización a una nueva tarea asignada (sin configurar manualmente una condición para la tarea), Adobe Workfront muestra la condición predeterminada de las tareas, lo que se establece en Configuración. Lo mismo ocurre con los problemas.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 97%

---

# Establecer una condición personalizada como predeterminada para tareas y problemas

Cuando un usuario hace clic en Trabajar en ello o añada un comentario de actualización a una nueva tarea asignada (sin configurar manualmente una condición para la tarea), Adobe Workfront muestra la condición predeterminada de las tareas, lo que se establece en Configuración. Lo mismo ocurre con los problemas.

Workfront usa la condición integrada Sin problemas como condición predeterminada para las tareas y, por separado, para los problemas. Como administrador de Workfront, puede cambiar la condición predeterminada para ambos tipos de objetos a una condición personalizada que haya creado.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Administrador del sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Establezca una condición personalizada como condición predeterminada para las tareas o para los problemas:

{{step-1-to-setup}}

1. Haga clic en **Preferencias del proyecto** > **Condiciones**.

1. Haga clic en la pestaña **Tareas** o en la pestaña **Problemas**.

1. Haga clic en **Establecer condiciones predeterminadas**.
1. En el menú desplegable, haga clic en la condición personalizada que quiera que sea la condición predeterminada de las tareas (o problemas).
1. Haga clic en **Guardar**.

>[!NOTE]
>
>* Un usuario asignado a una tarea o un problema, o que tenga permisos de administración en ellos, puede cambiar su condición manualmente. Para obtener más información, consulte [Actualizar condición para tareas y problemas](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* Las tres condiciones predeterminadas para las tareas y los problemas que se incluyen en Workfront son Sin problemas, Algunas preocupaciones e Impedimentos mayores. No es posible ocultar ni eliminar estas condiciones, pero sí cambiar sus nombres y colores. O se pueden crear otras nuevas para usarlas en su lugar, tal y como se describe en [Crear o editar una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Para obtener información acerca de cómo configurar una condición personalizada como condición predeterminada para los proyectos, consulte [Establecer una condición personalizada como predeterminada para proyectos](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).
