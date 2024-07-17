---
product-area: projects
navigation-topic: convert-issues
title: Conversión de un problema en una tarea en Adobe Workfront
description: Si es necesario trabajar más para completar un problema una vez enviado, puede convertir el problema en una tarea.
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: 44f01128ef4e6581dc8eaca318a999f2e7274f2a
workflow-type: tm+mt
source-wordcount: '1058'
ht-degree: 1%

---

# Conversión de un problema en una tarea en Adobe Workfront

Si es necesario trabajar más para completar un problema una vez enviado, puede convertir el problema en una tarea.

Para obtener información general sobre la conversión de problemas, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas, Tareas y Proyectos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos para el problema</p> <p>Permisos de Contribute para el proyecto</p> <p>Puede obtener permisos de administración para la tarea después de convertir el problema</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Convertir un problema en una tarea

1. Vaya a un proyecto y haga clic en [!UICONTROL **Problemas**] en el panel izquierdo.
1. Haga clic en el problema que desee convertir para ir a la página de aterrizaje del problema.
1. Haga clic en el menú [!UICONTROL **Más**] del problema y luego [!UICONTROL **Convertir a tarea**].

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >Si el problema está asociado a un proceso de aprobación o ya está asociado a un objeto de resolución, Workfront muestra una advertencia en la parte superior del cuadro [!UICONTROL Convertir en proyecto] para notificarle que la aprobación se ha eliminado o que el objeto de resolución se ha sobrescrito durante la conversión. Para obtener más información, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Actualice el nombre de la tarea en la sección [!UICONTROL Nombre de tarea]. De forma predeterminada, el nombre de la tarea tendrá el mismo nombre que el del problema original.

   ![](assets/convert-to-task-box-nwe.png)

1. Haga clic en [!UICONTROL **Proyecto de destino**] y, a continuación, empiece a escribir el nombre del proyecto donde desea colocar la nueva tarea en el campo [!UICONTROL **Proyecto de destino**] y selecciónelo cuando se muestre en la lista. El proyecto del problema está seleccionado de forma predeterminada.

1. Haga clic en [!UICONTROL **Información general**] y, a continuación, escriba una [!UICONTROL **Descripción**] para la tarea.

   >[!TIP]
   >
   >   Un administrador de sistemas o de grupos puede cambiar el orden de las secciones del panel izquierdo del cuadro de conversión modificando la plantilla de diseño.

1. (Opcional y condicional) Haga clic en [!UICONTROL **Opciones**] y seleccione cualquiera de las siguientes opciones.

   El administrador de Workfront o del grupo debe habilitar estas preferencias antes de que sean visibles durante la conversión de problemas:

   * [!UICONTROL **Mantener el problema original y enlazar su solución a esta tarea**]

     Si no se selecciona, se elimina el problema original.

     >[!NOTE]
     >
     >Los usuarios sin acceso o permisos para eliminar problemas no podrán eliminar el problema a medida que lo vayan convirtiendo, independientemente del estado de esta configuración. Para obtener información sobre el acceso y los permisos a los problemas, consulte:
     >   
     >   * [Conceder acceso a problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     >   * [Compartir un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)
     >   
     >

   * [!UICONTROL **Permitir que (Nombre de usuario) tenga acceso a esta tarea**]

     Si no se selecciona, el contacto principal del problema no tiene acceso a la nueva tarea.

   * [!UICONTROL **Conservar la fecha planificada de finalización del problema**]

     Si no se selecciona, la [!UICONTROL Fecha planificada de finalización] de la nueva tarea se calcula a partir de la [!UICONTROL Fecha planificada de inicio] de la tarea. La [!UICONTROL fecha planificada de inicio] de la nueva tarea se ha establecido de acuerdo con las preferencias del sistema para las nuevas tareas.

     >[!NOTE]
     >
     >
     >Las opciones que se muestran aquí dependen de cómo las haya configurado el administrador de Workfront para todos los miembros del sistema. Para obtener más información, consulte [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >O bien, si los grupos de nivel superior de su organización los configuraron por separado, las opciones que se muestran aquí dependen del grupo asociado al proyecto seleccionado en el paso 6. Para obtener más información, consulte [Configurar las preferencias de tareas y problemas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. (Opcional) Haga clic en [!UICONTROL **Forms personalizado**] y adjunte un formulario personalizado para la nueva tarea.

   >[!TIP]
   >
   >* Si un formulario personalizado de varios objetos adjunto al problema está configurado para utilizarse tanto con problemas como con tareas, toda la información guardada en el formulario se conservará al realizar la conversión si los campos existen tanto en el problema como en los formularios personalizados de la tarea.
   >* Si se adjunta al problema y a la tarea un formulario personalizado de varios objetos con un campo calculado, el problema y la tarea deben ser compatibles con todos los campos a los que se hace referencia en los campos personalizados calculados del formulario. Si se produce una incompatibilidad, un mensaje le advierte de que realice los ajustes necesarios. Para obtener más información, consulte la sección &quot;Campos personalizados calculados en formularios personalizados de varios objetos&quot; en [Agregar datos calculados a un formulario personalizado con el generador de formularios heredados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
   >* Si el proyecto de destino tiene formularios predeterminados definidos en el campo Forms personalizado predeterminado de la tarea al editar el proyecto, esos formularios de tareas también se agregan a la nueva tarea. Todos los campos personalizados que sean comunes entre el problema original y los campos de los formularios de tarea predeterminados se rellenan previamente con información de los campos de problema.


1. Haga clic en [!UICONTROL **Convertir en tarea**].

   El problema ahora es una tarea en el proyecto designado, si ha decidido eliminar el problema original.

   O

   El problema ahora está vinculado a la nueva tarea del proyecto que eligió y se completará una vez que la tarea se complete, si decidió mantener el problema original.

   Algunos campos de problema se transfieren a la tarea. Para obtener más información, consulte la sección [Ver información original del problema sobre proyectos y tareas](#view-original-issue-information-on-projects-and-tasks) de este artículo.

1. (Opcional) Continúe editando la tarea según sea necesario.

## Ver información del problema original de proyectos y tareas {#view-original-issue-information-on-projects-and-tasks}

Puede ver la información original del problema en las listas y los informes de proyectos y tareas, o en el área Detalles del proyecto. Para obtener información sobre cómo generar informes, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

La siguiente tabla ilustra qué campos de problema son visibles desde los proyectos y tareas convertidos.

| Campos de problema | Campo de proyecto o tarea | Lista o informe de proyecto | Área Detalles del proyecto | Lista de tareas o informe | Área Detalles de la tarea |
|---|---|---|---|---|---|
| [!UICONTROL Nombre de problema] | [!UICONTROL Nombre de problema convertido] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL Contacto principal] | [!UICONTROL Nombre del creador del problema convertido] | ✔ | ✔ | ✔ |
| [!UICONTROL Fecha de entrada] | [!UICONTROL Fecha de entrada de problema convertido] | ✔ |  | ✔ |


>[!CAUTION]
>
>Si el [!UICONTROL Contacto principal] de un problema cambia o si el problema se desenlaza del proyecto o tarea después de que se haya convertido el problema, el [!UICONTROL Nombre del creador del problema convertido]no se actualiza y muestra el [!UICONTROL Contacto principal] original del problema en el momento en que se convirtió el problema.
