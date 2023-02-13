---
product-area: projects
navigation-topic: use-the-home-area
title: Marcar un elemento como Hecho en el área de inicio
description: Puede marcar una tarea o un problema como Listo si es la tarea o el usuario asignado del problema. Cuando marca una tarea o un problema como Listo, el estado de la tarea o del problema cambia a Completado.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# Marcar un elemento como [!UICONTROL Listo] en el [!UICONTROL Página principal] area

Puede marcar una tarea o un problema como Listo si es la tarea o el usuario asignado del problema. Al marcar una tarea o un problema como [!UICONTROL Listo], el estado de la tarea o del problema se cambia a [!UICONTROL Completar].

>[!NOTE]
>
>No ve la variable [!UICONTROL Listo] a menos que sea uno de los recursos asignados a la tarea o al problema.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Work] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Acceso de [!UICONTROL Edit] a Tareas y problemas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Permisos de Contribute o superior a las tareas y problemas en los que debe trabajar</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Marcar una tarea o un problema como [!UICONTROL Listo]

Solo el usuario asignado a la tarea o al problema puede marcarla como [!UICONTROL Listo].

1. Haga clic en el **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **[!UICONTROL Página principal]**.
1. En el **[!UICONTROL Lista de trabajo]**, localice cualquiera de los elementos en espera de trabajar.
1. Realice una de las siguientes acciones:

* Haga clic en **[!UICONTROL Listo]** en el elemento de trabajo.\
   Consulte [Comprender las opciones de [!UICONTROL Listo] botón](#understand-the-options-of-the-done-button) para obtener información más detallada sobre cómo puede aparecer este botón.

* Seleccione el elemento que desea marcar como hecho y, a continuación, en el panel derecho, haga clic en **[!UICONTROL Actualizar estado]** y, a continuación, cambie el estado del elemento a un estado que sea igual a [!UICONTROL Completar] o [!UICONTROL Cerrado].

## Comprender las opciones de [!UICONTROL Listo] botón

De forma predeterminada, al hacer clic en el botón [!UICONTROL Listo] en un elemento de trabajo cambia el estado de ese elemento a [!UICONTROL Completar] (para tareas) o [!UICONTROL Resuelto] (para problemas).

Su [!DNL Adobe Workfront] el administrador puede personalizar los estados asociados a la variable [!UICONTROL Listo] y aplique esas personalizaciones a su equipo de inicio.

Dependiendo de cuántos estados estén asociados con la variable [!UICONTROL Listo] o cuántos recursos se asignan a la tarea o al problema, el aspecto del [!UICONTROL Listo] puede cambiar.

* [[!UICONTROL Listo] botón asociado a un estado](#done-button-associated-with-one-status)
* [[!UICONTROL Listo] botón asociado a varios estados](#done-button-associated-with-multiple-statuses)
* [[!UICONTROL Listo] botón para elementos asignados a varios recursos](#done-button-for-items-assigned-to-multiple-resources)

### [!UICONTROL Listo] botón asociado a un estado

Cuando la variable [!UICONTROL Listo] está asociado con un estado y el elemento de trabajo solo está asignado a usted, el botón lee **[!UICONTROL Listo]**. Al hacer clic en él, el estado de la tarea o del problema se cambia al estado asociado con la variable [!UICONTROL Listo] botón.

![Botón Listo](assets/Done.png)

Para comprender qué estado está asociado con la variable [!UICONTROL Listo] , marque [!UICONTROL Configuración de equipo] de su equipo de origen para [!UICONTROL Botón Listo] , tal como se describe en [Editar configuración de equipo](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

Si no está asignado a un equipo de inicio, se elige el estado predeterminado al hacer clic en [!UICONTROL Listo], tal como se describe anteriormente en [Comprender las opciones de [!UICONTROL Listo] botón](#understand-the-options-of-the-done-button).

### [!UICONTROL Listo] botón asociado a varios estados

Cuando la variable [!UICONTROL Listo] está asociado con más de un estado, el botón muestra la palabra **[!UICONTROL Listo]** que va seguido de un menú desplegable. En esta situación, no puede hacer clic en [!UICONTROL Listo]. Debe seleccionar un estado en el menú desplegable. Seleccione el estado que mejor se adapte a la finalización del elemento de trabajo. Al hacerlo, está cambiando el estado del elemento de trabajo.

Para comprender cómo se pueden asociar varios estados con la variable [!UICONTROL Listo] botón, consulte [Configure las variables [!UICONTROL Listo] botón para tareas](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md) y [Configure las variables [!UICONTROL Listo] botón para problemas](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md).

<!--
<img src="assets/marking-an-item-done-multiple-statuses-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

### [!UICONTROL Listo] botón para elementos asignados a varios recursos

Cuando la tarea o el problema se asignan a más de un recurso, el botón muestra la palabra **[!UICONTROL Listo]** que va seguido de un menú desplegable. En el menú desplegable, tiene la opción de elegir entre **[!UICONTROL Hecho con mi parte]** (lo que permite a los integrantes del equipo saber que se ha completado con la parte de la tarea) o el estado asociado con la variable [!UICONTROL Listo] (que completa el elemento). Después de seleccionar **[!UICONTROL Hecho con mi parte]**, el elemento de trabajo se elimina de la lista de trabajo, pero permanece en la lista de trabajo de los que aún están asignados al elemento de trabajo.\
Si el botón Listo está asociado con varios estados, estos se enumeran en **Hecho con mi parte**.

>[!NOTE]
>
>En una tarea o problema con varios asignadores, cada usuario es responsable de indicar que su propia asignación en la tarea o el problema se ha completado. Por este motivo, cada usuario asignado debe hacer clic en [!UICONTROL Listo] para mostrar que han completado el trabajo asignado en el elemento.

![](assets/marking-an-item-done-with-my-part-grop-by-drop-down-nwe-350x266.png)
