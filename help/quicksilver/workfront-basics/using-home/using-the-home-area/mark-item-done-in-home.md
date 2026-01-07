---
product-area: projects
navigation-topic: use-the-home-area
title: Marcar un elemento como Listo en el área de Inicio
description: Puede marcar una tarea o un problema como Listo si es el usuario asignado de la tarea o el problema. Cuando marca una tarea o un problema como Listo, el estado cambia a Completado.
author: Courtney
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 78%

---

# Marcar un elemento como [!UICONTROL Listo] en el área de [!UICONTROL Inicio]

Puede marcar una tarea o un problema como Listo si es el usuario asignado de la tarea o el problema. Cuando marca una tarea o un problema como [!UICONTROL Listo], el estado cambia a [!UICONTROL Completado].

>[!NOTE]
>
>No verá el botón [!UICONTROL Listo] salvo que usted sea uno de los recursos asignados a la tarea o al problema.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia</strong></td> 
   <td> 
   <p>Estándar</p>
   <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>Acceso de [!UICONTROL Edit] a tareas y problemas</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Permisos de aportación o superiores para las tareas y problemas en los que debe trabajar</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Marcar un elemento de trabajo como Listo en el widget Mi trabajo

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Haga clic en **Personalizar** para agregar el widget **Mi trabajo**.
1. Busque el elemento de trabajo y haga clic en **[!UICONTROL Marcar como listo]** en el elemento de trabajo.
Consulte [Comprender las opciones del botón [!UICONTROL Listo]](#understand-the-options-of-the-done-button) para obtener información más detallada sobre cómo puede aparecer este botón.
   ![Mi marca de trabajo como terminada](assets/my-work-done.png)


## Marcar un elemento de trabajo como Listo en el panel Resumen

Puede marcar un elemento de trabajo como Listo en el widget Mis tareas y Mis problemas mediante el Panel de resumen.

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Haga clic en **Personalizar** para agregar los widgets **Mis tareas** o **Mis problemas**.
1. Pase el ratón sobre el elemento de trabajo y luego haga clic en el icono **Resumen**.
   ![Abrir resumen](assets/open-summary-new-home.png)
1. Haga clic en **Marcar como listo** en la parte superior del panel Resumen.


## Comprender las opciones del botón [!UICONTROL Listo]

De manera predeterminada, al hacer clic en el botón [!UICONTROL Listo] en un elemento de trabajo, se cambia el estado de ese elemento a [!UICONTROL Completado] (para tareas) o [!UICONTROL Resuelto] (para problemas).

El administrador de [!DNL Adobe Workfront] puede personalizar los estados asociados con el botón [!UICONTROL Listo] y aplicar esas personalizaciones a su equipo de Inicio.

Dependiendo de cuántos estados estén asociados al botón [!UICONTROL Listo] o de cuántos recursos estén asignados a la tarea o al problema, la apariencia del botón [!UICONTROL Listo] puede cambiar.

* [Botón [!UICONTROL Listo] asociado a un estado](#done-button-associated-with-one-status)
* [Botón [!UICONTROL Listo] asociado a varios estados](#done-button-associated-with-multiple-statuses)
* [Botón [!UICONTROL Listo] para elementos asignados a varios recursos](#done-button-for-items-assigned-to-multiple-resources)

### Botón [!UICONTROL Listo] asociado a un estado

Cuando el botón [!UICONTROL Listo] está asociado a un estado y el elemento de trabajo se le asigna únicamente a usted, el botón indica **[!UICONTROL Listo]**. Al hacer clic en él, el estado de la tarea o del problema cambia al estado asociado con el botón [!UICONTROL Listo].

![Botón Listo](assets/done-button-status.png)

Para saber qué estado está asociado con el botón [!UICONTROL Listo], consulte la sección [!UICONTROL Configuración del equipo] de su equipo de Inicio para el [!UICONTROL Botón Listo], tal como se describe en [Editar configuración del equipo](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

Si no tiene asignado un equipo de Inicio, se elige el estado predeterminado al hacer clic en [!UICONTROL Listo], tal como se describe más arriba en [Comprender las opciones del botón [!UICONTROL Listo]](#understand-the-options-of-the-done-button).

### Botón [!UICONTROL Listo] asociado a varios estados

Cuando el botón [!UICONTROL Listo] está asociado con más de un estado, el botón muestra la palabra **[!UICONTROL Listo]**, que va seguida de un menú desplegable. En este escenario, no es posible simplemente hacer clic en [!UICONTROL Listo]. Debe seleccionar un estado en el menú desplegable. Seleccione el estado que mejor se ajuste a la finalización del elemento de trabajo. Al hacerlo, cambia el estado del elemento de trabajo.

Para comprender cómo puede asociar varios estados al botón [!UICONTROL Listo], consulte [Configurar el botón [!UICONTROL Listo] para las tareas](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md) y [Configurar el botón [!UICONTROL Listo] para los problemas](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md).

### Botón [!UICONTROL Listo] para elementos asignados a varios recursos

Cuando la tarea o el problema se asignan a más de un recurso, el botón muestra la palabra **[!UICONTROL Listo]**, seguida de un menú desplegable. En el menú desplegable, tiene la opción de elegir entre **[!UICONTROL Listo con mi parte]** (lo que permite a los integrantes del equipo saber que ha completado su parte de la tarea) o el estado asociado con el botón [!UICONTROL Listo] (lo que completa el elemento). Después de seleccionar **[!UICONTROL Terminé mi parte]**, el elemento de trabajo se quitará de su Lista de trabajos, pero permanecerá en la Lista de trabajos de los que aún tengan asignado el elemento de trabajo.\
Si el botón Listo está asociado a varios estados, se enumeran en **Terminé mi parte**.

>[!NOTE]
>
>En una tarea o un problema con varias personas asignadas, los usuarios son responsables de indicar que se ha completado su propia asignación en la tarea o el problema. Por ello, los usuarios asignados debe hacer clic en [!UICONTROL Listo] para mostrar que han completado el trabajo que se les ha asignado en el elemento.

![Terminé mi parte](assets/done-with-my-part.png)

