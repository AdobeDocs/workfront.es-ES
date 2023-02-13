---
product-area: projects
navigation-topic: convert-issues
title: Conversión de un problema en una tarea en Adobe Workfront
description: Si se debe trabajar más para completar un problema después de que se envíe el problema, se puede convertir el problema en una tarea.
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 2%

---

# Conversión de un problema en una tarea en Adobe Workfront

Si se debe trabajar más para completar un problema después de que se envíe el problema, se puede convertir el problema en una tarea.

Para obtener información general sobre la conversión de problemas, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

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
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas, Tareas y Proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos para el problema</p> <p>Permisos de Contribute para el proyecto</p> <p>Obtenga permisos de administración para la tarea después de convertir el problema</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Convertir un problema en una tarea

1. Vaya a un proyecto y haga clic en [!UICONTROL **Problemas** ] en el panel izquierdo.
1. Haga clic en el problema que desea convertir para ir a la página de aterrizaje del problema.
1. Haga clic en el [!UICONTROL **Más**] en el número y, a continuación, [!UICONTROL **Convertir en tarea**].

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >Si el problema está asociado con un proceso de aprobación o ya está asociado con un objeto de resolución, Workfront muestra una advertencia en la parte superior del [!UICONTROL Convertir en proyecto] para notificarle que la aprobación se ha eliminado o que el objeto de resolución se ha sobrescrito durante la conversión. Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Actualice el nombre de la tarea en el [!UICONTROL Nombre de la tarea] para obtener más información. De forma predeterminada, el nombre de la tarea será el mismo que el del problema original.

   ![](assets/convert-to-task-box-nwe.png)

1. Haga clic en [!UICONTROL **Proyecto de destino**] y, a continuación, empiece a escribir el nombre del proyecto en el que desea colocar la nueva tarea en la [!UICONTROL **Proyecto de destino**] y selecciónelo cuando aparezca en la lista. El proyecto del problema está seleccionado de forma predeterminada.

1. Haga clic en [!UICONTROL **Información general**] y, a continuación, escriba un [!UICONTROL **Descripción**] para la tarea.

   >[!TIP]
   >
   >   Un administrador de sistemas o grupos puede cambiar el orden de las secciones en el panel izquierdo del cuadro de conversión modificando la plantilla de diseño.

1. (Opcional y condicional) Haga clic en [!UICONTROL **Opciones**], seleccione cualquiera de las siguientes opciones.

   El administrador de Workfront o el administrador de grupos deben habilitar estas preferencias antes de que sean visibles durante la conversión de problemas:

   * [!UICONTROL **Mantener el problema original y enlazar su resolución a esta tarea**]

      Si no se selecciona, se elimina el problema original.

      >[!NOTE]
      >
      >Los usuarios sin acceso o permisos para eliminar problemas no podrán eliminar el problema a medida que lo estén convirtiendo, independientemente del estado de esta configuración. Para obtener información sobre el acceso y los permisos a los problemas, consulte:
      >   
      >   * [Concesión de acceso a problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
      >   * [Compartir un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)


   * [!UICONTROL **Permitir (nombre de usuario) tener acceso a esta tarea**]

      Si no está seleccionado, el contacto principal del problema no tiene acceso a la nueva tarea.

   * [!UICONTROL **Conservar la fecha de finalización de tarea del problema**]

      Si no se selecciona, la variable [!UICONTROL Fecha de finalización planeada] de la nueva tarea se calcula a partir del [!UICONTROL Fecha de inicio planeada] de la tarea. La variable [!UICONTROL Fecha de inicio planeada] de la nueva tarea se establece según las preferencias del sistema para las nuevas tareas.

      >[!NOTE]
      >
      >
      >Las opciones que se muestran aquí dependen de cómo las haya configurado el administrador de Workfront para todos los miembros del sistema. Para obtener más información, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
      >
      >O bien, si los grupos de nivel superior de su organización los configuran por separado, las opciones que se muestran aquí dependen de qué grupo esté asociado con el proyecto que ha seleccionado en el paso 6. Para obtener más información, consulte [Configuración de las preferencias de tarea y problema para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. (Opcional) Haga clic en [!UICONTROL **Forms personalizado**] y adjuntar un formulario personalizado para la nueva tarea.

   >[!TIP]
   >
   >Si un formulario personalizado de varios objetos adjunto al problema está configurado para su uso con problemas y tareas, el formulario se adjunta de forma predeterminada. Toda la información guardada en el formulario de problemas se conserva para la tarea cuando realiza la conversión.
   >
   >Si el proyecto de destino tiene formularios predeterminados definidos en el campo Forms personalizado predeterminado de tarea al editar el proyecto, esos formularios de tareas también se agregan a la nueva tarea. Los campos personalizados que sean comunes entre el problema original y los campos de los formularios de tareas predeterminados se rellenarán previamente con información de los campos de problema.

1. Haga clic en [!UICONTROL **Convertir en tarea**].

   El problema ahora es una tarea del proyecto designado, si ha decidido eliminar el problema original.

   O

   El problema ahora está vinculado a la nueva tarea del proyecto que ha elegido y se completará una vez finalizada la tarea, si ha decidido mantener el problema original.

   Algunos campos de problema se transfieren a la tarea. Para obtener más información, consulte la [Ver la información del problema original en proyectos y tareas](#view-original-issue-information-on-projects-and-tasks) en este artículo.

1. (Opcional) Continúe editando la tarea según sea necesario.

## Ver la información del problema original en proyectos y tareas {#view-original-issue-information-on-projects-and-tasks}

Puede ver la información del problema original en listas e informes de proyectos y tareas o en el área Detalles del proyecto . Para obtener información sobre la creación de informes, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

La siguiente tabla ilustra qué campos de problema son visibles desde los proyectos y tareas convertidos.

| Campos de problema | Campo de proyecto o tarea | Lista de proyectos o informe | Área Detalles del proyecto | Lista de tareas o informe | Área Detalles de la tarea |
|---|---|---|---|---|---|
| [!UICONTROL Nombre de problema] | [!UICONTROL Nombre de problema convertido] | š | ✔ | ✔ | ✔ |
| [!UICONTROL Contacto primario] | [!UICONTROL Nombre del creador del problema convertido] | ✔ | ✔ | ✔ |
| [!UICONTROL Fecha de entrada] | [!UICONTROL Fecha de entrada de problema convertido] | ✔ |  | ✔ |


>[!CAUTION]
>
>Si la variable [!UICONTROL Contacto principal] de un problema cambia o si el problema se desvincula del proyecto o la tarea después de que se haya convertido el problema, la variable [!UICONTROL Nombre del creador del problema convertido ]no se actualiza y muestra el original [!UICONTROL Contacto principal] del problema en el momento en que se convirtió el problema.
